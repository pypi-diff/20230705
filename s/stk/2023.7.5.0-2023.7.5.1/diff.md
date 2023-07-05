# Comparing `tmp/stk-2023.7.5.0.tar.gz` & `tmp/stk-2023.7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stk-2023.7.5.0.tar", last modified: Wed Jul  5 15:50:04 2023, max compression
+gzip compressed data, was "stk-2023.7.5.1.tar", last modified: Wed Jul  5 16:29:39 2023, max compression
```

## Comparing `stk-2023.7.5.0.tar` & `stk-2023.7.5.1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.563074 stk-2023.7.5.0/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-07-05 15:49:52.000000 stk-2023.7.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 15:50:04.563074 stk-2023.7.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5735 2023-07-05 15:49:52.000000 stk-2023.7.5.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-05 15:49:52.000000 stk-2023.7.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 15:50:04.563074 stk-2023.7.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.515075 stk-2023.7.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.523074 stk-2023.7.5.0/src/stk/
--rw-r--r--   0 root         (0) root         (0)    14877 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.523074 stk-2023.7.5.0/src/stk/_internal/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/atom.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/atom_info.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/bond.py
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/bond_info.py
--rw-r--r--   0 root         (0) root         (0)    37484 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/building_block.py
--rw-r--r--   0 root         (0) root         (0)    14393 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/constructed_molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/construction_result/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_result/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_result/construction_result.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_result/periodic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/construction_state/
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11906 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/construction_state.py
--rw-r--r--   0 root         (0) root         (0)    10688 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/graph_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5684 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/deletions_summary.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/molecule_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py
--rw-r--r--   0 root         (0) root         (0)     7311 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py
--rw-r--r--   0 root         (0) root         (0)     5218 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/databases/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27693 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)    17958 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/molecule.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/utilities.py
--rw-r--r--   0 root         (0) root         (0)     6457 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/value.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/databases/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.527074 stk-2023.7.5.0/src/stk/_internal/ea/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/crossover/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/crossover/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/crossover/genetic_recombination.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/crossover/molecule_crosser.py
--rw-r--r--   0 root         (0) root         (0)     7633 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/crossover/random.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/crossover/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/serial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py
--rw-r--r--   0 root         (0) root         (0)     9713 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/fitness_function.py
--rw-r--r--   0 root         (0) root         (0)    11219 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/property_vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5818 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/add.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/multiply.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/null.py
--rw-r--r--   0 root         (0) root         (0)     7166 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/power.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/sequence.py
--rw-r--r--   0 root         (0) root         (0)     7017 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/shift_up.py
--rw-r--r--   0 root         (0) root         (0)     4455 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/sum.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.531074 stk-2023.7.5.0/src/stk/_internal/ea/molecule_records/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/molecule_records/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/molecule_records/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.535075 stk-2023.7.5.0/src/stk/_internal/ea/mutation/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/mutator.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/random.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/random_building_block.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/random_topology_graph.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/record.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/mutation/similar_building_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.535075 stk-2023.7.5.0/src/stk/_internal/ea/plotters/
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/plotters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13994 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/plotters/progress.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/plotters/selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.535075 stk-2023.7.5.0/src/stk/_internal/ea/selection/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7886 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.535075 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/above_average.py
--rw-r--r--   0 root         (0) root         (0)     5939 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/best.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/filter_batches.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/filter_molecules.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/remove_batches.py
--rw-r--r--   0 root         (0) root         (0)     2629 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/remove_molecules.py
--rw-r--r--   0 root         (0) root         (0)     6006 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/roulette.py
--rw-r--r--   0 root         (0) root         (0)     7396 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/selector.py
--rw-r--r--   0 root         (0) root         (0)     7125 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py
--rw-r--r--   0 root         (0) root         (0)     4934 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/tournament.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.535075 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/utilities/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/worst.py
--rw-r--r--   0 root         (0) root         (0)    25498 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/elements.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.539075 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4502 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/alcohol_factory.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/aldehyde_factory.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/amide_factory.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/boronic_acid_factory.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/bromo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py
--rw-r--r--   0 root         (0) root         (0)     4280 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/dibromo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/difluoro_factory.py
--rw-r--r--   0 root         (0) root         (0)     4412 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/diol_factory.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/fluoro_factory.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/functional_group_factory.py
--rw-r--r--   0 root         (0) root         (0)     2702 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/iodo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/primary_amino_factory.py
--rw-r--r--   0 root         (0) root         (0)     1326 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/ring_amine_factory.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/secondary_amino_factory.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/smarts.py
--rw-r--r--   0 root         (0) root         (0)     4479 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/thioacid_factory.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/thiol_factory.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_group_factories/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.543074 stk-2023.7.5.0/src/stk/_internal/functional_groups/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3224 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/alcohol.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/aldehyde.py
--rw-r--r--   0 root         (0) root         (0)     4507 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/alkene.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/alkyne.py
--rw-r--r--   0 root         (0) root         (0)     4815 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/amide.py
--rw-r--r--   0 root         (0) root         (0)     4869 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/boronic_acid.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/bromo.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/carboxylic_acid.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/dibromo.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/difluoro.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/diol.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/fluoro.py
--rw-r--r--   0 root         (0) root         (0)    11798 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/functional_group.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/generic_functional_group.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/iodo.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/primary_amino.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/ring_amine.py
--rw-r--r--   0 root         (0) root         (0)     3382 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/secondary_amino.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/single_atom.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/thioacid.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/functional_groups/thiol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.543074 stk-2023.7.5.0/src/stk/_internal/json_serde/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/json_serde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9926 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/json_serde/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/json_serde/molecule.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/json_serde/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.543074 stk-2023.7.5.0/src/stk/_internal/key_makers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/inchi.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/inchi_key.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/molecule.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/smiles.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/key_makers/utilities.py
--rw-r--r--   0 root         (0) root         (0)    25466 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.543074 stk-2023.7.5.0/src/stk/_internal/optimizers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/collapser.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/mchammer.py
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/null.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3839 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/periodic_collapser.py
--rw-r--r--   0 root         (0) root         (0)     4456 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/spinner.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/optimizers/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/periodic_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.547074 stk-2023.7.5.0/src/stk/_internal/reaction_factories/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reaction_factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reaction_factories/dative_reaction_factory.py
--rw-r--r--   0 root         (0) root         (0)     6034 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reaction_factories/generic_reaction_factory.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reaction_factories/reaction_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.547074 stk-2023.7.5.0/src/stk/_internal/reactions/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.547074 stk-2023.7.5.0/src/stk/_internal/reactions/dative_reaction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/dative_reaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/dative_reaction/dative_reaction.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/dative_reaction/utilities.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/one_one_reaction.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/one_two_reaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.547074 stk-2023.7.5.0/src/stk/_internal/reactions/reaction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/reaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/reaction/new_atom.py
--rw-r--r--   0 root         (0) root         (0)     3615 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/reaction/reaction.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/reaction/reaction_result.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/ring_amine_reaction.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/reactions/two_two_reaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.547074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.551074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42840 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/cage.py
--rw-r--r--   0 root         (0) root         (0)     8079 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/cage_construction_state.py
--rw-r--r--   0 root         (0) root         (0)     8062 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py
--rw-r--r--   0 root         (0) root         (0)     6824 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/five_plus_ten.py
--rw-r--r--   0 root         (0) root         (0)     5034 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_eight.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_four.py
--rw-r--r--   0 root         (0) root         (0)     4907 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_six.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py
--rw-r--r--   0 root         (0) root         (0)     7536 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m12l24.py
--rw-r--r--   0 root         (0) root         (0)    13449 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m24l48.py
--rw-r--r--   0 root         (0) root         (0)     5151 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py
--rw-r--r--   0 root         (0) root         (0)     8175 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py
--rw-r--r--   0 root         (0) root         (0)     7429 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m3l6.py
--rw-r--r--   0 root         (0) root         (0)     7982 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l4_square.py
--rw-r--r--   0 root         (0) root         (0)     7987 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     9248 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     8786 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l8.py
--rw-r--r--   0 root         (0) root         (0)     6744 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m6l12_cube.py
--rw-r--r--   0 root         (0) root         (0)     9469 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py
--rw-r--r--   0 root         (0) root         (0)     9502 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m8l6_cube.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/one_plus_one.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_eight.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_nine.py
--rw-r--r--   0 root         (0) root         (0)     6684 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py
--rw-r--r--   0 root         (0) root         (0)     8949 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/three_plus_six.py
--rw-r--r--   0 root         (0) root         (0)    11770 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py
--rw-r--r--   0 root         (0) root         (0)    10975 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_four.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_three.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_two.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.555074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/
--rw-r--r--   0 root         (0) root         (0)      412 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27030 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/cof.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/edge.py
--rw-r--r--   0 root         (0) root         (0)     8245 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/hexagonal.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/honeycomb.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/kagome.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py
--rw-r--r--   0 root         (0) root         (0)     8737 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)    10199 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_kagome.py
--rw-r--r--   0 root         (0) root         (0)     7760 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)     8551 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_square.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/square.py
--rw-r--r--   0 root         (0) root         (0)    11377 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/vertices.py
--rw-r--r--   0 root         (0) root         (0)     5569 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/edge.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/edge_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.555074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17325 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/complex.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.555074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18837 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py
--rw-r--r--   0 root         (0) root         (0)    26537 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral.py
--rw-r--r--   0 root         (0) root         (0)     3944 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/square_planar.py
--rw-r--r--   0 root         (0) root         (0)     4667 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24349 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/linear.py
--rw-r--r--   0 root         (0) root         (0)     6057 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20644 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/parallel.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/serial.py
--rw-r--r--   0 root         (0) root         (0)    19701 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/edge_sorter.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/sorter.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/topology_graphs/vertex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/utilities/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.559074 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/mae.py
--rw-r--r--   0 root         (0) root         (0)      745 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/pdb.py
--rw-r--r--   0 root         (0) root         (0)     5796 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/turbomole.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/updaters/xyz.py
--rw-r--r--   0 root         (0) root         (0)    23774 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.563074 stk-2023.7.5.0/src/stk/_internal/utilities/writers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/writers/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/writers/pdb.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/utilities/writers/xyz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.563074 stk-2023.7.5.0/src/stk/_internal/writers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/writers/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)     6082 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/writers/pdb.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/writers/turbomole.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/_internal/writers/xyz.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk/_version.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/cage.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/cof.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/host_guest.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/macrocycle.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/metal_complex.py
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/polymer.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-05 15:49:52.000000 stk-2023.7.5.0/src/stk/rotaxane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:50:04.523074 stk-2023.7.5.0/src/stk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15113 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 15:50:04.000000 stk-2023.7.5.0/src/stk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.910579 stk-2023.7.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-07-05 16:29:28.000000 stk-2023.7.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 16:29:39.910579 stk-2023.7.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5735 2023-07-05 16:29:28.000000 stk-2023.7.5.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-05 16:29:28.000000 stk-2023.7.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 16:29:39.910579 stk-2023.7.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.846577 stk-2023.7.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.854577 stk-2023.7.5.1/src/stk/
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/atom.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/atom_info.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/bond.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/bond_info.py
+-rw-r--r--   0 root         (0) root         (0)    37484 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/building_block.py
+-rw-r--r--   0 root         (0) root         (0)    14393 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/constructed_molecule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/construction_result/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_result/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_result/construction_result.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_result/periodic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/construction_state/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11906 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/construction_state.py
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/graph_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5684 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/deletions_summary.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/molecule_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py
+-rw-r--r--   0 root         (0) root         (0)     7311 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.858578 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.862578 stk-2023.7.5.1/src/stk/_internal/databases/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/constructed_molecule.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/molecule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.862578 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27693 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/constructed_molecule.py
+-rw-r--r--   0 root         (0) root         (0)    17958 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/molecule.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     6457 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/value.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/databases/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.862578 stk-2023.7.5.1/src/stk/_internal/ea/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.862578 stk-2023.7.5.1/src/stk/_internal/ea/crossover/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/crossover/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/crossover/genetic_recombination.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/crossover/molecule_crosser.py
+-rw-r--r--   0 root         (0) root         (0)     7633 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/crossover/random.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/crossover/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.862578 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.866578 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/serial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.866578 stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py
+-rw-r--r--   0 root         (0) root         (0)     9713 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/fitness_function.py
+-rw-r--r--   0 root         (0) root         (0)    11219 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/property_vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.866578 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5818 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/add.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/multiply.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/null.py
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/power.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/sequence.py
+-rw-r--r--   0 root         (0) root         (0)     7017 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/shift_up.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/sum.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.866578 stk-2023.7.5.1/src/stk/_internal/ea/molecule_records/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/molecule_records/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/molecule_records/molecule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.870578 stk-2023.7.5.1/src/stk/_internal/ea/mutation/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/mutator.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/random.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/random_building_block.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/random_topology_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/record.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/mutation/similar_building_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.870578 stk-2023.7.5.1/src/stk/_internal/ea/plotters/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/plotters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13994 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/plotters/progress.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/plotters/selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.870578 stk-2023.7.5.1/src/stk/_internal/ea/selection/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7886 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.870578 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/above_average.py
+-rw-r--r--   0 root         (0) root         (0)     5939 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/best.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/filter_batches.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/filter_molecules.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/remove_batches.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/remove_molecules.py
+-rw-r--r--   0 root         (0) root         (0)     6006 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/roulette.py
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/selector.py
+-rw-r--r--   0 root         (0) root         (0)     7125 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/tournament.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.874578 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/utilities/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/worst.py
+-rw-r--r--   0 root         (0) root         (0)    25498 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/elements.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.878578 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4502 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/alcohol_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/aldehyde_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/amide_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/boronic_acid_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/bromo_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4280 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/dibromo_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/difluoro_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4412 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/diol_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/fluoro_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/functional_group_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/iodo_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/primary_amino_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/ring_amine_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/secondary_amino_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/smarts.py
+-rw-r--r--   0 root         (0) root         (0)     4479 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/thioacid_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/thiol_factory.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_group_factories/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.882578 stk-2023.7.5.1/src/stk/_internal/functional_groups/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/alcohol.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/aldehyde.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/alkene.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/alkyne.py
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/amide.py
+-rw-r--r--   0 root         (0) root         (0)     4869 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/boronic_acid.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/bromo.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/carboxylic_acid.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/dibromo.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/difluoro.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/diol.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/fluoro.py
+-rw-r--r--   0 root         (0) root         (0)    11798 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/functional_group.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/generic_functional_group.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/iodo.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/primary_amino.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/ring_amine.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/secondary_amino.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/single_atom.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/thioacid.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/functional_groups/thiol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.882578 stk-2023.7.5.1/src/stk/_internal/json_serde/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/json_serde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9926 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/json_serde/constructed_molecule.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/json_serde/molecule.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/json_serde/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.882578 stk-2023.7.5.1/src/stk/_internal/key_makers/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/inchi.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/inchi_key.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/molecule.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/smiles.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/key_makers/utilities.py
+-rw-r--r--   0 root         (0) root         (0)    25466 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/molecule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/optimizers/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/collapser.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/mchammer.py
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/null.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/periodic_collapser.py
+-rw-r--r--   0 root         (0) root         (0)     4456 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/optimizers/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/periodic_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/reaction_factories/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reaction_factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reaction_factories/dative_reaction_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6034 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reaction_factories/generic_reaction_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reaction_factories/reaction_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/reactions/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/reactions/dative_reaction/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/dative_reaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/dative_reaction/dative_reaction.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/dative_reaction/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/one_one_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/one_two_reaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/reactions/reaction/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/reaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/reaction/new_atom.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/reaction/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/reaction/reaction_result.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/ring_amine_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/reactions/two_two_reaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.886578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.894578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42840 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/cage.py
+-rw-r--r--   0 root         (0) root         (0)     8079 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/cage_construction_state.py
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py
+-rw-r--r--   0 root         (0) root         (0)     6824 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/five_plus_ten.py
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_eight.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_four.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_six.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py
+-rw-r--r--   0 root         (0) root         (0)     7536 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m12l24.py
+-rw-r--r--   0 root         (0) root         (0)    13449 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m24l48.py
+-rw-r--r--   0 root         (0) root         (0)     5151 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py
+-rw-r--r--   0 root         (0) root         (0)     8175 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py
+-rw-r--r--   0 root         (0) root         (0)     7429 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m3l6.py
+-rw-r--r--   0 root         (0) root         (0)     7982 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l4_square.py
+-rw-r--r--   0 root         (0) root         (0)     7987 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py
+-rw-r--r--   0 root         (0) root         (0)     9248 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py
+-rw-r--r--   0 root         (0) root         (0)     8786 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l8.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m6l12_cube.py
+-rw-r--r--   0 root         (0) root         (0)     9469 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py
+-rw-r--r--   0 root         (0) root         (0)     9502 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m8l6_cube.py
+-rw-r--r--   0 root         (0) root         (0)     6066 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/one_plus_one.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_eight.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_nine.py
+-rw-r--r--   0 root         (0) root         (0)     6684 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py
+-rw-r--r--   0 root         (0) root         (0)     8949 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/three_plus_six.py
+-rw-r--r--   0 root         (0) root         (0)    11770 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py
+-rw-r--r--   0 root         (0) root         (0)    10975 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_four.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_three.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_two.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.898578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27030 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/cof.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/edge.py
+-rw-r--r--   0 root         (0) root         (0)     8245 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/hexagonal.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/honeycomb.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/kagome.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py
+-rw-r--r--   0 root         (0) root         (0)     8737 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py
+-rw-r--r--   0 root         (0) root         (0)    10199 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_kagome.py
+-rw-r--r--   0 root         (0) root         (0)     7760 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py
+-rw-r--r--   0 root         (0) root         (0)     8551 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_square.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/square.py
+-rw-r--r--   0 root         (0) root         (0)    11377 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/vertices.py
+-rw-r--r--   0 root         (0) root         (0)     5569 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/edge.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/edge_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.898578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/complex.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.898578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.902578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py
+-rw-r--r--   0 root         (0) root         (0)    26537 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral.py
+-rw-r--r--   0 root         (0) root         (0)     3944 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/square_planar.py
+-rw-r--r--   0 root         (0) root         (0)     4667 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.902578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.902578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24349 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/linear.py
+-rw-r--r--   0 root         (0) root         (0)     6057 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.902578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20644 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/vertices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.902578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/parallel.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/serial.py
+-rw-r--r--   0 root         (0) root         (0)    19701 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.906578 stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/edge_sorter.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/sorter.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/topology_graphs/vertex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.906578 stk-2023.7.5.1/src/stk/_internal/utilities/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/molecule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.906578 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/mae.py
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/mdl_mol.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/pdb.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/turbomole.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/updaters/xyz.py
+-rw-r--r--   0 root         (0) root         (0)    23774 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.906578 stk-2023.7.5.1/src/stk/_internal/utilities/writers/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/writers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/writers/mdl_mol.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/writers/pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/utilities/writers/xyz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.906578 stk-2023.7.5.1/src/stk/_internal/writers/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/writers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/writers/mdl_mol.py
+-rw-r--r--   0 root         (0) root         (0)     6082 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/writers/pdb.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/writers/turbomole.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/_internal/writers/xyz.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/cage.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/cof.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/host_guest.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/macrocycle.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/metal_complex.py
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/polymer.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-05 16:29:28.000000 stk-2023.7.5.1/src/stk/rotaxane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:29:39.854577 stk-2023.7.5.1/src/stk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15113 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 16:29:39.000000 stk-2023.7.5.1/src/stk.egg-info/top_level.txt
```

### Comparing `stk-2023.7.5.0/LICENSE` & `stk-2023.7.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/PKG-INFO` & `stk-2023.7.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stk
-Version: 2023.7.5.0
+Version: 2023.7.5.1
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>, Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/stk
 Project-URL: documentation, https://stk.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `stk-2023.7.5.0/README.rst` & `stk-2023.7.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/pyproject.toml` & `stk-2023.7.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/__init__.py` & `stk-2023.7.5.1/src/stk/__init__.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/atom.py` & `stk-2023.7.5.1/src/stk/_internal/atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/atom_info.py` & `stk-2023.7.5.1/src/stk/_internal/atom_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/bond.py` & `stk-2023.7.5.1/src/stk/_internal/bond.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/bond_info.py` & `stk-2023.7.5.1/src/stk/_internal/bond_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/building_block.py` & `stk-2023.7.5.1/src/stk/_internal/building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/constructed_molecule.py` & `stk-2023.7.5.1/src/stk/_internal/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_result/construction_result.py` & `stk-2023.7.5.1/src/stk/_internal/construction_result/construction_result.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_result/periodic.py` & `stk-2023.7.5.1/src/stk/_internal/construction_result/periodic.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/construction_state.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/construction_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/graph_state.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/graph_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/deletions_summary.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/deletions_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/molecule_state.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/molecule_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py` & `stk-2023.7.5.1/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/constructed_molecule.py` & `stk-2023.7.5.1/src/stk/_internal/databases/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/databases/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/constructed_molecule.py` & `stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/mongo_db/value.py` & `stk-2023.7.5.1/src/stk/_internal/databases/mongo_db/value.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/databases/value.py` & `stk-2023.7.5.1/src/stk/_internal/databases/value.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/crossover/genetic_recombination.py` & `stk-2023.7.5.1/src/stk/_internal/ea/crossover/genetic_recombination.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/crossover/molecule_crosser.py` & `stk-2023.7.5.1/src/stk/_internal/ea/crossover/molecule_crosser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/crossover/random.py` & `stk-2023.7.5.1/src/stk/_internal/ea/crossover/random.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/crossover/record.py` & `stk-2023.7.5.1/src/stk/_internal/ea/crossover/record.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py` & `stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py` & `stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py` & `stk-2023.7.5.1/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/fitness_function.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/fitness_function.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_calculators/property_vector.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_calculators/property_vector.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/add.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/add.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/multiply.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/multiply.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/power.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/power.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/sequence.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/sequence.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/shift_up.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/shift_up.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/fitness_normalizers/sum.py` & `stk-2023.7.5.1/src/stk/_internal/ea/fitness_normalizers/sum.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/generation.py` & `stk-2023.7.5.1/src/stk/_internal/ea/generation.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/molecule_records/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/ea/molecule_records/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/mutator.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/mutator.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/random.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/random.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/random_building_block.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/random_building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/random_topology_graph.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/random_topology_graph.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/record.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/record.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/mutation/similar_building_block.py` & `stk-2023.7.5.1/src/stk/_internal/ea/mutation/similar_building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/plotters/progress.py` & `stk-2023.7.5.1/src/stk/_internal/ea/plotters/progress.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/plotters/selection.py` & `stk-2023.7.5.1/src/stk/_internal/ea/plotters/selection.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/batch.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/above_average.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/above_average.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/best.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/best.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/filter_batches.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/filter_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/filter_molecules.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/remove_batches.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/remove_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/remove_molecules.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/remove_molecules.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/roulette.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/roulette.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/selector.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/tournament.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/tournament.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/ea/selection/selectors/worst.py` & `stk-2023.7.5.1/src/stk/_internal/ea/selection/selectors/worst.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/elements.py` & `stk-2023.7.5.1/src/stk/_internal/elements.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/alcohol_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/alcohol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/aldehyde_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/aldehyde_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/amide_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/amide_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/boronic_acid_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/boronic_acid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/bromo_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/bromo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/dibromo_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/dibromo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/difluoro_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/difluoro_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/diol_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/diol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/fluoro_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/fluoro_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/functional_group_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/functional_group_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/iodo_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/iodo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/primary_amino_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/primary_amino_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/ring_amine_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/ring_amine_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/secondary_amino_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/secondary_amino_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/smarts.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/smarts.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/thioacid_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/thioacid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/thiol_factory.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/thiol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_group_factories/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/functional_group_factories/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/alcohol.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/alcohol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/aldehyde.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/aldehyde.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/alkene.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/alkene.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/alkyne.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/alkyne.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/amide.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/amide.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/boronic_acid.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/boronic_acid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/bromo.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/bromo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/carboxylic_acid.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/carboxylic_acid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/dibromo.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/dibromo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/difluoro.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/difluoro.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/diol.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/diol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/fluoro.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/fluoro.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/functional_group.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/functional_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/generic_functional_group.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/generic_functional_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/iodo.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/iodo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/primary_amino.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/primary_amino.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/ring_amine.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/ring_amine.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/secondary_amino.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/secondary_amino.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/single_atom.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/single_atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/thioacid.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/thioacid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/functional_groups/thiol.py` & `stk-2023.7.5.1/src/stk/_internal/functional_groups/thiol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/json_serde/constructed_molecule.py` & `stk-2023.7.5.1/src/stk/_internal/json_serde/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/json_serde/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/json_serde/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/json_serde/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/json_serde/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/key_makers/inchi.py` & `stk-2023.7.5.1/src/stk/_internal/key_makers/inchi.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/key_makers/inchi_key.py` & `stk-2023.7.5.1/src/stk/_internal/key_makers/inchi_key.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/key_makers/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/key_makers/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/key_makers/smiles.py` & `stk-2023.7.5.1/src/stk/_internal/key_makers/smiles.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/key_makers/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/key_makers/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/collapser.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/collapser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/mchammer.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/mchammer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/optimizer.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/periodic_collapser.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/periodic_collapser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/spinner.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/spinner.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/optimizers/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/optimizers/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/periodic_info.py` & `stk-2023.7.5.1/src/stk/_internal/periodic_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reaction_factories/dative_reaction_factory.py` & `stk-2023.7.5.1/src/stk/_internal/reaction_factories/dative_reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reaction_factories/generic_reaction_factory.py` & `stk-2023.7.5.1/src/stk/_internal/reaction_factories/generic_reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reaction_factories/reaction_factory.py` & `stk-2023.7.5.1/src/stk/_internal/reaction_factories/reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/dative_reaction/dative_reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/dative_reaction/dative_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/one_one_reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/one_one_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/one_two_reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/one_two_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/reaction/new_atom.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/reaction/new_atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/reaction/reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/reaction/reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/reaction/reaction_result.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/reaction/reaction_result.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/ring_amine_reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/ring_amine_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/reactions/two_two_reaction.py` & `stk-2023.7.5.1/src/stk/_internal/reactions/two_two_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/cage.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/cage.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/cage_construction_state.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/cage_construction_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/five_plus_ten.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/five_plus_ten.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_eight.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_eight.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_four.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_four.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_six.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_six.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m12l24.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m12l24.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m24l48.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m24l48.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m3l6.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m3l6.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l4_square.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l4_square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m4l8.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m4l8.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m6l12_cube.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m6l12_cube.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/m8l6_cube.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/m8l6_cube.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/one_plus_one.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/one_plus_one.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_eight.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_eight.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_nine.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_nine.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/three_plus_six.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/three_plus_six.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_four.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_four.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_three.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_three.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/two_plus_two.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/two_plus_two.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cage/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cage/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/cof.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/cof.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/edge.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/edge.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/hexagonal.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/hexagonal.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/honeycomb.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/kagome.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/kagome.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_kagome.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_kagome.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/periodic_square.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/periodic_square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/square.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/cof/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/cof/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/edge.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/edge.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/edge_group.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/edge_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/complex.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/host_guest/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/host_guest/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/macrocycle/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/macrocycle/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/square_planar.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/metal_complex/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/metal_complex/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/linear.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/linear.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/polymer/linear/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/polymer/linear/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/rotaxane/vertices.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/rotaxane/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/parallel.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/parallel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/serial.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/serial.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/topology_graph/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/topology_graph/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/edge_sorter.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/edge_sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/utilities/sorter.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/utilities/sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/topology_graphs/vertex.py` & `stk-2023.7.5.1/src/stk/_internal/topology_graphs/vertex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/molecule.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/updaters/mae.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/updaters/mae.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/updaters/mdl_mol.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/updaters/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/updaters/pdb.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/updaters/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/updaters/turbomole.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/updaters/turbomole.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/updaters/xyz.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/updaters/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/utilities.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/writers/mdl_mol.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/writers/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/writers/pdb.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/writers/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/utilities/writers/xyz.py` & `stk-2023.7.5.1/src/stk/_internal/utilities/writers/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/writers/mdl_mol.py` & `stk-2023.7.5.1/src/stk/_internal/writers/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/writers/pdb.py` & `stk-2023.7.5.1/src/stk/_internal/writers/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/writers/turbomole.py` & `stk-2023.7.5.1/src/stk/_internal/writers/turbomole.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/_internal/writers/xyz.py` & `stk-2023.7.5.1/src/stk/_internal/writers/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/cage.py` & `stk-2023.7.5.1/src/stk/cage.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/cof.py` & `stk-2023.7.5.1/src/stk/cof.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk/metal_complex.py` & `stk-2023.7.5.1/src/stk/metal_complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.0/src/stk.egg-info/PKG-INFO` & `stk-2023.7.5.1/src/stk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stk
-Version: 2023.7.5.0
+Version: 2023.7.5.1
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>, Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/stk
 Project-URL: documentation, https://stk.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `stk-2023.7.5.0/src/stk.egg-info/SOURCES.txt` & `stk-2023.7.5.1/src/stk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

