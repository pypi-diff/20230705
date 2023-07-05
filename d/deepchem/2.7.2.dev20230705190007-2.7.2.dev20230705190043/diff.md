# Comparing `tmp/deepchem-2.7.2.dev20230705190007.tar.gz` & `tmp/deepchem-2.7.2.dev20230705190043.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230705190007.tar", last modified: Wed Jul  5 19:00:07 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230705190043.tar", last modified: Wed Jul  5 19:00:44 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230705190007.tar` & `deepchem-2.7.2.dev20230705190043.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.952293 deepchem-2.7.2.dev20230705190007/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-05 18:59:50.000000 deepchem-2.7.2.dev20230705190007/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 19:00:07.952293 deepchem-2.7.2.dev20230705190007/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-05 18:59:50.000000 deepchem-2.7.2.dev20230705190007/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.848290 deepchem-2.7.2.dev20230705190007/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.852290 deepchem-2.7.2.dev20230705190007/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.856290 deepchem-2.7.2.dev20230705190007/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.860291 deepchem-2.7.2.dev20230705190007/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.860291 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.864291 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.876291 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.876291 deepchem-2.7.2.dev20230705190007/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.876291 deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.880291 deepchem-2.7.2.dev20230705190007/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.880291 deepchem-2.7.2.dev20230705190007/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.880291 deepchem-2.7.2.dev20230705190007/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.892292 deepchem-2.7.2.dev20230705190007/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.892292 deepchem-2.7.2.dev20230705190007/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.896292 deepchem-2.7.2.dev20230705190007/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.896292 deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.896292 deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.900292 deepchem-2.7.2.dev20230705190007/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.912292 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   145843 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.916293 deepchem-2.7.2.dev20230705190007/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.932293 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.936293 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.936293 deepchem-2.7.2.dev20230705190007/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.936293 deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.940293 deepchem-2.7.2.dev20230705190007/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.940293 deepchem-2.7.2.dev20230705190007/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.948294 deepchem-2.7.2.dev20230705190007/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.948294 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:07.848290 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 19:00:07.000000 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-05 19:00:07.000000 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:00:07.000000 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 19:00:07.000000 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 19:00:07.000000 deepchem-2.7.2.dev20230705190007/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-05 19:00:07.952293 deepchem-2.7.2.dev20230705190007/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-05 18:59:51.000000 deepchem-2.7.2.dev20230705190007/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.117984 deepchem-2.7.2.dev20230705190043/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 19:00:44.117984 deepchem-2.7.2.dev20230705190043/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.073984 deepchem-2.7.2.dev20230705190043/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.073984 deepchem-2.7.2.dev20230705190043/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.073984 deepchem-2.7.2.dev20230705190043/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.077984 deepchem-2.7.2.dev20230705190043/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.077984 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.077984 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-05 19:00:28.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.081984 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.081984 deepchem-2.7.2.dev20230705190043/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.085984 deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.085984 deepchem-2.7.2.dev20230705190043/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.085984 deepchem-2.7.2.dev20230705190043/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.085984 deepchem-2.7.2.dev20230705190043/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.089984 deepchem-2.7.2.dev20230705190043/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.089984 deepchem-2.7.2.dev20230705190043/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.089984 deepchem-2.7.2.dev20230705190043/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.089984 deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.093984 deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.093984 deepchem-2.7.2.dev20230705190043/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.097984 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146027 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.097984 deepchem-2.7.2.dev20230705190043/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.105984 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.109984 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.109984 deepchem-2.7.2.dev20230705190043/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.109984 deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.109984 deepchem-2.7.2.dev20230705190043/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.109984 deepchem-2.7.2.dev20230705190043/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.113983 deepchem-2.7.2.dev20230705190043/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.117984 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:44.073984 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 19:00:43.000000 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-05 19:00:44.000000 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:00:43.000000 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 19:00:43.000000 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 19:00:43.000000 deepchem-2.7.2.dev20230705190043/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-05 19:00:44.117984 deepchem-2.7.2.dev20230705190043/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-05 19:00:29.000000 deepchem-2.7.2.dev20230705190043/setup.py
```

### Comparing `deepchem-2.7.2.dev20230705190007/LICENSE` & `deepchem-2.7.2.dev20230705190043/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/PKG-INFO` & `deepchem-2.7.2.dev20230705190043/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230705190007
+Version: 2.7.2.dev20230705190043
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230705190007/README.md` & `deepchem-2.7.2.dev20230705190043/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230705190043/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230705190043/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230705190043/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230705190043/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230705190043/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230705190043/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230705190043/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230705190043/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230705190043/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230705190043/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230705190043/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230705190043/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230705190043/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230705190043/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230705190043/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/models.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7751,1366 +7751,1377 @@
 0001e460: 7420 616c 2e20 2251 7561 6e74 756d 2d63  t al. "Quantum-c
 0001e470: 6865 6d69 6361 6c20 696e 7369 6768 7473  hemical insights
 0001e480: 2066 726f 6d20 6465 6570 0a20 2020 2020   from deep.     
 0001e490: 2020 2074 656e 736f 7220 6e65 7572 616c     tensor neural
 0001e4a0: 206e 6574 776f 726b 732e 2220 4e61 7475   networks." Natu
 0001e4b0: 7265 2063 6f6d 6d75 6e69 6361 7469 6f6e  re communication
 0001e4c0: 7320 382e 3120 2832 3031 3729 3a20 312d  s 8.1 (2017): 1-
-0001e4d0: 382e 0a0a 2020 2020 5061 7261 6d65 7465  8...    Paramete
-0001e4e0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0001e4f0: 2d0a 2020 2020 6e5f 656d 6265 6464 696e  -.    n_embeddin
-0001e500: 673a 2069 6e74 2c20 6f70 7469 6f6e 616c  g: int, optional
-0001e510: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
-0001e520: 6f66 2066 6561 7475 7265 7320 666f 7220  of features for 
-0001e530: 6561 6368 2061 746f 6d0a 2020 2020 6e5f  each atom.    n_
-0001e540: 6469 7374 616e 6365 3a20 696e 742c 206f  distance: int, o
-0001e550: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0001e560: 6772 616e 756c 6172 6974 7920 6f66 2064  granularity of d
-0001e570: 6973 7461 6e63 6520 6d61 7472 6978 0a20  istance matrix. 
-0001e580: 2020 206e 5f68 6964 6465 6e3a 2069 6e74     n_hidden: int
-0001e590: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0001e5a0: 2020 204e 756d 6265 7220 6f66 206e 6f64     Number of nod
-0001e5b0: 6573 2069 6e20 6869 6464 656e 206c 6179  es in hidden lay
-0001e5c0: 6572 0a20 2020 2069 6e69 7469 616c 697a  er.    initializ
-0001e5d0: 6572 3a20 7374 722c 206f 7074 696f 6e61  er: str, optiona
-0001e5e0: 6c0a 2020 2020 2020 2020 5765 6967 6874  l.        Weight
-0001e5f0: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
-0001e600: 666f 7220 6669 6c74 6572 732e 0a20 2020  for filters..   
-0001e610: 2020 2020 204f 7074 696f 6e73 3a20 7b78       Options: {x
-0001e620: 6176 6965 725f 756e 6966 6f72 6d5f 2c20  avier_uniform_, 
-0001e630: 7861 7669 6572 5f6e 6f72 6d61 6c5f 2c20  xavier_normal_, 
-0001e640: 6b61 696d 696e 675f 756e 6966 6f72 6d5f  kaiming_uniform_
-0001e650: 2c20 6b61 696d 696e 675f 6e6f 726d 616c  , kaiming_normal
-0001e660: 5f2c 2074 7275 6e63 5f6e 6f72 6d61 6c5f  _, trunc_normal_
-0001e670: 7d0a 2020 2020 6163 7469 7661 7469 6f6e  }.    activation
-0001e680: 3a20 7374 722c 206f 7074 696f 6e61 6c0a  : str, optional.
-0001e690: 2020 2020 2020 2020 4163 7469 7661 7469          Activati
-0001e6a0: 6f6e 2066 756e 6374 696f 6e20 6170 706c  on function appl
-0001e6b0: 6965 640a 0a20 2020 2045 7861 6d70 6c65  ied..    Example
-0001e6c0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-0001e6d0: 2020 203e 3e3e 2066 726f 6d20 6465 6570     >>> from deep
-0001e6e0: 6368 656d 2e6d 6f64 656c 732e 746f 7263  chem.models.torc
-0001e6f0: 685f 6d6f 6465 6c73 2069 6d70 6f72 7420  h_models import 
-0001e700: 6c61 7965 7273 0a20 2020 203e 3e3e 2069  layers.    >>> i
-0001e710: 6d70 6f72 7420 746f 7263 680a 2020 2020  mport torch.    
-0001e720: 3e3e 3e20 656d 6265 6464 696e 675f 6c61  >>> embedding_la
-0001e730: 7965 7220 3d20 6c61 7965 7273 2e44 544e  yer = layers.DTN
-0001e740: 4e45 6d62 6564 6469 6e67 2834 2c20 3429  NEmbedding(4, 4)
-0001e750: 0a20 2020 203e 3e3e 2065 6d62 203d 2065  .    >>> emb = e
-0001e760: 6d62 6564 6469 6e67 5f6c 6179 6572 2874  mbedding_layer(t
-0001e770: 6f72 6368 2e54 656e 736f 7228 5b30 2c31  orch.Tensor([0,1
-0001e780: 2c32 2c33 5d29 2e74 6f28 746f 7263 682e  ,2,3]).to(torch.
-0001e790: 696e 7436 3429 290a 2020 2020 3e3e 3e20  int64)).    >>> 
-0001e7a0: 7374 6570 5f6c 6179 6572 203d 206c 6179  step_layer = lay
-0001e7b0: 6572 732e 4454 4e4e 5374 6570 2834 2c20  ers.DTNNStep(4, 
-0001e7c0: 362c 2038 290a 2020 2020 3e3e 3e20 6f75  6, 8).    >>> ou
-0001e7d0: 7470 7574 5f74 6f72 6368 203d 2073 7465  tput_torch = ste
-0001e7e0: 705f 6c61 7965 7228 5b0a 2020 2020 2e2e  p_layer([.    ..
-0001e7f0: 2e20 2020 2020 746f 7263 682e 5465 6e73  .     torch.Tens
-0001e800: 6f72 2865 6d62 292c 0a20 2020 202e 2e2e  or(emb),.    ...
-0001e810: 2020 2020 2074 6f72 6368 2e54 656e 736f       torch.Tenso
-0001e820: 7228 5b30 2c20 312c 2032 2c20 332c 2034  r([0, 1, 2, 3, 4
-0001e830: 2c20 355d 292e 746f 2874 6f72 6368 2e66  , 5]).to(torch.f
-0001e840: 6c6f 6174 3332 292c 0a20 2020 202e 2e2e  loat32),.    ...
-0001e850: 2020 2020 2074 6f72 6368 2e54 656e 736f       torch.Tenso
-0001e860: 7228 5b31 5d29 2e74 6f28 746f 7263 682e  r([1]).to(torch.
-0001e870: 696e 7436 3429 2c0a 2020 2020 2e2e 2e20  int64),.    ... 
-0001e880: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
-0001e890: 285b 5b31 5d5d 292e 746f 2874 6f72 6368  ([[1]]).to(torch
-0001e8a0: 2e69 6e74 3634 290a 2020 2020 2e2e 2e20  .int64).    ... 
-0001e8b0: 5d29 0a20 2020 203e 3e3e 206f 7574 7075  ]).    >>> outpu
-0001e8c0: 745f 746f 7263 682e 7368 6170 650a 2020  t_torch.shape.  
-0001e8d0: 2020 746f 7263 682e 5369 7a65 285b 322c    torch.Size([2,
-0001e8e0: 2034 2c20 345d 290a 0a20 2020 2022 2222   4, 4])..    """
-0001e8f0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0001e900: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
-0001e910: 2020 2020 2020 2020 2020 6e5f 656d 6265            n_embe
-0001e920: 6464 696e 673a 2069 6e74 203d 2033 302c  dding: int = 30,
-0001e930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e940: 2020 6e5f 6469 7374 616e 6365 3a20 696e    n_distance: in
-0001e950: 7420 3d20 3130 302c 0a20 2020 2020 2020  t = 100,.       
-0001e960: 2020 2020 2020 2020 2020 6e5f 6869 6464            n_hidd
-0001e970: 656e 3a20 696e 7420 3d20 3630 2c0a 2020  en: int = 60,.  
-0001e980: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e990: 6e69 7469 616c 697a 6572 3a20 7374 7220  nitializer: str 
-0001e9a0: 3d20 2778 6176 6965 725f 756e 6966 6f72  = 'xavier_unifor
-0001e9b0: 6d5f 272c 0a20 2020 2020 2020 2020 2020  m_',.           
-0001e9c0: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
-0001e9d0: 3d27 7461 6e68 272c 0a20 2020 2020 2020  ='tanh',.       
-0001e9e0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0001e9f0: 6773 293a 0a0a 2020 2020 2020 2020 7375  gs):..        su
-0001ea00: 7065 7228 4454 4e4e 5374 6570 2c20 7365  per(DTNNStep, se
-0001ea10: 6c66 292e 5f5f 696e 6974 5f5f 282a 2a6b  lf).__init__(**k
-0001ea20: 7761 7267 7329 0a20 2020 2020 2020 2073  wargs).        s
-0001ea30: 656c 662e 6e5f 656d 6265 6464 696e 6720  elf.n_embedding 
-0001ea40: 3d20 6e5f 656d 6265 6464 696e 670a 2020  = n_embedding.  
-0001ea50: 2020 2020 2020 7365 6c66 2e6e 5f64 6973        self.n_dis
-0001ea60: 7461 6e63 6520 3d20 6e5f 6469 7374 616e  tance = n_distan
-0001ea70: 6365 0a20 2020 2020 2020 2073 656c 662e  ce.        self.
-0001ea80: 6e5f 6869 6464 656e 203d 206e 5f68 6964  n_hidden = n_hid
-0001ea90: 6465 6e0a 2020 2020 2020 2020 7365 6c66  den.        self
-0001eaa0: 2e69 6e69 7469 616c 697a 6572 203d 2069  .initializer = i
-0001eab0: 6e69 7469 616c 697a 6572 2020 2320 5365  nitializer  # Se
-0001eac0: 7420 7765 6967 6874 2069 6e69 7469 616c  t weight initial
-0001ead0: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
-0001eae0: 7365 6c66 2e61 6374 6976 6174 696f 6e20  self.activation 
-0001eaf0: 3d20 6163 7469 7661 7469 6f6e 2020 2320  = activation  # 
-0001eb00: 4765 7420 6163 7469 7661 7469 6f6e 730a  Get activations.
-0001eb10: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-0001eb20: 6976 6174 696f 6e5f 666e 203d 2067 6574  ivation_fn = get
-0001eb30: 5f61 6374 6976 6174 696f 6e28 7365 6c66  _activation(self
-0001eb40: 2e61 6374 6976 6174 696f 6e29 0a0a 2020  .activation)..  
-0001eb50: 2020 2020 2020 696e 6974 5f66 756e 633a        init_func:
-0001eb60: 2043 616c 6c61 626c 6520 3d20 6765 7461   Callable = geta
-0001eb70: 7474 7228 696e 6974 6961 6c69 7a65 7273  ttr(initializers
-0001eb80: 2c20 7365 6c66 2e69 6e69 7469 616c 697a  , self.initializ
-0001eb90: 6572 290a 0a20 2020 2020 2020 2073 656c  er)..        sel
-0001eba0: 662e 575f 6366 203d 2069 6e69 745f 6675  f.W_cf = init_fu
-0001ebb0: 6e63 2874 6f72 6368 2e65 6d70 7479 285b  nc(torch.empty([
-0001ebc0: 7365 6c66 2e6e 5f65 6d62 6564 6469 6e67  self.n_embedding
-0001ebd0: 2c20 7365 6c66 2e6e 5f68 6964 6465 6e5d  , self.n_hidden]
-0001ebe0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001ebf0: 575f 6466 203d 2069 6e69 745f 6675 6e63  W_df = init_func
-0001ec00: 2874 6f72 6368 2e65 6d70 7479 285b 7365  (torch.empty([se
-0001ec10: 6c66 2e6e 5f64 6973 7461 6e63 652c 2073  lf.n_distance, s
-0001ec20: 656c 662e 6e5f 6869 6464 656e 5d29 290a  elf.n_hidden])).
-0001ec30: 2020 2020 2020 2020 7365 6c66 2e57 5f66          self.W_f
-0001ec40: 6320 3d20 696e 6974 5f66 756e 6328 746f  c = init_func(to
-0001ec50: 7263 682e 656d 7074 7928 5b73 656c 662e  rch.empty([self.
-0001ec60: 6e5f 6869 6464 656e 2c20 7365 6c66 2e6e  n_hidden, self.n
-0001ec70: 5f65 6d62 6564 6469 6e67 5d29 290a 2020  _embedding])).  
-0001ec80: 2020 2020 2020 7365 6c66 2e62 5f63 6620        self.b_cf 
-0001ec90: 3d20 746f 7263 682e 7a65 726f 7328 7369  = torch.zeros(si
-0001eca0: 7a65 3d5b 0a20 2020 2020 2020 2020 2020  ze=[.           
-0001ecb0: 2073 656c 662e 6e5f 6869 6464 656e 2c0a   self.n_hidden,.
-0001ecc0: 2020 2020 2020 2020 5d29 0a20 2020 2020          ]).     
-0001ecd0: 2020 2073 656c 662e 625f 6466 203d 2074     self.b_df = t
-0001ece0: 6f72 6368 2e7a 6572 6f73 2873 697a 653d  orch.zeros(size=
-0001ecf0: 5b0a 2020 2020 2020 2020 2020 2020 7365  [.            se
-0001ed00: 6c66 2e6e 5f68 6964 6465 6e2c 0a20 2020  lf.n_hidden,.   
-0001ed10: 2020 2020 205d 290a 0a20 2020 2064 6566       ])..    def
-0001ed20: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-0001ed30: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0001ed40: 726e 7320 6120 7374 7269 6e67 2072 6570  rns a string rep
-0001ed50: 7265 7365 6e74 696e 6720 7468 6520 636f  resenting the co
-0001ed60: 6e66 6967 7572 6174 696f 6e20 6f66 2074  nfiguration of t
-0001ed70: 6865 206c 6179 6572 2e0a 0a20 2020 2020  he layer...     
-0001ed80: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0001ed90: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0001eda0: 2020 206e 5f65 6d62 6564 6469 6e67 3a20     n_embedding: 
-0001edb0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0001edc0: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
-0001edd0: 206f 6620 6665 6174 7572 6573 2066 6f72   of features for
-0001ede0: 2065 6163 6820 6174 6f6d 0a20 2020 2020   each atom.     
-0001edf0: 2020 206e 5f64 6973 7461 6e63 653a 2069     n_distance: i
-0001ee00: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-0001ee10: 2020 2020 2020 2020 2067 7261 6e75 6c61           granula
-0001ee20: 7269 7479 206f 6620 6469 7374 616e 6365  rity of distance
-0001ee30: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-0001ee40: 6e5f 6869 6464 656e 3a20 696e 742c 206f  n_hidden: int, o
-0001ee50: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0001ee60: 2020 2020 4e75 6d62 6572 206f 6620 6e6f      Number of no
-0001ee70: 6465 7320 696e 2068 6964 6465 6e20 6c61  des in hidden la
-0001ee80: 7965 720a 2020 2020 2020 2020 696e 6974  yer.        init
-0001ee90: 6961 6c69 7a65 723a 2073 7472 2c20 6f70  ializer: str, op
-0001eea0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0001eeb0: 2020 2057 6569 6768 7420 696e 6974 6961     Weight initia
-0001eec0: 6c69 7a61 7469 6f6e 2066 6f72 2066 696c  lization for fil
-0001eed0: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
-0001eee0: 2020 4f70 7469 6f6e 733a 207b 7861 7669    Options: {xavi
-0001eef0: 6572 5f75 6e69 666f 726d 5f2c 2078 6176  er_uniform_, xav
-0001ef00: 6965 725f 6e6f 726d 616c 5f2c 206b 6169  ier_normal_, kai
-0001ef10: 6d69 6e67 5f75 6e69 666f 726d 5f2c 206b  ming_uniform_, k
-0001ef20: 6169 6d69 6e67 5f6e 6f72 6d61 6c5f 2c20  aiming_normal_, 
-0001ef30: 7472 756e 635f 6e6f 726d 616c 5f7d 0a20  trunc_normal_}. 
-0001ef40: 2020 2020 2020 2061 6374 6976 6174 696f         activatio
-0001ef50: 6e3a 2073 7472 2c20 6f70 7469 6f6e 616c  n: str, optional
-0001ef60: 0a20 2020 2020 2020 2020 2020 2041 6374  .            Act
-0001ef70: 6976 6174 696f 6e20 6675 6e63 7469 6f6e  ivation function
-0001ef80: 2061 7070 6c69 6564 0a0a 2020 2020 2020   applied..      
-0001ef90: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0001efa0: 7475 726e 2066 277b 7365 6c66 2e5f 5f63  turn f'{self.__c
-0001efb0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
-0001efc0: 286e 5f65 6d62 6564 6469 6e67 3d7b 7365  (n_embedding={se
-0001efd0: 6c66 2e6e 5f65 6d62 6564 6469 6e67 7d2c  lf.n_embedding},
-0001efe0: 206e 5f64 6973 7461 6e63 653d 7b73 656c   n_distance={sel
-0001eff0: 662e 6e5f 6469 7374 616e 6365 7d2c 206e  f.n_distance}, n
-0001f000: 5f68 6964 6465 6e3d 7b73 656c 662e 6e5f  _hidden={self.n_
-0001f010: 6869 6464 656e 7d2c 2069 6e69 7469 616c  hidden}, initial
-0001f020: 697a 6572 3d7b 7365 6c66 2e69 6e69 7469  izer={self.initi
-0001f030: 616c 697a 6572 7d2c 2061 6374 6976 6174  alizer}, activat
-0001f040: 696f 6e3d 7b73 656c 662e 6163 7469 7661  ion={self.activa
-0001f050: 7469 6f6e 7d29 270a 0a20 2020 2064 6566  tion})'..    def
-0001f060: 2066 6f72 7761 7264 2873 656c 662c 2069   forward(self, i
-0001f070: 6e70 7574 7329 3a0a 2020 2020 2020 2020  nputs):.        
-0001f080: 2222 2245 7865 6375 7465 7320 7468 6520  """Executes the 
-0001f090: 6571 7561 7469 6f6e 7320 616e 6420 5265  equations and Re
-0001f0a0: 7475 726e 7320 7468 6520 696e 7472 6163  turns the intrac
-0001f0b0: 7469 6f6e 2076 6563 746f 7220 6f66 2074  tion vector of t
-0001f0c0: 6865 2061 746f 6d20 7769 7468 206f 7468  he atom with oth
-0001f0d0: 6572 2061 746f 6d73 2e0a 0a20 2020 2020  er atoms...     
-0001f0e0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001f0f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0001f100: 0a20 2020 2020 2020 2069 6e70 7574 733a  .        inputs:
-0001f110: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
-0001f120: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
-0001f130: 6620 5465 6e73 6f72 7320 6861 7669 6e67  f Tensors having
-0001f140: 2061 746f 6d5f 6665 6174 7572 6573 2c20   atom_features, 
-0001f150: 6469 7374 616e 6365 2c20 6469 7374 616e  distance, distan
-0001f160: 6365 5f6d 656d 6265 7273 6869 705f 692c  ce_membership_i,
-0001f170: 2064 6973 7461 6e63 655f 6d65 6d62 6572   distance_member
-0001f180: 7368 6970 5f6a 2e0a 0a20 2020 2020 2020  ship_j...       
-0001f190: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0001f1a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0001f1b0: 2069 6e74 6572 6163 7469 6f6e 5f76 6563   interaction_vec
-0001f1c0: 746f 723a 2074 6f72 6368 2e54 656e 736f  tor: torch.Tenso
-0001f1d0: 720a 2020 2020 2020 2020 2020 2020 696e  r.            in
-0001f1e0: 7465 7261 6374 696f 6e20 6f66 2074 6865  teraction of the
-0001f1f0: 2061 746f 6d20 7769 7468 206f 7468 6572   atom with other
-0001f200: 2061 746f 6d73 2062 6173 6564 206f 6e20   atoms based on 
-0001f210: 6469 7374 616e 6365 2061 6e64 2064 6973  distance and dis
-0001f220: 7461 6e63 655f 6d65 6d62 6572 7368 6970  tance_membership
-0001f230: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-0001f240: 2020 2020 2020 2061 746f 6d5f 6665 6174         atom_feat
-0001f250: 7572 6573 203d 2069 6e70 7574 735b 305d  ures = inputs[0]
-0001f260: 0a20 2020 2020 2020 2064 6973 7461 6e63  .        distanc
-0001f270: 6520 3d20 696e 7075 7473 5b31 5d0a 2020  e = inputs[1].  
-0001f280: 2020 2020 2020 6469 7374 616e 6365 5f6d        distance_m
-0001f290: 656d 6265 7273 6869 705f 6920 3d20 696e  embership_i = in
-0001f2a0: 7075 7473 5b32 5d0a 2020 2020 2020 2020  puts[2].        
-0001f2b0: 6469 7374 616e 6365 5f6d 656d 6265 7273  distance_members
-0001f2c0: 6869 705f 6a20 3d20 696e 7075 7473 5b33  hip_j = inputs[3
-0001f2d0: 5d0a 2020 2020 2020 2020 6469 7374 616e  ].        distan
-0001f2e0: 6365 5f68 6964 6465 6e20 3d20 746f 7263  ce_hidden = torc
-0001f2f0: 682e 6d61 746d 756c 2864 6973 7461 6e63  h.matmul(distanc
-0001f300: 652c 2073 656c 662e 575f 6466 2920 2b20  e, self.W_df) + 
-0001f310: 7365 6c66 2e62 5f64 660a 2020 2020 2020  self.b_df.      
-0001f320: 2020 6174 6f6d 5f66 6561 7475 7265 735f    atom_features_
-0001f330: 6869 6464 656e 203d 2074 6f72 6368 2e6d  hidden = torch.m
-0001f340: 6174 6d75 6c28 6174 6f6d 5f66 6561 7475  atmul(atom_featu
-0001f350: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
-0001f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f380: 2073 656c 662e 575f 6366 2920 2b20 7365   self.W_cf) + se
-0001f390: 6c66 2e62 5f63 660a 2020 2020 2020 2020  lf.b_cf.        
-0001f3a0: 6f75 7470 7574 7320 3d20 746f 7263 682e  outputs = torch.
-0001f3b0: 6d75 6c28 0a20 2020 2020 2020 2020 2020  mul(.           
-0001f3c0: 2064 6973 7461 6e63 655f 6869 6464 656e   distance_hidden
-0001f3d0: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-0001f3e0: 7263 682e 656d 6265 6464 696e 6728 6174  rch.embedding(at
-0001f3f0: 6f6d 5f66 6561 7475 7265 735f 6869 6464  om_features_hidd
-0001f400: 656e 2c20 6469 7374 616e 6365 5f6d 656d  en, distance_mem
-0001f410: 6265 7273 6869 705f 6a29 290a 0a20 2020  bership_j))..   
-0001f420: 2020 2020 2023 2066 6f72 2061 746f 6d20       # for atom 
-0001f430: 6920 696e 2061 206d 6f6c 6563 756c 6520  i in a molecule 
-0001f440: 6d2c 2074 6869 7320 7374 6570 206d 756c  m, this step mul
-0001f450: 7469 706c 6965 7320 746f 6765 7468 6572  tiplies together
-0001f460: 2064 6973 7461 6e63 6520 696e 666f 206f   distance info o
-0001f470: 6620 6174 6f6d 2070 6169 7228 692c 6a29  f atom pair(i,j)
-0001f480: 0a20 2020 2020 2020 2023 2061 6e64 2065  .        # and e
-0001f490: 6d62 6564 6469 6e67 7320 6f66 2061 746f  mbeddings of ato
-0001f4a0: 6d20 6a28 626f 7468 2067 6f6e 6520 7468  m j(both gone th
-0001f4b0: 726f 7567 6820 6120 6869 6464 656e 206c  rough a hidden l
-0001f4c0: 6179 6572 290a 2020 2020 2020 2020 6f75  ayer).        ou
-0001f4d0: 7470 7574 7320 3d20 746f 7263 682e 6d61  tputs = torch.ma
-0001f4e0: 746d 756c 286f 7574 7075 7473 2c20 7365  tmul(outputs, se
-0001f4f0: 6c66 2e57 5f66 6329 0a20 2020 2020 2020  lf.W_fc).       
-0001f500: 206f 7574 7075 7473 203d 2073 656c 662e   outputs = self.
-0001f510: 6163 7469 7661 7469 6f6e 5f66 6e28 6f75  activation_fn(ou
-0001f520: 7470 7574 7329 0a0a 2020 2020 2020 2020  tputs)..        
-0001f530: 6f75 7470 7574 5f69 6920 3d20 746f 7263  output_ii = torc
-0001f540: 682e 6d75 6c28 7365 6c66 2e62 5f64 662c  h.mul(self.b_df,
-0001f550: 2061 746f 6d5f 6665 6174 7572 6573 5f68   atom_features_h
-0001f560: 6964 6465 6e29 0a20 2020 2020 2020 206f  idden).        o
-0001f570: 7574 7075 745f 6969 203d 2074 6f72 6368  utput_ii = torch
-0001f580: 2e6d 6174 6d75 6c28 6f75 7470 7574 5f69  .matmul(output_i
-0001f590: 692c 2073 656c 662e 575f 6663 290a 2020  i, self.W_fc).  
-0001f5a0: 2020 2020 2020 6f75 7470 7574 5f69 6920        output_ii 
-0001f5b0: 3d20 7365 6c66 2e61 6374 6976 6174 696f  = self.activatio
-0001f5c0: 6e5f 666e 286f 7574 7075 745f 6969 290a  n_fn(output_ii).
-0001f5d0: 0a20 2020 2020 2020 2023 2066 6f72 2061  .        # for a
-0001f5e0: 746f 6d20 692c 2073 756d 2074 6865 2069  tom i, sum the i
-0001f5f0: 6e66 6c75 656e 6365 2066 726f 6d20 616c  nfluence from al
-0001f600: 6c20 6f74 6865 7220 6174 6f6d 206a 2069  l other atom j i
-0001f610: 6e20 7468 6520 6d6f 6c65 6375 6c65 0a20  n the molecule. 
-0001f620: 2020 2020 2020 2069 6e74 7261 6374 696f         intractio
-0001f630: 6e5f 7665 6374 6f72 203d 2073 6361 7474  n_vector = scatt
-0001f640: 6572 286f 7574 7075 7473 2c20 6469 7374  er(outputs, dist
-0001f650: 616e 6365 5f6d 656d 6265 7273 6869 705f  ance_membership_
-0001f660: 692c 0a20 2020 2020 2020 2020 2020 2020  i,.             
-0001f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f680: 2020 2020 2020 2064 696d 3d30 2920 2d20         dim=0) - 
-0001f690: 6f75 7470 7574 5f69 6920 2b20 6174 6f6d  output_ii + atom
-0001f6a0: 5f66 6561 7475 7265 730a 2020 2020 2020  _features.      
-0001f6b0: 2020 7265 7475 726e 2069 6e74 7261 6374    return intract
-0001f6c0: 696f 6e5f 7665 6374 6f72 0a0a 0a63 6c61  ion_vector...cla
-0001f6d0: 7373 2045 6467 654e 6574 776f 726b 286e  ss EdgeNetwork(n
-0001f6e0: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2022  n.Module):.    "
-0001f6f0: 2222 5468 6520 4564 6765 4e65 7477 6f72  ""The EdgeNetwor
-0001f700: 6b20 6d6f 6475 6c65 2069 7320 6120 5079  k module is a Py
-0001f710: 546f 7263 6820 7375 626d 6f64 756c 6520  Torch submodule 
-0001f720: 6465 7369 676e 6564 2066 6f72 206d 6573  designed for mes
-0001f730: 7361 6765 2070 6173 7369 6e67 2069 6e20  sage passing in 
-0001f740: 6772 6170 6820 6e65 7572 616c 206e 6574  graph neural net
-0001f750: 776f 726b 732e 0a0a 2020 2020 4578 616d  works...    Exam
-0001f760: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-0001f770: 2d0a 2020 2020 3e3e 3e20 7061 6972 5f66  -.    >>> pair_f
-0001f780: 6561 7475 7265 7320 3d20 746f 7263 682e  eatures = torch.
-0001f790: 7261 6e64 2828 342c 2032 292c 2064 7479  rand((4, 2), dty
-0001f7a0: 7065 3d74 6f72 6368 2e66 6c6f 6174 3332  pe=torch.float32
-0001f7b0: 290a 2020 2020 3e3e 3e20 6174 6f6d 5f66  ).    >>> atom_f
-0001f7c0: 6561 7475 7265 7320 3d20 746f 7263 682e  eatures = torch.
-0001f7d0: 7261 6e64 2828 352c 2032 292c 2064 7479  rand((5, 2), dty
-0001f7e0: 7065 3d74 6f72 6368 2e66 6c6f 6174 3332  pe=torch.float32
-0001f7f0: 290a 2020 2020 3e3e 3e20 6174 6f6d 5f74  ).    >>> atom_t
-0001f800: 6f5f 7061 6972 203d 205b 5d0a 2020 2020  o_pair = [].    
-0001f810: 3e3e 3e20 6e5f 6174 6f6d 7320 3d20 320a  >>> n_atoms = 2.
-0001f820: 2020 2020 3e3e 3e20 7374 6172 7420 3d20      >>> start = 
-0001f830: 300a 2020 2020 3e3e 3e20 4330 2c20 4331  0.    >>> C0, C1
-0001f840: 203d 206e 702e 6d65 7368 6772 6964 286e   = np.meshgrid(n
-0001f850: 702e 6172 616e 6765 286e 5f61 746f 6d73  p.arange(n_atoms
-0001f860: 292c 206e 702e 6172 616e 6765 286e 5f61  ), np.arange(n_a
-0001f870: 746f 6d73 2929 0a20 2020 203e 3e3e 2061  toms)).    >>> a
-0001f880: 746f 6d5f 746f 5f70 6169 722e 6170 7065  tom_to_pair.appe
-0001f890: 6e64 286e 702e 7472 616e 7370 6f73 6528  nd(np.transpose(
-0001f8a0: 6e70 2e61 7272 6179 285b 4331 2e66 6c61  np.array([C1.fla
-0001f8b0: 7474 656e 2829 202b 2073 7461 7274 2c20  tten() + start, 
-0001f8c0: 4330 2e66 6c61 7474 656e 2829 202b 2073  C0.flatten() + s
-0001f8d0: 7461 7274 5d29 2929 0a20 2020 203e 3e3e  tart]))).    >>>
-0001f8e0: 2061 746f 6d5f 746f 5f70 6169 7220 3d20   atom_to_pair = 
-0001f8f0: 746f 7263 682e 5465 6e73 6f72 2861 746f  torch.Tensor(ato
-0001f900: 6d5f 746f 5f70 6169 7229 0a20 2020 203e  m_to_pair).    >
-0001f910: 3e3e 2061 746f 6d5f 746f 5f70 6169 7220  >> atom_to_pair 
-0001f920: 3d20 746f 7263 682e 7371 7565 657a 6528  = torch.squeeze(
-0001f930: 6174 6f6d 5f74 6f5f 7061 6972 2e74 6f28  atom_to_pair.to(
-0001f940: 746f 7263 682e 696e 7436 3429 2c20 6469  torch.int64), di
-0001f950: 6d3d 3029 0a20 2020 203e 3e3e 2069 6e70  m=0).    >>> inp
-0001f960: 7574 7320 3d20 5b70 6169 725f 6665 6174  uts = [pair_feat
-0001f970: 7572 6573 2c20 6174 6f6d 5f66 6561 7475  ures, atom_featu
-0001f980: 7265 732c 2061 746f 6d5f 746f 5f70 6169  res, atom_to_pai
-0001f990: 725d 0a20 2020 203e 3e3e 206e 5f70 6169  r].    >>> n_pai
-0001f9a0: 725f 6665 6174 7572 6573 203d 2032 0a20  r_features = 2. 
-0001f9b0: 2020 203e 3e3e 206e 5f68 6964 6465 6e20     >>> n_hidden 
-0001f9c0: 3d20 320a 2020 2020 3e3e 3e20 696e 6974  = 2.    >>> init
-0001f9d0: 203d 2027 7861 7669 6572 5f75 6e69 666f   = 'xavier_unifo
-0001f9e0: 726d 5f27 0a20 2020 203e 3e3e 206c 6179  rm_'.    >>> lay
-0001f9f0: 6572 203d 2045 6467 654e 6574 776f 726b  er = EdgeNetwork
-0001fa00: 286e 5f70 6169 725f 6665 6174 7572 6573  (n_pair_features
-0001fa10: 2c20 6e5f 6869 6464 656e 2c20 696e 6974  , n_hidden, init
-0001fa20: 290a 2020 2020 3e3e 3e20 7265 7375 6c74  ).    >>> result
-0001fa30: 203d 206c 6179 6572 2869 6e70 7574 7329   = layer(inputs)
-0001fa40: 0a20 2020 203e 3e3e 2072 6573 756c 742e  .    >>> result.
-0001fa50: 7368 6170 655b 315d 0a20 2020 2032 0a20  shape[1].    2. 
-0001fa60: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
-0001fa70: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
-0001fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa90: 6e5f 7061 6972 5f66 6561 7475 7265 733a  n_pair_features:
-0001faa0: 2069 6e74 203d 2038 2c0a 2020 2020 2020   int = 8,.      
-0001fab0: 2020 2020 2020 2020 2020 206e 5f68 6964             n_hid
-0001fac0: 6465 6e3a 2069 6e74 203d 2031 3030 2c0a  den: int = 100,.
-0001fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fae0: 2069 6e69 743a 2073 7472 203d 2027 7861   init: str = 'xa
-0001faf0: 7669 6572 5f75 6e69 666f 726d 5f27 2c0a  vier_uniform_',.
-0001fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb10: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-0001fb20: 2020 2020 2222 2249 6e69 7461 6c69 7365      """Initalise
-0001fb30: 7320 6120 4564 6765 4e65 7477 6f72 6b20  s a EdgeNetwork 
-0001fb40: 4c61 7965 720a 0a20 2020 2020 2020 2050  Layer..        P
-0001fb50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0001fb60: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001fb70: 2020 2020 206e 5f70 6169 725f 6665 6174       n_pair_feat
-0001fb80: 7572 6573 3a20 696e 742c 206f 7074 696f  ures: int, optio
-0001fb90: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0001fba0: 5468 6520 6c65 6e67 7468 206f 6620 7468  The length of th
-0001fbb0: 6520 7061 6972 2066 6561 7475 7265 7320  e pair features 
-0001fbc0: 7665 6374 6f72 2e0a 2020 2020 2020 2020  vector..        
-0001fbd0: 6e5f 6869 6464 656e 3a20 696e 742c 206f  n_hidden: int, o
-0001fbe0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0001fbf0: 2020 2020 6e75 6d62 6572 206f 6620 6869      number of hi
-0001fc00: 6464 656e 2075 6e69 7473 2069 6e20 7468  dden units in th
-0001fc10: 6520 7061 7373 696e 6720 7068 6173 650a  e passing phase.
-0001fc20: 2020 2020 2020 2020 696e 6974 3a20 7374          init: st
-0001fc30: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
-0001fc40: 2020 2020 2020 2020 496e 6974 6961 6c69          Initiali
-0001fc50: 7a61 7469 6f6e 2066 756e 6374 696f 6e20  zation function 
-0001fc60: 746f 2062 6520 7573 6564 2069 6e20 7468  to be used in th
-0001fc70: 6520 6d65 7373 6167 6520 7061 7373 696e  e message passin
-0001fc80: 6720 6c61 7965 722e 0a20 2020 2020 2020  g layer..       
-0001fc90: 2022 2222 0a0a 2020 2020 2020 2020 7375   """..        su
-0001fca0: 7065 7228 4564 6765 4e65 7477 6f72 6b2c  per(EdgeNetwork,
-0001fcb0: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-0001fcc0: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0001fcd0: 2020 7365 6c66 2e6e 5f70 6169 725f 6665    self.n_pair_fe
-0001fce0: 6174 7572 6573 3a20 696e 7420 3d20 6e5f  atures: int = n_
-0001fcf0: 7061 6972 5f66 6561 7475 7265 730a 2020  pair_features.  
-0001fd00: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
-0001fd10: 6465 6e3a 2069 6e74 203d 206e 5f68 6964  den: int = n_hid
-0001fd20: 6465 6e0a 2020 2020 2020 2020 7365 6c66  den.        self
-0001fd30: 2e69 6e69 743a 2073 7472 203d 2069 6e69  .init: str = ini
-0001fd40: 740a 0a20 2020 2020 2020 2069 6e69 745f  t..        init_
-0001fd50: 6675 6e63 3a20 4361 6c6c 6162 6c65 203d  func: Callable =
-0001fd60: 2067 6574 6174 7472 2869 6e69 7469 616c   getattr(initial
-0001fd70: 697a 6572 732c 2073 656c 662e 696e 6974  izers, self.init
-0001fd80: 290a 2020 2020 2020 2020 7365 6c66 2e57  ).        self.W
-0001fd90: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-0001fda0: 2069 6e69 745f 6675 6e63 280a 2020 2020   init_func(.    
-0001fdb0: 2020 2020 2020 2020 746f 7263 682e 656d          torch.em
-0001fdc0: 7074 7928 5b73 656c 662e 6e5f 7061 6972  pty([self.n_pair
-0001fdd0: 5f66 6561 7475 7265 732c 2073 656c 662e  _features, self.
-0001fde0: 6e5f 6869 6464 656e 202a 2073 656c 662e  n_hidden * self.
-0001fdf0: 6e5f 6869 6464 656e 5d29 290a 2020 2020  n_hidden])).    
-0001fe00: 2020 2020 7365 6c66 2e62 3a20 746f 7263      self.b: torc
-0001fe10: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-0001fe20: 2e7a 6572 6f73 2828 7365 6c66 2e6e 5f68  .zeros((self.n_h
-0001fe30: 6964 6465 6e20 2a20 7365 6c66 2e6e 5f68  idden * self.n_h
-0001fe40: 6964 6465 6e2c 2929 0a20 2020 2020 2020  idden,)).       
-0001fe50: 2073 656c 662e 6275 696c 743a 2062 6f6f   self.built: boo
-0001fe60: 6c20 3d20 5472 7565 0a0a 2020 2020 6465  l = True..    de
-0001fe70: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-0001fe80: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-0001fe90: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-0001fea0: 2020 2020 2020 6627 7b73 656c 662e 5f5f        f'{self.__
-0001feb0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-0001fec0: 7d28 6e5f 7061 6972 5f66 6561 7475 7265  }(n_pair_feature
-0001fed0: 733a 7b73 656c 662e 6e5f 7061 6972 5f66  s:{self.n_pair_f
-0001fee0: 6561 7475 7265 737d 2c6e 5f68 6964 6465  eatures},n_hidde
-0001fef0: 6e3a 7b73 656c 662e 6e5f 6869 6464 656e  n:{self.n_hidden
-0001ff00: 7d2c 696e 6974 3a7b 7365 6c66 2e69 6e69  },init:{self.ini
-0001ff10: 747d 2927 0a20 2020 2020 2020 2029 0a0a  t})'.        )..
-0001ff20: 2020 2020 6465 6620 666f 7277 6172 6428      def forward(
-0001ff30: 7365 6c66 2c20 696e 7075 7473 3a20 4c69  self, inputs: Li
-0001ff40: 7374 5b74 6f72 6368 2e54 656e 736f 725d  st[torch.Tensor]
-0001ff50: 2920 2d3e 2074 6f72 6368 2e54 656e 736f  ) -> torch.Tenso
-0001ff60: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
-0001ff70: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0001ff80: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0001ff90: 2d2d 2d2d 0a20 2020 2020 2020 2069 6e70  ----.        inp
-0001ffa0: 7574 733a 204c 6973 745b 746f 7263 682e  uts: List[torch.
-0001ffb0: 5465 6e73 6f72 5d0a 2020 2020 2020 2020  Tensor].        
-0001ffc0: 2020 2020 5468 6520 6c65 6e67 7468 206f      The length o
-0001ffd0: 6620 6174 6f6d 5f74 6f5f 7061 6972 2073  f atom_to_pair s
-0001ffe0: 686f 756c 6420 6265 2073 616d 6520 6173  hould be same as
-0001fff0: 206e 5f70 6169 725f 6665 6174 7572 6573   n_pair_features
-00020000: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00020010: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00020020: 2d0a 2020 2020 2020 2020 7265 7375 6c74  -.        result
-00020030: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
-00020040: 2020 2020 2020 2020 2020 2054 656e 736f             Tenso
-00020050: 7220 636f 6e74 6169 6e69 6e67 2074 6865  r containing the
-00020060: 206d 6170 7069 6e67 206f 6620 7468 6520   mapping of the 
-00020070: 6564 6765 2076 6563 746f 7220 746f 2061  edge vector to a
-00020080: 2064 20c3 9720 6420 6d61 7472 6978 2c20   d .. d matrix, 
-00020090: 7768 6572 6520 6420 6465 6e6f 7465 7320  where d denotes 
-000200a0: 7468 6520 6469 6d65 6e73 696f 6e20 6f66  the dimension of
-000200b0: 2074 6865 2069 6e74 6572 6e61 6c20 6869   the internal hi
-000200c0: 6464 656e 2072 6570 7265 7365 6e74 6174  dden representat
-000200d0: 696f 6e20 6f66 2065 6163 6820 6e6f 6465  ion of each node
-000200e0: 2069 6e20 7468 6520 6772 6170 682e 0a20   in the graph.. 
-000200f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00020100: 2020 2070 6169 725f 6665 6174 7572 6573     pair_features
-00020110: 3a20 746f 7263 682e 5465 6e73 6f72 0a20  : torch.Tensor. 
-00020120: 2020 2020 2020 2061 746f 6d5f 6665 6174         atom_feat
-00020130: 7572 6573 3a20 746f 7263 682e 5465 6e73  ures: torch.Tens
-00020140: 6f72 0a20 2020 2020 2020 2061 746f 6d5f  or.        atom_
-00020150: 746f 5f70 6169 723a 2074 6f72 6368 2e54  to_pair: torch.T
-00020160: 656e 736f 720a 2020 2020 2020 2020 7061  ensor.        pa
-00020170: 6972 5f66 6561 7475 7265 732c 2061 746f  ir_features, ato
-00020180: 6d5f 6665 6174 7572 6573 2c20 6174 6f6d  m_features, atom
-00020190: 5f74 6f5f 7061 6972 203d 2069 6e70 7574  _to_pair = input
-000201a0: 730a 0a20 2020 2020 2020 2041 3a20 746f  s..        A: to
-000201b0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-000201c0: 6368 2e61 6464 2874 6f72 6368 2e6d 6174  ch.add(torch.mat
-000201d0: 6d75 6c28 7061 6972 5f66 6561 7475 7265  mul(pair_feature
-000201e0: 732c 2073 656c 662e 5729 2c20 7365 6c66  s, self.W), self
-000201f0: 2e62 290a 2020 2020 2020 2020 4120 3d20  .b).        A = 
-00020200: 746f 7263 682e 7265 7368 6170 6528 412c  torch.reshape(A,
-00020210: 2028 2d31 2c20 7365 6c66 2e6e 5f68 6964   (-1, self.n_hid
-00020220: 6465 6e2c 2073 656c 662e 6e5f 6869 6464  den, self.n_hidd
-00020230: 656e 2929 0a20 2020 2020 2020 206f 7574  en)).        out
-00020240: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00020250: 2074 6f72 6368 2e75 6e73 7175 6565 7a65   torch.unsqueeze
-00020260: 2861 746f 6d5f 6665 6174 7572 6573 5b61  (atom_features[a
-00020270: 746f 6d5f 746f 5f70 6169 725b 3a2c 2031  tom_to_pair[:, 1
-00020280: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
-00020290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000202a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000202b0: 6469 6d3d 3229 0a20 2020 2020 2020 206f  dim=2).        o
-000202c0: 7574 5f73 7175 6565 7a65 3a20 746f 7263  ut_squeeze: torc
-000202d0: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-000202e0: 2e73 7175 6565 7a65 2874 6f72 6368 2e6d  .squeeze(torch.m
-000202f0: 6174 6d75 6c28 412c 206f 7574 292c 2064  atmul(A, out), d
-00020300: 696d 3d32 290a 2020 2020 2020 2020 696e  im=2).        in
-00020310: 643a 2074 6f72 6368 2e54 656e 736f 7220  d: torch.Tensor 
-00020320: 3d20 6174 6f6d 5f74 6f5f 7061 6972 5b3a  = atom_to_pair[:
-00020330: 2c20 305d 0a0a 2020 2020 2020 2020 7265  , 0]..        re
-00020340: 7375 6c74 3a20 746f 7263 682e 5465 6e73  sult: torch.Tens
-00020350: 6f72 203d 2073 6567 6d65 6e74 5f73 756d  or = segment_sum
-00020360: 286f 7574 5f73 7175 6565 7a65 2c20 696e  (out_squeeze, in
-00020370: 6429 0a0a 2020 2020 2020 2020 7265 7475  d)..        retu
-00020380: 726e 2072 6573 756c 740a 0a0a 636c 6173  rn result...clas
-00020390: 7320 5765 6176 654c 6179 6572 286e 6e2e  s WeaveLayer(nn.
-000203a0: 4d6f 6475 6c65 293a 0a20 2020 2022 2222  Module):.    """
-000203b0: 5468 6973 2063 6c61 7373 2069 6d70 6c65  This class imple
-000203c0: 6d65 6e74 7320 7468 6520 636f 7265 2057  ments the core W
-000203d0: 6561 7665 2063 6f6e 766f 6c75 7469 6f6e  eave convolution
-000203e0: 2066 726f 6d20 7468 6520 476f 6f67 6c65   from the Google
-000203f0: 2067 7261 7068 2063 6f6e 766f 6c75 7469   graph convoluti
-00020400: 6f6e 2070 6170 6572 205b 315d 5f0a 2020  on paper [1]_.  
-00020410: 5468 6973 2069 7320 7468 6520 546f 7263  This is the Torc
-00020420: 6820 6571 7569 7661 6c65 6e74 206f 6620  h equivalent of 
-00020430: 7468 6520 6f72 6967 696e 616c 2069 6d70  the original imp
-00020440: 6c65 6d65 6e74 6174 696f 6e20 7573 696e  lementation usin
-00020450: 6720 4b65 7261 732e 0a0a 2020 5468 6973  g Keras...  This
-00020460: 206d 6f64 656c 2063 6f6e 7461 696e 7320   model contains 
-00020470: 6174 6f6d 2066 6561 7475 7265 7320 616e  atom features an
-00020480: 6420 626f 6e64 2066 6561 7475 7265 730a  d bond features.
-00020490: 2020 7365 7061 7261 7465 6c79 2e48 6572    separately.Her
-000204a0: 652c 2062 6f6e 6420 6665 6174 7572 6573  e, bond features
-000204b0: 2061 7265 2061 6c73 6f20 6361 6c6c 6564   are also called
-000204c0: 2070 6169 7220 6665 6174 7572 6573 2e0a   pair features..
-000204d0: 2020 5468 6572 6520 6172 6520 3220 7479    There are 2 ty
-000204e0: 7065 7320 6f66 2074 7261 6e73 666f 726d  pes of transform
-000204f0: 6174 696f 6e2c 2061 746f 6d2d 3e61 746f  ation, atom->ato
-00020500: 6d2c 2061 746f 6d2d 3e70 6169 722c 2070  m, atom->pair, p
-00020510: 6169 722d 3e61 746f 6d2c 2070 6169 722d  air->atom, pair-
-00020520: 3e70 6169 7220 7468 6174 2074 6869 7320  >pair that this 
-00020530: 6d6f 6465 6c20 696d 706c 656d 656e 7473  model implements
-00020540: 2e0a 0a20 2045 7861 6d70 6c65 730a 2020  ...  Examples.  
-00020550: 2d2d 2d2d 2d2d 2d2d 0a20 2054 6869 7320  --------.  This 
-00020560: 6c61 7965 7220 6578 7065 6374 7320 3420  layer expects 4 
-00020570: 696e 7075 7473 2069 6e20 6120 6c69 7374  inputs in a list
-00020580: 206f 6620 7468 6520 666f 726d 2060 5b61   of the form `[a
-00020590: 746f 6d5f 6665 6174 7572 6573 2c0a 2020  tom_features,.  
-000205a0: 7061 6972 5f66 6561 7475 7265 732c 2070  pair_features, p
-000205b0: 6169 725f 7370 6c69 742c 2061 746f 6d5f  air_split, atom_
-000205c0: 746f 5f70 6169 725d 602e 2057 6527 6c6c  to_pair]`. We'll
-000205d0: 2077 616c 6b20 7468 726f 7567 6820 7468   walk through th
-000205e0: 6520 7374 7275 6374 7572 6520 6f66 2074  e structure of t
-000205f0: 6865 7365 2069 6e70 7574 732e 204c 6574  hese inputs. Let
-00020600: 2773 2073 7461 7274 2077 6974 6820 736f  's start with so
-00020610: 6d65 2062 6173 6963 2064 6566 696e 6974  me basic definit
-00020620: 696f 6e73 2e0a 2020 3e3e 3e20 696d 706f  ions..  >>> impo
-00020630: 7274 2064 6565 7063 6865 6d20 6173 2064  rt deepchem as d
-00020640: 630a 2020 3e3e 3e20 696d 706f 7274 206e  c.  >>> import n
-00020650: 756d 7079 2061 7320 6e70 0a20 203e 3e3e  umpy as np.  >>>
-00020660: 2073 6d69 6c65 7320 3d20 5b22 4343 4322   smiles = ["CCC"
-00020670: 2c20 2243 225d 0a0a 2020 4e6f 7465 2074  , "C"]..  Note t
-00020680: 6861 7420 7468 6572 6520 6172 6520 3420  hat there are 4 
-00020690: 6174 6f6d 7320 696e 2074 6f74 616c 2069  atoms in total i
-000206a0: 6e20 7468 6973 2073 7973 7465 6d2e 2054  n this system. T
-000206b0: 6869 7320 6c61 7965 7220 6578 7065 6374  his layer expect
-000206c0: 7320 6974 7320 696e 7075 7420 6d6f 6c65  s its input mole
-000206d0: 6375 6c65 7320 746f 2062 6520 6261 7463  cules to be batc
-000206e0: 6865 6420 746f 6765 7468 6572 2e0a 0a20  hed together... 
-000206f0: 203e 3e3e 2074 6f74 616c 5f6e 5f61 746f   >>> total_n_ato
-00020700: 6d73 203d 2034 0a0a 2020 4c65 7427 7320  ms = 4..  Let's 
-00020710: 7375 7070 6f73 6520 7468 6174 2077 6520  suppose that we 
-00020720: 6861 7665 2061 2066 6561 7475 7269 7a65  have a featurize
-00020730: 7220 7468 6174 2063 6f6d 7075 7465 7320  r that computes 
-00020740: 606e 5f61 746f 6d5f 6665 6174 6020 6665  `n_atom_feat` fe
-00020750: 6174 7572 6573 2070 6572 2061 746f 6d2e  atures per atom.
-00020760: 0a0a 2020 3e3e 3e20 6e5f 6174 6f6d 5f66  ..  >>> n_atom_f
-00020770: 6561 7420 3d20 3735 0a0a 2020 5468 656e  eat = 75..  Then
-00020780: 2063 6f6e 6365 7074 7561 6c6c 792c 2060   conceptually, `
-00020790: 6174 6f6d 5f66 6561 7460 2069 7320 7468  atom_feat` is th
-000207a0: 6520 6172 7261 7920 6f66 2073 6861 7065  e array of shape
-000207b0: 2060 2874 6f74 616c 5f6e 5f61 746f 6d73   `(total_n_atoms
-000207c0: 2c0a 2020 6e5f 6174 6f6d 5f66 6561 7429  ,.  n_atom_feat)
-000207d0: 6020 6f66 2061 746f 6d69 6320 6665 6174  ` of atomic feat
-000207e0: 7572 6573 2e20 466f 7220 7369 6d70 6c69  ures. For simpli
-000207f0: 6369 7479 2c20 6c65 7427 7320 6a75 7374  city, let's just
-00020800: 2067 6f20 7769 7468 2061 0a20 2072 616e   go with a.  ran
-00020810: 646f 6d20 7375 6368 206d 6174 7269 782e  dom such matrix.
-00020820: 0a0a 2020 3e3e 3e20 6174 6f6d 5f66 6561  ..  >>> atom_fea
-00020830: 7420 3d20 6e70 2e72 616e 646f 6d2e 7261  t = np.random.ra
-00020840: 6e64 2874 6f74 616c 5f6e 5f61 746f 6d73  nd(total_n_atoms
-00020850: 2c20 6e5f 6174 6f6d 5f66 6561 7429 0a0a  , n_atom_feat)..
-00020860: 2020 4c65 7427 7320 7375 7070 6f73 6520    Let's suppose 
-00020870: 7765 2068 6176 6520 606e 5f70 6169 725f  we have `n_pair_
-00020880: 6665 6174 6020 7061 6972 7769 7365 2066  feat` pairwise f
-00020890: 6561 7475 7265 730a 0a20 203e 3e3e 206e  eatures..  >>> n
-000208a0: 5f70 6169 725f 6665 6174 203d 2031 340a  _pair_feat = 14.
-000208b0: 0a20 2046 6f72 2065 6163 6820 6d6f 6c65  .  For each mole
-000208c0: 6375 6c65 2c20 7765 2063 6f6d 7075 7465  cule, we compute
-000208d0: 2061 206d 6174 7269 7820 6f66 2073 6861   a matrix of sha
-000208e0: 7065 2060 286e 5f61 746f 6d73 2a6e 5f61  pe `(n_atoms*n_a
-000208f0: 746f 6d73 2c0a 2020 6e5f 7061 6972 5f66  toms,.  n_pair_f
-00020900: 6561 7429 6020 6f66 2070 6169 7277 6973  eat)` of pairwis
-00020910: 6520 6665 6174 7572 6573 2066 6f72 2065  e features for e
-00020920: 6163 6820 7061 6972 206f 6620 6174 6f6d  ach pair of atom
-00020930: 7320 696e 2074 6865 206d 6f6c 6563 756c  s in the molecul
-00020940: 652e 0a20 204c 6574 2773 2063 6f6e 7374  e..  Let's const
-00020950: 7275 6374 2074 6869 7320 636f 6e63 6570  ruct this concep
-00020960: 7475 616c 6c79 2066 6f72 206f 7572 2065  tually for our e
-00020970: 7861 6d70 6c65 2e0a 0a20 203e 3e3e 2070  xample...  >>> p
-00020980: 6169 725f 6665 6174 203d 205b 6e70 2e72  air_feat = [np.r
-00020990: 616e 646f 6d2e 7261 6e64 2833 2a33 2c20  andom.rand(3*3, 
-000209a0: 6e5f 7061 6972 5f66 6561 7429 2c20 6e70  n_pair_feat), np
-000209b0: 2e72 616e 646f 6d2e 7261 6e64 2831 2a31  .random.rand(1*1
-000209c0: 2c6e 5f70 6169 725f 6665 6174 295d 0a20  ,n_pair_feat)]. 
-000209d0: 203e 3e3e 2070 6169 725f 6665 6174 203d   >>> pair_feat =
-000209e0: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
-000209f0: 7061 6972 5f66 6561 742c 2061 7869 733d  pair_feat, axis=
-00020a00: 3029 0a20 203e 3e3e 2070 6169 725f 6665  0).  >>> pair_fe
-00020a10: 6174 2e73 6861 7065 0a20 2028 3130 2c20  at.shape.  (10, 
-00020a20: 3134 290a 0a20 2060 7061 6972 5f73 706c  14)..  `pair_spl
-00020a30: 6974 6020 6973 2061 6e20 696e 6465 7820  it` is an index 
-00020a40: 696e 746f 2060 7061 6972 5f66 6561 7460  into `pair_feat`
-00020a50: 2077 6869 6368 2074 656c 6c73 2075 7320   which tells us 
-00020a60: 7768 6963 6820 6174 6f6d 2065 6163 6820  which atom each 
-00020a70: 726f 7720 6265 6c6f 6e67 7320 746f 2e20  row belongs to. 
-00020a80: 496e 206f 7572 2063 6173 652c 2077 6520  In our case, we 
-00020a90: 6876 650a 0a20 203e 3e3e 2070 6169 725f  hve..  >>> pair_
-00020aa0: 7370 6c69 7420 3d20 6e70 2e61 7272 6179  split = np.array
-00020ab0: 285b 302c 2030 2c20 302c 2031 2c20 312c  ([0, 0, 0, 1, 1,
-00020ac0: 2031 2c20 322c 2032 2c20 322c 2033 5d29   1, 2, 2, 2, 3])
-00020ad0: 0a0a 2020 5468 6174 2069 732c 2074 6865  ..  That is, the
-00020ae0: 2066 6972 7374 2039 2065 6e74 7269 6573   first 9 entries
-00020af0: 2062 656c 6f6e 6720 746f 2022 4343 4322   belong to "CCC"
-00020b00: 2061 6e64 2074 6865 206c 6173 7420 656e   and the last en
-00020b10: 7472 7920 746f 2022 4322 2e20 5468 650a  try to "C". The.
-00020b20: 2020 6669 6e61 6c20 656e 7472 7920 6061    final entry `a
-00020b30: 746f 6d5f 746f 5f70 6169 7260 2067 6f65  tom_to_pair` goe
-00020b40: 7320 696e 2061 206c 6974 746c 6520 6d6f  s in a little mo
-00020b50: 7265 2069 6e2d 6465 7074 6820 7468 616e  re in-depth than
-00020b60: 2060 7061 6972 5f73 706c 6974 600a 2020   `pair_split`.  
-00020b70: 616e 6420 7465 6c6c 7320 7573 2074 6865  and tells us the
-00020b80: 2070 7265 6369 7365 2070 6169 7220 6561   precise pair ea
-00020b90: 6368 2070 6169 7220 6665 6174 7572 6520  ch pair feature 
-00020ba0: 6265 6c6f 6e67 7320 746f 2e20 496e 206f  belongs to. In o
-00020bb0: 7572 2063 6173 650a 0a20 203e 3e3e 2061  ur case..  >>> a
-00020bc0: 746f 6d5f 746f 5f70 6169 7220 3d20 6e70  tom_to_pair = np
-00020bd0: 2e61 7272 6179 285b 5b30 2c20 305d 2c0a  .array([[0, 0],.
-00020be0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00020bf0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00020c00: 302c 2031 5d2c 0a20 202e 2e2e 2020 2020  0, 1],.  ...    
-00020c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c20: 2020 2020 2020 5b30 2c20 325d 2c0a 2020        [0, 2],.  
-00020c30: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-00020c40: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
-00020c50: 2030 5d2c 0a20 202e 2e2e 2020 2020 2020   0],.  ...      
-00020c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c70: 2020 2020 5b31 2c20 315d 2c0a 2020 2e2e      [1, 1],.  ..
-00020c80: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00020c90: 2020 2020 2020 2020 2020 205b 312c 2032             [1, 2
-00020ca0: 5d2c 0a20 202e 2e2e 2020 2020 2020 2020  ],.  ...        
-00020cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cc0: 2020 5b32 2c20 305d 2c0a 2020 2e2e 2e20    [2, 0],.  ... 
-00020cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ce0: 2020 2020 2020 2020 205b 322c 2031 5d2c           [2, 1],
-00020cf0: 0a20 202e 2e2e 2020 2020 2020 2020 2020  .  ...          
-00020d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d10: 5b32 2c20 325d 2c0a 2020 2e2e 2e20 2020  [2, 2],.  ...   
-00020d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d30: 2020 2020 2020 205b 332c 2033 5d5d 290a         [3, 3]]).
-00020d40: 0a20 204c 6574 2773 206e 6f77 2064 6566  .  Let's now def
-00020d50: 696e 6520 7468 6520 6163 7475 616c 206c  ine the actual l
-00020d60: 6179 6572 0a0a 2020 3e3e 3e20 6c61 7965  ayer..  >>> laye
-00020d70: 7220 3d20 5765 6176 654c 6179 6572 2829  r = WeaveLayer()
-00020d80: 0a0a 2020 416e 6420 696e 766f 6b65 2069  ..  And invoke i
-00020d90: 740a 0a20 203e 3e3e 205b 412c 2050 5d20  t..  >>> [A, P] 
-00020da0: 3d20 6c61 7965 7228 5b61 746f 6d5f 6665  = layer([atom_fe
-00020db0: 6174 2c20 7061 6972 5f66 6561 742c 2070  at, pair_feat, p
-00020dc0: 6169 725f 7370 6c69 742c 2061 746f 6d5f  air_split, atom_
-00020dd0: 746f 5f70 6169 725d 290a 0a20 2054 6865  to_pair])..  The
-00020de0: 2077 6561 7665 206c 6179 6572 2070 726f   weave layer pro
-00020df0: 6475 6365 7320 6e65 7720 6174 6f6d 2f70  duces new atom/p
-00020e00: 6169 7220 6665 6174 7572 6573 2e20 4c65  air features. Le
-00020e10: 7427 7320 6368 6563 6b20 7468 6569 7220  t's check their 
-00020e20: 7368 6170 6573 0a0a 2020 3e3e 3e20 4120  shapes..  >>> A 
-00020e30: 3d20 412e 6465 7461 6368 2829 2e6e 756d  = A.detach().num
-00020e40: 7079 2829 0a20 203e 3e3e 2041 2e73 6861  py().  >>> A.sha
-00020e50: 7065 0a20 2028 342c 2035 3029 0a20 203e  pe.  (4, 50).  >
-00020e60: 3e3e 2050 203d 2050 2e64 6574 6163 6828  >> P = P.detach(
-00020e70: 292e 6e75 6d70 7928 290a 2020 3e3e 3e20  ).numpy().  >>> 
-00020e80: 502e 7368 6170 650a 2020 2831 302c 2035  P.shape.  (10, 5
-00020e90: 3029 0a0a 2020 5468 6520 3420 6973 2060  0)..  The 4 is `
-00020ea0: 746f 7461 6c5f 6e75 6d5f 6174 6f6d 7360  total_num_atoms`
-00020eb0: 2061 6e64 2074 6865 2031 3020 6973 2074   and the 10 is t
-00020ec0: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
-00020ed0: 6f66 2070 6169 7273 2e20 5768 6572 650a  of pairs. Where.
-00020ee0: 2020 646f 6573 2060 3530 6020 636f 6d65    does `50` come
-00020ef0: 2066 726f 6d3f 2049 7427 7320 6672 6f6d   from? It's from
-00020f00: 2074 6865 2064 6566 6175 6c74 2061 7267   the default arg
-00020f10: 756d 656e 7473 2060 6e5f 6174 6f6d 5f69  uments `n_atom_i
-00020f20: 6e70 7574 5f66 6561 7460 2061 6e64 0a20  nput_feat` and. 
-00020f30: 2060 6e5f 7061 6972 5f69 6e70 7574 5f66   `n_pair_input_f
-00020f40: 6561 7460 2e0a 0a20 2052 6566 6572 656e  eat`...  Referen
-00020f50: 6365 730a 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ces.  ----------
-00020f60: 0a20 202e 2e20 5b31 5d20 4b65 6172 6e65  .  .. [1] Kearne
-00020f70: 732c 2053 7465 7665 6e2c 2065 7420 616c  s, Steven, et al
-00020f80: 2e20 224d 6f6c 6563 756c 6172 2067 7261  . "Molecular gra
-00020f90: 7068 2063 6f6e 766f 6c75 7469 6f6e 733a  ph convolutions:
-00020fa0: 206d 6f76 696e 6720 6265 796f 6e64 0a20   moving beyond. 
-00020fb0: 2020 2020 2020 2066 696e 6765 7270 7269         fingerpri
-00020fc0: 6e74 732e 2220 4a6f 7572 6e61 6c20 6f66  nts." Journal of
-00020fd0: 2063 6f6d 7075 7465 722d 6169 6465 6420   computer-aided 
-00020fe0: 6d6f 6c65 6375 6c61 7220 6465 7369 676e  molecular design
-00020ff0: 2033 302e 3820 2832 3031 3629 3a0a 2020   30.8 (2016):.  
-00021000: 2020 2020 2020 3539 352d 3630 382e 0a20        595-608.. 
-00021010: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-00021020: 696e 6974 5f5f 2873 656c 662c 0a20 2020  init__(self,.   
-00021030: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-00021040: 6174 6f6d 5f69 6e70 7574 5f66 6561 743a  atom_input_feat:
-00021050: 2069 6e74 203d 2037 352c 0a20 2020 2020   int = 75,.     
-00021060: 2020 2020 2020 2020 2020 2020 6e5f 7061              n_pa
-00021070: 6972 5f69 6e70 7574 5f66 6561 743a 2069  ir_input_feat: i
-00021080: 6e74 203d 2031 342c 0a20 2020 2020 2020  nt = 14,.       
-00021090: 2020 2020 2020 2020 2020 6e5f 6174 6f6d            n_atom
-000210a0: 5f6f 7574 7075 745f 6665 6174 3a20 696e  _output_feat: in
-000210b0: 7420 3d20 3530 2c0a 2020 2020 2020 2020  t = 50,.        
-000210c0: 2020 2020 2020 2020 206e 5f70 6169 725f           n_pair_
-000210d0: 6f75 7470 7574 5f66 6561 743a 2069 6e74  output_feat: int
-000210e0: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
-000210f0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-00021100: 5f41 413a 2069 6e74 203d 2035 302c 0a20  _AA: int = 50,. 
-00021110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021120: 6e5f 6869 6464 656e 5f50 413a 2069 6e74  n_hidden_PA: int
-00021130: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
-00021140: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-00021150: 5f41 503a 2069 6e74 203d 2035 302c 0a20  _AP: int = 50,. 
-00021160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021170: 6e5f 6869 6464 656e 5f50 503a 2069 6e74  n_hidden_PP: int
-00021180: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
-00021190: 2020 2020 2020 2020 7570 6461 7465 5f70          update_p
-000211a0: 6169 723a 2062 6f6f 6c20 3d20 5472 7565  air: bool = True
-000211b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000211c0: 2020 2069 6e69 745f 3a20 7374 7220 3d20     init_: str = 
-000211d0: 2778 6176 6965 725f 756e 6966 6f72 6d5f  'xavier_uniform_
-000211e0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000211f0: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
-00021200: 7374 7220 3d20 2772 656c 7527 2c0a 2020  str = 'relu',.  
-00021210: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00021220: 6174 6368 5f6e 6f72 6d61 6c69 7a65 3a20  atch_normalize: 
-00021230: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-00021240: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-00021250: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00021260: 2022 2222 0a20 2020 2050 6172 616d 6574   """.    Paramet
-00021270: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00021280: 2d2d 0a20 2020 206e 5f61 746f 6d5f 696e  --.    n_atom_in
-00021290: 7075 745f 6665 6174 3a20 696e 742c 206f  put_feat: int, o
-000212a0: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-000212b0: 2037 3529 0a20 2020 2020 204e 756d 6265   75).      Numbe
-000212c0: 7220 6f66 2066 6561 7475 7265 7320 666f  r of features fo
-000212d0: 7220 6561 6368 2061 746f 6d20 696e 2069  r each atom in i
-000212e0: 6e70 7574 2e0a 2020 2020 6e5f 7061 6972  nput..    n_pair
-000212f0: 5f69 6e70 7574 5f66 6561 743a 2069 6e74  _input_feat: int
-00021300: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
-00021310: 756c 7420 3134 290a 2020 2020 2020 4e75  ult 14).      Nu
-00021320: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
-00021330: 2066 6f72 2065 6163 6820 7061 6972 206f   for each pair o
-00021340: 6620 6174 6f6d 7320 696e 2069 6e70 7574  f atoms in input
-00021350: 2e0a 2020 2020 6e5f 6174 6f6d 5f6f 7574  ..    n_atom_out
-00021360: 7075 745f 6665 6174 3a20 696e 742c 206f  put_feat: int, o
-00021370: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-00021380: 2035 3029 0a20 2020 2020 204e 756d 6265   50).      Numbe
-00021390: 7220 6f66 2066 6561 7475 7265 7320 666f  r of features fo
-000213a0: 7220 6561 6368 2061 746f 6d20 696e 206f  r each atom in o
-000213b0: 7574 7075 742e 0a20 2020 206e 5f70 6169  utput..    n_pai
-000213c0: 725f 6f75 7470 7574 5f66 6561 743a 2069  r_output_feat: i
-000213d0: 6e74 2c20 6f70 7469 6f6e 616c 2028 6465  nt, optional (de
-000213e0: 6661 756c 7420 3530 290a 2020 2020 2020  fault 50).      
-000213f0: 4e75 6d62 6572 206f 6620 6665 6174 7572  Number of featur
-00021400: 6573 2066 6f72 2065 6163 6820 7061 6972  es for each pair
-00021410: 206f 6620 6174 6f6d 7320 696e 206f 7574   of atoms in out
-00021420: 7075 742e 0a20 2020 206e 5f68 6964 6465  put..    n_hidde
-00021430: 6e5f 4141 3a20 696e 742c 206f 7074 696f  n_AA: int, optio
-00021440: 6e61 6c20 2864 6566 6175 6c74 2035 3029  nal (default 50)
-00021450: 0a20 2020 2020 204e 756d 6265 7220 6f66  .      Number of
-00021460: 2075 6e69 7473 2863 6f6e 766f 6c75 7469   units(convoluti
-00021470: 6f6e 2064 6570 7468 7329 2069 6e20 636f  on depths) in co
-00021480: 7272 6573 706f 6e64 696e 6720 6869 6464  rresponding hidd
-00021490: 656e 206c 6179 6572 0a20 2020 206e 5f68  en layer.    n_h
-000214a0: 6964 6465 6e5f 5041 3a20 696e 742c 206f  idden_PA: int, o
-000214b0: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-000214c0: 2035 3029 0a20 2020 2020 204e 756d 6265   50).      Numbe
-000214d0: 7220 6f66 2075 6e69 7473 2863 6f6e 766f  r of units(convo
-000214e0: 6c75 7469 6f6e 2064 6570 7468 7329 2069  lution depths) i
-000214f0: 6e20 636f 7272 6573 706f 6e64 696e 6720  n corresponding 
-00021500: 6869 6464 656e 206c 6179 6572 0a20 2020  hidden layer.   
-00021510: 206e 5f68 6964 6465 6e5f 4150 3a20 696e   n_hidden_AP: in
-00021520: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
-00021530: 6175 6c74 2035 3029 0a20 2020 2020 204e  ault 50).      N
-00021540: 756d 6265 7220 6f66 2075 6e69 7473 2863  umber of units(c
-00021550: 6f6e 766f 6c75 7469 6f6e 2064 6570 7468  onvolution depth
-00021560: 7329 2069 6e20 636f 7272 6573 706f 6e64  s) in correspond
-00021570: 696e 6720 6869 6464 656e 206c 6179 6572  ing hidden layer
-00021580: 0a20 2020 206e 5f68 6964 6465 6e5f 5050  .    n_hidden_PP
-00021590: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
-000215a0: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
-000215b0: 2020 204e 756d 6265 7220 6f66 2075 6e69     Number of uni
-000215c0: 7473 2863 6f6e 766f 6c75 7469 6f6e 2064  ts(convolution d
-000215d0: 6570 7468 7329 2069 6e20 636f 7272 6573  epths) in corres
-000215e0: 706f 6e64 696e 6720 6869 6464 656e 206c  ponding hidden l
-000215f0: 6179 6572 0a20 2020 2075 7064 6174 655f  ayer.    update_
-00021600: 7061 6972 3a20 626f 6f6c 2c20 6f70 7469  pair: bool, opti
-00021610: 6f6e 616c 2028 6465 6661 756c 7420 5472  onal (default Tr
-00021620: 7565 290a 2020 2020 2020 5768 6574 6865  ue).      Whethe
-00021630: 7220 746f 2063 616c 6375 6c61 7465 2066  r to calculate f
-00021640: 6f72 2070 6169 7220 6665 6174 7572 6573  or pair features
-00021650: 2c0a 2020 2020 2020 636f 756c 6420 6265  ,.      could be
-00021660: 2074 7572 6e65 6420 6f66 6620 666f 7220   turned off for 
-00021670: 6c61 7374 206c 6179 6572 0a20 2020 2069  last layer.    i
-00021680: 6e69 743a 2073 7472 2c20 6f70 7469 6f6e  nit: str, option
-00021690: 616c 2028 6465 6661 756c 7420 2778 6176  al (default 'xav
-000216a0: 6965 725f 756e 6966 6f72 6d5f 2729 0a20  ier_uniform_'). 
-000216b0: 2020 2020 2057 6569 6768 7420 696e 6974       Weight init
-000216c0: 6961 6c69 7a61 7469 6f6e 2066 6f72 2066  ialization for f
-000216d0: 696c 7465 7273 2e0a 2020 2020 6163 7469  ilters..    acti
-000216e0: 7661 7469 6f6e 3a20 7374 722c 206f 7074  vation: str, opt
-000216f0: 696f 6e61 6c20 2864 6566 6175 6c74 2027  ional (default '
-00021700: 7265 6c75 2729 0a20 2020 2020 2041 6374  relu').      Act
-00021710: 6976 6174 696f 6e20 6675 6e63 7469 6f6e  ivation function
-00021720: 2061 7070 6c69 6564 0a20 2020 2062 6174   applied.    bat
-00021730: 6368 5f6e 6f72 6d61 6c69 7a65 3a20 626f  ch_normalize: bo
-00021740: 6f6c 2c20 6f70 7469 6f6e 616c 2028 6465  ol, optional (de
-00021750: 6661 756c 7420 5472 7565 290a 2020 2020  fault True).    
-00021760: 2020 4966 2074 6869 7320 6973 2074 7572    If this is tur
-00021770: 6e65 6420 6f6e 2c20 6170 706c 7920 6261  ned on, apply ba
-00021780: 7463 6820 6e6f 726d 616c 697a 6174 696f  tch normalizatio
-00021790: 6e20 6265 666f 7265 2061 7070 6c79 696e  n before applyin
-000217a0: 670a 2020 2020 2020 6163 7469 7661 7469  g.      activati
-000217b0: 6f6e 2066 756e 6374 696f 6e73 206f 6e20  on functions on 
-000217c0: 636f 6e76 6f6c 7574 696f 6e61 6c20 6c61  convolutional la
-000217d0: 7965 7273 2e0a 2020 2020 2222 220a 2020  yers..    """.  
-000217e0: 2020 2020 2020 7375 7065 7228 5765 6176        super(Weav
-000217f0: 654c 6179 6572 2c20 7365 6c66 292e 5f5f  eLayer, self).__
-00021800: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
-00021810: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00021820: 6974 3a20 7374 7220 3d20 696e 6974 5f20  it: str = init_ 
-00021830: 2023 2053 6574 2077 6569 6768 7420 696e   # Set weight in
-00021840: 6974 6961 6c69 7a61 7469 6f6e 0a20 2020  itialization.   
-00021850: 2020 2020 2073 656c 662e 6163 7469 7661       self.activa
-00021860: 7469 6f6e 3a20 7374 7220 3d20 6163 7469  tion: str = acti
-00021870: 7661 7469 6f6e 2020 2320 4765 7420 6163  vation  # Get ac
-00021880: 7469 7661 7469 6f6e 730a 2020 2020 2020  tivations.      
-00021890: 2020 7365 6c66 2e61 6374 6976 6174 696f    self.activatio
-000218a0: 6e5f 666e 3a20 746f 7263 682e 6e6e 2e4d  n_fn: torch.nn.M
-000218b0: 6f64 756c 6520 3d20 6765 745f 6163 7469  odule = get_acti
-000218c0: 7661 7469 6f6e 2861 6374 6976 6174 696f  vation(activatio
-000218d0: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-000218e0: 7570 6461 7465 5f70 6169 723a 2062 6f6f  update_pair: boo
-000218f0: 6c20 3d20 7570 6461 7465 5f70 6169 7220  l = update_pair 
-00021900: 2023 206c 6173 7420 7765 6176 6520 6c61   # last weave la
-00021910: 7965 7220 646f 6573 206e 6f74 206e 6565  yer does not nee
-00021920: 6420 746f 2075 7064 6174 650a 2020 2020  d to update.    
-00021930: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
-00021940: 6e5f 4141 3a20 696e 7420 3d20 6e5f 6869  n_AA: int = n_hi
-00021950: 6464 656e 5f41 410a 2020 2020 2020 2020  dden_AA.        
-00021960: 7365 6c66 2e6e 5f68 6964 6465 6e5f 5041  self.n_hidden_PA
-00021970: 3a20 696e 7420 3d20 6e5f 6869 6464 656e  : int = n_hidden
-00021980: 5f50 410a 2020 2020 2020 2020 7365 6c66  _PA.        self
-00021990: 2e6e 5f68 6964 6465 6e5f 4150 3a20 696e  .n_hidden_AP: in
-000219a0: 7420 3d20 6e5f 6869 6464 656e 5f41 500a  t = n_hidden_AP.
-000219b0: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
-000219c0: 6964 6465 6e5f 5050 3a20 696e 7420 3d20  idden_PP: int = 
-000219d0: 6e5f 6869 6464 656e 5f50 500a 2020 2020  n_hidden_PP.    
-000219e0: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
-000219f0: 6e5f 413a 2069 6e74 203d 206e 5f68 6964  n_A: int = n_hid
-00021a00: 6465 6e5f 4141 202b 206e 5f68 6964 6465  den_AA + n_hidde
-00021a10: 6e5f 5041 0a20 2020 2020 2020 2073 656c  n_PA.        sel
-00021a20: 662e 6e5f 6869 6464 656e 5f50 3a20 696e  f.n_hidden_P: in
-00021a30: 7420 3d20 6e5f 6869 6464 656e 5f41 5020  t = n_hidden_AP 
-00021a40: 2b20 6e5f 6869 6464 656e 5f50 500a 2020  + n_hidden_PP.  
-00021a50: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-00021a60: 5f6e 6f72 6d61 6c69 7a65 3a20 626f 6f6c  _normalize: bool
-00021a70: 203d 2062 6174 6368 5f6e 6f72 6d61 6c69   = batch_normali
-00021a80: 7a65 0a0a 2020 2020 2020 2020 7365 6c66  ze..        self
-00021a90: 2e6e 5f61 746f 6d5f 696e 7075 745f 6665  .n_atom_input_fe
-00021aa0: 6174 3a20 696e 7420 3d20 6e5f 6174 6f6d  at: int = n_atom
-00021ab0: 5f69 6e70 7574 5f66 6561 740a 2020 2020  _input_feat.    
-00021ac0: 2020 2020 7365 6c66 2e6e 5f70 6169 725f      self.n_pair_
-00021ad0: 696e 7075 745f 6665 6174 3a20 696e 7420  input_feat: int 
-00021ae0: 3d20 6e5f 7061 6972 5f69 6e70 7574 5f66  = n_pair_input_f
-00021af0: 6561 740a 2020 2020 2020 2020 7365 6c66  eat.        self
-00021b00: 2e6e 5f61 746f 6d5f 6f75 7470 7574 5f66  .n_atom_output_f
-00021b10: 6561 743a 2069 6e74 203d 206e 5f61 746f  eat: int = n_ato
-00021b20: 6d5f 6f75 7470 7574 5f66 6561 740a 2020  m_output_feat.  
-00021b30: 2020 2020 2020 7365 6c66 2e6e 5f70 6169        self.n_pai
-00021b40: 725f 6f75 7470 7574 5f66 6561 743a 2069  r_output_feat: i
-00021b50: 6e74 203d 206e 5f70 6169 725f 6f75 7470  nt = n_pair_outp
-00021b60: 7574 5f66 6561 740a 0a20 2020 2020 2020  ut_feat..       
-00021b70: 2023 2043 6f6e 7374 7275 6374 2069 6e74   # Construct int
-00021b80: 6572 6e61 6c20 7472 6169 6e61 626c 6520  ernal trainable 
-00021b90: 7765 6967 6874 730a 2020 2020 2020 2020  weights.        
-00021ba0: 696e 6974 203d 2067 6574 6174 7472 2869  init = getattr(i
-00021bb0: 6e69 7469 616c 697a 6572 732c 2073 656c  nitializers, sel
-00021bc0: 662e 696e 6974 290a 2020 2020 2020 2020  f.init).        
-00021bd0: 2320 5765 6967 6874 206d 6174 7269 7820  # Weight matrix 
-00021be0: 616e 6420 6269 6173 206d 6174 7269 7820  and bias matrix 
-00021bf0: 7265 7175 6972 6564 2074 6f20 636f 6d70  required to comp
-00021c00: 7574 6520 6e65 7720 6174 6f6d 206c 6179  ute new atom lay
-00021c10: 6572 2066 726f 6d20 7468 6520 7072 6576  er from the prev
-00021c20: 696f 7573 2061 746f 6d20 6c61 7965 720a  ious atom layer.
-00021c30: 2020 2020 2020 2020 7365 6c66 2e57 5f41          self.W_A
-00021c40: 413a 2074 6f72 6368 2e54 656e 736f 7220  A: torch.Tensor 
-00021c50: 3d20 696e 6974 280a 2020 2020 2020 2020  = init(.        
-00021c60: 2020 2020 746f 7263 682e 656d 7074 7928      torch.empty(
-00021c70: 7365 6c66 2e6e 5f61 746f 6d5f 696e 7075  self.n_atom_inpu
-00021c80: 745f 6665 6174 2c20 7365 6c66 2e6e 5f68  t_feat, self.n_h
-00021c90: 6964 6465 6e5f 4141 2929 0a20 2020 2020  idden_AA)).     
-00021ca0: 2020 2073 656c 662e 625f 4141 3a20 746f     self.b_AA: to
-00021cb0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-00021cc0: 6368 2e7a 6572 6f73 2828 7365 6c66 2e6e  ch.zeros((self.n
-00021cd0: 5f68 6964 6465 6e5f 4141 2c29 290a 2020  _hidden_AA,)).  
-00021ce0: 2020 2020 2020 7365 6c66 2e41 415f 626e        self.AA_bn
-00021cf0: 3a20 6e6e 2e42 6174 6368 4e6f 726d 3164  : nn.BatchNorm1d
-00021d00: 203d 206e 6e2e 4261 7463 684e 6f72 6d31   = nn.BatchNorm1
-00021d10: 6428 0a20 2020 2020 2020 2020 2020 206e  d(.            n
-00021d20: 756d 5f66 6561 7475 7265 733d 7365 6c66  um_features=self
-00021d30: 2e6e 5f68 6964 6465 6e5f 4141 2c0a 2020  .n_hidden_AA,.  
-00021d40: 2020 2020 2020 2020 2020 6570 733d 3165            eps=1e
-00021d50: 2d33 2c0a 2020 2020 2020 2020 2020 2020  -3,.            
-00021d60: 6d6f 6d65 6e74 756d 3d30 2e39 392c 0a20  momentum=0.99,. 
-00021d70: 2020 2020 2020 2020 2020 2061 6666 696e             affin
-00021d80: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
-00021d90: 2020 2020 7472 6163 6b5f 7275 6e6e 696e      track_runnin
-00021da0: 675f 7374 6174 733d 5472 7565 290a 0a20  g_stats=True).. 
-00021db0: 2020 2020 2020 2023 2057 6569 6768 7420         # Weight 
-00021dc0: 6d61 7472 6978 2061 6e64 2062 6961 7320  matrix and bias 
-00021dd0: 6d61 7472 6978 2072 6571 7569 7265 6420  matrix required 
-00021de0: 746f 2063 6f6d 7075 7465 206e 6577 2061  to compute new a
-00021df0: 746f 6d20 6c61 7965 7220 6672 6f6d 2074  tom layer from t
-00021e00: 6865 2070 7265 7669 6f75 7320 7061 6972  he previous pair
-00021e10: 206c 6179 6572 0a20 2020 2020 2020 2073   layer.        s
-00021e20: 656c 662e 575f 5041 3a20 746f 7263 682e  elf.W_PA: torch.
-00021e30: 5465 6e73 6f72 203d 2069 6e69 7428 0a20  Tensor = init(. 
-00021e40: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
-00021e50: 2e65 6d70 7479 2873 656c 662e 6e5f 7061  .empty(self.n_pa
-00021e60: 6972 5f69 6e70 7574 5f66 6561 742c 2073  ir_input_feat, s
-00021e70: 656c 662e 6e5f 6869 6464 656e 5f50 4129  elf.n_hidden_PA)
-00021e80: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
-00021e90: 5f50 413a 2074 6f72 6368 2e54 656e 736f  _PA: torch.Tenso
-00021ea0: 7220 3d20 746f 7263 682e 7a65 726f 7328  r = torch.zeros(
-00021eb0: 2873 656c 662e 6e5f 6869 6464 656e 5f50  (self.n_hidden_P
-00021ec0: 412c 2929 0a20 2020 2020 2020 2073 656c  A,)).        sel
-00021ed0: 662e 5041 5f62 6e3a 206e 6e2e 4261 7463  f.PA_bn: nn.Batc
-00021ee0: 684e 6f72 6d31 6420 3d20 6e6e 2e42 6174  hNorm1d = nn.Bat
-00021ef0: 6368 4e6f 726d 3164 280a 2020 2020 2020  chNorm1d(.      
-00021f00: 2020 2020 2020 6e75 6d5f 6665 6174 7572        num_featur
-00021f10: 6573 3d73 656c 662e 6e5f 6869 6464 656e  es=self.n_hidden
-00021f20: 5f50 412c 0a20 2020 2020 2020 2020 2020  _PA,.           
-00021f30: 2065 7073 3d31 652d 332c 0a20 2020 2020   eps=1e-3,.     
-00021f40: 2020 2020 2020 206d 6f6d 656e 7475 6d3d         momentum=
-00021f50: 302e 3939 2c0a 2020 2020 2020 2020 2020  0.99,.          
-00021f60: 2020 6166 6669 6e65 3d54 7275 652c 0a20    affine=True,. 
-00021f70: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00021f80: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
-00021f90: 7275 6529 0a0a 2020 2020 2020 2020 7365  rue)..        se
-00021fa0: 6c66 2e57 5f41 3a20 746f 7263 682e 5465  lf.W_A: torch.Te
-00021fb0: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
-00021fc0: 2020 2020 2020 2020 2074 6f72 6368 2e65           torch.e
-00021fd0: 6d70 7479 2873 656c 662e 6e5f 6869 6464  mpty(self.n_hidd
-00021fe0: 656e 5f41 2c20 7365 6c66 2e6e 5f61 746f  en_A, self.n_ato
-00021ff0: 6d5f 6f75 7470 7574 5f66 6561 7429 290a  m_output_feat)).
-00022000: 2020 2020 2020 2020 7365 6c66 2e62 5f41          self.b_A
-00022010: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00022020: 2074 6f72 6368 2e7a 6572 6f73 2828 7365   torch.zeros((se
-00022030: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
-00022040: 5f66 6561 742c 2929 0a20 2020 2020 2020  _feat,)).       
-00022050: 2073 656c 662e 415f 626e 3a20 6e6e 2e42   self.A_bn: nn.B
-00022060: 6174 6368 4e6f 726d 3164 203d 206e 6e2e  atchNorm1d = nn.
-00022070: 4261 7463 684e 6f72 6d31 6428 0a20 2020  BatchNorm1d(.   
-00022080: 2020 2020 2020 2020 206e 756d 5f66 6561           num_fea
-00022090: 7475 7265 733d 7365 6c66 2e6e 5f61 746f  tures=self.n_ato
-000220a0: 6d5f 6f75 7470 7574 5f66 6561 742c 0a20  m_output_feat,. 
-000220b0: 2020 2020 2020 2020 2020 2065 7073 3d31             eps=1
-000220c0: 652d 332c 0a20 2020 2020 2020 2020 2020  e-3,.           
-000220d0: 206d 6f6d 656e 7475 6d3d 302e 3939 2c0a   momentum=0.99,.
-000220e0: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-000220f0: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
-00022100: 2020 2020 2074 7261 636b 5f72 756e 6e69       track_runni
-00022110: 6e67 5f73 7461 7473 3d54 7275 6529 0a0a  ng_stats=True)..
-00022120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00022130: 7570 6461 7465 5f70 6169 723a 0a20 2020  update_pair:.   
-00022140: 2020 2020 2020 2020 2023 2057 6569 6768           # Weigh
-00022150: 7420 6d61 7472 6978 2061 6e64 2062 6961  t matrix and bia
-00022160: 7320 6d61 7472 6978 2072 6571 7569 7265  s matrix require
-00022170: 6420 746f 2063 6f6d 7075 7465 206e 6577  d to compute new
-00022180: 2070 6169 7220 6c61 7965 7220 6672 6f6d   pair layer from
-00022190: 2074 6865 2070 7265 7669 6f75 7320 6174   the previous at
-000221a0: 6f6d 206c 6179 6572 0a20 2020 2020 2020  om layer.       
-000221b0: 2020 2020 2073 656c 662e 575f 4150 3a20       self.W_AP: 
-000221c0: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
-000221d0: 6e69 7428 0a20 2020 2020 2020 2020 2020  nit(.           
-000221e0: 2020 2020 2074 6f72 6368 2e65 6d70 7479       torch.empty
-000221f0: 2873 656c 662e 6e5f 6174 6f6d 5f69 6e70  (self.n_atom_inp
-00022200: 7574 5f66 6561 7420 2a20 322c 2073 656c  ut_feat * 2, sel
-00022210: 662e 6e5f 6869 6464 656e 5f41 5029 290a  f.n_hidden_AP)).
-00022220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00022230: 2e62 5f41 503a 2074 6f72 6368 2e54 656e  .b_AP: torch.Ten
-00022240: 736f 7220 3d20 746f 7263 682e 7a65 726f  sor = torch.zero
-00022250: 7328 2873 656c 662e 6e5f 6869 6464 656e  s((self.n_hidden
-00022260: 5f41 502c 2929 0a20 2020 2020 2020 2020  _AP,)).         
-00022270: 2020 2073 656c 662e 4150 5f62 6e3a 206e     self.AP_bn: n
-00022280: 6e2e 4261 7463 684e 6f72 6d31 6420 3d20  n.BatchNorm1d = 
-00022290: 6e6e 2e42 6174 6368 4e6f 726d 3164 280a  nn.BatchNorm1d(.
-000222a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222b0: 6e75 6d5f 6665 6174 7572 6573 3d73 656c  num_features=sel
-000222c0: 662e 6e5f 6869 6464 656e 5f41 502c 0a20  f.n_hidden_AP,. 
-000222d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000222e0: 7073 3d31 652d 332c 0a20 2020 2020 2020  ps=1e-3,.       
-000222f0: 2020 2020 2020 2020 206d 6f6d 656e 7475           momentu
-00022300: 6d3d 302e 3939 2c0a 2020 2020 2020 2020  m=0.99,.        
-00022310: 2020 2020 2020 2020 6166 6669 6e65 3d54          affine=T
-00022320: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00022330: 2020 2020 2074 7261 636b 5f72 756e 6e69       track_runni
-00022340: 6e67 5f73 7461 7473 3d54 7275 6529 0a20  ng_stats=True). 
-00022350: 2020 2020 2020 2020 2020 2023 2057 6569             # Wei
-00022360: 6768 7420 6d61 7472 6978 2061 6e64 2062  ght matrix and b
-00022370: 6961 7320 6d61 7472 6978 2072 6571 7569  ias matrix requi
-00022380: 7265 6420 746f 2063 6f6d 7075 7465 206e  red to compute n
-00022390: 6577 2070 6169 7220 6c61 7965 7220 6672  ew pair layer fr
-000223a0: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
-000223b0: 7061 6972 206c 6179 6572 0a20 2020 2020  pair layer.     
-000223c0: 2020 2020 2020 2073 656c 662e 575f 5050         self.W_PP
-000223d0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-000223e0: 2069 6e69 7428 0a20 2020 2020 2020 2020   init(.         
-000223f0: 2020 2020 2020 2074 6f72 6368 2e65 6d70         torch.emp
-00022400: 7479 2873 656c 662e 6e5f 7061 6972 5f69  ty(self.n_pair_i
-00022410: 6e70 7574 5f66 6561 742c 2073 656c 662e  nput_feat, self.
-00022420: 6e5f 6869 6464 656e 5f50 5029 290a 2020  n_hidden_PP)).  
-00022430: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00022440: 5f50 503a 2074 6f72 6368 2e54 656e 736f  _PP: torch.Tenso
-00022450: 7220 3d20 746f 7263 682e 7a65 726f 7328  r = torch.zeros(
-00022460: 2873 656c 662e 6e5f 6869 6464 656e 5f50  (self.n_hidden_P
-00022470: 502c 2929 0a20 2020 2020 2020 2020 2020  P,)).           
-00022480: 2073 656c 662e 5050 5f62 6e3a 206e 6e2e   self.PP_bn: nn.
-00022490: 4261 7463 684e 6f72 6d31 6420 3d20 6e6e  BatchNorm1d = nn
-000224a0: 2e42 6174 6368 4e6f 726d 3164 280a 2020  .BatchNorm1d(.  
-000224b0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-000224c0: 6d5f 6665 6174 7572 6573 3d73 656c 662e  m_features=self.
-000224d0: 6e5f 6869 6464 656e 5f50 502c 0a20 2020  n_hidden_PP,.   
-000224e0: 2020 2020 2020 2020 2020 2020 2065 7073               eps
-000224f0: 3d31 652d 332c 0a20 2020 2020 2020 2020  =1e-3,.         
-00022500: 2020 2020 2020 206d 6f6d 656e 7475 6d3d         momentum=
-00022510: 302e 3939 2c0a 2020 2020 2020 2020 2020  0.99,.          
-00022520: 2020 2020 2020 6166 6669 6e65 3d54 7275        affine=Tru
-00022530: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00022540: 2020 2074 7261 636b 5f72 756e 6e69 6e67     track_running
-00022550: 5f73 7461 7473 3d54 7275 6529 0a0a 2020  _stats=True)..  
-00022560: 2020 2020 2020 2020 2020 7365 6c66 2e57            self.W
-00022570: 5f50 3a20 746f 7263 682e 5465 6e73 6f72  _P: torch.Tensor
-00022580: 203d 2069 6e69 7428 0a20 2020 2020 2020   = init(.       
-00022590: 2020 2020 2020 2020 2074 6f72 6368 2e65           torch.e
-000225a0: 6d70 7479 2873 656c 662e 6e5f 6869 6464  mpty(self.n_hidd
-000225b0: 656e 5f50 2c20 7365 6c66 2e6e 5f70 6169  en_P, self.n_pai
-000225c0: 725f 6f75 7470 7574 5f66 6561 7429 290a  r_output_feat)).
-000225d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000225e0: 2e62 5f50 3a20 746f 7263 682e 5465 6e73  .b_P: torch.Tens
-000225f0: 6f72 203d 2074 6f72 6368 2e7a 6572 6f73  or = torch.zeros
-00022600: 2828 7365 6c66 2e6e 5f70 6169 725f 6f75  ((self.n_pair_ou
-00022610: 7470 7574 5f66 6561 742c 2929 0a20 2020  tput_feat,)).   
-00022620: 2020 2020 2020 2020 2073 656c 662e 505f           self.P_
-00022630: 626e 3a20 6e6e 2e42 6174 6368 4e6f 726d  bn: nn.BatchNorm
-00022640: 3164 203d 206e 6e2e 4261 7463 684e 6f72  1d = nn.BatchNor
-00022650: 6d31 6428 0a20 2020 2020 2020 2020 2020  m1d(.           
-00022660: 2020 2020 206e 756d 5f66 6561 7475 7265       num_feature
-00022670: 733d 7365 6c66 2e6e 5f70 6169 725f 6f75  s=self.n_pair_ou
-00022680: 7470 7574 5f66 6561 742c 0a20 2020 2020  tput_feat,.     
-00022690: 2020 2020 2020 2020 2020 2065 7073 3d31             eps=1
-000226a0: 652d 332c 0a20 2020 2020 2020 2020 2020  e-3,.           
-000226b0: 2020 2020 206d 6f6d 656e 7475 6d3d 302e       momentum=0.
-000226c0: 3939 2c0a 2020 2020 2020 2020 2020 2020  99,.            
-000226d0: 2020 2020 6166 6669 6e65 3d54 7275 652c      affine=True,
-000226e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000226f0: 2074 7261 636b 5f72 756e 6e69 6e67 5f73   track_running_s
-00022700: 7461 7473 3d54 7275 6529 0a20 2020 2020  tats=True).     
-00022710: 2020 2073 656c 662e 6275 696c 7420 3d20     self.built = 
-00022720: 5472 7565 0a0a 2020 2020 6465 6620 5f5f  True..    def __
-00022730: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
-00022740: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-00022750: 0a20 2020 2052 6574 7572 6e73 2061 2073  .    Returns a s
-00022760: 7472 696e 6720 7265 7072 6573 656e 7461  tring representa
-00022770: 7469 6f6e 206f 6620 7468 6520 6f62 6a65  tion of the obje
-00022780: 6374 2e0a 0a20 2020 2052 6574 7572 6e73  ct...    Returns
-00022790: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  :.    -------.  
-000227a0: 2020 7374 723a 2041 2073 7472 696e 6720    str: A string 
-000227b0: 7468 6174 2063 6f6e 7461 696e 7320 7468  that contains th
-000227c0: 6520 636c 6173 7320 6e61 6d65 2066 6f6c  e class name fol
-000227d0: 6c6f 7765 6420 6279 2074 6865 2076 616c  lowed by the val
-000227e0: 7565 7320 6f66 2069 7473 2069 6e73 7461  ues of its insta
-000227f0: 6e63 6520 7661 7269 6162 6c65 2e0a 2020  nce variable..  
-00022800: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-00022810: 666c 616b 6538 3a20 6e6f 7161 0a20 2020  flake8: noqa.   
-00022820: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-00022830: 2020 2020 2020 2020 2020 6627 7b73 656c            f'{sel
-00022840: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
-00022850: 6d65 5f5f 7d28 6e5f 6174 6f6d 5f69 6e70  me__}(n_atom_inp
-00022860: 7574 5f66 6561 743a 7b73 656c 662e 6e5f  ut_feat:{self.n_
-00022870: 6174 6f6d 5f69 6e70 7574 5f66 6561 747d  atom_input_feat}
-00022880: 2c6e 5f70 6169 725f 696e 7075 745f 6665  ,n_pair_input_fe
-00022890: 6174 3a7b 7365 6c66 2e6e 5f70 6169 725f  at:{self.n_pair_
-000228a0: 696e 7075 745f 6665 6174 7d2c 6e5f 6174  input_feat},n_at
-000228b0: 6f6d 5f6f 7574 7075 745f 6665 6174 3a7b  om_output_feat:{
-000228c0: 7365 6c66 2e6e 5f61 746f 6d5f 6f75 7470  self.n_atom_outp
-000228d0: 7574 5f66 6561 747d 2c6e 5f70 6169 725f  ut_feat},n_pair_
-000228e0: 6f75 7470 7574 5f66 6561 743a 7b73 656c  output_feat:{sel
-000228f0: 662e 6e5f 7061 6972 5f6f 7574 7075 745f  f.n_pair_output_
-00022900: 6665 6174 7d2c 6e5f 6869 6464 656e 5f41  feat},n_hidden_A
-00022910: 413a 7b73 656c 662e 6e5f 6869 6464 656e  A:{self.n_hidden
-00022920: 5f41 417d 2c6e 5f68 6964 6465 6e5f 5041  _AA},n_hidden_PA
-00022930: 3a7b 7365 6c66 2e6e 5f68 6964 6465 6e5f  :{self.n_hidden_
-00022940: 5041 7d2c 6e5f 6869 6464 656e 5f41 503a  PA},n_hidden_AP:
-00022950: 7b73 656c 662e 6e5f 6869 6464 656e 5f41  {self.n_hidden_A
-00022960: 507d 2c6e 5f68 6964 6465 6e5f 5050 3a7b  P},n_hidden_PP:{
-00022970: 7365 6c66 2e6e 5f68 6964 6465 6e5f 5050  self.n_hidden_PP
-00022980: 7d2c 6261 7463 685f 6e6f 726d 616c 697a  },batch_normaliz
-00022990: 653a 7b73 656c 662e 6261 7463 685f 6e6f  e:{self.batch_no
-000229a0: 726d 616c 697a 657d 2c75 7064 6174 655f  rmalize},update_
-000229b0: 7061 6972 3a7b 7365 6c66 2e75 7064 6174  pair:{self.updat
-000229c0: 655f 7061 6972 7d2c 696e 6974 3a7b 7365  e_pair},init:{se
-000229d0: 6c66 2e69 6e69 747d 2c61 6374 6976 6174  lf.init},activat
-000229e0: 696f 6e3a 7b73 656c 662e 6163 7469 7661  ion:{self.activa
-000229f0: 7469 6f6e 7d29 270a 2020 2020 2020 2020  tion})'.        
-00022a00: 290a 0a20 2020 2064 6566 2066 6f72 7761  )..    def forwa
-00022a10: 7264 280a 2020 2020 2020 2020 7365 6c66  rd(.        self
-00022a20: 2c20 696e 7075 7473 3a20 4c69 7374 5b55  , inputs: List[U
-00022a30: 6e69 6f6e 5b6e 702e 6e64 6172 7261 792c  nion[np.ndarray,
-00022a40: 206e 702e 6e64 6172 7261 792c 206e 702e   np.ndarray, np.
-00022a50: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
-00022a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a70: 2020 2020 2020 2020 2020 6e70 2e6e 6461            np.nda
-00022a80: 7272 6179 5d5d 0a20 2020 2029 202d 3e20  rray]].    ) -> 
-00022a90: 4c69 7374 5b55 6e69 6f6e 5b74 6f72 6368  List[Union[torch
-00022aa0: 2e54 656e 736f 722c 2074 6f72 6368 2e54  .Tensor, torch.T
-00022ab0: 656e 736f 725d 5d3a 0a20 2020 2020 2020  ensor]]:.       
-00022ac0: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
-00022ad0: 2077 6561 7665 2074 656e 736f 7273 2e0a   weave tensors..
-00022ae0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00022af0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00022b00: 2020 2069 6e70 7574 733a 204c 6973 745b     inputs: List[
-00022b10: 556e 696f 6e5b 6e70 2e6e 6461 7272 6179  Union[np.ndarray
-00022b20: 2c20 6e70 2e6e 6461 7272 6179 2c20 6e70  , np.ndarray, np
-00022b30: 2e6e 6461 7272 6179 2c20 6e70 2e6e 6461  .ndarray, np.nda
-00022b40: 7272 6179 5d5d 0a20 2020 2053 686f 756c  rray]].    Shoul
-00022b50: 6420 636f 6e74 6169 6e20 3420 7465 6e73  d contain 4 tens
-00022b60: 6f72 7320 5b61 746f 6d5f 6665 6174 7572  ors [atom_featur
-00022b70: 6573 2c20 7061 6972 5f66 6561 7475 7265  es, pair_feature
-00022b80: 732c 2070 6169 725f 7370 6c69 742c 0a20  s, pair_split,. 
-00022b90: 2020 2061 746f 6d5f 746f 5f70 6169 725d     atom_to_pair]
-00022ba0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00022bb0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 204c     -------.    L
-00022bc0: 6973 745b 556e 696f 6e5b 746f 7263 682e  ist[Union[torch.
-00022bd0: 5465 6e73 6f72 2c20 746f 7263 682e 5465  Tensor, torch.Te
-00022be0: 6e73 6f72 5d5d 0a20 2020 2020 2041 3a20  nsor]].      A: 
-00022bf0: 4174 6f6d 2066 6561 7475 7265 7320 7465  Atom features te
-00022c00: 6e73 6f72 2077 6974 6820 7368 6170 655b  nsor with shape[
-00022c10: 746f 7461 6c5f 6e75 6d5f 6174 6f6d 732c  total_num_atoms,
-00022c20: 6174 6f6d 2066 6561 7475 7265 2073 697a  atom feature siz
-00022c30: 655d 0a20 2020 2020 2050 3a20 5061 6972  e].      P: Pair
-00022c40: 2066 6561 7475 7265 7320 7465 6e73 6f72   features tensor
-00022c50: 2077 6974 6820 7368 6170 655b 746f 7461   with shape[tota
-00022c60: 6c20 6e75 6d20 6f66 2070 6169 7273 2c62  l num of pairs,b
-00022c70: 6f6e 6420 6665 6174 7572 6520 7369 7a65  ond feature size
-00022c80: 5d0a 2020 2020 2222 220a 2020 2020 2020  ].    """.      
-00022c90: 2020 2320 436f 6e76 6572 7469 6e67 2074    # Converting t
-00022ca0: 6865 2069 6e70 7574 2074 6f20 746f 7263  he input to torc
-00022cb0: 6820 7465 6e73 6f72 730a 2020 2020 2020  h tensors.      
-00022cc0: 2020 6174 6f6d 5f66 6561 7475 7265 733a    atom_features:
-00022cd0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-00022ce0: 746f 7263 682e 7465 6e73 6f72 2869 6e70  torch.tensor(inp
-00022cf0: 7574 735b 305d 290a 2020 2020 2020 2020  uts[0]).        
-00022d00: 7061 6972 5f66 6561 7475 7265 733a 2074  pair_features: t
-00022d10: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00022d20: 7263 682e 7465 6e73 6f72 2869 6e70 7574  rch.tensor(input
-00022d30: 735b 315d 290a 0a20 2020 2020 2020 2070  s[1])..        p
-00022d40: 6169 725f 7370 6c69 743a 2074 6f72 6368  air_split: torch
-00022d50: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-00022d60: 7465 6e73 6f72 2869 6e70 7574 735b 325d  tensor(inputs[2]
-00022d70: 290a 2020 2020 2020 2020 6174 6f6d 5f74  ).        atom_t
-00022d80: 6f5f 7061 6972 3a20 746f 7263 682e 5465  o_pair: torch.Te
-00022d90: 6e73 6f72 203d 2074 6f72 6368 2e74 656e  nsor = torch.ten
-00022da0: 736f 7228 696e 7075 7473 5b33 5d29 0a0a  sor(inputs[3])..
-00022db0: 2020 2020 2020 2020 6163 7469 7661 7469          activati
-00022dc0: 6f6e 203d 2073 656c 662e 6163 7469 7661  on = self.activa
-00022dd0: 7469 6f6e 5f66 6e0a 0a20 2020 2020 2020  tion_fn..       
-00022de0: 2023 2041 4120 6973 2061 2074 656e 736f   # AA is a tenso
-00022df0: 7220 7769 7468 2073 6861 7065 5b74 6f74  r with shape[tot
-00022e00: 616c 5f6e 756d 5f61 746f 6d73 2c6e 5f68  al_num_atoms,n_h
-00022e10: 6964 6465 6e5f 4141 5d0a 2020 2020 2020  idden_AA].      
-00022e20: 2020 4141 3a20 746f 7263 682e 5465 6e73    AA: torch.Tens
-00022e30: 6f72 203d 2074 6f72 6368 2e6d 6174 6d75  or = torch.matmu
-00022e40: 6c28 6174 6f6d 5f66 6561 7475 7265 732e  l(atom_features.
-00022e50: 7479 7065 2874 6f72 6368 2e66 6c6f 6174  type(torch.float
-00022e60: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
-00022e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00022e90: 662e 575f 4141 2920 2b20 7365 6c66 2e62  f.W_AA) + self.b
-00022ea0: 5f41 410a 2020 2020 2020 2020 6966 2073  _AA.        if s
-00022eb0: 656c 662e 6261 7463 685f 6e6f 726d 616c  elf.batch_normal
-00022ec0: 697a 653a 0a20 2020 2020 2020 2020 2020  ize:.           
-00022ed0: 2073 656c 662e 4141 5f62 6e2e 6576 616c   self.AA_bn.eval
-00022ee0: 2829 0a20 2020 2020 2020 2020 2020 2041  ().            A
-00022ef0: 4120 3d20 7365 6c66 2e41 415f 626e 2841  A = self.AA_bn(A
-00022f00: 4129 0a20 2020 2020 2020 2041 4120 3d20  A).        AA = 
-00022f10: 6163 7469 7661 7469 6f6e 2841 4129 0a20  activation(AA). 
-00022f20: 2020 2020 2020 2023 2050 4120 6973 2061         # PA is a
-00022f30: 2074 656e 736f 7220 7769 7468 2073 6861   tensor with sha
-00022f40: 7065 5b74 6f74 616c 206e 756d 6265 7220  pe[total number 
-00022f50: 6f66 2070 6169 7273 2c6e 5f68 6964 6465  of pairs,n_hidde
-00022f60: 6e5f 5041 5d0a 2020 2020 2020 2020 5041  n_PA].        PA
-00022f70: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00022f80: 2074 6f72 6368 2e6d 6174 6d75 6c28 7061   torch.matmul(pa
-00022f90: 6972 5f66 6561 7475 7265 732e 7479 7065  ir_features.type
-00022fa0: 2874 6f72 6368 2e66 6c6f 6174 3332 292c  (torch.float32),
-00022fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022fd0: 2020 2020 2020 2020 2073 656c 662e 575f           self.W_
-00022fe0: 5041 2920 2b20 7365 6c66 2e62 5f50 410a  PA) + self.b_PA.
-00022ff0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00023000: 6261 7463 685f 6e6f 726d 616c 697a 653a  batch_normalize:
-00023010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00023020: 662e 5041 5f62 6e2e 6576 616c 2829 0a20  f.PA_bn.eval(). 
-00023030: 2020 2020 2020 2020 2020 2050 4120 3d20             PA = 
-00023040: 7365 6c66 2e50 415f 626e 2850 4129 0a20  self.PA_bn(PA). 
-00023050: 2020 2020 2020 2050 4120 3d20 6163 7469         PA = acti
-00023060: 7661 7469 6f6e 2850 4129 0a0a 2020 2020  vation(PA)..    
-00023070: 2020 2020 2320 5370 6c69 7420 7468 6520      # Split the 
-00023080: 5041 2074 656e 736f 7220 6163 636f 7264  PA tensor accord
-00023090: 696e 6720 746f 2074 6865 2027 7061 6972  ing to the 'pair
-000230a0: 5f73 706c 6974 2720 7465 6e73 6f72 0a20  _split' tensor. 
-000230b0: 2020 2020 2020 2074 5f67 7270 3a20 4469         t_grp: Di
-000230c0: 6374 5b54 656e 736f 722c 2054 656e 736f  ct[Tensor, Tenso
-000230d0: 725d 203d 207b 7d0a 2020 2020 2020 2020  r] = {}.        
-000230e0: 6964 783a 2069 6e74 203d 2030 0a20 2020  idx: int = 0.   
-000230f0: 2020 2020 2066 6f72 2069 2c20 735f 6964       for i, s_id
-00023100: 2069 6e20 656e 756d 6572 6174 6528 7061   in enumerate(pa
-00023110: 6972 5f73 706c 6974 293a 0a20 2020 2020  ir_split):.     
-00023120: 2020 2020 2020 2073 5f69 6420 3d20 735f         s_id = s_
-00023130: 6964 2e69 7465 6d28 290a 2020 2020 2020  id.item().      
-00023140: 2020 2020 2020 6966 2073 5f69 6420 696e        if s_id in
-00023150: 2074 5f67 7270 3a0a 2020 2020 2020 2020   t_grp:.        
-00023160: 2020 2020 2020 2020 745f 6772 705b 735f          t_grp[s_
-00023170: 6964 5d20 3d20 745f 6772 705b 735f 6964  id] = t_grp[s_id
-00023180: 5d20 2b20 5041 5b69 6478 5d0a 2020 2020  ] + PA[idx].    
-00023190: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000231a0: 2020 2020 2020 2020 2020 2020 2020 745f                t_
-000231b0: 6772 705b 735f 6964 5d20 3d20 5041 5b69  grp[s_id] = PA[i
-000231c0: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-000231d0: 6964 7820 3d20 6920 2b20 310a 0a20 2020  idx = i + 1..   
-000231e0: 2020 2020 2020 2020 206c 7374 203d 206c           lst = l
-000231f0: 6973 7428 745f 6772 702e 7661 6c75 6573  ist(t_grp.values
-00023200: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00023210: 7465 6e73 6f72 203d 2074 6f72 6368 2e73  tensor = torch.s
-00023220: 7461 636b 286c 7374 290a 2020 2020 2020  tack(lst).      
-00023230: 2020 5041 203d 2074 656e 736f 720a 0a20    PA = tensor.. 
-00023240: 2020 2020 2020 2041 3a20 746f 7263 682e         A: torch.
-00023250: 5465 6e73 6f72 203d 2074 6f72 6368 2e6d  Tensor = torch.m
-00023260: 6174 6d75 6c28 746f 7263 682e 636f 6e63  atmul(torch.conc
-00023270: 6174 285b 4141 2c20 5041 5d2c 2031 292c  at([AA, PA], 1),
-00023280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232a0: 2020 2020 2020 2020 7365 6c66 2e57 5f41          self.W_A
-000232b0: 2920 2b20 7365 6c66 2e62 5f41 0a20 2020  ) + self.b_A.   
-000232c0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-000232d0: 6368 5f6e 6f72 6d61 6c69 7a65 3a0a 2020  ch_normalize:.  
-000232e0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-000232f0: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
-00023300: 2020 2020 2020 2041 203d 2073 656c 662e         A = self.
-00023310: 415f 626e 2841 290a 2020 2020 2020 2020  A_bn(A).        
-00023320: 4120 3d20 6163 7469 7661 7469 6f6e 2841  A = activation(A
-00023330: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00023340: 6c66 2e75 7064 6174 655f 7061 6972 3a0a  lf.update_pair:.
-00023350: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-00023360: 7465 2074 6861 7420 4150 5f69 6a20 616e  te that AP_ij an
-00023370: 6420 4150 5f6a 6920 7368 6172 6520 7468  d AP_ji share th
-00023380: 6520 7361 6d65 2073 656c 662e 4150 5f62  e same self.AP_b
-00023390: 6e20 6261 7463 680a 2020 2020 2020 2020  n batch.        
-000233a0: 2020 2020 2320 6e6f 726d 616c 697a 6174      # normalizat
-000233b0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000233c0: 4150 5f69 6a3a 2074 6f72 6368 2e54 656e  AP_ij: torch.Ten
-000233d0: 736f 7220 3d20 746f 7263 682e 6d61 746d  sor = torch.matm
-000233e0: 756c 280a 2020 2020 2020 2020 2020 2020  ul(.            
-000233f0: 2020 2020 746f 7263 682e 7265 7368 6170      torch.reshap
-00023400: 6528 6174 6f6d 5f66 6561 7475 7265 735b  e(atom_features[
-00023410: 6174 6f6d 5f74 6f5f 7061 6972 5d2c 0a20  atom_to_pair],. 
-00023420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023430: 2020 2020 2020 2020 2020 2020 205b 2d31               [-1
-00023440: 2c20 3220 2a20 7365 6c66 2e6e 5f61 746f  , 2 * self.n_ato
-00023450: 6d5f 696e 7075 745f 6665 6174 5d29 2e74  m_input_feat]).t
-00023460: 7970 6528 0a20 2020 2020 2020 2020 2020  ype(.           
-00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023480: 2020 2020 2020 2074 6f72 6368 2e66 6c6f         torch.flo
-00023490: 6174 3332 292c 2073 656c 662e 575f 4150  at32), self.W_AP
-000234a0: 2920 2b20 7365 6c66 2e62 5f41 500a 2020  ) + self.b_AP.  
-000234b0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000234c0: 662e 6261 7463 685f 6e6f 726d 616c 697a  f.batch_normaliz
-000234d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000234e0: 2020 2073 656c 662e 4150 5f62 6e2e 6576     self.AP_bn.ev
-000234f0: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
-00023500: 2020 2020 2041 505f 696a 203d 2073 656c       AP_ij = sel
-00023510: 662e 4150 5f62 6e28 4150 5f69 6a29 0a20  f.AP_bn(AP_ij). 
-00023520: 2020 2020 2020 2020 2020 2041 505f 696a             AP_ij
-00023530: 203d 2061 6374 6976 6174 696f 6e28 4150   = activation(AP
-00023540: 5f69 6a29 0a20 2020 2020 2020 2020 2020  _ij).           
-00023550: 2041 505f 6a69 3a20 746f 7263 682e 5465   AP_ji: torch.Te
-00023560: 6e73 6f72 203d 2074 6f72 6368 2e6d 6174  nsor = torch.mat
-00023570: 6d75 6c28 0a20 2020 2020 2020 2020 2020  mul(.           
-00023580: 2020 2020 2074 6f72 6368 2e72 6573 6861       torch.resha
-00023590: 7065 2861 746f 6d5f 6665 6174 7572 6573  pe(atom_features
-000235a0: 5b74 6f72 6368 2e66 6c69 7028 6174 6f6d  [torch.flip(atom
-000235b0: 5f74 6f5f 7061 6972 2c20 5b31 5d29 5d2c  _to_pair, [1])],
-000235c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000235d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000235e0: 2d31 2c20 3220 2a20 7365 6c66 2e6e 5f61  -1, 2 * self.n_a
-000235f0: 746f 6d5f 696e 7075 745f 6665 6174 5d29  tom_input_feat])
-00023600: 2e74 7970 6528 0a20 2020 2020 2020 2020  .type(.         
-00023610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023620: 2020 2020 2020 2020 2074 6f72 6368 2e66           torch.f
-00023630: 6c6f 6174 3332 292c 2073 656c 662e 575f  loat32), self.W_
-00023640: 4150 2920 2b20 7365 6c66 2e62 5f41 500a  AP) + self.b_AP.
-00023650: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00023660: 656c 662e 6261 7463 685f 6e6f 726d 616c  elf.batch_normal
-00023670: 697a 653a 0a20 2020 2020 2020 2020 2020  ize:.           
-00023680: 2020 2020 2073 656c 662e 4150 5f62 6e2e       self.AP_bn.
-00023690: 6576 616c 2829 0a20 2020 2020 2020 2020  eval().         
-000236a0: 2020 2020 2020 2041 505f 6a69 203d 2073         AP_ji = s
-000236b0: 656c 662e 4150 5f62 6e28 4150 5f6a 6929  elf.AP_bn(AP_ji)
-000236c0: 0a20 2020 2020 2020 2020 2020 2041 505f  .            AP_
-000236d0: 6a69 203d 2061 6374 6976 6174 696f 6e28  ji = activation(
-000236e0: 4150 5f6a 6929 0a20 2020 2020 2020 2020  AP_ji).         
-000236f0: 2020 2023 2050 5020 6973 2061 2074 656e     # PP is a ten
-00023700: 736f 7220 7769 7468 2073 6861 7065 205b  sor with shape [
-00023710: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
-00023720: 7061 6972 732c 6e5f 6869 6464 656e 5f50  pairs,n_hidden_P
-00023730: 505d 0a20 2020 2020 2020 2020 2020 2050  P].            P
-00023740: 503a 2074 6f72 6368 2e54 656e 736f 7220  P: torch.Tensor 
-00023750: 3d20 746f 7263 682e 6d61 746d 756c 2870  = torch.matmul(p
-00023760: 6169 725f 6665 6174 7572 6573 2e74 7970  air_features.typ
-00023770: 6528 746f 7263 682e 666c 6f61 7433 3229  e(torch.float32)
-00023780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00023790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000237b0: 6c66 2e57 5f50 5029 202b 2073 656c 662e  lf.W_PP) + self.
-000237c0: 625f 5050 0a20 2020 2020 2020 2020 2020  b_PP.           
-000237d0: 2069 6620 7365 6c66 2e62 6174 6368 5f6e   if self.batch_n
-000237e0: 6f72 6d61 6c69 7a65 3a0a 2020 2020 2020  ormalize:.      
-000237f0: 2020 2020 2020 2020 2020 7365 6c66 2e50            self.P
-00023800: 505f 626e 2e65 7661 6c28 290a 2020 2020  P_bn.eval().    
-00023810: 2020 2020 2020 2020 2020 2020 5050 203d              PP =
-00023820: 2073 656c 662e 5050 5f62 6e28 5050 290a   self.PP_bn(PP).
-00023830: 2020 2020 2020 2020 2020 2020 5050 203d              PP =
-00023840: 2061 6374 6976 6174 696f 6e28 5050 290a   activation(PP).
-00023850: 2020 2020 2020 2020 2020 2020 503a 2074              P: t
-00023860: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00023870: 7263 682e 6d61 746d 756c 280a 2020 2020  rch.matmul(.    
-00023880: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-00023890: 682e 636f 6e63 6174 285b 4150 5f69 6a20  h.concat([AP_ij 
-000238a0: 2b20 4150 5f6a 692c 2050 505d 2c20 3129  + AP_ji, PP], 1)
-000238b0: 2e74 7970 6528 746f 7263 682e 666c 6f61  .type(torch.floa
-000238c0: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
-000238d0: 2020 2020 2020 7365 6c66 2e57 5f50 2920        self.W_P) 
-000238e0: 2b20 7365 6c66 2e62 5f50 0a20 2020 2020  + self.b_P.     
-000238f0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00023900: 6174 6368 5f6e 6f72 6d61 6c69 7a65 3a0a  atch_normalize:.
-00023910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023920: 7365 6c66 2e50 5f62 6e2e 6576 616c 2829  self.P_bn.eval()
-00023930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023940: 2050 203d 2073 656c 662e 505f 626e 2850   P = self.P_bn(P
-00023950: 290a 2020 2020 2020 2020 2020 2020 5020  ).            P 
-00023960: 3d20 6163 7469 7661 7469 6f6e 2850 290a  = activation(P).
-00023970: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00023980: 2020 2020 2020 2020 2020 5020 3d20 7061            P = pa
-00023990: 6972 5f66 6561 7475 7265 730a 0a20 2020  ir_features..   
-000239a0: 2020 2020 2072 6574 7572 6e20 5b41 2c20       return [A, 
-000239b0: 505d 0a                                  P].
+0001e4d0: 382e 0a0a 2020 2020 4578 616d 706c 6573  8...    Examples
+0001e4e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+0001e4f0: 2020 3e3e 3e20 6672 6f6d 2064 6565 7063    >>> from deepc
+0001e500: 6865 6d2e 6d6f 6465 6c73 2e74 6f72 6368  hem.models.torch
+0001e510: 5f6d 6f64 656c 7320 696d 706f 7274 206c  _models import l
+0001e520: 6179 6572 730a 2020 2020 3e3e 3e20 696d  ayers.    >>> im
+0001e530: 706f 7274 2074 6f72 6368 0a20 2020 203e  port torch.    >
+0001e540: 3e3e 2065 6d62 6564 6469 6e67 5f6c 6179  >> embedding_lay
+0001e550: 6572 203d 206c 6179 6572 732e 4454 4e4e  er = layers.DTNN
+0001e560: 456d 6265 6464 696e 6728 342c 2034 290a  Embedding(4, 4).
+0001e570: 2020 2020 3e3e 3e20 656d 6220 3d20 656d      >>> emb = em
+0001e580: 6265 6464 696e 675f 6c61 7965 7228 746f  bedding_layer(to
+0001e590: 7263 682e 5465 6e73 6f72 285b 302c 312c  rch.Tensor([0,1,
+0001e5a0: 322c 335d 292e 746f 2874 6f72 6368 2e69  2,3]).to(torch.i
+0001e5b0: 6e74 3634 2929 0a20 2020 203e 3e3e 2073  nt64)).    >>> s
+0001e5c0: 7465 705f 6c61 7965 7220 3d20 6c61 7965  tep_layer = laye
+0001e5d0: 7273 2e44 544e 4e53 7465 7028 342c 2036  rs.DTNNStep(4, 6
+0001e5e0: 2c20 3829 0a20 2020 203e 3e3e 206f 7574  , 8).    >>> out
+0001e5f0: 7075 745f 746f 7263 6820 3d20 7374 6570  put_torch = step
+0001e600: 5f6c 6179 6572 285b 0a20 2020 202e 2e2e  _layer([.    ...
+0001e610: 2020 2020 2074 6f72 6368 2e54 656e 736f       torch.Tenso
+0001e620: 7228 656d 6229 2c0a 2020 2020 2e2e 2e20  r(emb),.    ... 
+0001e630: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
+0001e640: 285b 302c 2031 2c20 322c 2033 2c20 342c  ([0, 1, 2, 3, 4,
+0001e650: 2035 5d29 2e74 6f28 746f 7263 682e 666c   5]).to(torch.fl
+0001e660: 6f61 7433 3229 2c0a 2020 2020 2e2e 2e20  oat32),.    ... 
+0001e670: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
+0001e680: 285b 315d 292e 746f 2874 6f72 6368 2e69  ([1]).to(torch.i
+0001e690: 6e74 3634 292c 0a20 2020 202e 2e2e 2020  nt64),.    ...  
+0001e6a0: 2020 2074 6f72 6368 2e54 656e 736f 7228     torch.Tensor(
+0001e6b0: 5b5b 315d 5d29 2e74 6f28 746f 7263 682e  [[1]]).to(torch.
+0001e6c0: 696e 7436 3429 0a20 2020 202e 2e2e 205d  int64).    ... ]
+0001e6d0: 290a 2020 2020 3e3e 3e20 6f75 7470 7574  ).    >>> output
+0001e6e0: 5f74 6f72 6368 2e73 6861 7065 0a20 2020  _torch.shape.   
+0001e6f0: 2074 6f72 6368 2e53 697a 6528 5b32 2c20   torch.Size([2, 
+0001e700: 342c 2034 5d29 0a0a 2020 2020 2222 220a  4, 4])..    """.
+0001e710: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0001e720: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
+0001e730: 2020 2020 2020 2020 206e 5f65 6d62 6564           n_embed
+0001e740: 6469 6e67 3a20 696e 7420 3d20 3330 2c0a  ding: int = 30,.
+0001e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e760: 206e 5f64 6973 7461 6e63 653a 2069 6e74   n_distance: int
+0001e770: 203d 2031 3030 2c0a 2020 2020 2020 2020   = 100,.        
+0001e780: 2020 2020 2020 2020 206e 5f68 6964 6465           n_hidde
+0001e790: 6e3a 2069 6e74 203d 2036 302c 0a20 2020  n: int = 60,.   
+0001e7a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0001e7b0: 6974 6961 6c69 7a65 723a 2073 7472 203d  itializer: str =
+0001e7c0: 2027 7861 7669 6572 5f75 6e69 666f 726d   'xavier_uniform
+0001e7d0: 5f27 2c0a 2020 2020 2020 2020 2020 2020  _',.            
+0001e7e0: 2020 2020 2061 6374 6976 6174 696f 6e3d       activation=
+0001e7f0: 2774 616e 6827 2c0a 2020 2020 2020 2020  'tanh',.        
+0001e800: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+0001e810: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
+0001e820: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001e830: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0001e840: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e5f  -----.        n_
+0001e850: 656d 6265 6464 696e 673a 2069 6e74 2c20  embedding: int, 
+0001e860: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001e870: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
+0001e880: 6561 7475 7265 7320 666f 7220 6561 6368  eatures for each
+0001e890: 2061 746f 6d0a 2020 2020 2020 2020 6e5f   atom.        n_
+0001e8a0: 6469 7374 616e 6365 3a20 696e 742c 206f  distance: int, o
+0001e8b0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0001e8c0: 2020 2020 6772 616e 756c 6172 6974 7920      granularity 
+0001e8d0: 6f66 2064 6973 7461 6e63 6520 6d61 7472  of distance matr
+0001e8e0: 6978 0a20 2020 2020 2020 206e 5f68 6964  ix.        n_hid
+0001e8f0: 6465 6e3a 2069 6e74 2c20 6f70 7469 6f6e  den: int, option
+0001e900: 616c 0a20 2020 2020 2020 2020 2020 204e  al.            N
+0001e910: 756d 6265 7220 6f66 206e 6f64 6573 2069  umber of nodes i
+0001e920: 6e20 6869 6464 656e 206c 6179 6572 0a20  n hidden layer. 
+0001e930: 2020 2020 2020 2069 6e69 7469 616c 697a         initializ
+0001e940: 6572 3a20 7374 722c 206f 7074 696f 6e61  er: str, optiona
+0001e950: 6c0a 2020 2020 2020 2020 2020 2020 5765  l.            We
+0001e960: 6967 6874 2069 6e69 7469 616c 697a 6174  ight initializat
+0001e970: 696f 6e20 666f 7220 6669 6c74 6572 732e  ion for filters.
+0001e980: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
+0001e990: 696f 6e73 3a20 7b78 6176 6965 725f 756e  ions: {xavier_un
+0001e9a0: 6966 6f72 6d5f 2c20 7861 7669 6572 5f6e  iform_, xavier_n
+0001e9b0: 6f72 6d61 6c5f 2c20 6b61 696d 696e 675f  ormal_, kaiming_
+0001e9c0: 756e 6966 6f72 6d5f 2c20 6b61 696d 696e  uniform_, kaimin
+0001e9d0: 675f 6e6f 726d 616c 5f2c 2074 7275 6e63  g_normal_, trunc
+0001e9e0: 5f6e 6f72 6d61 6c5f 7d0a 2020 2020 2020  _normal_}.      
+0001e9f0: 2020 6163 7469 7661 7469 6f6e 3a20 7374    activation: st
+0001ea00: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
+0001ea10: 2020 2020 2020 2020 4163 7469 7661 7469          Activati
+0001ea20: 6f6e 2066 756e 6374 696f 6e20 6170 706c  on function appl
+0001ea30: 6965 640a 0a20 2020 2020 2020 2022 2222  ied..        """
+0001ea40: 0a20 2020 2020 2020 2073 7570 6572 2844  .        super(D
+0001ea50: 544e 4e53 7465 702c 2073 656c 6629 2e5f  TNNStep, self)._
+0001ea60: 5f69 6e69 745f 5f28 2a2a 6b77 6172 6773  _init__(**kwargs
+0001ea70: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+0001ea80: 5f65 6d62 6564 6469 6e67 203d 206e 5f65  _embedding = n_e
+0001ea90: 6d62 6564 6469 6e67 0a20 2020 2020 2020  mbedding.       
+0001eaa0: 2073 656c 662e 6e5f 6469 7374 616e 6365   self.n_distance
+0001eab0: 203d 206e 5f64 6973 7461 6e63 650a 2020   = n_distance.  
+0001eac0: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
+0001ead0: 6465 6e20 3d20 6e5f 6869 6464 656e 0a20  den = n_hidden. 
+0001eae0: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+0001eaf0: 6961 6c69 7a65 7220 3d20 696e 6974 6961  ializer = initia
+0001eb00: 6c69 7a65 7220 2023 2053 6574 2077 6569  lizer  # Set wei
+0001eb10: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
+0001eb20: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+0001eb30: 6163 7469 7661 7469 6f6e 203d 2061 6374  activation = act
+0001eb40: 6976 6174 696f 6e20 2023 2047 6574 2061  ivation  # Get a
+0001eb50: 6374 6976 6174 696f 6e73 0a20 2020 2020  ctivations.     
+0001eb60: 2020 2073 656c 662e 6163 7469 7661 7469     self.activati
+0001eb70: 6f6e 5f66 6e20 3d20 6765 745f 6163 7469  on_fn = get_acti
+0001eb80: 7661 7469 6f6e 2873 656c 662e 6163 7469  vation(self.acti
+0001eb90: 7661 7469 6f6e 290a 0a20 2020 2020 2020  vation)..       
+0001eba0: 2069 6e69 745f 6675 6e63 3a20 4361 6c6c   init_func: Call
+0001ebb0: 6162 6c65 203d 2067 6574 6174 7472 2869  able = getattr(i
+0001ebc0: 6e69 7469 616c 697a 6572 732c 2073 656c  nitializers, sel
+0001ebd0: 662e 696e 6974 6961 6c69 7a65 7229 0a0a  f.initializer)..
+0001ebe0: 2020 2020 2020 2020 7365 6c66 2e57 5f63          self.W_c
+0001ebf0: 6620 3d20 6e6e 2e50 6172 616d 6574 6572  f = nn.Parameter
+0001ec00: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+0001ec10: 6974 5f66 756e 6328 746f 7263 682e 656d  it_func(torch.em
+0001ec20: 7074 7928 5b73 656c 662e 6e5f 656d 6265  pty([self.n_embe
+0001ec30: 6464 696e 672c 2073 656c 662e 6e5f 6869  dding, self.n_hi
+0001ec40: 6464 656e 5d29 2929 0a20 2020 2020 2020  dden]))).       
+0001ec50: 2073 656c 662e 575f 6466 203d 206e 6e2e   self.W_df = nn.
+0001ec60: 5061 7261 6d65 7465 7228 0a20 2020 2020  Parameter(.     
+0001ec70: 2020 2020 2020 2069 6e69 745f 6675 6e63         init_func
+0001ec80: 2874 6f72 6368 2e65 6d70 7479 285b 7365  (torch.empty([se
+0001ec90: 6c66 2e6e 5f64 6973 7461 6e63 652c 2073  lf.n_distance, s
+0001eca0: 656c 662e 6e5f 6869 6464 656e 5d29 2929  elf.n_hidden])))
+0001ecb0: 0a20 2020 2020 2020 2073 656c 662e 575f  .        self.W_
+0001ecc0: 6663 203d 206e 6e2e 5061 7261 6d65 7465  fc = nn.Paramete
+0001ecd0: 7228 0a20 2020 2020 2020 2020 2020 2069  r(.            i
+0001ece0: 6e69 745f 6675 6e63 2874 6f72 6368 2e65  nit_func(torch.e
+0001ecf0: 6d70 7479 285b 7365 6c66 2e6e 5f68 6964  mpty([self.n_hid
+0001ed00: 6465 6e2c 2073 656c 662e 6e5f 656d 6265  den, self.n_embe
+0001ed10: 6464 696e 675d 2929 290a 2020 2020 2020  dding]))).      
+0001ed20: 2020 7365 6c66 2e62 5f63 6620 3d20 6e6e    self.b_cf = nn
+0001ed30: 2e50 6172 616d 6574 6572 2874 6f72 6368  .Parameter(torch
+0001ed40: 2e7a 6572 6f73 2873 697a 653d 5b0a 2020  .zeros(size=[.  
+0001ed50: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001ed60: 5f68 6964 6465 6e2c 0a20 2020 2020 2020  _hidden,.       
+0001ed70: 205d 2929 0a20 2020 2020 2020 2073 656c   ])).        sel
+0001ed80: 662e 625f 6466 203d 206e 6e2e 5061 7261  f.b_df = nn.Para
+0001ed90: 6d65 7465 7228 746f 7263 682e 7a65 726f  meter(torch.zero
+0001eda0: 7328 7369 7a65 3d5b 0a20 2020 2020 2020  s(size=[.       
+0001edb0: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
+0001edc0: 656e 2c0a 2020 2020 2020 2020 5d29 290a  en,.        ])).
+0001edd0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+0001ede0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+0001edf0: 2022 2222 5265 7475 726e 7320 6120 7374   """Returns a st
+0001ee00: 7269 6e67 2072 6570 7265 7365 6e74 696e  ring representin
+0001ee10: 6720 7468 6520 636f 6e66 6967 7572 6174  g the configurat
+0001ee20: 696f 6e20 6f66 2074 6865 206c 6179 6572  ion of the layer
+0001ee30: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0001ee40: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0001ee50: 2d2d 0a20 2020 2020 2020 206e 5f65 6d62  --.        n_emb
+0001ee60: 6564 6469 6e67 3a20 696e 742c 206f 7074  edding: int, opt
+0001ee70: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0001ee80: 2020 4e75 6d62 6572 206f 6620 6665 6174    Number of feat
+0001ee90: 7572 6573 2066 6f72 2065 6163 6820 6174  ures for each at
+0001eea0: 6f6d 0a20 2020 2020 2020 206e 5f64 6973  om.        n_dis
+0001eeb0: 7461 6e63 653a 2069 6e74 2c20 6f70 7469  tance: int, opti
+0001eec0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0001eed0: 2067 7261 6e75 6c61 7269 7479 206f 6620   granularity of 
+0001eee0: 6469 7374 616e 6365 206d 6174 7269 780a  distance matrix.
+0001eef0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+0001ef00: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+0001ef10: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
+0001ef20: 6572 206f 6620 6e6f 6465 7320 696e 2068  er of nodes in h
+0001ef30: 6964 6465 6e20 6c61 7965 720a 2020 2020  idden layer.    
+0001ef40: 2020 2020 696e 6974 6961 6c69 7a65 723a      initializer:
+0001ef50: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+0001ef60: 2020 2020 2020 2020 2020 2057 6569 6768             Weigh
+0001ef70: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
+0001ef80: 2066 6f72 2066 696c 7465 7273 2e0a 2020   for filters..  
+0001ef90: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
+0001efa0: 733a 207b 7861 7669 6572 5f75 6e69 666f  s: {xavier_unifo
+0001efb0: 726d 5f2c 2078 6176 6965 725f 6e6f 726d  rm_, xavier_norm
+0001efc0: 616c 5f2c 206b 6169 6d69 6e67 5f75 6e69  al_, kaiming_uni
+0001efd0: 666f 726d 5f2c 206b 6169 6d69 6e67 5f6e  form_, kaiming_n
+0001efe0: 6f72 6d61 6c5f 2c20 7472 756e 635f 6e6f  ormal_, trunc_no
+0001eff0: 726d 616c 5f7d 0a20 2020 2020 2020 2061  rmal_}.        a
+0001f000: 6374 6976 6174 696f 6e3a 2073 7472 2c20  ctivation: str, 
+0001f010: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001f020: 2020 2020 2041 6374 6976 6174 696f 6e20       Activation 
+0001f030: 6675 6e63 7469 6f6e 2061 7070 6c69 6564  function applied
+0001f040: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0001f050: 2020 2020 2020 7265 7475 726e 2066 277b        return f'{
+0001f060: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+0001f070: 5f6e 616d 655f 5f7d 286e 5f65 6d62 6564  _name__}(n_embed
+0001f080: 6469 6e67 3d7b 7365 6c66 2e6e 5f65 6d62  ding={self.n_emb
+0001f090: 6564 6469 6e67 7d2c 206e 5f64 6973 7461  edding}, n_dista
+0001f0a0: 6e63 653d 7b73 656c 662e 6e5f 6469 7374  nce={self.n_dist
+0001f0b0: 616e 6365 7d2c 206e 5f68 6964 6465 6e3d  ance}, n_hidden=
+0001f0c0: 7b73 656c 662e 6e5f 6869 6464 656e 7d2c  {self.n_hidden},
+0001f0d0: 2069 6e69 7469 616c 697a 6572 3d7b 7365   initializer={se
+0001f0e0: 6c66 2e69 6e69 7469 616c 697a 6572 7d2c  lf.initializer},
+0001f0f0: 2061 6374 6976 6174 696f 6e3d 7b73 656c   activation={sel
+0001f100: 662e 6163 7469 7661 7469 6f6e 7d29 270a  f.activation})'.
+0001f110: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
+0001f120: 2873 656c 662c 2069 6e70 7574 7329 3a0a  (self, inputs):.
+0001f130: 2020 2020 2020 2020 2222 2245 7865 6375          """Execu
+0001f140: 7465 7320 7468 6520 6571 7561 7469 6f6e  tes the equation
+0001f150: 7320 616e 6420 5265 7475 726e 7320 7468  s and Returns th
+0001f160: 6520 696e 7472 6163 7469 6f6e 2076 6563  e intraction vec
+0001f170: 746f 7220 6f66 2074 6865 2061 746f 6d20  tor of the atom 
+0001f180: 7769 7468 206f 7468 6572 2061 746f 6d73  with other atoms
+0001f190: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0001f1a0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0001f1b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0001f1c0: 2069 6e70 7574 733a 2074 6f72 6368 2e54   inputs: torch.T
+0001f1d0: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
+0001f1e0: 2020 4c69 7374 206f 6620 5465 6e73 6f72    List of Tensor
+0001f1f0: 7320 6861 7669 6e67 2061 746f 6d5f 6665  s having atom_fe
+0001f200: 6174 7572 6573 2c20 6469 7374 616e 6365  atures, distance
+0001f210: 2c20 6469 7374 616e 6365 5f6d 656d 6265  , distance_membe
+0001f220: 7273 6869 705f 692c 2064 6973 7461 6e63  rship_i, distanc
+0001f230: 655f 6d65 6d62 6572 7368 6970 5f6a 2e0a  e_membership_j..
+0001f240: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001f250: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001f260: 0a20 2020 2020 2020 2069 6e74 6572 6163  .        interac
+0001f270: 7469 6f6e 5f76 6563 746f 723a 2074 6f72  tion_vector: tor
+0001f280: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+0001f290: 2020 2020 2020 696e 7465 7261 6374 696f        interactio
+0001f2a0: 6e20 6f66 2074 6865 2061 746f 6d20 7769  n of the atom wi
+0001f2b0: 7468 206f 7468 6572 2061 746f 6d73 2062  th other atoms b
+0001f2c0: 6173 6564 206f 6e20 6469 7374 616e 6365  ased on distance
+0001f2d0: 2061 6e64 2064 6973 7461 6e63 655f 6d65   and distance_me
+0001f2e0: 6d62 6572 7368 6970 2e0a 0a20 2020 2020  mbership...     
+0001f2f0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0001f300: 746f 6d5f 6665 6174 7572 6573 203d 2069  tom_features = i
+0001f310: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
+0001f320: 2064 6973 7461 6e63 6520 3d20 696e 7075   distance = inpu
+0001f330: 7473 5b31 5d0a 2020 2020 2020 2020 6469  ts[1].        di
+0001f340: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
+0001f350: 705f 6920 3d20 696e 7075 7473 5b32 5d0a  p_i = inputs[2].
+0001f360: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+0001f370: 5f6d 656d 6265 7273 6869 705f 6a20 3d20  _membership_j = 
+0001f380: 696e 7075 7473 5b33 5d0a 2020 2020 2020  inputs[3].      
+0001f390: 2020 6469 7374 616e 6365 5f68 6964 6465    distance_hidde
+0001f3a0: 6e20 3d20 746f 7263 682e 6d61 746d 756c  n = torch.matmul
+0001f3b0: 2864 6973 7461 6e63 652c 2073 656c 662e  (distance, self.
+0001f3c0: 575f 6466 2920 2b20 7365 6c66 2e62 5f64  W_df) + self.b_d
+0001f3d0: 660a 2020 2020 2020 2020 6174 6f6d 5f66  f.        atom_f
+0001f3e0: 6561 7475 7265 735f 6869 6464 656e 203d  eatures_hidden =
+0001f3f0: 2074 6f72 6368 2e6d 6174 6d75 6c28 6174   torch.matmul(at
+0001f400: 6f6d 5f66 6561 7475 7265 732c 0a20 2020  om_features,.   
+0001f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f430: 2020 2020 2020 2020 2073 656c 662e 575f           self.W_
+0001f440: 6366 2920 2b20 7365 6c66 2e62 5f63 660a  cf) + self.b_cf.
+0001f450: 2020 2020 2020 2020 6f75 7470 7574 7320          outputs 
+0001f460: 3d20 746f 7263 682e 6d75 6c28 0a20 2020  = torch.mul(.   
+0001f470: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+0001f480: 655f 6869 6464 656e 2c0a 2020 2020 2020  e_hidden,.      
+0001f490: 2020 2020 2020 746f 7263 682e 656d 6265        torch.embe
+0001f4a0: 6464 696e 6728 6174 6f6d 5f66 6561 7475  dding(atom_featu
+0001f4b0: 7265 735f 6869 6464 656e 2c20 6469 7374  res_hidden, dist
+0001f4c0: 616e 6365 5f6d 656d 6265 7273 6869 705f  ance_membership_
+0001f4d0: 6a29 290a 0a20 2020 2020 2020 2023 2066  j))..        # f
+0001f4e0: 6f72 2061 746f 6d20 6920 696e 2061 206d  or atom i in a m
+0001f4f0: 6f6c 6563 756c 6520 6d2c 2074 6869 7320  olecule m, this 
+0001f500: 7374 6570 206d 756c 7469 706c 6965 7320  step multiplies 
+0001f510: 746f 6765 7468 6572 2064 6973 7461 6e63  together distanc
+0001f520: 6520 696e 666f 206f 6620 6174 6f6d 2070  e info of atom p
+0001f530: 6169 7228 692c 6a29 0a20 2020 2020 2020  air(i,j).       
+0001f540: 2023 2061 6e64 2065 6d62 6564 6469 6e67   # and embedding
+0001f550: 7320 6f66 2061 746f 6d20 6a28 626f 7468  s of atom j(both
+0001f560: 2067 6f6e 6520 7468 726f 7567 6820 6120   gone through a 
+0001f570: 6869 6464 656e 206c 6179 6572 290a 2020  hidden layer).  
+0001f580: 2020 2020 2020 6f75 7470 7574 7320 3d20        outputs = 
+0001f590: 746f 7263 682e 6d61 746d 756c 286f 7574  torch.matmul(out
+0001f5a0: 7075 7473 2c20 7365 6c66 2e57 5f66 6329  puts, self.W_fc)
+0001f5b0: 0a20 2020 2020 2020 206f 7574 7075 7473  .        outputs
+0001f5c0: 203d 2073 656c 662e 6163 7469 7661 7469   = self.activati
+0001f5d0: 6f6e 5f66 6e28 6f75 7470 7574 7329 0a0a  on_fn(outputs)..
+0001f5e0: 2020 2020 2020 2020 6f75 7470 7574 5f69          output_i
+0001f5f0: 6920 3d20 746f 7263 682e 6d75 6c28 7365  i = torch.mul(se
+0001f600: 6c66 2e62 5f64 662c 2061 746f 6d5f 6665  lf.b_df, atom_fe
+0001f610: 6174 7572 6573 5f68 6964 6465 6e29 0a20  atures_hidden). 
+0001f620: 2020 2020 2020 206f 7574 7075 745f 6969         output_ii
+0001f630: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
+0001f640: 6f75 7470 7574 5f69 692c 2073 656c 662e  output_ii, self.
+0001f650: 575f 6663 290a 2020 2020 2020 2020 6f75  W_fc).        ou
+0001f660: 7470 7574 5f69 6920 3d20 7365 6c66 2e61  tput_ii = self.a
+0001f670: 6374 6976 6174 696f 6e5f 666e 286f 7574  ctivation_fn(out
+0001f680: 7075 745f 6969 290a 0a20 2020 2020 2020  put_ii)..       
+0001f690: 2023 2066 6f72 2061 746f 6d20 692c 2073   # for atom i, s
+0001f6a0: 756d 2074 6865 2069 6e66 6c75 656e 6365  um the influence
+0001f6b0: 2066 726f 6d20 616c 6c20 6f74 6865 7220   from all other 
+0001f6c0: 6174 6f6d 206a 2069 6e20 7468 6520 6d6f  atom j in the mo
+0001f6d0: 6c65 6375 6c65 0a20 2020 2020 2020 2069  lecule.        i
+0001f6e0: 6e74 7261 6374 696f 6e5f 7665 6374 6f72  ntraction_vector
+0001f6f0: 203d 2073 6361 7474 6572 286f 7574 7075   = scatter(outpu
+0001f700: 7473 2c20 6469 7374 616e 6365 5f6d 656d  ts, distance_mem
+0001f710: 6265 7273 6869 705f 692c 0a20 2020 2020  bership_i,.     
+0001f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f730: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001f740: 696d 3d30 2920 2d20 6f75 7470 7574 5f69  im=0) - output_i
+0001f750: 6920 2b20 6174 6f6d 5f66 6561 7475 7265  i + atom_feature
+0001f760: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+0001f770: 2069 6e74 7261 6374 696f 6e5f 7665 6374   intraction_vect
+0001f780: 6f72 0a0a 0a63 6c61 7373 2045 6467 654e  or...class EdgeN
+0001f790: 6574 776f 726b 286e 6e2e 4d6f 6475 6c65  etwork(nn.Module
+0001f7a0: 293a 0a20 2020 2022 2222 5468 6520 4564  ):.    """The Ed
+0001f7b0: 6765 4e65 7477 6f72 6b20 6d6f 6475 6c65  geNetwork module
+0001f7c0: 2069 7320 6120 5079 546f 7263 6820 7375   is a PyTorch su
+0001f7d0: 626d 6f64 756c 6520 6465 7369 676e 6564  bmodule designed
+0001f7e0: 2066 6f72 206d 6573 7361 6765 2070 6173   for message pas
+0001f7f0: 7369 6e67 2069 6e20 6772 6170 6820 6e65  sing in graph ne
+0001f800: 7572 616c 206e 6574 776f 726b 732e 0a0a  ural networks...
+0001f810: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+0001f820: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
+0001f830: 3e20 7061 6972 5f66 6561 7475 7265 7320  > pair_features 
+0001f840: 3d20 746f 7263 682e 7261 6e64 2828 342c  = torch.rand((4,
+0001f850: 2032 292c 2064 7479 7065 3d74 6f72 6368   2), dtype=torch
+0001f860: 2e66 6c6f 6174 3332 290a 2020 2020 3e3e  .float32).    >>
+0001f870: 3e20 6174 6f6d 5f66 6561 7475 7265 7320  > atom_features 
+0001f880: 3d20 746f 7263 682e 7261 6e64 2828 352c  = torch.rand((5,
+0001f890: 2032 292c 2064 7479 7065 3d74 6f72 6368   2), dtype=torch
+0001f8a0: 2e66 6c6f 6174 3332 290a 2020 2020 3e3e  .float32).    >>
+0001f8b0: 3e20 6174 6f6d 5f74 6f5f 7061 6972 203d  > atom_to_pair =
+0001f8c0: 205b 5d0a 2020 2020 3e3e 3e20 6e5f 6174   [].    >>> n_at
+0001f8d0: 6f6d 7320 3d20 320a 2020 2020 3e3e 3e20  oms = 2.    >>> 
+0001f8e0: 7374 6172 7420 3d20 300a 2020 2020 3e3e  start = 0.    >>
+0001f8f0: 3e20 4330 2c20 4331 203d 206e 702e 6d65  > C0, C1 = np.me
+0001f900: 7368 6772 6964 286e 702e 6172 616e 6765  shgrid(np.arange
+0001f910: 286e 5f61 746f 6d73 292c 206e 702e 6172  (n_atoms), np.ar
+0001f920: 616e 6765 286e 5f61 746f 6d73 2929 0a20  ange(n_atoms)). 
+0001f930: 2020 203e 3e3e 2061 746f 6d5f 746f 5f70     >>> atom_to_p
+0001f940: 6169 722e 6170 7065 6e64 286e 702e 7472  air.append(np.tr
+0001f950: 616e 7370 6f73 6528 6e70 2e61 7272 6179  anspose(np.array
+0001f960: 285b 4331 2e66 6c61 7474 656e 2829 202b  ([C1.flatten() +
+0001f970: 2073 7461 7274 2c20 4330 2e66 6c61 7474   start, C0.flatt
+0001f980: 656e 2829 202b 2073 7461 7274 5d29 2929  en() + start])))
+0001f990: 0a20 2020 203e 3e3e 2061 746f 6d5f 746f  .    >>> atom_to
+0001f9a0: 5f70 6169 7220 3d20 746f 7263 682e 5465  _pair = torch.Te
+0001f9b0: 6e73 6f72 2861 746f 6d5f 746f 5f70 6169  nsor(atom_to_pai
+0001f9c0: 7229 0a20 2020 203e 3e3e 2061 746f 6d5f  r).    >>> atom_
+0001f9d0: 746f 5f70 6169 7220 3d20 746f 7263 682e  to_pair = torch.
+0001f9e0: 7371 7565 657a 6528 6174 6f6d 5f74 6f5f  squeeze(atom_to_
+0001f9f0: 7061 6972 2e74 6f28 746f 7263 682e 696e  pair.to(torch.in
+0001fa00: 7436 3429 2c20 6469 6d3d 3029 0a20 2020  t64), dim=0).   
+0001fa10: 203e 3e3e 2069 6e70 7574 7320 3d20 5b70   >>> inputs = [p
+0001fa20: 6169 725f 6665 6174 7572 6573 2c20 6174  air_features, at
+0001fa30: 6f6d 5f66 6561 7475 7265 732c 2061 746f  om_features, ato
+0001fa40: 6d5f 746f 5f70 6169 725d 0a20 2020 203e  m_to_pair].    >
+0001fa50: 3e3e 206e 5f70 6169 725f 6665 6174 7572  >> n_pair_featur
+0001fa60: 6573 203d 2032 0a20 2020 203e 3e3e 206e  es = 2.    >>> n
+0001fa70: 5f68 6964 6465 6e20 3d20 320a 2020 2020  _hidden = 2.    
+0001fa80: 3e3e 3e20 696e 6974 203d 2027 7861 7669  >>> init = 'xavi
+0001fa90: 6572 5f75 6e69 666f 726d 5f27 0a20 2020  er_uniform_'.   
+0001faa0: 203e 3e3e 206c 6179 6572 203d 2045 6467   >>> layer = Edg
+0001fab0: 654e 6574 776f 726b 286e 5f70 6169 725f  eNetwork(n_pair_
+0001fac0: 6665 6174 7572 6573 2c20 6e5f 6869 6464  features, n_hidd
+0001fad0: 656e 2c20 696e 6974 290a 2020 2020 3e3e  en, init).    >>
+0001fae0: 3e20 7265 7375 6c74 203d 206c 6179 6572  > result = layer
+0001faf0: 2869 6e70 7574 7329 0a20 2020 203e 3e3e  (inputs).    >>>
+0001fb00: 2072 6573 756c 742e 7368 6170 655b 315d   result.shape[1]
+0001fb10: 0a20 2020 2032 0a20 2020 2022 2222 0a0a  .    2.    """..
+0001fb20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0001fb30: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+0001fb40: 2020 2020 2020 2020 6e5f 7061 6972 5f66          n_pair_f
+0001fb50: 6561 7475 7265 733a 2069 6e74 203d 2038  eatures: int = 8
+0001fb60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001fb70: 2020 206e 5f68 6964 6465 6e3a 2069 6e74     n_hidden: int
+0001fb80: 203d 2031 3030 2c0a 2020 2020 2020 2020   = 100,.        
+0001fb90: 2020 2020 2020 2020 2069 6e69 743a 2073           init: s
+0001fba0: 7472 203d 2027 7861 7669 6572 5f75 6e69  tr = 'xavier_uni
+0001fbb0: 666f 726d 5f27 2c0a 2020 2020 2020 2020  form_',.        
+0001fbc0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+0001fbd0: 7329 3a0a 2020 2020 2020 2020 2222 2249  s):.        """I
+0001fbe0: 6e69 7461 6c69 7365 7320 6120 4564 6765  nitalises a Edge
+0001fbf0: 4e65 7477 6f72 6b20 4c61 7965 720a 0a20  Network Layer.. 
+0001fc00: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001fc10: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001fc20: 2d2d 2d2d 0a20 2020 2020 2020 206e 5f70  ----.        n_p
+0001fc30: 6169 725f 6665 6174 7572 6573 3a20 696e  air_features: in
+0001fc40: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0001fc50: 2020 2020 2020 2020 5468 6520 6c65 6e67          The leng
+0001fc60: 7468 206f 6620 7468 6520 7061 6972 2066  th of the pair f
+0001fc70: 6561 7475 7265 7320 7665 6374 6f72 2e0a  eatures vector..
+0001fc80: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+0001fc90: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+0001fca0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+0001fcb0: 6572 206f 6620 6869 6464 656e 2075 6e69  er of hidden uni
+0001fcc0: 7473 2069 6e20 7468 6520 7061 7373 696e  ts in the passin
+0001fcd0: 6720 7068 6173 650a 2020 2020 2020 2020  g phase.        
+0001fce0: 696e 6974 3a20 7374 722c 206f 7074 696f  init: str, optio
+0001fcf0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0001fd00: 496e 6974 6961 6c69 7a61 7469 6f6e 2066  Initialization f
+0001fd10: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
+0001fd20: 6564 2069 6e20 7468 6520 6d65 7373 6167  ed in the messag
+0001fd30: 6520 7061 7373 696e 6720 6c61 7965 722e  e passing layer.
+0001fd40: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0001fd50: 2020 2020 2020 7375 7065 7228 4564 6765        super(Edge
+0001fd60: 4e65 7477 6f72 6b2c 2073 656c 6629 2e5f  Network, self)._
+0001fd70: 5f69 6e69 745f 5f28 2a2a 6b77 6172 6773  _init__(**kwargs
+0001fd80: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+0001fd90: 5f70 6169 725f 6665 6174 7572 6573 3a20  _pair_features: 
+0001fda0: 696e 7420 3d20 6e5f 7061 6972 5f66 6561  int = n_pair_fea
+0001fdb0: 7475 7265 730a 2020 2020 2020 2020 7365  tures.        se
+0001fdc0: 6c66 2e6e 5f68 6964 6465 6e3a 2069 6e74  lf.n_hidden: int
+0001fdd0: 203d 206e 5f68 6964 6465 6e0a 2020 2020   = n_hidden.    
+0001fde0: 2020 2020 7365 6c66 2e69 6e69 743a 2073      self.init: s
+0001fdf0: 7472 203d 2069 6e69 740a 0a20 2020 2020  tr = init..     
+0001fe00: 2020 2069 6e69 745f 6675 6e63 3a20 4361     init_func: Ca
+0001fe10: 6c6c 6162 6c65 203d 2067 6574 6174 7472  llable = getattr
+0001fe20: 2869 6e69 7469 616c 697a 6572 732c 2073  (initializers, s
+0001fe30: 656c 662e 696e 6974 290a 2020 2020 2020  elf.init).      
+0001fe40: 2020 7365 6c66 2e57 3a20 746f 7263 682e    self.W: torch.
+0001fe50: 5465 6e73 6f72 203d 2069 6e69 745f 6675  Tensor = init_fu
+0001fe60: 6e63 280a 2020 2020 2020 2020 2020 2020  nc(.            
+0001fe70: 746f 7263 682e 656d 7074 7928 5b73 656c  torch.empty([sel
+0001fe80: 662e 6e5f 7061 6972 5f66 6561 7475 7265  f.n_pair_feature
+0001fe90: 732c 2073 656c 662e 6e5f 6869 6464 656e  s, self.n_hidden
+0001fea0: 202a 2073 656c 662e 6e5f 6869 6464 656e   * self.n_hidden
+0001feb0: 5d29 290a 2020 2020 2020 2020 7365 6c66  ])).        self
+0001fec0: 2e62 3a20 746f 7263 682e 5465 6e73 6f72  .b: torch.Tensor
+0001fed0: 203d 2074 6f72 6368 2e7a 6572 6f73 2828   = torch.zeros((
+0001fee0: 7365 6c66 2e6e 5f68 6964 6465 6e20 2a20  self.n_hidden * 
+0001fef0: 7365 6c66 2e6e 5f68 6964 6465 6e2c 2929  self.n_hidden,))
+0001ff00: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+0001ff10: 696c 743a 2062 6f6f 6c20 3d20 5472 7565  ilt: bool = True
+0001ff20: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+0001ff30: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
+0001ff40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001ff50: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
+0001ff60: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
+0001ff70: 5f5f 6e61 6d65 5f5f 7d28 6e5f 7061 6972  __name__}(n_pair
+0001ff80: 5f66 6561 7475 7265 733a 7b73 656c 662e  _features:{self.
+0001ff90: 6e5f 7061 6972 5f66 6561 7475 7265 737d  n_pair_features}
+0001ffa0: 2c6e 5f68 6964 6465 6e3a 7b73 656c 662e  ,n_hidden:{self.
+0001ffb0: 6e5f 6869 6464 656e 7d2c 696e 6974 3a7b  n_hidden},init:{
+0001ffc0: 7365 6c66 2e69 6e69 747d 2927 0a20 2020  self.init})'.   
+0001ffd0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0001ffe0: 666f 7277 6172 6428 7365 6c66 2c20 696e  forward(self, in
+0001fff0: 7075 7473 3a20 4c69 7374 5b74 6f72 6368  puts: List[torch
+00020000: 2e54 656e 736f 725d 2920 2d3e 2074 6f72  .Tensor]) -> tor
+00020010: 6368 2e54 656e 736f 723a 0a20 2020 2020  ch.Tensor:.     
+00020020: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+00020030: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00020040: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00020050: 2020 2020 2069 6e70 7574 733a 204c 6973       inputs: Lis
+00020060: 745b 746f 7263 682e 5465 6e73 6f72 5d0a  t[torch.Tensor].
+00020070: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00020080: 6c65 6e67 7468 206f 6620 6174 6f6d 5f74  length of atom_t
+00020090: 6f5f 7061 6972 2073 686f 756c 6420 6265  o_pair should be
+000200a0: 2073 616d 6520 6173 206e 5f70 6169 725f   same as n_pair_
+000200b0: 6665 6174 7572 6573 2e0a 2020 2020 2020  features..      
+000200c0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000200d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000200e0: 2020 7265 7375 6c74 3a20 746f 7263 682e    result: torch.
+000200f0: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
+00020100: 2020 2054 656e 736f 7220 636f 6e74 6169     Tensor contai
+00020110: 6e69 6e67 2074 6865 206d 6170 7069 6e67  ning the mapping
+00020120: 206f 6620 7468 6520 6564 6765 2076 6563   of the edge vec
+00020130: 746f 7220 746f 2061 2064 20c3 9720 6420  tor to a d .. d 
+00020140: 6d61 7472 6978 2c20 7768 6572 6520 6420  matrix, where d 
+00020150: 6465 6e6f 7465 7320 7468 6520 6469 6d65  denotes the dime
+00020160: 6e73 696f 6e20 6f66 2074 6865 2069 6e74  nsion of the int
+00020170: 6572 6e61 6c20 6869 6464 656e 2072 6570  ernal hidden rep
+00020180: 7265 7365 6e74 6174 696f 6e20 6f66 2065  resentation of e
+00020190: 6163 6820 6e6f 6465 2069 6e20 7468 6520  ach node in the 
+000201a0: 6772 6170 682e 0a20 2020 2020 2020 2022  graph..        "
+000201b0: 2222 0a20 2020 2020 2020 2070 6169 725f  "".        pair_
+000201c0: 6665 6174 7572 6573 3a20 746f 7263 682e  features: torch.
+000201d0: 5465 6e73 6f72 0a20 2020 2020 2020 2061  Tensor.        a
+000201e0: 746f 6d5f 6665 6174 7572 6573 3a20 746f  tom_features: to
+000201f0: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+00020200: 2020 2061 746f 6d5f 746f 5f70 6169 723a     atom_to_pair:
+00020210: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
+00020220: 2020 2020 2020 7061 6972 5f66 6561 7475        pair_featu
+00020230: 7265 732c 2061 746f 6d5f 6665 6174 7572  res, atom_featur
+00020240: 6573 2c20 6174 6f6d 5f74 6f5f 7061 6972  es, atom_to_pair
+00020250: 203d 2069 6e70 7574 730a 0a20 2020 2020   = inputs..     
+00020260: 2020 2041 3a20 746f 7263 682e 5465 6e73     A: torch.Tens
+00020270: 6f72 203d 2074 6f72 6368 2e61 6464 2874  or = torch.add(t
+00020280: 6f72 6368 2e6d 6174 6d75 6c28 7061 6972  orch.matmul(pair
+00020290: 5f66 6561 7475 7265 732c 2073 656c 662e  _features, self.
+000202a0: 5729 2c20 7365 6c66 2e62 290a 2020 2020  W), self.b).    
+000202b0: 2020 2020 4120 3d20 746f 7263 682e 7265      A = torch.re
+000202c0: 7368 6170 6528 412c 2028 2d31 2c20 7365  shape(A, (-1, se
+000202d0: 6c66 2e6e 5f68 6964 6465 6e2c 2073 656c  lf.n_hidden, sel
+000202e0: 662e 6e5f 6869 6464 656e 2929 0a20 2020  f.n_hidden)).   
+000202f0: 2020 2020 206f 7574 3a20 746f 7263 682e       out: torch.
+00020300: 5465 6e73 6f72 203d 2074 6f72 6368 2e75  Tensor = torch.u
+00020310: 6e73 7175 6565 7a65 2861 746f 6d5f 6665  nsqueeze(atom_fe
+00020320: 6174 7572 6573 5b61 746f 6d5f 746f 5f70  atures[atom_to_p
+00020330: 6169 725b 3a2c 2031 5d5d 2c0a 2020 2020  air[:, 1]],.    
+00020340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020360: 2020 2020 2020 2020 6469 6d3d 3229 0a20          dim=2). 
+00020370: 2020 2020 2020 206f 7574 5f73 7175 6565         out_squee
+00020380: 7a65 3a20 746f 7263 682e 5465 6e73 6f72  ze: torch.Tensor
+00020390: 203d 2074 6f72 6368 2e73 7175 6565 7a65   = torch.squeeze
+000203a0: 2874 6f72 6368 2e6d 6174 6d75 6c28 412c  (torch.matmul(A,
+000203b0: 206f 7574 292c 2064 696d 3d32 290a 2020   out), dim=2).  
+000203c0: 2020 2020 2020 696e 643a 2074 6f72 6368        ind: torch
+000203d0: 2e54 656e 736f 7220 3d20 6174 6f6d 5f74  .Tensor = atom_t
+000203e0: 6f5f 7061 6972 5b3a 2c20 305d 0a0a 2020  o_pair[:, 0]..  
+000203f0: 2020 2020 2020 7265 7375 6c74 3a20 746f        result: to
+00020400: 7263 682e 5465 6e73 6f72 203d 2073 6567  rch.Tensor = seg
+00020410: 6d65 6e74 5f73 756d 286f 7574 5f73 7175  ment_sum(out_squ
+00020420: 6565 7a65 2c20 696e 6429 0a0a 2020 2020  eeze, ind)..    
+00020430: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00020440: 740a 0a0a 636c 6173 7320 5765 6176 654c  t...class WeaveL
+00020450: 6179 6572 286e 6e2e 4d6f 6475 6c65 293a  ayer(nn.Module):
+00020460: 0a20 2020 2022 2222 5468 6973 2063 6c61  .    """This cla
+00020470: 7373 2069 6d70 6c65 6d65 6e74 7320 7468  ss implements th
+00020480: 6520 636f 7265 2057 6561 7665 2063 6f6e  e core Weave con
+00020490: 766f 6c75 7469 6f6e 2066 726f 6d20 7468  volution from th
+000204a0: 6520 476f 6f67 6c65 2067 7261 7068 2063  e Google graph c
+000204b0: 6f6e 766f 6c75 7469 6f6e 2070 6170 6572  onvolution paper
+000204c0: 205b 315d 5f0a 2020 5468 6973 2069 7320   [1]_.  This is 
+000204d0: 7468 6520 546f 7263 6820 6571 7569 7661  the Torch equiva
+000204e0: 6c65 6e74 206f 6620 7468 6520 6f72 6967  lent of the orig
+000204f0: 696e 616c 2069 6d70 6c65 6d65 6e74 6174  inal implementat
+00020500: 696f 6e20 7573 696e 6720 4b65 7261 732e  ion using Keras.
+00020510: 0a0a 2020 5468 6973 206d 6f64 656c 2063  ..  This model c
+00020520: 6f6e 7461 696e 7320 6174 6f6d 2066 6561  ontains atom fea
+00020530: 7475 7265 7320 616e 6420 626f 6e64 2066  tures and bond f
+00020540: 6561 7475 7265 730a 2020 7365 7061 7261  eatures.  separa
+00020550: 7465 6c79 2e48 6572 652c 2062 6f6e 6420  tely.Here, bond 
+00020560: 6665 6174 7572 6573 2061 7265 2061 6c73  features are als
+00020570: 6f20 6361 6c6c 6564 2070 6169 7220 6665  o called pair fe
+00020580: 6174 7572 6573 2e0a 2020 5468 6572 6520  atures..  There 
+00020590: 6172 6520 3220 7479 7065 7320 6f66 2074  are 2 types of t
+000205a0: 7261 6e73 666f 726d 6174 696f 6e2c 2061  ransformation, a
+000205b0: 746f 6d2d 3e61 746f 6d2c 2061 746f 6d2d  tom->atom, atom-
+000205c0: 3e70 6169 722c 2070 6169 722d 3e61 746f  >pair, pair->ato
+000205d0: 6d2c 2070 6169 722d 3e70 6169 7220 7468  m, pair->pair th
+000205e0: 6174 2074 6869 7320 6d6f 6465 6c20 696d  at this model im
+000205f0: 706c 656d 656e 7473 2e0a 0a20 2045 7861  plements...  Exa
+00020600: 6d70 6c65 730a 2020 2d2d 2d2d 2d2d 2d2d  mples.  --------
+00020610: 0a20 2054 6869 7320 6c61 7965 7220 6578  .  This layer ex
+00020620: 7065 6374 7320 3420 696e 7075 7473 2069  pects 4 inputs i
+00020630: 6e20 6120 6c69 7374 206f 6620 7468 6520  n a list of the 
+00020640: 666f 726d 2060 5b61 746f 6d5f 6665 6174  form `[atom_feat
+00020650: 7572 6573 2c0a 2020 7061 6972 5f66 6561  ures,.  pair_fea
+00020660: 7475 7265 732c 2070 6169 725f 7370 6c69  tures, pair_spli
+00020670: 742c 2061 746f 6d5f 746f 5f70 6169 725d  t, atom_to_pair]
+00020680: 602e 2057 6527 6c6c 2077 616c 6b20 7468  `. We'll walk th
+00020690: 726f 7567 6820 7468 6520 7374 7275 6374  rough the struct
+000206a0: 7572 6520 6f66 2074 6865 7365 2069 6e70  ure of these inp
+000206b0: 7574 732e 204c 6574 2773 2073 7461 7274  uts. Let's start
+000206c0: 2077 6974 6820 736f 6d65 2062 6173 6963   with some basic
+000206d0: 2064 6566 696e 6974 696f 6e73 2e0a 2020   definitions..  
+000206e0: 3e3e 3e20 696d 706f 7274 2064 6565 7063  >>> import deepc
+000206f0: 6865 6d20 6173 2064 630a 2020 3e3e 3e20  hem as dc.  >>> 
+00020700: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+00020710: 6e70 0a20 203e 3e3e 2073 6d69 6c65 7320  np.  >>> smiles 
+00020720: 3d20 5b22 4343 4322 2c20 2243 225d 0a0a  = ["CCC", "C"]..
+00020730: 2020 4e6f 7465 2074 6861 7420 7468 6572    Note that ther
+00020740: 6520 6172 6520 3420 6174 6f6d 7320 696e  e are 4 atoms in
+00020750: 2074 6f74 616c 2069 6e20 7468 6973 2073   total in this s
+00020760: 7973 7465 6d2e 2054 6869 7320 6c61 7965  ystem. This laye
+00020770: 7220 6578 7065 6374 7320 6974 7320 696e  r expects its in
+00020780: 7075 7420 6d6f 6c65 6375 6c65 7320 746f  put molecules to
+00020790: 2062 6520 6261 7463 6865 6420 746f 6765   be batched toge
+000207a0: 7468 6572 2e0a 0a20 203e 3e3e 2074 6f74  ther...  >>> tot
+000207b0: 616c 5f6e 5f61 746f 6d73 203d 2034 0a0a  al_n_atoms = 4..
+000207c0: 2020 4c65 7427 7320 7375 7070 6f73 6520    Let's suppose 
+000207d0: 7468 6174 2077 6520 6861 7665 2061 2066  that we have a f
+000207e0: 6561 7475 7269 7a65 7220 7468 6174 2063  eaturizer that c
+000207f0: 6f6d 7075 7465 7320 606e 5f61 746f 6d5f  omputes `n_atom_
+00020800: 6665 6174 6020 6665 6174 7572 6573 2070  feat` features p
+00020810: 6572 2061 746f 6d2e 0a0a 2020 3e3e 3e20  er atom...  >>> 
+00020820: 6e5f 6174 6f6d 5f66 6561 7420 3d20 3735  n_atom_feat = 75
+00020830: 0a0a 2020 5468 656e 2063 6f6e 6365 7074  ..  Then concept
+00020840: 7561 6c6c 792c 2060 6174 6f6d 5f66 6561  ually, `atom_fea
+00020850: 7460 2069 7320 7468 6520 6172 7261 7920  t` is the array 
+00020860: 6f66 2073 6861 7065 2060 2874 6f74 616c  of shape `(total
+00020870: 5f6e 5f61 746f 6d73 2c0a 2020 6e5f 6174  _n_atoms,.  n_at
+00020880: 6f6d 5f66 6561 7429 6020 6f66 2061 746f  om_feat)` of ato
+00020890: 6d69 6320 6665 6174 7572 6573 2e20 466f  mic features. Fo
+000208a0: 7220 7369 6d70 6c69 6369 7479 2c20 6c65  r simplicity, le
+000208b0: 7427 7320 6a75 7374 2067 6f20 7769 7468  t's just go with
+000208c0: 2061 0a20 2072 616e 646f 6d20 7375 6368   a.  random such
+000208d0: 206d 6174 7269 782e 0a0a 2020 3e3e 3e20   matrix...  >>> 
+000208e0: 6174 6f6d 5f66 6561 7420 3d20 6e70 2e72  atom_feat = np.r
+000208f0: 616e 646f 6d2e 7261 6e64 2874 6f74 616c  andom.rand(total
+00020900: 5f6e 5f61 746f 6d73 2c20 6e5f 6174 6f6d  _n_atoms, n_atom
+00020910: 5f66 6561 7429 0a0a 2020 4c65 7427 7320  _feat)..  Let's 
+00020920: 7375 7070 6f73 6520 7765 2068 6176 6520  suppose we have 
+00020930: 606e 5f70 6169 725f 6665 6174 6020 7061  `n_pair_feat` pa
+00020940: 6972 7769 7365 2066 6561 7475 7265 730a  irwise features.
+00020950: 0a20 203e 3e3e 206e 5f70 6169 725f 6665  .  >>> n_pair_fe
+00020960: 6174 203d 2031 340a 0a20 2046 6f72 2065  at = 14..  For e
+00020970: 6163 6820 6d6f 6c65 6375 6c65 2c20 7765  ach molecule, we
+00020980: 2063 6f6d 7075 7465 2061 206d 6174 7269   compute a matri
+00020990: 7820 6f66 2073 6861 7065 2060 286e 5f61  x of shape `(n_a
+000209a0: 746f 6d73 2a6e 5f61 746f 6d73 2c0a 2020  toms*n_atoms,.  
+000209b0: 6e5f 7061 6972 5f66 6561 7429 6020 6f66  n_pair_feat)` of
+000209c0: 2070 6169 7277 6973 6520 6665 6174 7572   pairwise featur
+000209d0: 6573 2066 6f72 2065 6163 6820 7061 6972  es for each pair
+000209e0: 206f 6620 6174 6f6d 7320 696e 2074 6865   of atoms in the
+000209f0: 206d 6f6c 6563 756c 652e 0a20 204c 6574   molecule..  Let
+00020a00: 2773 2063 6f6e 7374 7275 6374 2074 6869  's construct thi
+00020a10: 7320 636f 6e63 6570 7475 616c 6c79 2066  s conceptually f
+00020a20: 6f72 206f 7572 2065 7861 6d70 6c65 2e0a  or our example..
+00020a30: 0a20 203e 3e3e 2070 6169 725f 6665 6174  .  >>> pair_feat
+00020a40: 203d 205b 6e70 2e72 616e 646f 6d2e 7261   = [np.random.ra
+00020a50: 6e64 2833 2a33 2c20 6e5f 7061 6972 5f66  nd(3*3, n_pair_f
+00020a60: 6561 7429 2c20 6e70 2e72 616e 646f 6d2e  eat), np.random.
+00020a70: 7261 6e64 2831 2a31 2c6e 5f70 6169 725f  rand(1*1,n_pair_
+00020a80: 6665 6174 295d 0a20 203e 3e3e 2070 6169  feat)].  >>> pai
+00020a90: 725f 6665 6174 203d 206e 702e 636f 6e63  r_feat = np.conc
+00020aa0: 6174 656e 6174 6528 7061 6972 5f66 6561  atenate(pair_fea
+00020ab0: 742c 2061 7869 733d 3029 0a20 203e 3e3e  t, axis=0).  >>>
+00020ac0: 2070 6169 725f 6665 6174 2e73 6861 7065   pair_feat.shape
+00020ad0: 0a20 2028 3130 2c20 3134 290a 0a20 2060  .  (10, 14)..  `
+00020ae0: 7061 6972 5f73 706c 6974 6020 6973 2061  pair_split` is a
+00020af0: 6e20 696e 6465 7820 696e 746f 2060 7061  n index into `pa
+00020b00: 6972 5f66 6561 7460 2077 6869 6368 2074  ir_feat` which t
+00020b10: 656c 6c73 2075 7320 7768 6963 6820 6174  ells us which at
+00020b20: 6f6d 2065 6163 6820 726f 7720 6265 6c6f  om each row belo
+00020b30: 6e67 7320 746f 2e20 496e 206f 7572 2063  ngs to. In our c
+00020b40: 6173 652c 2077 6520 6876 650a 0a20 203e  ase, we hve..  >
+00020b50: 3e3e 2070 6169 725f 7370 6c69 7420 3d20  >> pair_split = 
+00020b60: 6e70 2e61 7272 6179 285b 302c 2030 2c20  np.array([0, 0, 
+00020b70: 302c 2031 2c20 312c 2031 2c20 322c 2032  0, 1, 1, 1, 2, 2
+00020b80: 2c20 322c 2033 5d29 0a0a 2020 5468 6174  , 2, 3])..  That
+00020b90: 2069 732c 2074 6865 2066 6972 7374 2039   is, the first 9
+00020ba0: 2065 6e74 7269 6573 2062 656c 6f6e 6720   entries belong 
+00020bb0: 746f 2022 4343 4322 2061 6e64 2074 6865  to "CCC" and the
+00020bc0: 206c 6173 7420 656e 7472 7920 746f 2022   last entry to "
+00020bd0: 4322 2e20 5468 650a 2020 6669 6e61 6c20  C". The.  final 
+00020be0: 656e 7472 7920 6061 746f 6d5f 746f 5f70  entry `atom_to_p
+00020bf0: 6169 7260 2067 6f65 7320 696e 2061 206c  air` goes in a l
+00020c00: 6974 746c 6520 6d6f 7265 2069 6e2d 6465  ittle more in-de
+00020c10: 7074 6820 7468 616e 2060 7061 6972 5f73  pth than `pair_s
+00020c20: 706c 6974 600a 2020 616e 6420 7465 6c6c  plit`.  and tell
+00020c30: 7320 7573 2074 6865 2070 7265 6369 7365  s us the precise
+00020c40: 2070 6169 7220 6561 6368 2070 6169 7220   pair each pair 
+00020c50: 6665 6174 7572 6520 6265 6c6f 6e67 7320  feature belongs 
+00020c60: 746f 2e20 496e 206f 7572 2063 6173 650a  to. In our case.
+00020c70: 0a20 203e 3e3e 2061 746f 6d5f 746f 5f70  .  >>> atom_to_p
+00020c80: 6169 7220 3d20 6e70 2e61 7272 6179 285b  air = np.array([
+00020c90: 5b30 2c20 305d 2c0a 2020 2e2e 2e20 2020  [0, 0],.  ...   
+00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020cb0: 2020 2020 2020 205b 302c 2031 5d2c 0a20         [0, 1],. 
+00020cc0: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
+00020cd0: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
+00020ce0: 2c20 325d 2c0a 2020 2e2e 2e20 2020 2020  , 2],.  ...     
+00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d00: 2020 2020 205b 312c 2030 5d2c 0a20 202e       [1, 0],.  .
+00020d10: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
+00020d20: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+00020d30: 315d 2c0a 2020 2e2e 2e20 2020 2020 2020  1],.  ...       
+00020d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d50: 2020 205b 312c 2032 5d2c 0a20 202e 2e2e     [1, 2],.  ...
+00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d70: 2020 2020 2020 2020 2020 5b32 2c20 305d            [2, 0]
+00020d80: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
+00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020da0: 205b 322c 2031 5d2c 0a20 202e 2e2e 2020   [2, 1],.  ...  
+00020db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020dc0: 2020 2020 2020 2020 5b32 2c20 325d 2c0a          [2, 2],.
+00020dd0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
+00020de0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00020df0: 332c 2033 5d5d 290a 0a20 204c 6574 2773  3, 3]])..  Let's
+00020e00: 206e 6f77 2064 6566 696e 6520 7468 6520   now define the 
+00020e10: 6163 7475 616c 206c 6179 6572 0a0a 2020  actual layer..  
+00020e20: 3e3e 3e20 6c61 7965 7220 3d20 5765 6176  >>> layer = Weav
+00020e30: 654c 6179 6572 2829 0a0a 2020 416e 6420  eLayer()..  And 
+00020e40: 696e 766f 6b65 2069 740a 0a20 203e 3e3e  invoke it..  >>>
+00020e50: 205b 412c 2050 5d20 3d20 6c61 7965 7228   [A, P] = layer(
+00020e60: 5b61 746f 6d5f 6665 6174 2c20 7061 6972  [atom_feat, pair
+00020e70: 5f66 6561 742c 2070 6169 725f 7370 6c69  _feat, pair_spli
+00020e80: 742c 2061 746f 6d5f 746f 5f70 6169 725d  t, atom_to_pair]
+00020e90: 290a 0a20 2054 6865 2077 6561 7665 206c  )..  The weave l
+00020ea0: 6179 6572 2070 726f 6475 6365 7320 6e65  ayer produces ne
+00020eb0: 7720 6174 6f6d 2f70 6169 7220 6665 6174  w atom/pair feat
+00020ec0: 7572 6573 2e20 4c65 7427 7320 6368 6563  ures. Let's chec
+00020ed0: 6b20 7468 6569 7220 7368 6170 6573 0a0a  k their shapes..
+00020ee0: 2020 3e3e 3e20 4120 3d20 412e 6465 7461    >>> A = A.deta
+00020ef0: 6368 2829 2e6e 756d 7079 2829 0a20 203e  ch().numpy().  >
+00020f00: 3e3e 2041 2e73 6861 7065 0a20 2028 342c  >> A.shape.  (4,
+00020f10: 2035 3029 0a20 203e 3e3e 2050 203d 2050   50).  >>> P = P
+00020f20: 2e64 6574 6163 6828 292e 6e75 6d70 7928  .detach().numpy(
+00020f30: 290a 2020 3e3e 3e20 502e 7368 6170 650a  ).  >>> P.shape.
+00020f40: 2020 2831 302c 2035 3029 0a0a 2020 5468    (10, 50)..  Th
+00020f50: 6520 3420 6973 2060 746f 7461 6c5f 6e75  e 4 is `total_nu
+00020f60: 6d5f 6174 6f6d 7360 2061 6e64 2074 6865  m_atoms` and the
+00020f70: 2031 3020 6973 2074 6865 2074 6f74 616c   10 is the total
+00020f80: 206e 756d 6265 7220 6f66 2070 6169 7273   number of pairs
+00020f90: 2e20 5768 6572 650a 2020 646f 6573 2060  . Where.  does `
+00020fa0: 3530 6020 636f 6d65 2066 726f 6d3f 2049  50` come from? I
+00020fb0: 7427 7320 6672 6f6d 2074 6865 2064 6566  t's from the def
+00020fc0: 6175 6c74 2061 7267 756d 656e 7473 2060  ault arguments `
+00020fd0: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
+00020fe0: 7460 2061 6e64 0a20 2060 6e5f 7061 6972  t` and.  `n_pair
+00020ff0: 5f69 6e70 7574 5f66 6561 7460 2e0a 0a20  _input_feat`... 
+00021000: 2052 6566 6572 656e 6365 730a 2020 2d2d   References.  --
+00021010: 2d2d 2d2d 2d2d 2d2d 0a20 202e 2e20 5b31  --------.  .. [1
+00021020: 5d20 4b65 6172 6e65 732c 2053 7465 7665  ] Kearnes, Steve
+00021030: 6e2c 2065 7420 616c 2e20 224d 6f6c 6563  n, et al. "Molec
+00021040: 756c 6172 2067 7261 7068 2063 6f6e 766f  ular graph convo
+00021050: 6c75 7469 6f6e 733a 206d 6f76 696e 6720  lutions: moving 
+00021060: 6265 796f 6e64 0a20 2020 2020 2020 2066  beyond.        f
+00021070: 696e 6765 7270 7269 6e74 732e 2220 4a6f  ingerprints." Jo
+00021080: 7572 6e61 6c20 6f66 2063 6f6d 7075 7465  urnal of compute
+00021090: 722d 6169 6465 6420 6d6f 6c65 6375 6c61  r-aided molecula
+000210a0: 7220 6465 7369 676e 2033 302e 3820 2832  r design 30.8 (2
+000210b0: 3031 3629 3a0a 2020 2020 2020 2020 3539  016):.        59
+000210c0: 352d 3630 382e 0a20 2022 2222 0a0a 2020  5-608..  """..  
+000210d0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+000210e0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000210f0: 2020 2020 2020 6e5f 6174 6f6d 5f69 6e70        n_atom_inp
+00021100: 7574 5f66 6561 743a 2069 6e74 203d 2037  ut_feat: int = 7
+00021110: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+00021120: 2020 2020 6e5f 7061 6972 5f69 6e70 7574      n_pair_input
+00021130: 5f66 6561 743a 2069 6e74 203d 2031 342c  _feat: int = 14,
+00021140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021150: 2020 6e5f 6174 6f6d 5f6f 7574 7075 745f    n_atom_output_
+00021160: 6665 6174 3a20 696e 7420 3d20 3530 2c0a  feat: int = 50,.
+00021170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021180: 206e 5f70 6169 725f 6f75 7470 7574 5f66   n_pair_output_f
+00021190: 6561 743a 2069 6e74 203d 2035 302c 0a20  eat: int = 50,. 
+000211a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211b0: 6e5f 6869 6464 656e 5f41 413a 2069 6e74  n_hidden_AA: int
+000211c0: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
+000211d0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+000211e0: 5f50 413a 2069 6e74 203d 2035 302c 0a20  _PA: int = 50,. 
+000211f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021200: 6e5f 6869 6464 656e 5f41 503a 2069 6e74  n_hidden_AP: int
+00021210: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
+00021220: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+00021230: 5f50 503a 2069 6e74 203d 2035 302c 0a20  _PP: int = 50,. 
+00021240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021250: 7570 6461 7465 5f70 6169 723a 2062 6f6f  update_pair: boo
+00021260: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+00021270: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
+00021280: 3a20 7374 7220 3d20 2778 6176 6965 725f  : str = 'xavier_
+00021290: 756e 6966 6f72 6d5f 272c 0a20 2020 2020  uniform_',.     
+000212a0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+000212b0: 7661 7469 6f6e 3a20 7374 7220 3d20 2772  vation: str = 'r
+000212c0: 656c 7527 2c0a 2020 2020 2020 2020 2020  elu',.          
+000212d0: 2020 2020 2020 2062 6174 6368 5f6e 6f72         batch_nor
+000212e0: 6d61 6c69 7a65 3a20 626f 6f6c 203d 2054  malize: bool = T
+000212f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00021300: 2020 2020 2020 2a2a 6b77 6172 6773 293a        **kwargs):
+00021310: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00021320: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00021330: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
+00021340: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
+00021350: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
+00021360: 2864 6566 6175 6c74 2037 3529 0a20 2020  (default 75).   
+00021370: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
+00021380: 7475 7265 7320 666f 7220 6561 6368 2061  tures for each a
+00021390: 746f 6d20 696e 2069 6e70 7574 2e0a 2020  tom in input..  
+000213a0: 2020 6e5f 7061 6972 5f69 6e70 7574 5f66    n_pair_input_f
+000213b0: 6561 743a 2069 6e74 2c20 6f70 7469 6f6e  eat: int, option
+000213c0: 616c 2028 6465 6661 756c 7420 3134 290a  al (default 14).
+000213d0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+000213e0: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
+000213f0: 6820 7061 6972 206f 6620 6174 6f6d 7320  h pair of atoms 
+00021400: 696e 2069 6e70 7574 2e0a 2020 2020 6e5f  in input..    n_
+00021410: 6174 6f6d 5f6f 7574 7075 745f 6665 6174  atom_output_feat
+00021420: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
+00021430: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
+00021440: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
+00021450: 7475 7265 7320 666f 7220 6561 6368 2061  tures for each a
+00021460: 746f 6d20 696e 206f 7574 7075 742e 0a20  tom in output.. 
+00021470: 2020 206e 5f70 6169 725f 6f75 7470 7574     n_pair_output
+00021480: 5f66 6561 743a 2069 6e74 2c20 6f70 7469  _feat: int, opti
+00021490: 6f6e 616c 2028 6465 6661 756c 7420 3530  onal (default 50
+000214a0: 290a 2020 2020 2020 4e75 6d62 6572 206f  ).      Number o
+000214b0: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
+000214c0: 6163 6820 7061 6972 206f 6620 6174 6f6d  ach pair of atom
+000214d0: 7320 696e 206f 7574 7075 742e 0a20 2020  s in output..   
+000214e0: 206e 5f68 6964 6465 6e5f 4141 3a20 696e   n_hidden_AA: in
+000214f0: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
+00021500: 6175 6c74 2035 3029 0a20 2020 2020 204e  ault 50).      N
+00021510: 756d 6265 7220 6f66 2075 6e69 7473 2863  umber of units(c
+00021520: 6f6e 766f 6c75 7469 6f6e 2064 6570 7468  onvolution depth
+00021530: 7329 2069 6e20 636f 7272 6573 706f 6e64  s) in correspond
+00021540: 696e 6720 6869 6464 656e 206c 6179 6572  ing hidden layer
+00021550: 0a20 2020 206e 5f68 6964 6465 6e5f 5041  .    n_hidden_PA
+00021560: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
+00021570: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
+00021580: 2020 204e 756d 6265 7220 6f66 2075 6e69     Number of uni
+00021590: 7473 2863 6f6e 766f 6c75 7469 6f6e 2064  ts(convolution d
+000215a0: 6570 7468 7329 2069 6e20 636f 7272 6573  epths) in corres
+000215b0: 706f 6e64 696e 6720 6869 6464 656e 206c  ponding hidden l
+000215c0: 6179 6572 0a20 2020 206e 5f68 6964 6465  ayer.    n_hidde
+000215d0: 6e5f 4150 3a20 696e 742c 206f 7074 696f  n_AP: int, optio
+000215e0: 6e61 6c20 2864 6566 6175 6c74 2035 3029  nal (default 50)
+000215f0: 0a20 2020 2020 204e 756d 6265 7220 6f66  .      Number of
+00021600: 2075 6e69 7473 2863 6f6e 766f 6c75 7469   units(convoluti
+00021610: 6f6e 2064 6570 7468 7329 2069 6e20 636f  on depths) in co
+00021620: 7272 6573 706f 6e64 696e 6720 6869 6464  rresponding hidd
+00021630: 656e 206c 6179 6572 0a20 2020 206e 5f68  en layer.    n_h
+00021640: 6964 6465 6e5f 5050 3a20 696e 742c 206f  idden_PP: int, o
+00021650: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
+00021660: 2035 3029 0a20 2020 2020 204e 756d 6265   50).      Numbe
+00021670: 7220 6f66 2075 6e69 7473 2863 6f6e 766f  r of units(convo
+00021680: 6c75 7469 6f6e 2064 6570 7468 7329 2069  lution depths) i
+00021690: 6e20 636f 7272 6573 706f 6e64 696e 6720  n corresponding 
+000216a0: 6869 6464 656e 206c 6179 6572 0a20 2020  hidden layer.   
+000216b0: 2075 7064 6174 655f 7061 6972 3a20 626f   update_pair: bo
+000216c0: 6f6c 2c20 6f70 7469 6f6e 616c 2028 6465  ol, optional (de
+000216d0: 6661 756c 7420 5472 7565 290a 2020 2020  fault True).    
+000216e0: 2020 5768 6574 6865 7220 746f 2063 616c    Whether to cal
+000216f0: 6375 6c61 7465 2066 6f72 2070 6169 7220  culate for pair 
+00021700: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
+00021710: 636f 756c 6420 6265 2074 7572 6e65 6420  could be turned 
+00021720: 6f66 6620 666f 7220 6c61 7374 206c 6179  off for last lay
+00021730: 6572 0a20 2020 2069 6e69 743a 2073 7472  er.    init: str
+00021740: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
+00021750: 756c 7420 2778 6176 6965 725f 756e 6966  ult 'xavier_unif
+00021760: 6f72 6d5f 2729 0a20 2020 2020 2057 6569  orm_').      Wei
+00021770: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
+00021780: 6f6e 2066 6f72 2066 696c 7465 7273 2e0a  on for filters..
+00021790: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
+000217a0: 7374 722c 206f 7074 696f 6e61 6c20 2864  str, optional (d
+000217b0: 6566 6175 6c74 2027 7265 6c75 2729 0a20  efault 'relu'). 
+000217c0: 2020 2020 2041 6374 6976 6174 696f 6e20       Activation 
+000217d0: 6675 6e63 7469 6f6e 2061 7070 6c69 6564  function applied
+000217e0: 0a20 2020 2062 6174 6368 5f6e 6f72 6d61  .    batch_norma
+000217f0: 6c69 7a65 3a20 626f 6f6c 2c20 6f70 7469  lize: bool, opti
+00021800: 6f6e 616c 2028 6465 6661 756c 7420 5472  onal (default Tr
+00021810: 7565 290a 2020 2020 2020 4966 2074 6869  ue).      If thi
+00021820: 7320 6973 2074 7572 6e65 6420 6f6e 2c20  s is turned on, 
+00021830: 6170 706c 7920 6261 7463 6820 6e6f 726d  apply batch norm
+00021840: 616c 697a 6174 696f 6e20 6265 666f 7265  alization before
+00021850: 2061 7070 6c79 696e 670a 2020 2020 2020   applying.      
+00021860: 6163 7469 7661 7469 6f6e 2066 756e 6374  activation funct
+00021870: 696f 6e73 206f 6e20 636f 6e76 6f6c 7574  ions on convolut
+00021880: 696f 6e61 6c20 6c61 7965 7273 2e0a 2020  ional layers..  
+00021890: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
+000218a0: 7065 7228 5765 6176 654c 6179 6572 2c20  per(WeaveLayer, 
+000218b0: 7365 6c66 292e 5f5f 696e 6974 5f5f 282a  self).__init__(*
+000218c0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+000218d0: 2073 656c 662e 696e 6974 3a20 7374 7220   self.init: str 
+000218e0: 3d20 696e 6974 5f20 2023 2053 6574 2077  = init_  # Set w
+000218f0: 6569 6768 7420 696e 6974 6961 6c69 7a61  eight initializa
+00021900: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
+00021910: 662e 6163 7469 7661 7469 6f6e 3a20 7374  f.activation: st
+00021920: 7220 3d20 6163 7469 7661 7469 6f6e 2020  r = activation  
+00021930: 2320 4765 7420 6163 7469 7661 7469 6f6e  # Get activation
+00021940: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
+00021950: 6374 6976 6174 696f 6e5f 666e 3a20 746f  ctivation_fn: to
+00021960: 7263 682e 6e6e 2e4d 6f64 756c 6520 3d20  rch.nn.Module = 
+00021970: 6765 745f 6163 7469 7661 7469 6f6e 2861  get_activation(a
+00021980: 6374 6976 6174 696f 6e29 0a20 2020 2020  ctivation).     
+00021990: 2020 2073 656c 662e 7570 6461 7465 5f70     self.update_p
+000219a0: 6169 723a 2062 6f6f 6c20 3d20 7570 6461  air: bool = upda
+000219b0: 7465 5f70 6169 7220 2023 206c 6173 7420  te_pair  # last 
+000219c0: 7765 6176 6520 6c61 7965 7220 646f 6573  weave layer does
+000219d0: 206e 6f74 206e 6565 6420 746f 2075 7064   not need to upd
+000219e0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
+000219f0: 2e6e 5f68 6964 6465 6e5f 4141 3a20 696e  .n_hidden_AA: in
+00021a00: 7420 3d20 6e5f 6869 6464 656e 5f41 410a  t = n_hidden_AA.
+00021a10: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
+00021a20: 6964 6465 6e5f 5041 3a20 696e 7420 3d20  idden_PA: int = 
+00021a30: 6e5f 6869 6464 656e 5f50 410a 2020 2020  n_hidden_PA.    
+00021a40: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
+00021a50: 6e5f 4150 3a20 696e 7420 3d20 6e5f 6869  n_AP: int = n_hi
+00021a60: 6464 656e 5f41 500a 2020 2020 2020 2020  dden_AP.        
+00021a70: 7365 6c66 2e6e 5f68 6964 6465 6e5f 5050  self.n_hidden_PP
+00021a80: 3a20 696e 7420 3d20 6e5f 6869 6464 656e  : int = n_hidden
+00021a90: 5f50 500a 2020 2020 2020 2020 7365 6c66  _PP.        self
+00021aa0: 2e6e 5f68 6964 6465 6e5f 413a 2069 6e74  .n_hidden_A: int
+00021ab0: 203d 206e 5f68 6964 6465 6e5f 4141 202b   = n_hidden_AA +
+00021ac0: 206e 5f68 6964 6465 6e5f 5041 0a20 2020   n_hidden_PA.   
+00021ad0: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
+00021ae0: 656e 5f50 3a20 696e 7420 3d20 6e5f 6869  en_P: int = n_hi
+00021af0: 6464 656e 5f41 5020 2b20 6e5f 6869 6464  dden_AP + n_hidd
+00021b00: 656e 5f50 500a 2020 2020 2020 2020 7365  en_PP.        se
+00021b10: 6c66 2e62 6174 6368 5f6e 6f72 6d61 6c69  lf.batch_normali
+00021b20: 7a65 3a20 626f 6f6c 203d 2062 6174 6368  ze: bool = batch
+00021b30: 5f6e 6f72 6d61 6c69 7a65 0a0a 2020 2020  _normalize..    
+00021b40: 2020 2020 7365 6c66 2e6e 5f61 746f 6d5f      self.n_atom_
+00021b50: 696e 7075 745f 6665 6174 3a20 696e 7420  input_feat: int 
+00021b60: 3d20 6e5f 6174 6f6d 5f69 6e70 7574 5f66  = n_atom_input_f
+00021b70: 6561 740a 2020 2020 2020 2020 7365 6c66  eat.        self
+00021b80: 2e6e 5f70 6169 725f 696e 7075 745f 6665  .n_pair_input_fe
+00021b90: 6174 3a20 696e 7420 3d20 6e5f 7061 6972  at: int = n_pair
+00021ba0: 5f69 6e70 7574 5f66 6561 740a 2020 2020  _input_feat.    
+00021bb0: 2020 2020 7365 6c66 2e6e 5f61 746f 6d5f      self.n_atom_
+00021bc0: 6f75 7470 7574 5f66 6561 743a 2069 6e74  output_feat: int
+00021bd0: 203d 206e 5f61 746f 6d5f 6f75 7470 7574   = n_atom_output
+00021be0: 5f66 6561 740a 2020 2020 2020 2020 7365  _feat.        se
+00021bf0: 6c66 2e6e 5f70 6169 725f 6f75 7470 7574  lf.n_pair_output
+00021c00: 5f66 6561 743a 2069 6e74 203d 206e 5f70  _feat: int = n_p
+00021c10: 6169 725f 6f75 7470 7574 5f66 6561 740a  air_output_feat.
+00021c20: 0a20 2020 2020 2020 2023 2043 6f6e 7374  .        # Const
+00021c30: 7275 6374 2069 6e74 6572 6e61 6c20 7472  ruct internal tr
+00021c40: 6169 6e61 626c 6520 7765 6967 6874 730a  ainable weights.
+00021c50: 2020 2020 2020 2020 696e 6974 203d 2067          init = g
+00021c60: 6574 6174 7472 2869 6e69 7469 616c 697a  etattr(initializ
+00021c70: 6572 732c 2073 656c 662e 696e 6974 290a  ers, self.init).
+00021c80: 2020 2020 2020 2020 2320 5765 6967 6874          # Weight
+00021c90: 206d 6174 7269 7820 616e 6420 6269 6173   matrix and bias
+00021ca0: 206d 6174 7269 7820 7265 7175 6972 6564   matrix required
+00021cb0: 2074 6f20 636f 6d70 7574 6520 6e65 7720   to compute new 
+00021cc0: 6174 6f6d 206c 6179 6572 2066 726f 6d20  atom layer from 
+00021cd0: 7468 6520 7072 6576 696f 7573 2061 746f  the previous ato
+00021ce0: 6d20 6c61 7965 720a 2020 2020 2020 2020  m layer.        
+00021cf0: 7365 6c66 2e57 5f41 413a 2074 6f72 6368  self.W_AA: torch
+00021d00: 2e54 656e 736f 7220 3d20 696e 6974 280a  .Tensor = init(.
+00021d10: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+00021d20: 682e 656d 7074 7928 7365 6c66 2e6e 5f61  h.empty(self.n_a
+00021d30: 746f 6d5f 696e 7075 745f 6665 6174 2c20  tom_input_feat, 
+00021d40: 7365 6c66 2e6e 5f68 6964 6465 6e5f 4141  self.n_hidden_AA
+00021d50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00021d60: 625f 4141 3a20 746f 7263 682e 5465 6e73  b_AA: torch.Tens
+00021d70: 6f72 203d 2074 6f72 6368 2e7a 6572 6f73  or = torch.zeros
+00021d80: 2828 7365 6c66 2e6e 5f68 6964 6465 6e5f  ((self.n_hidden_
+00021d90: 4141 2c29 290a 2020 2020 2020 2020 7365  AA,)).        se
+00021da0: 6c66 2e41 415f 626e 3a20 6e6e 2e42 6174  lf.AA_bn: nn.Bat
+00021db0: 6368 4e6f 726d 3164 203d 206e 6e2e 4261  chNorm1d = nn.Ba
+00021dc0: 7463 684e 6f72 6d31 6428 0a20 2020 2020  tchNorm1d(.     
+00021dd0: 2020 2020 2020 206e 756d 5f66 6561 7475         num_featu
+00021de0: 7265 733d 7365 6c66 2e6e 5f68 6964 6465  res=self.n_hidde
+00021df0: 6e5f 4141 2c0a 2020 2020 2020 2020 2020  n_AA,.          
+00021e00: 2020 6570 733d 3165 2d33 2c0a 2020 2020    eps=1e-3,.    
+00021e10: 2020 2020 2020 2020 6d6f 6d65 6e74 756d          momentum
+00021e20: 3d30 2e39 392c 0a20 2020 2020 2020 2020  =0.99,.         
+00021e30: 2020 2061 6666 696e 653d 5472 7565 2c0a     affine=True,.
+00021e40: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00021e50: 6b5f 7275 6e6e 696e 675f 7374 6174 733d  k_running_stats=
+00021e60: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
+00021e70: 2057 6569 6768 7420 6d61 7472 6978 2061   Weight matrix a
+00021e80: 6e64 2062 6961 7320 6d61 7472 6978 2072  nd bias matrix r
+00021e90: 6571 7569 7265 6420 746f 2063 6f6d 7075  equired to compu
+00021ea0: 7465 206e 6577 2061 746f 6d20 6c61 7965  te new atom laye
+00021eb0: 7220 6672 6f6d 2074 6865 2070 7265 7669  r from the previ
+00021ec0: 6f75 7320 7061 6972 206c 6179 6572 0a20  ous pair layer. 
+00021ed0: 2020 2020 2020 2073 656c 662e 575f 5041         self.W_PA
+00021ee0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+00021ef0: 2069 6e69 7428 0a20 2020 2020 2020 2020   init(.         
+00021f00: 2020 2074 6f72 6368 2e65 6d70 7479 2873     torch.empty(s
+00021f10: 656c 662e 6e5f 7061 6972 5f69 6e70 7574  elf.n_pair_input
+00021f20: 5f66 6561 742c 2073 656c 662e 6e5f 6869  _feat, self.n_hi
+00021f30: 6464 656e 5f50 4129 290a 2020 2020 2020  dden_PA)).      
+00021f40: 2020 7365 6c66 2e62 5f50 413a 2074 6f72    self.b_PA: tor
+00021f50: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00021f60: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
+00021f70: 6869 6464 656e 5f50 412c 2929 0a20 2020  hidden_PA,)).   
+00021f80: 2020 2020 2073 656c 662e 5041 5f62 6e3a       self.PA_bn:
+00021f90: 206e 6e2e 4261 7463 684e 6f72 6d31 6420   nn.BatchNorm1d 
+00021fa0: 3d20 6e6e 2e42 6174 6368 4e6f 726d 3164  = nn.BatchNorm1d
+00021fb0: 280a 2020 2020 2020 2020 2020 2020 6e75  (.            nu
+00021fc0: 6d5f 6665 6174 7572 6573 3d73 656c 662e  m_features=self.
+00021fd0: 6e5f 6869 6464 656e 5f50 412c 0a20 2020  n_hidden_PA,.   
+00021fe0: 2020 2020 2020 2020 2065 7073 3d31 652d           eps=1e-
+00021ff0: 332c 0a20 2020 2020 2020 2020 2020 206d  3,.            m
+00022000: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
+00022010: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
+00022020: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00022030: 2020 2074 7261 636b 5f72 756e 6e69 6e67     track_running
+00022040: 5f73 7461 7473 3d54 7275 6529 0a0a 2020  _stats=True)..  
+00022050: 2020 2020 2020 7365 6c66 2e57 5f41 3a20        self.W_A: 
+00022060: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
+00022070: 6e69 7428 0a20 2020 2020 2020 2020 2020  nit(.           
+00022080: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
+00022090: 662e 6e5f 6869 6464 656e 5f41 2c20 7365  f.n_hidden_A, se
+000220a0: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
+000220b0: 5f66 6561 7429 290a 2020 2020 2020 2020  _feat)).        
+000220c0: 7365 6c66 2e62 5f41 3a20 746f 7263 682e  self.b_A: torch.
+000220d0: 5465 6e73 6f72 203d 2074 6f72 6368 2e7a  Tensor = torch.z
+000220e0: 6572 6f73 2828 7365 6c66 2e6e 5f61 746f  eros((self.n_ato
+000220f0: 6d5f 6f75 7470 7574 5f66 6561 742c 2929  m_output_feat,))
+00022100: 0a20 2020 2020 2020 2073 656c 662e 415f  .        self.A_
+00022110: 626e 3a20 6e6e 2e42 6174 6368 4e6f 726d  bn: nn.BatchNorm
+00022120: 3164 203d 206e 6e2e 4261 7463 684e 6f72  1d = nn.BatchNor
+00022130: 6d31 6428 0a20 2020 2020 2020 2020 2020  m1d(.           
+00022140: 206e 756d 5f66 6561 7475 7265 733d 7365   num_features=se
+00022150: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
+00022160: 5f66 6561 742c 0a20 2020 2020 2020 2020  _feat,.         
+00022170: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
+00022180: 2020 2020 2020 2020 206d 6f6d 656e 7475           momentu
+00022190: 6d3d 302e 3939 2c0a 2020 2020 2020 2020  m=0.99,.        
+000221a0: 2020 2020 6166 6669 6e65 3d54 7275 652c      affine=True,
+000221b0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+000221c0: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
+000221d0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+000221e0: 6966 2073 656c 662e 7570 6461 7465 5f70  if self.update_p
+000221f0: 6169 723a 0a20 2020 2020 2020 2020 2020  air:.           
+00022200: 2023 2057 6569 6768 7420 6d61 7472 6978   # Weight matrix
+00022210: 2061 6e64 2062 6961 7320 6d61 7472 6978   and bias matrix
+00022220: 2072 6571 7569 7265 6420 746f 2063 6f6d   required to com
+00022230: 7075 7465 206e 6577 2070 6169 7220 6c61  pute new pair la
+00022240: 7965 7220 6672 6f6d 2074 6865 2070 7265  yer from the pre
+00022250: 7669 6f75 7320 6174 6f6d 206c 6179 6572  vious atom layer
+00022260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00022270: 662e 575f 4150 3a20 746f 7263 682e 5465  f.W_AP: torch.Te
+00022280: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
+00022290: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
+000222a0: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
+000222b0: 6174 6f6d 5f69 6e70 7574 5f66 6561 7420  atom_input_feat 
+000222c0: 2a20 322c 2073 656c 662e 6e5f 6869 6464  * 2, self.n_hidd
+000222d0: 656e 5f41 5029 290a 2020 2020 2020 2020  en_AP)).        
+000222e0: 2020 2020 7365 6c66 2e62 5f41 503a 2074      self.b_AP: t
+000222f0: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00022300: 7263 682e 7a65 726f 7328 2873 656c 662e  rch.zeros((self.
+00022310: 6e5f 6869 6464 656e 5f41 502c 2929 0a20  n_hidden_AP,)). 
+00022320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00022330: 4150 5f62 6e3a 206e 6e2e 4261 7463 684e  AP_bn: nn.BatchN
+00022340: 6f72 6d31 6420 3d20 6e6e 2e42 6174 6368  orm1d = nn.Batch
+00022350: 4e6f 726d 3164 280a 2020 2020 2020 2020  Norm1d(.        
+00022360: 2020 2020 2020 2020 6e75 6d5f 6665 6174          num_feat
+00022370: 7572 6573 3d73 656c 662e 6e5f 6869 6464  ures=self.n_hidd
+00022380: 656e 5f41 502c 0a20 2020 2020 2020 2020  en_AP,.         
+00022390: 2020 2020 2020 2065 7073 3d31 652d 332c         eps=1e-3,
+000223a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000223b0: 206d 6f6d 656e 7475 6d3d 302e 3939 2c0a   momentum=0.99,.
+000223c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223d0: 6166 6669 6e65 3d54 7275 652c 0a20 2020  affine=True,.   
+000223e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000223f0: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
+00022400: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00022410: 2020 2023 2057 6569 6768 7420 6d61 7472     # Weight matr
+00022420: 6978 2061 6e64 2062 6961 7320 6d61 7472  ix and bias matr
+00022430: 6978 2072 6571 7569 7265 6420 746f 2063  ix required to c
+00022440: 6f6d 7075 7465 206e 6577 2070 6169 7220  ompute new pair 
+00022450: 6c61 7965 7220 6672 6f6d 2074 6865 2070  layer from the p
+00022460: 7265 7669 6f75 7320 7061 6972 206c 6179  revious pair lay
+00022470: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
+00022480: 656c 662e 575f 5050 3a20 746f 7263 682e  elf.W_PP: torch.
+00022490: 5465 6e73 6f72 203d 2069 6e69 7428 0a20  Tensor = init(. 
+000224a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000224b0: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
+000224c0: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
+000224d0: 742c 2073 656c 662e 6e5f 6869 6464 656e  t, self.n_hidden
+000224e0: 5f50 5029 290a 2020 2020 2020 2020 2020  _PP)).          
+000224f0: 2020 7365 6c66 2e62 5f50 503a 2074 6f72    self.b_PP: tor
+00022500: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00022510: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
+00022520: 6869 6464 656e 5f50 502c 2929 0a20 2020  hidden_PP,)).   
+00022530: 2020 2020 2020 2020 2073 656c 662e 5050           self.PP
+00022540: 5f62 6e3a 206e 6e2e 4261 7463 684e 6f72  _bn: nn.BatchNor
+00022550: 6d31 6420 3d20 6e6e 2e42 6174 6368 4e6f  m1d = nn.BatchNo
+00022560: 726d 3164 280a 2020 2020 2020 2020 2020  rm1d(.          
+00022570: 2020 2020 2020 6e75 6d5f 6665 6174 7572        num_featur
+00022580: 6573 3d73 656c 662e 6e5f 6869 6464 656e  es=self.n_hidden
+00022590: 5f50 502c 0a20 2020 2020 2020 2020 2020  _PP,.           
+000225a0: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
+000225b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000225c0: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
+000225d0: 2020 2020 2020 2020 2020 2020 2020 6166                af
+000225e0: 6669 6e65 3d54 7275 652c 0a20 2020 2020  fine=True,.     
+000225f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00022600: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
+00022610: 7275 6529 0a0a 2020 2020 2020 2020 2020  rue)..          
+00022620: 2020 7365 6c66 2e57 5f50 3a20 746f 7263    self.W_P: torc
+00022630: 682e 5465 6e73 6f72 203d 2069 6e69 7428  h.Tensor = init(
+00022640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022650: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
+00022660: 662e 6e5f 6869 6464 656e 5f50 2c20 7365  f.n_hidden_P, se
+00022670: 6c66 2e6e 5f70 6169 725f 6f75 7470 7574  lf.n_pair_output
+00022680: 5f66 6561 7429 290a 2020 2020 2020 2020  _feat)).        
+00022690: 2020 2020 7365 6c66 2e62 5f50 3a20 746f      self.b_P: to
+000226a0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+000226b0: 6368 2e7a 6572 6f73 2828 7365 6c66 2e6e  ch.zeros((self.n
+000226c0: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
+000226d0: 742c 2929 0a20 2020 2020 2020 2020 2020  t,)).           
+000226e0: 2073 656c 662e 505f 626e 3a20 6e6e 2e42   self.P_bn: nn.B
+000226f0: 6174 6368 4e6f 726d 3164 203d 206e 6e2e  atchNorm1d = nn.
+00022700: 4261 7463 684e 6f72 6d31 6428 0a20 2020  BatchNorm1d(.   
+00022710: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00022720: 5f66 6561 7475 7265 733d 7365 6c66 2e6e  _features=self.n
+00022730: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
+00022740: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00022750: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
+00022760: 2020 2020 2020 2020 2020 2020 206d 6f6d               mom
+00022770: 656e 7475 6d3d 302e 3939 2c0a 2020 2020  entum=0.99,.    
+00022780: 2020 2020 2020 2020 2020 2020 6166 6669              affi
+00022790: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
+000227a0: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
+000227b0: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
+000227c0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+000227d0: 6275 696c 7420 3d20 5472 7565 0a0a 2020  built = True..  
+000227e0: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+000227f0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00022800: 2020 2020 2022 2222 0a20 2020 2052 6574       """.    Ret
+00022810: 7572 6e73 2061 2073 7472 696e 6720 7265  urns a string re
+00022820: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+00022830: 7468 6520 6f62 6a65 6374 2e0a 0a20 2020  the object...   
+00022840: 2052 6574 7572 6e73 3a0a 2020 2020 2d2d   Returns:.    --
+00022850: 2d2d 2d2d 2d0a 2020 2020 7374 723a 2041  -----.    str: A
+00022860: 2073 7472 696e 6720 7468 6174 2063 6f6e   string that con
+00022870: 7461 696e 7320 7468 6520 636c 6173 7320  tains the class 
+00022880: 6e61 6d65 2066 6f6c 6c6f 7765 6420 6279  name followed by
+00022890: 2074 6865 2076 616c 7565 7320 6f66 2069   the values of i
+000228a0: 7473 2069 6e73 7461 6e63 6520 7661 7269  ts instance vari
+000228b0: 6162 6c65 2e0a 2020 2020 2222 220a 2020  able..    """.  
+000228c0: 2020 2020 2020 2320 666c 616b 6538 3a20        # flake8: 
+000228d0: 6e6f 7161 0a20 2020 2020 2020 2072 6574  noqa.        ret
+000228e0: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+000228f0: 2020 6627 7b73 656c 662e 5f5f 636c 6173    f'{self.__clas
+00022900: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f  s__.__name__}(n_
+00022910: 6174 6f6d 5f69 6e70 7574 5f66 6561 743a  atom_input_feat:
+00022920: 7b73 656c 662e 6e5f 6174 6f6d 5f69 6e70  {self.n_atom_inp
+00022930: 7574 5f66 6561 747d 2c6e 5f70 6169 725f  ut_feat},n_pair_
+00022940: 696e 7075 745f 6665 6174 3a7b 7365 6c66  input_feat:{self
+00022950: 2e6e 5f70 6169 725f 696e 7075 745f 6665  .n_pair_input_fe
+00022960: 6174 7d2c 6e5f 6174 6f6d 5f6f 7574 7075  at},n_atom_outpu
+00022970: 745f 6665 6174 3a7b 7365 6c66 2e6e 5f61  t_feat:{self.n_a
+00022980: 746f 6d5f 6f75 7470 7574 5f66 6561 747d  tom_output_feat}
+00022990: 2c6e 5f70 6169 725f 6f75 7470 7574 5f66  ,n_pair_output_f
+000229a0: 6561 743a 7b73 656c 662e 6e5f 7061 6972  eat:{self.n_pair
+000229b0: 5f6f 7574 7075 745f 6665 6174 7d2c 6e5f  _output_feat},n_
+000229c0: 6869 6464 656e 5f41 413a 7b73 656c 662e  hidden_AA:{self.
+000229d0: 6e5f 6869 6464 656e 5f41 417d 2c6e 5f68  n_hidden_AA},n_h
+000229e0: 6964 6465 6e5f 5041 3a7b 7365 6c66 2e6e  idden_PA:{self.n
+000229f0: 5f68 6964 6465 6e5f 5041 7d2c 6e5f 6869  _hidden_PA},n_hi
+00022a00: 6464 656e 5f41 503a 7b73 656c 662e 6e5f  dden_AP:{self.n_
+00022a10: 6869 6464 656e 5f41 507d 2c6e 5f68 6964  hidden_AP},n_hid
+00022a20: 6465 6e5f 5050 3a7b 7365 6c66 2e6e 5f68  den_PP:{self.n_h
+00022a30: 6964 6465 6e5f 5050 7d2c 6261 7463 685f  idden_PP},batch_
+00022a40: 6e6f 726d 616c 697a 653a 7b73 656c 662e  normalize:{self.
+00022a50: 6261 7463 685f 6e6f 726d 616c 697a 657d  batch_normalize}
+00022a60: 2c75 7064 6174 655f 7061 6972 3a7b 7365  ,update_pair:{se
+00022a70: 6c66 2e75 7064 6174 655f 7061 6972 7d2c  lf.update_pair},
+00022a80: 696e 6974 3a7b 7365 6c66 2e69 6e69 747d  init:{self.init}
+00022a90: 2c61 6374 6976 6174 696f 6e3a 7b73 656c  ,activation:{sel
+00022aa0: 662e 6163 7469 7661 7469 6f6e 7d29 270a  f.activation})'.
+00022ab0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00022ac0: 6566 2066 6f72 7761 7264 280a 2020 2020  ef forward(.    
+00022ad0: 2020 2020 7365 6c66 2c20 696e 7075 7473      self, inputs
+00022ae0: 3a20 4c69 7374 5b55 6e69 6f6e 5b6e 702e  : List[Union[np.
+00022af0: 6e64 6172 7261 792c 206e 702e 6e64 6172  ndarray, np.ndar
+00022b00: 7261 792c 206e 702e 6e64 6172 7261 792c  ray, np.ndarray,
+00022b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b30: 2020 6e70 2e6e 6461 7272 6179 5d5d 0a20    np.ndarray]]. 
+00022b40: 2020 2029 202d 3e20 4c69 7374 5b55 6e69     ) -> List[Uni
+00022b50: 6f6e 5b74 6f72 6368 2e54 656e 736f 722c  on[torch.Tensor,
+00022b60: 2074 6f72 6368 2e54 656e 736f 725d 5d3a   torch.Tensor]]:
+00022b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00022b80: 2043 7265 6174 6573 2077 6561 7665 2074   Creates weave t
+00022b90: 656e 736f 7273 2e0a 0a20 2020 2050 6172  ensors...    Par
+00022ba0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00022bb0: 2d2d 2d2d 2d2d 0a20 2020 2069 6e70 7574  ------.    input
+00022bc0: 733a 204c 6973 745b 556e 696f 6e5b 6e70  s: List[Union[np
+00022bd0: 2e6e 6461 7272 6179 2c20 6e70 2e6e 6461  .ndarray, np.nda
+00022be0: 7272 6179 2c20 6e70 2e6e 6461 7272 6179  rray, np.ndarray
+00022bf0: 2c20 6e70 2e6e 6461 7272 6179 5d5d 0a20  , np.ndarray]]. 
+00022c00: 2020 2053 686f 756c 6420 636f 6e74 6169     Should contai
+00022c10: 6e20 3420 7465 6e73 6f72 7320 5b61 746f  n 4 tensors [ato
+00022c20: 6d5f 6665 6174 7572 6573 2c20 7061 6972  m_features, pair
+00022c30: 5f66 6561 7475 7265 732c 2070 6169 725f  _features, pair_
+00022c40: 7370 6c69 742c 0a20 2020 2061 746f 6d5f  split,.    atom_
+00022c50: 746f 5f70 6169 725d 0a0a 2020 2020 5265  to_pair]..    Re
+00022c60: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+00022c70: 2d2d 0a20 2020 204c 6973 745b 556e 696f  --.    List[Unio
+00022c80: 6e5b 746f 7263 682e 5465 6e73 6f72 2c20  n[torch.Tensor, 
+00022c90: 746f 7263 682e 5465 6e73 6f72 5d5d 0a20  torch.Tensor]]. 
+00022ca0: 2020 2020 2041 3a20 4174 6f6d 2066 6561       A: Atom fea
+00022cb0: 7475 7265 7320 7465 6e73 6f72 2077 6974  tures tensor wit
+00022cc0: 6820 7368 6170 655b 746f 7461 6c5f 6e75  h shape[total_nu
+00022cd0: 6d5f 6174 6f6d 732c 6174 6f6d 2066 6561  m_atoms,atom fea
+00022ce0: 7475 7265 2073 697a 655d 0a20 2020 2020  ture size].     
+00022cf0: 2050 3a20 5061 6972 2066 6561 7475 7265   P: Pair feature
+00022d00: 7320 7465 6e73 6f72 2077 6974 6820 7368  s tensor with sh
+00022d10: 6170 655b 746f 7461 6c20 6e75 6d20 6f66  ape[total num of
+00022d20: 2070 6169 7273 2c62 6f6e 6420 6665 6174   pairs,bond feat
+00022d30: 7572 6520 7369 7a65 5d0a 2020 2020 2222  ure size].    ""
+00022d40: 220a 2020 2020 2020 2020 2320 436f 6e76  ".        # Conv
+00022d50: 6572 7469 6e67 2074 6865 2069 6e70 7574  erting the input
+00022d60: 2074 6f20 746f 7263 6820 7465 6e73 6f72   to torch tensor
+00022d70: 730a 2020 2020 2020 2020 6174 6f6d 5f66  s.        atom_f
+00022d80: 6561 7475 7265 733a 2074 6f72 6368 2e54  eatures: torch.T
+00022d90: 656e 736f 7220 3d20 746f 7263 682e 7465  ensor = torch.te
+00022da0: 6e73 6f72 2869 6e70 7574 735b 305d 290a  nsor(inputs[0]).
+00022db0: 2020 2020 2020 2020 7061 6972 5f66 6561          pair_fea
+00022dc0: 7475 7265 733a 2074 6f72 6368 2e54 656e  tures: torch.Ten
+00022dd0: 736f 7220 3d20 746f 7263 682e 7465 6e73  sor = torch.tens
+00022de0: 6f72 2869 6e70 7574 735b 315d 290a 0a20  or(inputs[1]).. 
+00022df0: 2020 2020 2020 2070 6169 725f 7370 6c69         pair_spli
+00022e00: 743a 2074 6f72 6368 2e54 656e 736f 7220  t: torch.Tensor 
+00022e10: 3d20 746f 7263 682e 7465 6e73 6f72 2869  = torch.tensor(i
+00022e20: 6e70 7574 735b 325d 290a 2020 2020 2020  nputs[2]).      
+00022e30: 2020 6174 6f6d 5f74 6f5f 7061 6972 3a20    atom_to_pair: 
+00022e40: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00022e50: 6f72 6368 2e74 656e 736f 7228 696e 7075  orch.tensor(inpu
+00022e60: 7473 5b33 5d29 0a0a 2020 2020 2020 2020  ts[3])..        
+00022e70: 6163 7469 7661 7469 6f6e 203d 2073 656c  activation = sel
+00022e80: 662e 6163 7469 7661 7469 6f6e 5f66 6e0a  f.activation_fn.
+00022e90: 0a20 2020 2020 2020 2023 2041 4120 6973  .        # AA is
+00022ea0: 2061 2074 656e 736f 7220 7769 7468 2073   a tensor with s
+00022eb0: 6861 7065 5b74 6f74 616c 5f6e 756d 5f61  hape[total_num_a
+00022ec0: 746f 6d73 2c6e 5f68 6964 6465 6e5f 4141  toms,n_hidden_AA
+00022ed0: 5d0a 2020 2020 2020 2020 4141 3a20 746f  ].        AA: to
+00022ee0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+00022ef0: 6368 2e6d 6174 6d75 6c28 6174 6f6d 5f66  ch.matmul(atom_f
+00022f00: 6561 7475 7265 732e 7479 7065 2874 6f72  eatures.type(tor
+00022f10: 6368 2e66 6c6f 6174 3332 292c 0a20 2020  ch.float32),.   
+00022f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f40: 2020 2020 2073 656c 662e 575f 4141 2920       self.W_AA) 
+00022f50: 2b20 7365 6c66 2e62 5f41 410a 2020 2020  + self.b_AA.    
+00022f60: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
+00022f70: 685f 6e6f 726d 616c 697a 653a 0a20 2020  h_normalize:.   
+00022f80: 2020 2020 2020 2020 2073 656c 662e 4141           self.AA
+00022f90: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
+00022fa0: 2020 2020 2020 2041 4120 3d20 7365 6c66         AA = self
+00022fb0: 2e41 415f 626e 2841 4129 0a20 2020 2020  .AA_bn(AA).     
+00022fc0: 2020 2041 4120 3d20 6163 7469 7661 7469     AA = activati
+00022fd0: 6f6e 2841 4129 0a20 2020 2020 2020 2023  on(AA).        #
+00022fe0: 2050 4120 6973 2061 2074 656e 736f 7220   PA is a tensor 
+00022ff0: 7769 7468 2073 6861 7065 5b74 6f74 616c  with shape[total
+00023000: 206e 756d 6265 7220 6f66 2070 6169 7273   number of pairs
+00023010: 2c6e 5f68 6964 6465 6e5f 5041 5d0a 2020  ,n_hidden_PA].  
+00023020: 2020 2020 2020 5041 3a20 746f 7263 682e        PA: torch.
+00023030: 5465 6e73 6f72 203d 2074 6f72 6368 2e6d  Tensor = torch.m
+00023040: 6174 6d75 6c28 7061 6972 5f66 6561 7475  atmul(pair_featu
+00023050: 7265 732e 7479 7065 2874 6f72 6368 2e66  res.type(torch.f
+00023060: 6c6f 6174 3332 292c 0a20 2020 2020 2020  loat32),.       
+00023070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023090: 2073 656c 662e 575f 5041 2920 2b20 7365   self.W_PA) + se
+000230a0: 6c66 2e62 5f50 410a 2020 2020 2020 2020  lf.b_PA.        
+000230b0: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
+000230c0: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
+000230d0: 2020 2020 2073 656c 662e 5041 5f62 6e2e       self.PA_bn.
+000230e0: 6576 616c 2829 0a20 2020 2020 2020 2020  eval().         
+000230f0: 2020 2050 4120 3d20 7365 6c66 2e50 415f     PA = self.PA_
+00023100: 626e 2850 4129 0a20 2020 2020 2020 2050  bn(PA).        P
+00023110: 4120 3d20 6163 7469 7661 7469 6f6e 2850  A = activation(P
+00023120: 4129 0a0a 2020 2020 2020 2020 2320 5370  A)..        # Sp
+00023130: 6c69 7420 7468 6520 5041 2074 656e 736f  lit the PA tenso
+00023140: 7220 6163 636f 7264 696e 6720 746f 2074  r according to t
+00023150: 6865 2027 7061 6972 5f73 706c 6974 2720  he 'pair_split' 
+00023160: 7465 6e73 6f72 0a20 2020 2020 2020 2074  tensor.        t
+00023170: 5f67 7270 3a20 4469 6374 5b54 656e 736f  _grp: Dict[Tenso
+00023180: 722c 2054 656e 736f 725d 203d 207b 7d0a  r, Tensor] = {}.
+00023190: 2020 2020 2020 2020 6964 783a 2069 6e74          idx: int
+000231a0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
+000231b0: 2069 2c20 735f 6964 2069 6e20 656e 756d   i, s_id in enum
+000231c0: 6572 6174 6528 7061 6972 5f73 706c 6974  erate(pair_split
+000231d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000231e0: 5f69 6420 3d20 735f 6964 2e69 7465 6d28  _id = s_id.item(
+000231f0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00023200: 2073 5f69 6420 696e 2074 5f67 7270 3a0a   s_id in t_grp:.
+00023210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023220: 745f 6772 705b 735f 6964 5d20 3d20 745f  t_grp[s_id] = t_
+00023230: 6772 705b 735f 6964 5d20 2b20 5041 5b69  grp[s_id] + PA[i
+00023240: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
+00023250: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00023260: 2020 2020 2020 745f 6772 705b 735f 6964        t_grp[s_id
+00023270: 5d20 3d20 5041 5b69 6478 5d0a 2020 2020  ] = PA[idx].    
+00023280: 2020 2020 2020 2020 6964 7820 3d20 6920          idx = i 
+00023290: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
+000232a0: 206c 7374 203d 206c 6973 7428 745f 6772   lst = list(t_gr
+000232b0: 702e 7661 6c75 6573 2829 290a 2020 2020  p.values()).    
+000232c0: 2020 2020 2020 2020 7465 6e73 6f72 203d          tensor =
+000232d0: 2074 6f72 6368 2e73 7461 636b 286c 7374   torch.stack(lst
+000232e0: 290a 2020 2020 2020 2020 5041 203d 2074  ).        PA = t
+000232f0: 656e 736f 720a 0a20 2020 2020 2020 2041  ensor..        A
+00023300: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+00023310: 2074 6f72 6368 2e6d 6174 6d75 6c28 746f   torch.matmul(to
+00023320: 7263 682e 636f 6e63 6174 285b 4141 2c20  rch.concat([AA, 
+00023330: 5041 5d2c 2031 292c 0a20 2020 2020 2020  PA], 1),.       
+00023340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023360: 7365 6c66 2e57 5f41 2920 2b20 7365 6c66  self.W_A) + self
+00023370: 2e62 5f41 0a20 2020 2020 2020 2069 6620  .b_A.        if 
+00023380: 7365 6c66 2e62 6174 6368 5f6e 6f72 6d61  self.batch_norma
+00023390: 6c69 7a65 3a0a 2020 2020 2020 2020 2020  lize:.          
+000233a0: 2020 7365 6c66 2e41 5f62 6e2e 6576 616c    self.A_bn.eval
+000233b0: 2829 0a20 2020 2020 2020 2020 2020 2041  ().            A
+000233c0: 203d 2073 656c 662e 415f 626e 2841 290a   = self.A_bn(A).
+000233d0: 2020 2020 2020 2020 4120 3d20 6163 7469          A = acti
+000233e0: 7661 7469 6f6e 2841 290a 0a20 2020 2020  vation(A)..     
+000233f0: 2020 2069 6620 7365 6c66 2e75 7064 6174     if self.updat
+00023400: 655f 7061 6972 3a0a 2020 2020 2020 2020  e_pair:.        
+00023410: 2020 2020 2320 4e6f 7465 2074 6861 7420      # Note that 
+00023420: 4150 5f69 6a20 616e 6420 4150 5f6a 6920  AP_ij and AP_ji 
+00023430: 7368 6172 6520 7468 6520 7361 6d65 2073  share the same s
+00023440: 656c 662e 4150 5f62 6e20 6261 7463 680a  elf.AP_bn batch.
+00023450: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+00023460: 726d 616c 697a 6174 696f 6e0a 2020 2020  rmalization.    
+00023470: 2020 2020 2020 2020 4150 5f69 6a3a 2074          AP_ij: t
+00023480: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00023490: 7263 682e 6d61 746d 756c 280a 2020 2020  rch.matmul(.    
+000234a0: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+000234b0: 682e 7265 7368 6170 6528 6174 6f6d 5f66  h.reshape(atom_f
+000234c0: 6561 7475 7265 735b 6174 6f6d 5f74 6f5f  eatures[atom_to_
+000234d0: 7061 6972 5d2c 0a20 2020 2020 2020 2020  pair],.         
+000234e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234f0: 2020 2020 205b 2d31 2c20 3220 2a20 7365       [-1, 2 * se
+00023500: 6c66 2e6e 5f61 746f 6d5f 696e 7075 745f  lf.n_atom_input_
+00023510: 6665 6174 5d29 2e74 7970 6528 0a20 2020  feat]).type(.   
+00023520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023530: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00023540: 6f72 6368 2e66 6c6f 6174 3332 292c 2073  orch.float32), s
+00023550: 656c 662e 575f 4150 2920 2b20 7365 6c66  elf.W_AP) + self
+00023560: 2e62 5f41 500a 2020 2020 2020 2020 2020  .b_AP.          
+00023570: 2020 6966 2073 656c 662e 6261 7463 685f    if self.batch_
+00023580: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
+00023590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000235a0: 4150 5f62 6e2e 6576 616c 2829 0a20 2020  AP_bn.eval().   
+000235b0: 2020 2020 2020 2020 2020 2020 2041 505f               AP_
+000235c0: 696a 203d 2073 656c 662e 4150 5f62 6e28  ij = self.AP_bn(
+000235d0: 4150 5f69 6a29 0a20 2020 2020 2020 2020  AP_ij).         
+000235e0: 2020 2041 505f 696a 203d 2061 6374 6976     AP_ij = activ
+000235f0: 6174 696f 6e28 4150 5f69 6a29 0a20 2020  ation(AP_ij).   
+00023600: 2020 2020 2020 2020 2041 505f 6a69 3a20           AP_ji: 
+00023610: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00023620: 6f72 6368 2e6d 6174 6d75 6c28 0a20 2020  orch.matmul(.   
+00023630: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
+00023640: 6368 2e72 6573 6861 7065 2861 746f 6d5f  ch.reshape(atom_
+00023650: 6665 6174 7572 6573 5b74 6f72 6368 2e66  features[torch.f
+00023660: 6c69 7028 6174 6f6d 5f74 6f5f 7061 6972  lip(atom_to_pair
+00023670: 2c20 5b31 5d29 5d2c 0a20 2020 2020 2020  , [1])],.       
+00023680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023690: 2020 2020 2020 205b 2d31 2c20 3220 2a20         [-1, 2 * 
+000236a0: 7365 6c66 2e6e 5f61 746f 6d5f 696e 7075  self.n_atom_inpu
+000236b0: 745f 6665 6174 5d29 2e74 7970 6528 0a20  t_feat]).type(. 
+000236c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000236e0: 2074 6f72 6368 2e66 6c6f 6174 3332 292c   torch.float32),
+000236f0: 2073 656c 662e 575f 4150 2920 2b20 7365   self.W_AP) + se
+00023700: 6c66 2e62 5f41 500a 2020 2020 2020 2020  lf.b_AP.        
+00023710: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
+00023720: 685f 6e6f 726d 616c 697a 653a 0a20 2020  h_normalize:.   
+00023730: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00023740: 662e 4150 5f62 6e2e 6576 616c 2829 0a20  f.AP_bn.eval(). 
+00023750: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00023760: 505f 6a69 203d 2073 656c 662e 4150 5f62  P_ji = self.AP_b
+00023770: 6e28 4150 5f6a 6929 0a20 2020 2020 2020  n(AP_ji).       
+00023780: 2020 2020 2041 505f 6a69 203d 2061 6374       AP_ji = act
+00023790: 6976 6174 696f 6e28 4150 5f6a 6929 0a20  ivation(AP_ji). 
+000237a0: 2020 2020 2020 2020 2020 2023 2050 5020             # PP 
+000237b0: 6973 2061 2074 656e 736f 7220 7769 7468  is a tensor with
+000237c0: 2073 6861 7065 205b 746f 7461 6c20 6e75   shape [total nu
+000237d0: 6d62 6572 206f 6620 7061 6972 732c 6e5f  mber of pairs,n_
+000237e0: 6869 6464 656e 5f50 505d 0a20 2020 2020  hidden_PP].     
+000237f0: 2020 2020 2020 2050 503a 2074 6f72 6368         PP: torch
+00023800: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+00023810: 6d61 746d 756c 2870 6169 725f 6665 6174  matmul(pair_feat
+00023820: 7572 6573 2e74 7970 6528 746f 7263 682e  ures.type(torch.
+00023830: 666c 6f61 7433 3229 2c0a 2020 2020 2020  float32),.      
+00023840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023860: 2020 2020 2020 7365 6c66 2e57 5f50 5029        self.W_PP)
+00023870: 202b 2073 656c 662e 625f 5050 0a20 2020   + self.b_PP.   
+00023880: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00023890: 2e62 6174 6368 5f6e 6f72 6d61 6c69 7a65  .batch_normalize
+000238a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000238b0: 2020 7365 6c66 2e50 505f 626e 2e65 7661    self.PP_bn.eva
+000238c0: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
+000238d0: 2020 2020 5050 203d 2073 656c 662e 5050      PP = self.PP
+000238e0: 5f62 6e28 5050 290a 2020 2020 2020 2020  _bn(PP).        
+000238f0: 2020 2020 5050 203d 2061 6374 6976 6174      PP = activat
+00023900: 696f 6e28 5050 290a 2020 2020 2020 2020  ion(PP).        
+00023910: 2020 2020 503a 2074 6f72 6368 2e54 656e      P: torch.Ten
+00023920: 736f 7220 3d20 746f 7263 682e 6d61 746d  sor = torch.matm
+00023930: 756c 280a 2020 2020 2020 2020 2020 2020  ul(.            
+00023940: 2020 2020 746f 7263 682e 636f 6e63 6174      torch.concat
+00023950: 285b 4150 5f69 6a20 2b20 4150 5f6a 692c  ([AP_ij + AP_ji,
+00023960: 2050 505d 2c20 3129 2e74 7970 6528 746f   PP], 1).type(to
+00023970: 7263 682e 666c 6f61 7433 3229 2c0a 2020  rch.float32),.  
+00023980: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00023990: 6c66 2e57 5f50 2920 2b20 7365 6c66 2e62  lf.W_P) + self.b
+000239a0: 5f50 0a20 2020 2020 2020 2020 2020 2069  _P.            i
+000239b0: 6620 7365 6c66 2e62 6174 6368 5f6e 6f72  f self.batch_nor
+000239c0: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
+000239d0: 2020 2020 2020 2020 7365 6c66 2e50 5f62          self.P_b
+000239e0: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
+000239f0: 2020 2020 2020 2020 2050 203d 2073 656c           P = sel
+00023a00: 662e 505f 626e 2850 290a 2020 2020 2020  f.P_bn(P).      
+00023a10: 2020 2020 2020 5020 3d20 6163 7469 7661        P = activa
+00023a20: 7469 6f6e 2850 290a 2020 2020 2020 2020  tion(P).        
+00023a30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00023a40: 2020 5020 3d20 7061 6972 5f66 6561 7475    P = pair_featu
+00023a50: 7265 730a 0a20 2020 2020 2020 2072 6574  res..        ret
+00023a60: 7572 6e20 5b41 2c20 505d 0a              urn [A, P].
```

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230705190043/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230705190043/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230705190043/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230705190043/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230705190043/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230705190043/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230705190043/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230705190043/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230705190043/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230705190043/deepchem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230705190007
+Version: 2.7.2.dev20230705190043
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230705190007/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230705190043/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/setup.cfg` & `deepchem-2.7.2.dev20230705190043/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230705190007/setup.py` & `deepchem-2.7.2.dev20230705190043/setup.py`

 * *Files identical despite different names*

