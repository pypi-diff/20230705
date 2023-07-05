# Comparing `tmp/splink-3.9.2.tar.gz` & `tmp/splink-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.9.2.tar", max compression
+gzip compressed data, was "splink-3.9.3.tar", max compression
```

## Comparing `splink-3.9.2.tar` & `splink-3.9.3.tar`

### file list

```diff
@@ -1,144 +1,150 @@
--rw-r--r--   0        0        0     1076 2023-06-21 11:04:52.562420 splink-3.9.2/LICENSE
--rw-r--r--   0        0        0     8755 2023-06-21 11:04:52.562420 splink-3.9.2/README.md
--rw-r--r--   0        0        0     2081 2023-06-21 11:04:52.598421 splink-3.9.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-21 11:04:52.598421 splink-3.9.2/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-06-21 11:04:52.598421 splink-3.9.2/splink/accuracy.py
--rw-r--r--   0        0        0     4759 2023-06-21 11:04:52.598421 splink-3.9.2/splink/analyse_blocking.py
--rw-r--r--   0        0        0      387 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_template_library.py
--rw-r--r--   0        0        0      661 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_base.py
--rw-r--r--   0        0        0     3120 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_comparison_imports.py
--rw-r--r--   0        0        0      350 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2903 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0      361 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      366 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_level_library.py
--rw-r--r--   0        0        0      221 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_library.py
--rw-r--r--   0        0        0      252 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_template_library.py
--rw-r--r--   0        0        0    20901 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/linker.py
--rw-r--r--   0        0        0     2867 2023-06-21 11:04:52.598421 splink-3.9.2/splink/block_from_labels.py
--rw-r--r--   0        0        0     6239 2023-06-21 11:04:52.598421 splink-3.9.2/splink/blocking.py
--rw-r--r--   0        0        0    11221 2023-06-21 11:04:52.598421 splink-3.9.2/splink/charts.py
--rw-r--r--   0        0        0     9244 2023-06-21 11:04:52.598421 splink-3.9.2/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison.py
--rw-r--r--   0        0        0     8766 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_helpers.py
--rw-r--r--   0        0        0      554 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_helpers_utils.py
--rw-r--r--   0        0        0    25479 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level.py
--rw-r--r--   0        0        0    16344 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    55194 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    61094 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_library.py
--rw-r--r--   0        0        0     4932 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    81134 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16917 2023-06-21 11:04:52.598421 splink-3.9.2/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-06-21 11:04:52.598421 splink-3.9.2/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-06-21 11:04:52.598421 splink-3.9.2/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-06-21 11:04:52.598421 splink-3.9.2/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-06-21 11:04:52.598421 splink-3.9.2/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1608 2023-06-21 11:04:52.598421 splink-3.9.2/splink/dialect_base.py
--rw-r--r--   0        0        0      476 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_level_library.py
--rw-r--r--   0        0        0      371 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_library.py
--rw-r--r--   0        0        0      194 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_template_library.py
--rw-r--r--   0        0        0      387 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1532 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_base.py
--rw-r--r--   0        0        0     5821 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
--rw-r--r--   0        0        0     1750 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0      367 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    11654 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/linker.py
--rw-r--r--   0        0        0    17471 2023-06-21 11:04:52.598421 splink-3.9.2/splink/em_training_session.py
--rw-r--r--   0        0        0     5655 2023-06-21 11:04:52.602421 splink-3.9.2/splink/estimate_u.py
--rw-r--r--   0        0        0      269 2023-06-21 11:04:52.602421 splink-3.9.2/splink/exceptions.py
--rw-r--r--   0        0        0     7333 2023-06-21 11:04:52.602421 splink-3.9.2/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1562 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     5153 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     1836 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2775 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     5795 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0     1111 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5691 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9113 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1714 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2753 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1891 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1654 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1125 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1805 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9910 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0     2910 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-06-21 11:04:52.606421 splink-3.9.2/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    13833 2023-06-21 11:04:52.606421 splink-3.9.2/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-06-21 11:04:52.614421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-06-21 11:04:52.618421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-06-21 11:04:52.626421 splink-3.9.2/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-06-21 11:04:52.626421 splink-3.9.2/splink/input_column.py
--rw-r--r--   0        0        0   129980 2023-06-21 11:04:52.626421 splink-3.9.2/splink/linker.py
--rw-r--r--   0        0        0      300 2023-06-21 11:04:52.626421 splink-3.9.2/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-06-21 11:04:52.626421 splink-3.9.2/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-06-21 11:04:52.626421 splink-3.9.2/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-06-21 11:04:52.626421 splink-3.9.2/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4548 2023-06-21 11:04:52.626421 splink-3.9.2/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-06-21 11:04:52.626421 splink-3.9.2/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-06-21 11:04:52.626421 splink-3.9.2/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-06-21 11:04:52.626421 splink-3.9.2/splink/pipeline.py
--rw-r--r--   0        0        0      390 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_level_library.py
--rw-r--r--   0        0        0      253 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_library.py
--rw-r--r--   0        0        0      394 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_template_library.py
--rw-r--r--   0        0        0    10365 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/linker.py
--rw-r--r--   0        0        0      393 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_level_library.py
--rw-r--r--   0        0        0      375 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_library.py
--rw-r--r--   0        0        0      402 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_template_library.py
--rw-r--r--   0        0        0     1530 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_helpers/postgres_base.py
--rw-r--r--   0        0        0     3241 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_helpers/postgres_comparison_imports.py
--rw-r--r--   0        0        0      371 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_linker.py
--rw-r--r--   0        0        0     3205 2023-06-21 11:04:52.626421 splink-3.9.2/splink/predict.py
--rw-r--r--   0        0        0     8241 2023-06-21 11:04:52.626421 splink-3.9.2/splink/profile_data.py
--rw-r--r--   0        0        0    18694 2023-06-21 11:04:52.626421 splink-3.9.2/splink/settings.py
--rw-r--r--   0        0        0      474 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_library.py
--rw-r--r--   0        0        0      192 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_template_library.py
--rw-r--r--   0        0        0      473 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/jar_location.py
--rw-r--r--   0        0        0    23143 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/linker.py
--rw-r--r--   0        0        0      384 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0      366 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      393 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0     1083 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     1875 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/spark_base.py
--rw-r--r--   0        0        0     5788 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/spark_comparison_imports.py
--rw-r--r--   0        0        0      356 2023-06-21 11:04:52.630421 splink-3.9.2/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-06-21 11:04:52.630421 splink-3.9.2/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3750 2023-06-21 11:04:52.630421 splink-3.9.2/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sql_transform.py
--rw-r--r--   0        0        0      384 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_level_library.py
--rw-r--r--   0        0        0      252 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_library.py
--rw-r--r--   0        0        0      126 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_template_library.py
--rw-r--r--   0        0        0     8472 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/linker.py
--rw-r--r--   0        0        0      387 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_template_library.py
--rw-r--r--   0        0        0      270 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_base.py
--rw-r--r--   0        0        0     3861 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
--rw-r--r--   0        0        0      361 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     9825 2023-06-21 11:04:52.630421 splink-3.9.2/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-06-21 11:04:52.630421 splink-3.9.2/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-06-21 11:04:52.630421 splink-3.9.2/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-06-21 11:04:52.630421 splink-3.9.2/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-06-21 11:04:52.630421 splink-3.9.2/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-06-21 11:04:52.630421 splink-3.9.2/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 splink-3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-05 16:14:53.842971 splink-3.9.3/LICENSE
+-rw-r--r--   0        0        0     8777 2023-07-05 16:14:53.842971 splink-3.9.3/README.md
+-rw-r--r--   0        0        0     2110 2023-07-05 16:14:53.878971 splink-3.9.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-07-05 16:14:53.882971 splink-3.9.3/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-07-05 16:14:53.882971 splink-3.9.3/splink/accuracy.py
+-rw-r--r--   0        0        0     4803 2023-07-05 16:14:53.882971 splink-3.9.3/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      387 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0     1365 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0     3322 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0      361 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      386 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_level_library.py
+-rw-r--r--   0        0        0      249 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_library.py
+-rw-r--r--   0        0        0      252 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_template_library.py
+-rw-r--r--   0        0        0    21171 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/linker.py
+-rw-r--r--   0        0        0     2867 2023-07-05 16:14:53.882971 splink-3.9.3/splink/block_from_labels.py
+-rw-r--r--   0        0        0     6439 2023-07-05 16:14:53.882971 splink-3.9.3/splink/blocking.py
+-rw-r--r--   0        0        0     2223 2023-07-05 16:14:53.882971 splink-3.9.3/splink/cache_dict_with_logging.py
+-rw-r--r--   0        0        0    11249 2023-07-05 16:14:53.882971 splink-3.9.3/splink/charts.py
+-rw-r--r--   0        0        0     9266 2023-07-05 16:14:53.882971 splink-3.9.3/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25479 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level.py
+-rw-r--r--   0        0        0    16560 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    57737 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    63328 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_library.py
+-rw-r--r--   0        0        0     4922 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    81390 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16699 2023-07-05 16:14:53.882971 splink-3.9.3/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-07-05 16:14:53.882971 splink-3.9.3/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-07-05 16:14:53.882971 splink-3.9.3/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-07-05 16:14:53.882971 splink-3.9.3/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0     5562 2023-07-05 16:14:53.882971 splink-3.9.3/splink/datasets/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-05 16:14:53.882971 splink-3.9.3/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-07-05 16:14:53.882971 splink-3.9.3/splink/dialect_base.py
+-rw-r--r--   0        0        0      476 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_library.py
+-rw-r--r--   0        0        0      194 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_template_library.py
+-rw-r--r--   0        0        0      387 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1555 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0     5623 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0      367 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    11906 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/linker.py
+-rw-r--r--   0        0        0    17650 2023-07-05 16:14:53.882971 splink-3.9.3/splink/em_training_session.py
+-rw-r--r--   0        0        0     5743 2023-07-05 16:14:53.882971 splink-3.9.3/splink/estimate_u.py
+-rw-r--r--   0        0        0      269 2023-07-05 16:14:53.882971 splink-3.9.3/splink/exceptions.py
+-rw-r--r--   0        0        0     9070 2023-07-05 16:14:53.882971 splink-3.9.3/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1562 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5153 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1836 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5691 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9113 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1714 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1891 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2910 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-07-05 16:14:53.886971 splink-3.9.3/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-07-05 16:14:53.886971 splink-3.9.3/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-07-05 16:14:53.890971 splink-3.9.3/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0   974616 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/labelling_tool/slt.js
+-rw-r--r--   0        0        0     2971 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/labelling_tool/template.j2
+-rw-r--r--   0        0        0    13833 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-07-05 16:14:53.898971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-07-05 16:14:53.906971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-07-05 16:14:53.914971 splink-3.9.3/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-07-05 16:14:53.914971 splink-3.9.3/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-07-05 16:14:53.914971 splink-3.9.3/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-07-05 16:14:53.914971 splink-3.9.3/splink/input_column.py
+-rw-r--r--   0        0        0     3413 2023-07-05 16:14:53.914971 splink-3.9.3/splink/labelling_tool.py
+-rw-r--r--   0        0        0   133602 2023-07-05 16:14:53.914971 splink-3.9.3/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-07-05 16:14:53.914971 splink-3.9.3/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-07-05 16:14:53.914971 splink-3.9.3/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-07-05 16:14:53.914971 splink-3.9.3/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-07-05 16:14:53.914971 splink-3.9.3/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     5911 2023-07-05 16:14:53.914971 splink-3.9.3/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-07-05 16:14:53.914971 splink-3.9.3/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-07-05 16:14:53.914971 splink-3.9.3/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-07-05 16:14:53.914971 splink-3.9.3/splink/pipeline.py
+-rw-r--r--   0        0        0      390 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_level_library.py
+-rw-r--r--   0        0        0      253 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_library.py
+-rw-r--r--   0        0        0      394 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_template_library.py
+-rw-r--r--   0        0        0    10873 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/linker.py
+-rw-r--r--   0        0        0      393 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_level_library.py
+-rw-r--r--   0        0        0      375 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_library.py
+-rw-r--r--   0        0        0      402 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_template_library.py
+-rw-r--r--   0        0        0     1530 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_helpers/postgres_base.py
+-rw-r--r--   0        0        0     3129 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_helpers/postgres_comparison_imports.py
+-rw-r--r--   0        0        0      362 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_linker.py
+-rw-r--r--   0        0        0     5624 2023-07-05 16:14:53.914971 splink-3.9.3/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-07-05 16:14:53.914971 splink-3.9.3/splink/profile_data.py
+-rw-r--r--   0        0        0    18987 2023-07-05 16:14:53.914971 splink-3.9.3/splink/settings.py
+-rw-r--r--   0        0        0    17972 2023-07-05 16:14:53.914971 splink-3.9.3/splink/settings_validator.py
+-rw-r--r--   0        0        0      474 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_library.py
+-rw-r--r--   0        0        0      192 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_template_library.py
+-rw-r--r--   0        0        0      473 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/jar_location.py
+-rw-r--r--   0        0        0    23599 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/linker.py
+-rw-r--r--   0        0        0      384 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      366 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      393 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     1875 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0     5584 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0      356 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-07-05 16:14:53.914971 splink-3.9.3/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     4152 2023-07-05 16:14:53.914971 splink-3.9.3/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1205 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sql_transform.py
+-rw-r--r--   0        0        0      384 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_level_library.py
+-rw-r--r--   0        0        0      252 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_library.py
+-rw-r--r--   0        0        0      126 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_template_library.py
+-rw-r--r--   0        0        0     8562 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/linker.py
+-rw-r--r--   0        0        0      387 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      270 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0     3761 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0      361 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     9772 2023-07-05 16:14:53.914971 splink-3.9.3/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-07-05 16:14:53.914971 splink-3.9.3/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1673 2023-07-05 16:14:53.914971 splink-3.9.3/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-07-05 16:14:53.914971 splink-3.9.3/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-07-05 16:14:53.914971 splink-3.9.3/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-07-05 16:14:53.914971 splink-3.9.3/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9760 1970-01-01 00:00:00.000000 splink-3.9.3/PKG-INFO
```

### Comparing `splink-3.9.2/LICENSE` & `splink-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/README.md` & `splink-3.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 [![pypi](https://img.shields.io/github/v/release/moj-analytical-services/splink?include_prereleases)](https://pypi.org/project/splink/#history)
 [![Downloads](https://pepy.tech/badge/splink/month)](https://pepy.tech/project/splink)
 [![Documentation](https://img.shields.io/badge/API-documentation-blue)](https://moj-analytical-services.github.io/splink/)
 
 # Fast, accurate and scalable probabilistic data linkage
 
-Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
+Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets that lack unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
-📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.  
+⚡ **Speed:** Capable of linking a million records on a laptop in around a minute.  
+🎯 **Accuracy:** Support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required for model training.  
+📊 **Interactive Outputs:** Multiple interactive visualisations help users understand their model and diagnose problems.  
 
-Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
+Splink's linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
 
 ![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_1.drawio.png)
 
@@ -46,15 +46,15 @@
 
 ## Documentation
 
 The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink_demos/tree/splink3_demos), or by clicking the following Binder link:
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
 
-The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. A [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
+The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. The [Splink documentation site](https://moj-analytical-services.github.io/splink/topic_guides/fellegi_sunter.html) and a [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
 
 The Office for National Statistics have written a [case study about using Splink](https://github.com/Data-Linkage/Splink-census-linkage/blob/main/SplinkCaseStudy.pdf) to link 2021 Census data to itself.
 
 ## Installation
 
 Splink supports python 3.7+. To obtain the latest released version of splink you can install from PyPI using pip:
 
@@ -71,24 +71,23 @@
 Should you require a more bare-bones version of Splink **without DuckDB**, please see the following area of the docs:
 > [DuckDBless Splink Installation](https://moj-analytical-services.github.io/splink/installations.html#duckdb-less-installation)
 
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
-For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
+For more detailed tutorial, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.linker import DuckDBLinker
 import splink.duckdb.comparison_library as cl
 import splink.duckdb.comparison_template_library as ctl
+from splink.datasets import splink_datasets
 
-import pandas as pd
-
-df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
+df = splink_datasets.fake_1000
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
         "l.first_name = r.first_name",
         "l.surname = r.surname",
     ],
@@ -119,15 +118,15 @@
 ## Videos
 
 - [A introductory presentation on Splink](https://www.youtube.com/watch?v=msz3T741KQI)
 - [An introduction to the Splink Comparison Viewer dashboard](https://www.youtube.com/watch?v=DNvCMqjipis)
 
 ## Support
 
-Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, pleaase raise an [issue](https://github.com/moj-analytical-services/splink/issues).
+Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, please raise an [issue](https://github.com/moj-analytical-services/splink/issues).
 
 ## Awards
 
 🥇 Analysis in Government Awards 2020: Innovative Methods: [Winner](https://www.gov.uk/government/news/launch-of-the-analysis-in-government-awards)
 
 🥇 MoJ DASD Awards 2020: Innovation and Impact - Winner
```

### Comparing `splink-3.9.2/pyproject.toml` & `splink-3.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "3.9.2"
+version = "3.9.3"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
@@ -61,14 +61,16 @@
     # Pycodestyle
     "E",
     "W",
     # isort
     "I001",
     # bugbear
     "B",
+    # flake8-print
+    "T20"
 ]
 ignore = [
     "B905", # `zip()` without an explicit `strict=` parameter
     "B006", # Do not use mutable data structures for argument defaults"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `splink-3.9.2/splink/accuracy.py` & `splink-3.9.3/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/analyse_blocking.py` & `splink-3.9.3/splink/analyse_blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             select count(*) as count
             from {concat.physical_name}
             {group_by_statement}
         """
         linker._enqueue_sql(sql, "__splink__cartesian_product")
         cartesian_count = linker._execute_sql_pipeline([concat])
         row_count_df = cartesian_count.as_record_dict()
-        cartesian_count.drop_table_from_database()
+        cartesian_count.drop_table_from_database_and_remove_from_cache()
 
         cartesian = calculate_cartesian(row_count_df, settings_obj._link_type)
 
     # Calculate the total number of rows generated by each blocking rule
     sql = block_using_rules_sql(linker)
     linker._enqueue_sql(sql, "__splink__df_blocked_data")
 
@@ -95,15 +95,15 @@
         from __splink__df_blocked_data
         group by match_key
         order by cast(match_key as int) asc
     """
     linker._enqueue_sql(sql, "__splink__df_count_cumulative_blocks")
     cumulative_blocking_rule_count = linker._execute_sql_pipeline([concat])
     br_n = cumulative_blocking_rule_count.as_pandas_dataframe()
-    cumulative_blocking_rule_count.drop_table_from_database()
+    cumulative_blocking_rule_count.drop_table_from_database_and_remove_from_cache()
     br_count, br_keys = list(br_n.row_count), list(br_n["match_key"].astype("int"))
 
     if len(br_count) != len(brs_as_objs):
         missing_br = [x for x in range(len(brs_as_objs)) if x not in br_keys]
         for n in missing_br:
             br_count.insert(n, 0)
```

### Comparing `splink-3.9.2/splink/athena/athena_helpers/athena_comparison_imports.py` & `splink-3.9.3/splink/athena/athena_helpers/athena_comparison_imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
+    DatediffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
-    ArrayIntersectAtSizesComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
-    DistanceInKMAtThresholdsComparisonBase,
+    ArrayIntersectAtSizesBase,
+    DatediffAtThresholdsBase,
+    DistanceFunctionAtThresholdsBase,
+    DistanceInKMAtThresholdsBase,
     ExactMatchBase,
-    LevenshteinAtThresholdsComparisonBase,
+    LevenshteinAtThresholdsBase,
 )
 from ...comparison_template_library import (
     PostcodeComparisonBase,
 )
 from .athena_base import (
     AthenaBase,
 )
@@ -43,14 +45,18 @@
         return array_intersect_level
 
     @property
     def _columns_reversed_level(self):
         return columns_reversed_level
 
     @property
+    def _datediff_level(self):
+        return datediff_level
+
+    @property
     def _distance_in_km_level(self):
         return distance_in_km_level
 
     @property
     def _distance_function_level(self):
         return distance_function_level
 
@@ -90,49 +96,55 @@
     pass
 
 
 class percentage_difference_level(AthenaBase, PercentageDifferenceLevelBase):
     pass
 
 
+class datediff_level(AthenaBase, DatediffLevelBase):
+    pass
+
+
 class distance_in_km_level(AthenaBase, DistanceInKMLevelBase):
     pass
 
 
 ##########################
 ### COMPARISON LIBRARY ###
 ##########################
 class exact_match(AthenaComparisonProperties, ExactMatchBase):
     pass
 
 
 class distance_function_at_thresholds(
-    AthenaComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+    AthenaComparisonProperties, DistanceFunctionAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._distance_function_level
 
 
 class levenshtein_at_thresholds(
-    AthenaComparisonProperties, LevenshteinAtThresholdsComparisonBase
+    AthenaComparisonProperties, LevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._levenshtein_level
 
 
-class array_intersect_at_sizes(
-    AthenaComparisonProperties, ArrayIntersectAtSizesComparisonBase
-):
+class array_intersect_at_sizes(AthenaComparisonProperties, ArrayIntersectAtSizesBase):
+    pass
+
+
+class datediff_at_thresholds(AthenaComparisonProperties, DatediffAtThresholdsBase):
     pass
 
 
 class distance_in_km_at_thresholds(
-    AthenaComparisonProperties, DistanceInKMAtThresholdsComparisonBase
+    AthenaComparisonProperties, DistanceInKMAtThresholdsBase
 ):
     pass
 
 
 ###################################
 ### COMPARISON TEMPLATE LIBRARY ###
 ###################################
```

### Comparing `splink-3.9.2/splink/athena/athena_helpers/athena_utils.py` & `splink-3.9.3/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/athena/linker.py` & `splink-3.9.3/splink/athena/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         cols = list(d.keys())
         return [InputColumn(c, sql_dialect="presto") for c in cols]
 
     def validate(self):
         pass
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         # Check folder and table set for deletion
         self._check_drop_folder_created_by_splink(force_non_splink_table)
         self._check_drop_table_created_by_splink(force_non_splink_table)
 
         # Delete the table from s3 and your database
         self.linker._drop_table_from_database_if_exists(self.physical_name)
         self.linker._delete_table_from_s3(self.physical_name)
@@ -116,14 +116,15 @@
         boto3_session: boto3.session.Session,
         output_database: str,
         output_bucket: str,
         settings_dict: dict | str = None,
         input_table_aliases: str | list = None,
         set_up_basic_logging=True,
         output_filepath: str = "",
+        validate_settings: bool = True,
     ):
         """An athena backend for our main linker class. This funnels our generated SQL
         through athena using awswrangler.
         See linker.py for more information on the main linker class.
         Attributes:
             input_table_or_tables (Union[str, list]): Input data into the linkage model.
                 Either a single string (the name of a table in a database) for
@@ -146,14 +147,16 @@
                 saves your tables under a custom name: '__splink__input_table_{n}';
                 where n is the list index.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             output_filepath (str, optional): Inside of your selected output bucket,
                 where to write output files to.
                 Defaults to "splink_warehouse/{unique_id}".
+            validate_settings (bool, optional): When True, check your settings
+                dictionary for any potential errors that may cause splink to fail.
         Examples:
             ```py
             # Creating a database in athena and writing to it
             import awswrangler as wr
             wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
             >>>
             from splink.athena.linker import AthenaLinker
@@ -231,14 +234,15 @@
 
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
+            validate_settings=validate_settings,
         )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
         return AthenaDataFrame(templated_name, physical_name, self)
 
     def change_output_filepath(self, new_filepath):
         self.output_filepath = new_filepath
@@ -293,15 +297,15 @@
             "ctas_database": self.output_schema,
             "ctas_table": alias,
         }
         self.ctas_query_info.update({alias: ctas_metadata})
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         self._delete_table_from_database(physical_name)
-        sql = sqlglot_transform_sql(sql, cast_concat_as_varchar)
+        sql = sqlglot_transform_sql(sql, cast_concat_as_varchar, dialect="presto")
         sql = sql.replace("FLOAT", "double").replace("float", "double")
 
         logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
         logger.log(5, log_sql(sql))
 
         # create our table on athena and extract the metadata information
         query_metadata = self.create_table(sql, physical_name=physical_name)
```

### Comparing `splink-3.9.2/splink/block_from_labels.py` & `splink-3.9.3/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/blocking.py` & `splink-3.9.3/splink/blocking.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,25 +123,30 @@
         # Need df_l to be the one with the lowest id to preeserve the property
         # that the left dataset is the one with the lowest concatenated id
         keys = linker._input_tables_dict.keys()
         keys = list(sorted(keys))
         df_l = linker._input_tables_dict[keys[0]]
         df_r = linker._input_tables_dict[keys[1]]
 
+        if linker._train_u_using_random_sample_mode:
+            sample_switch = "_sample"
+        else:
+            sample_switch = ""
+
         sql = f"""
-        select * from __splink__df_concat_with_tf
+        select * from __splink__df_concat_with_tf{sample_switch}
         where {source_dataset_col} = '{df_l.templated_name}'
         """
-        linker._enqueue_sql(sql, "__splink__df_concat_with_tf_left")
+        linker._enqueue_sql(sql, f"__splink__df_concat_with_tf{sample_switch}_left")
 
         sql = f"""
-        select * from __splink__df_concat_with_tf
+        select * from __splink__df_concat_with_tf{sample_switch}
         where {source_dataset_col} = '{df_r.templated_name}'
         """
-        linker._enqueue_sql(sql, "__splink_df_concat_with_tf_right")
+        linker._enqueue_sql(sql, f"__splink__df_concat_with_tf{sample_switch}_right")
 
     # Cover the case where there are no blocking rules
     # This is a bit of a hack where if you do a self-join on 'true'
     # you create a cartesian product, rather than having separate code
     # that generates a cross join for the case of no blocking rules
     if not blocking_rules:
         blocking_rules = [BlockingRule("1=1")]
```

### Comparing `splink-3.9.2/splink/charts.py` & `splink-3.9.3/splink/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
     fmt_dict["mychart"] = json.dumps(chart_dict)
 
     with open(filename, "w", encoding="utf-8") as f:
         f.write(template.format(**fmt_dict))
 
     if print_msg:
-        print(f"Chart saved to {filename}")
-        print(iframe_message.format(filename=filename))
+        print(f"Chart saved to {filename}")  # noqa: T201
+        print(iframe_message.format(filename=filename))  # noqa: T201
 
 
 def match_weights_chart(records, as_dict=False):
     chart_path = "match_weights_interactive_history.json"
     chart = load_chart_definition(chart_path)
 
     # Remove iteration history since this is a static chart
```

### Comparing `splink-3.9.2/splink/cluster_studio.py` & `splink-3.9.3/splink/cluster_studio.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     select count(distinct cluster_id) as count
     from {connected_components.physical_name}
     """
     df_cluster_count = linker._sql_to_splink_dataframe_checking_cache(
         sql, "__splink__cluster_count"
     )
     cluster_count = df_cluster_count.as_record_dict()[0]["count"]
-    df_cluster_count.drop_table_from_database()
+    df_cluster_count.drop_table_from_database_and_remove_from_cache()
 
     proportion = sample_size / cluster_count
 
     random_sample_sql = linker._random_sample_sql(
         proportion,
         sample_size,
         seed,
```

### Comparing `splink-3.9.2/splink/comparison.py` & `splink-3.9.3/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_helpers.py` & `splink-3.9.3/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_helpers_utils.py` & `splink-3.9.3/splink/comparison_helpers_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_level.py` & `splink-3.9.3/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_level_composition.py` & `splink-3.9.3/splink/comparison_level_composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         m_probability (float, optional): Starting value for m probability.
             Defaults to None.
         is_null_level (bool, optional): If true, m and u values will not be
             estimated and instead the match weight will be zero for this column.
             Defaults to None.
 
     Examples:
-        === "DuckDB"
+        === ":simple-duckdb: DuckDB"
             Simple null level composition with an `AND` clause
             ``` python
             import splink.duckdb.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -53,15 +53,15 @@
             merged.as_dict()
             ```
             >{
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "Spark"
+        === ":simple-apachespark: Spark"
             Simple null level composition with an `AND` clause
             ``` python
             import splink.spark.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -77,15 +77,15 @@
             merged.as_dict()
             ```
             >{
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "Athena"
+        === ":simple-amazonaws: Athena"
             Simple null level composition with an `AND` clause
             ``` python
             import splink.athena.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -101,15 +101,15 @@
             merged.as_dict()
             ```
             >{
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "SQLite"
+        === ":simple-sqlite: SQLite"
             Simple null level composition with an `AND` clause
             ``` python
             import splink.sqlite.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
 
     Returns:
@@ -149,15 +149,15 @@
         m_probability (float, optional): Starting value for m probability.
             Defaults to None.
         is_null_level (bool, optional): If true, m and u values will not be
             estimated and instead the match weight will be zero for this column.
             Defaults to None.
 
     Examples:
-        === "DuckDB"
+        === ":simple-duckdb: DuckDB"
             Simple null level composition with an `OR` clause
             ``` python
             import splink.duckdb.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -173,15 +173,15 @@
             merged.as_dict()
             ```
             >{
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "Spark"
+        === ":simple-apachespark: Spark"
             Simple null level composition with an `OR` clause
             ``` python
             import splink.spark.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -197,15 +197,15 @@
             merged.as_dict()
             ```
             >{
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "Athena"
+        === ":simple-amazonaws: Athena"
             Simple null level composition with an `OR` clause
             ``` python
             import splink.athena.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
@@ -221,15 +221,15 @@
             merged.as_dict()
             ```
             >{
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
-        === "SQLite"
+        === ":simple-sqlite: SQLite"
             Simple null level composition with an `OR` clause
             ``` python
             import splink.sqlite.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
 
     Returns:
@@ -265,15 +265,15 @@
             level dictionary
         label_for_charts (str, optional): A label for this comparson level,
             which will appear on charts as a reminder of what the level represents.
         m_probability (float, optional): Starting value for m probability.
             Defaults to None.
 
     Examples:
-        === "DuckDB"
+        === ":simple-duckdb: DuckDB"
             *Not* an exact match on first name
             ``` python
             import splink.duckdb.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
@@ -284,15 +284,15 @@
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
-        === "Spark"
+        === ":simple-apachespark: Spark"
             *Not* an exact match on first name
             ``` python
             import splink.spark.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
@@ -303,15 +303,15 @@
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
-        === "Athena"
+        === ":simple-amazonaws: Athena"
             *Not* an exact match on first name
             ``` python
             import splink.athena.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
@@ -322,15 +322,15 @@
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
-        === "SQLite"
+        === ":simple-sqlite: SQLite"
             *Not* an exact match on first name
             ``` python
             import splink.sqlite.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
```

### Comparing `splink-3.9.2/splink/comparison_level_library.py` & `splink-3.9.3/splink/comparison_level_library.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,60 +13,60 @@
         on overall match weight)
         Args:
             col_name (str): Input column name
             valid_string_regex (str): regular expression pattern that if not
                 matched will result in column being treated as a null.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Simple null comparison level
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Simple null level
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Simple null level
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Simple null level
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.null_level("name")
                 ```
-            === "PostgreSQL"
+            === ":simple-postgresql: PostgreSql"
                 Simple null level
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.null_level("name")
                 ```
         Returns:
             ComparisonLevel: Comparison level for null entries
         """
 
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
@@ -111,15 +111,15 @@
             include_colname_in_charts_label (bool, optional): If True, include col_name
                 in chart labels (e.g. linker.match_weights_chart())
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
                 include_colname_in_charts_label=True
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Simple Exact match level
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
@@ -128,15 +128,15 @@
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Simple Exact match level
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
@@ -145,15 +145,15 @@
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Simple Exact match level
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
@@ -162,33 +162,33 @@
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Simple Exact match level
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
-            === "PostgreSQL"
+            === ":simple-postgresql: PostgreSql"
                 Simple Exact match level
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
                 ```
         """
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
 
         if include_colname_in_charts_label:
             label_suffix = f" {col_name}"
@@ -225,36 +225,36 @@
         self,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level for all cases which have not been
         considered by preceding comparison levels,
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.else_level("name")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.else_level("name")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.else_level("name")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.else_level("name")
-            === "PostgreSQL"
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.else_level("name")
                 ```
         """
         if isinstance(m_probability, str):
             raise ValueError(
                 "You provided a string for the value of m probability when it should "
                 "be numeric.  Perhaps you passed a column name.  Note that you do "
@@ -302,52 +302,54 @@
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability
                 Defaults to None.
 
         Examples:
 
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Apply the `levenshtein_distance` function to a comparison level
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein_distance",
                                             2,
                                             False)
-            === "SQLite
+                ```
+            === ":simple-sqlite: SQLite"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
                 ```
 
         Returns:
@@ -426,72 +428,73 @@
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
                 import splink.duckdb.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
                 import splink.spark.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
                 import splink.athena.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
-            === "SQLite"
+                ```
+            === ":simple-sqlite: SQLite"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
-                ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 levenshtein similarity
         """
         super().__init__(
             col_name,
@@ -530,44 +533,45 @@
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1)
                 ```
 
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
                 import splink.duckdb.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1)
                 ```
 
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
                 import splink.spark.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
-            === "SQLite"
+                ```
+            === ":simple-sqlite: SQLite"
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1)
                 ```
 
@@ -611,41 +615,41 @@
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level with jaro score greater than 0.9
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaro_level("name", 0.9)
                 ```
                 Comparison level with a jaro score greater than 0.9 on a substring
                 of name column as determined by a regular expression.
 
                 ```python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaro_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level with jaro score greater than 0.9
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.jaro_level("name", 0.9)
                 ```
                 Comparison level with a jaro score greater than 0.9 on a substring
                 of name column as determined by a regular expression.
 
                 ```python
                 import splink.spark.comparison_level_library as cll
                 cll.jaro_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Comparison level with jaro score greater than 0.9
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.jaro_level("name", 0.9)
                 ```
 
         Returns:
@@ -689,39 +693,39 @@
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level with jaro-winkler score greater than 0.9
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level with jaro-winkler score greater than 0.9
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Comparison level with jaro-winkler score greater than 0.9
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
 
         Returns:
@@ -770,27 +774,27 @@
                 col_name in charts label
             manual_col_name_for_charts_label (str, optional): string to include as
                  column name in chart label. Acts as a manual overwrite of the
                  colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level with jaccard score greater than 0.9
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9)
                 ```
                 Comparison level with jaccard score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level with jaccard score greater than 0.9
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9)
                 ```
                 Comparison level with jaccard score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
@@ -834,64 +838,65 @@
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
             tf_adjustment_column (str, optional): Column to use for term frequency
                 adjustments if an exact match is observed. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Comparison level on first_name and surname columns reversed
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
 
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the exact match of two
                 columns.
@@ -952,37 +957,38 @@
                 comparisons against
             not_null (bool): If true, remove any . This is only necessary if you are not
                 capturing nulls elsewhere in your comparison level.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the distance between
@@ -1032,36 +1038,37 @@
             col_name (str): Input column name
             percentage_distance_threshold (float): Percentage difference threshold for
                 the comparison level
             m_probability (float, optional): Starting value for m probability. Defaults
                 to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the percentage difference
                 between two values
 
@@ -1106,31 +1113,32 @@
                 adjustments to the exact match level. Defaults to False.
             min_intersection (int, optional): The minimum cardinality of the
                 intersection of arrays for this comparison level. Defaults to 1
             include_colname_in_charts_label (bool, optional): Should the charts label
                 contain the column name? Defaults to False
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_level_library as cll
                 cll.array_intersect_level("name")
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the size of intersection
                 of arrays
         """
@@ -1158,15 +1166,15 @@
         super().__init__(level_dict, sql_dialect=self._sql_dialect)
 
     @property
     def _size_array_intersect_function(self):
         raise NotImplementedError("Intersect function not defined on base class")
 
 
-class DateDiffLevelBase(ComparisonLevel):
+class DatediffLevelBase(ComparisonLevel):
     def __init__(
         self,
         date_col: str,
         date_threshold: int,
         date_metric: str = "day",
         m_probability=None,
         cast_strings_to_date=False,
@@ -1192,15 +1200,15 @@
                 date-casting. Defaults to False.
             date_format (str, optional): Format of input dates if date-strings
                 are given. Must be consistent across record pairs. If None
                 (the default), downstream functions for each backend assign
                 date_format to ISO 8601 format (yyyy-mm-dd).
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Date Difference comparison level at threshold 1 year
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
                 cll.datediff_level("date",
                                     date_threshold=1,
                                     date_metric="year"
                                     )
@@ -1221,15 +1229,15 @@
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y'
                                     )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Date Difference comparison level at threshold 1 year
                 ``` python
                 import splink.spark.comparison_level_library as cll
                 cll.datediff_level("date",
                                     date_threshold=1,
                                     date_metric="year"
                                     )
@@ -1249,36 +1257,66 @@
                 import splink.spark.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y'
                                     )
-            === "PostgreSQL"
+                ```
+            === ":simple-amazonaws: Athena"
+                Date Difference comparison level at threshold 1 year
+                ``` python
+                import splink.athena.comparison_level_library as cll
+                cll.datediff_level("date",
+                                    date_threshold=1,
+                                    date_metric="year"
+                                    )
+                ```
+                Date Difference comparison with date-casting and unspecified
+                date_format (default = %Y-%m-%d)
+                ``` python
+                import splink.athena.comparison_level_library as cll
+                cll.datediff_level("dob",
+                                    date_threshold=3,
+                                    date_metric='month',
+                                    cast_strings_to_date=True
+                                    )
+                ```
+                Date Difference comparison with date-casting and specified date_format
+                ``` python
+                import splink.athena.comparison_level_library as cll
+                cll.datediff_level("dob",
+                                    date_threshold=3,
+                                    date_metric='month',
+                                    cast_strings_to_date=True,
+                                    date_format='%d/%m/%Y'
+                                    )
+                ```
+            === ":simple-postgresql: PostgreSql"
                 Date Difference comparison level at threshold 1 year
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.datediff_level("date",
                                     date_threshold=1,
                                     date_metric="year"
                                     )
                 ```
                 Date Difference comparison with date-casting and unspecified
                 date_format (default = yyyy-MM-dd)
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True
                                     )
                 ```
                 Date Difference comparison with date-casting and specified date_format
                 ``` python
-                import splink.postgres.postgres_comparison_level_library as cll
+                import splink.postgres.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True,
                                     date_format='dd/MM/yyyy'
                                     )
                 ```
```

### Comparing `splink-3.9.2/splink/comparison_level_sql.py` & `splink-3.9.3/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_library.py` & `splink-3.9.3/splink/comparison_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         set_to_lowercase: bool = False,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_else=None,
         include_colname_in_charts_label=False,
     ) -> Comparison:
         """A comparison of the data in `col_name` with two levels:
+
         - Exact match
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare
             regex_extract (str): Regular expression pattern to evaluate a match on.
             valid_string_regex (str): regular expression pattern that if not
@@ -38,59 +39,60 @@
                 default m probability for the exact match level. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
             include_colname_in_charts_label: If true, append col name to label for
                 charts.  Defaults to False.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Create comparison with exact match level
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with exact match level
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Create comparison with exact match level
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Create comparison with exact match level
                 ``` python
                 import splink.sqlite.comparison_library as cl
                 cl.exact_match("first_name")
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 Create comparison with exact match level
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
 
         Returns:
             Comparison: A comparison for exact match that can be included in the Splink
                 settings dictionary
         """
@@ -109,15 +111,15 @@
                 ),
                 self._else_level(m_probability=m_probability_else),
             ],
         }
         super().__init__(comparison_dict)
 
 
-class DistanceFunctionAtThresholdsComparisonBase(Comparison):
+class DistanceFunctionAtThresholdsBase(Comparison):
     def __init__(
         self,
         col_name: str,
         distance_function_name: str,
         distance_threshold_or_thresholds: float | list,
         regex_extract: str = None,
         valid_string_regex: str = None,
@@ -169,15 +171,15 @@
             m_probability_or_probabilities_thres (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7]
                                    )
@@ -188,15 +190,15 @@
                 import splink.duckdb.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7]
                                    )
@@ -207,15 +209,15 @@
                 import splink.spark.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Apply the `levenshtein_distance` function in a comparison with
                 levels 1 and 2
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'levenshtein_distance',
                                    distance_threshold_or_thresholds = [1, 2],
@@ -227,30 +229,31 @@
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
-            === "SQLite"
+                ```
+            === ":simple-sqlite: SQLite"
                 Apply the `levenshtein` function in a comparison with
                 levels 1 and 2
                 ``` python
                 import splink.sqlite.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'levenshtein',
                                    distance_threshold_or_thresholds = [1, 2],
                                    higher_is_more_similar = False
                                    )
                 ```
-            === "PostgreSQL"
+            === ":simple-postgresql: PostgreSql"
                 Apply the `levenshtein` function in a comparison with
                 levels 1 and 2
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'levenshtein',
                                    distance_threshold_or_thresholds = [1, 2],
                                    higher_is_more_similar = False
                                    )
                 ```
                 ```
@@ -315,15 +318,15 @@
         super().__init__(comparison_dict)
 
     @property
     def _is_distance_subclass(self):
         return False
 
 
-class LevenshteinAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
+class LevenshteinAtThresholdsBase(DistanceFunctionAtThresholdsBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [1, 2],
         regex_extract: str = None,
         valid_string_regex: str = None,
         set_to_lowercase: bool = False,
@@ -361,67 +364,68 @@
             m_probability_or_probabilities_lev (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
-            === "SQLite"
+                ```
+            === ":simple-sqlite: SQLite"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
-            === "PostgreSQL"
+            === ":simple-postgresql: PostgreSql"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 ```
 
         Returns:
             Comparison: A comparison for Levenshtein similarity that can be included
                 in the Splink settings dictionary.
@@ -443,17 +447,15 @@
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
-class DamerauLevenshteinAtThresholdsComparisonBase(
-    DistanceFunctionAtThresholdsComparisonBase
-):
+class DamerauLevenshteinAtThresholdsBase(DistanceFunctionAtThresholdsBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = 1,
         regex_extract: str = None,
         valid_string_regex: str = None,
         set_to_lowercase: bool = False,
@@ -489,15 +491,15 @@
                 default m probability for the exact match level. Defaults to None.
             m_probability_or_probabilities_dl (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Create comparison with damerau-levenshtein match levels with
                 distance <= 1, 2
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with damerau-levenshtein match levels with
@@ -505,15 +507,15 @@
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with damerau-levenshtein match levels with
                 distance <= 1, 2
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with damerau-evenshtein match levels with
@@ -521,15 +523,15 @@
                 on a substring of name column as determined by a regular expression
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Create comparison with damerau-levenshtein match levels with
                 distance <= 1, 2
                 ``` python
                 import splink.sqlite.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
 
@@ -554,15 +556,15 @@
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
-class JaccardAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
+class JaccardAtThresholdsBase(DistanceFunctionAtThresholdsBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
         set_to_lowercase: bool = False,
@@ -599,30 +601,30 @@
                 default m probability for the exact match level. Defaults to None.
             m_probability_or_probabilities_jac (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
-                Examples:
-            === "DuckDB"
+        Examples:
+            === ":simple-duckdb: DuckDB"
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with jaccard match levels with similarity score >=0.9
@@ -654,15 +656,15 @@
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
-class JaroAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
+class JaroAtThresholdsBase(DistanceFunctionAtThresholdsBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
         set_to_lowercase: bool = False,
@@ -700,43 +702,43 @@
             m_probability_or_probabilities_jar (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7], regex_extract="^[A-Z]")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7], regex_extract="^[A-Z]")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
                 import splink.sqlite.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7])
                 ```
 
@@ -760,15 +762,15 @@
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
-class JaroWinklerAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
+class JaroWinklerAtThresholdsBase(DistanceFunctionAtThresholdsBase):
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         regex_extract: str = None,
         valid_string_regex: str = None,
         set_to_lowercase: bool = False,
@@ -807,15 +809,15 @@
                 If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Create comparison with jaro_winkler match levels with similarity
                 score >= 0.9 and >=0.7
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro_winkler match levels with similarity
@@ -824,15 +826,15 @@
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Create comparison with jaro_winkler match levels with similarity
                 score >=0.9 and >=0.7
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro_winkler match levels with similarity
@@ -841,15 +843,15 @@
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Create comparison with jaro_winkler match levels with similarity
                 score >=0.9 and >=0.7
                 ``` python
                 import splink.sqlite.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
 
@@ -874,15 +876,15 @@
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
 
-class ArrayIntersectAtSizesComparisonBase(Comparison):
+class ArrayIntersectAtSizesBase(Comparison):
     def __init__(
         self,
         col_name: str,
         size_or_sizes: int | list = [1],
         m_probability_or_probabilities_sizes: float | list = None,
         m_probability_else=None,
     ) -> Comparison:
@@ -904,31 +906,32 @@
             m_probability_or_probabilities_sizes (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
 
         Returns:
             Comparison: A comparison for the intersection of arrays that can be included
                 in the Splink settings dictionary.
         """
@@ -975,15 +978,15 @@
         super().__init__(comparison_dict)
 
     @property
     def _array_intersect_level(self):
         raise NotImplementedError("Intersect level not defined on base class")
 
 
-class DateDiffAtThresholdsComparisonBase(Comparison):
+class DatediffAtThresholdsBase(Comparison):
     def __init__(
         self,
         col_name: str,
         date_thresholds: int | list = [1],
         date_metrics: str | list = ["year"],
         cast_strings_to_date=False,
         date_format: str = None,
@@ -1042,15 +1045,15 @@
             m_probability_or_probabilities_dat (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Date Difference comparison at thresholds 10 days, 12 months and 15 years
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds = [10, 12, 15],
                                             date_metrics = ['day', 'month', 'year']
                                             )
@@ -1073,15 +1076,15 @@
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True,
                                             date_format='%d/%m/%Y'
                                             )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Date Difference comparison at thresholds 10 days, 12 months and 15 years
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds = [10, 12, 15],
                                             date_metrics = ['day', 'month', 'year']
                                             )
@@ -1104,39 +1107,72 @@
                 import splink.spark.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True,
                                             date_format='%d/%m/%Y'
                                             )
-            === "PostgreSQL"
+                ```
+            === "":simple-amazonaws: Athena"
+                Date Difference comparison at thresholds 10 days, 12 months and 15 years
+                ``` python
+                import splink.athena.comparison_library as cl
+                cl.datediff_at_thresholds("date",
+                                            date_thresholds = [10, 12, 15],
+                                            date_metrics = ['day', 'month', 'year']
+                                            )
+                ```
+
+                Datediff comparison with date-casting and unspecified date_format
+                (default = %Y-%m-%d)
+                ``` python
+                    import splink.athena.comparison_library as cl
+                    cl.datediff_at_thresholds("date",
+                                                date_thresholds=[1,5],
+                                                date_metrics = ["day", "year"],
+                                                cast_strings_to_date=True
+                                                )
+                ```
+
+                Datediff comparison with date-casting and specified (non-default)
+                date_format
+                ``` python
+                import splink.athena.comparison_library as cl
+                cl.datediff_at_thresholds("date",
+                                            date_thresholds=[1,5],
+                                            date_metrics = ["day", "year"],
+                                            cast_strings_to_date=True,
+                                            date_format='%d/%m/%Y'
+                                            )
+                ```
+            === ":simple-postgresql: PostgreSql"
                 Date Difference comparison at thresholds 10 days, 12 months and 15 years
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds = [10, 12, 15],
                                             date_metrics = ['day', 'month', 'year']
                                             )
                 ```
 
                 Datediff comparison with date-casting and unspecified date_format
                 (default = yyyy-MM-dd)
                 ``` python
-                    import splink.postgres.postgres_comparison_library as cl
+                    import splink.postgres.comparison_library as cl
                     cl.datediff_at_thresholds("date",
                                                 date_thresholds=[1,5],
                                                 date_metrics = ["day", "year"],
                                                 cast_strings_to_date=True
                                                 )
                 ```
 
                 Datediff comparison with date-casting and specified (non-default)
                 date_format
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True,
                                             date_format='dd/MM/yyyy'
                                             )
                 ```
@@ -1206,15 +1242,15 @@
         super().__init__(comparison_dict)
 
     @property
     def _datediff_level(self):
         raise NotImplementedError("Datediff level not defined on base class")
 
 
-class DistanceInKMAtThresholdsComparisonBase(Comparison):
+class DistanceInKMAtThresholdsBase(Comparison):
     def __init__(
         self,
         lat_col: str,
         long_col: str,
         km_thresholds: int | list = [0.1, 1],
         include_exact_match_level=False,
         m_probability_exact_match=None,
@@ -1247,40 +1283,41 @@
             m_probability_or_probabilities_km (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
-            === "PostgreSQL"
+                ```
+            === ":simple-postgresql: PostgreSql"
                 ``` python
-                import splink.postgres.postgres_comparison_library as cl
+                import splink.postgres.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
 
         Returns:
```

### Comparing `splink-3.9.2/splink/comparison_library_utils.py` & `splink-3.9.3/splink/comparison_library_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         raise ValueError("\n\n".join(error_logger))
 
     return
 
 
 def datediff_error_logger(thresholds, metrics):
-    # Extracted from the DateDiffAtThresholdsComparisonBase class as that was overly
+    # Extracted from the DatediffAtThresholdsBase class as that was overly
     # verbose and failing the lint.
 
     error_logger = []
 
     if len(metrics) == 0:
         error_logger.append(
             "`date_metrics` must have at least one element, so that Comparison "
```

### Comparing `splink-3.9.2/splink/comparison_template_library.py` & `splink-3.9.3/splink/comparison_template_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             m_probability_or_probabilities_datediff (Union[float, list], optional):
                 If provided, overrides the default m probabilities
                 for the datediff thresholds specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Basic Date Comparison
                 ``` python
                 import splink.duckdb.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth")
                 ```
                 Bespoke Date Comparison
                 ``` python
@@ -125,15 +125,15 @@
                 ``` python
                 import splink.duckdb.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth",
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y',
                                     invalid_dates_as_null=True)
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Basic Date Comparison
                 ``` python
                 import splink.spark.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth")
                 ```
                 Bespoke Date Comparison
                 ``` python
@@ -385,15 +385,15 @@
                 Starting m probabilities for the jaccard thresholds specified.
                 Defaults to None.
             m_probability_else (_type_, optional): Starting m probability for
                 the 'everything else' level. Defaults to None.
 
         Examples:
 
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Basic Name Comparison
                 ``` python
                 import splink.duckdb.comparison_template_library as ctl
                 ctl.name_comparison("name")
                 ```
                 Bespoke Name Comparison
                 ``` python
@@ -403,15 +403,15 @@
                                     term_frequency_adjustments = True,
                                     levenshtein_thresholds=[2],
                                     damerau_levenshtein_thresholds=[],
                                     jaro_winkler_thresholds=[],
                                     jaccard_thresholds=[1]
                                     )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Basic Name Comparison
                 ``` python
                 import splink.spark.comparison_template_library as ctl
                 ctl.name_comparison("name")
                 ```
                 Bespoke Name Comparison
                 ``` python
@@ -420,15 +420,16 @@
                                     phonetic_col_name = "name_dm",
                                     term_frequency_adjustments = True,
                                     levenshtein_thresholds=[2],
                                     damerau_levenshtein_thresholds=[],
                                     jaro_winkler_thresholds=[],
                                     jaccard_thresholds=[1]
                                     )
-            === "SQLite"
+                ```
+            === ":simple-sqlite: SQLite"
                 Basic Name Comparison
                 ``` python
                 import splink.sqlite.comparison_template_library as ctl
                 ctl.name_comparison("name")
                 ```
                 Bespoke Name Comparison
                 ``` python
@@ -761,15 +762,15 @@
             m_probability_or_probabilities_forename_jac (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Basic Forename Surname Comparison
                 ```py
                 import splink.duckdb.comparison_template_library as ctl
                 ctl.forename_surname_comparison("first_name", "surname)
                 ```
 
                 Bespoke Forename Surname Comparison
@@ -783,15 +784,15 @@
                         phonetic_forename_col_name="forename_dm",
                         phonetic_surname_col_name="surname_dm",
                         levenshtein_thresholds=[2],
                         jaro_winkler_thresholds=[],
                         jaccard_thresholds=[1],
                     )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Basic Forename Surname Comparison
                 ```py
                 import splink.spark.comparison_template_library as ctl
                 ctl.forename_surname_comparison("first_name", "surname)
                 ```
 
                 Bespoke Forename Surname Comparison
@@ -805,15 +806,15 @@
                         phonetic_forename_col_name="forename_dm",
                         phonetic_surname_col_name="surname_dm",
                         levenshtein_thresholds=[2],
                         jaro_winkler_thresholds=[],
                         jaccard_thresholds=[1],
                     )
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 Basic Forename Surname Comparison
                 ```py
                 import splink.sqlite.comparison_template_library as ctl
                 ctl.forename_surname_comparison("first_name", "surname)
                 ```
 
                 Bespoke Forename Surname Comparison
@@ -1212,15 +1213,15 @@
                 probability for area match level. Defaults to None.
             m_probability_or_probabilities_km_distance (float, optional): Starting m
                 probability for 'distance in km' level. Defaults to None.
             m_probability_else (float, optional): Starting m probability for
                 the 'everything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Basic Postcode Comparison
                 ``` python
                 import splink.duckdb.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
@@ -1229,15 +1230,15 @@
                                     invalid_postcodes_as_null=True,
                                     include_distance_in_km_level=True,
                                     lat_col="lat",
                                     long_col="long",
                                     km_thresholds=[10, 100]
                                     )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Basic Postcode Comparison
                 ``` python
                 import splink.spark.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
@@ -1246,15 +1247,15 @@
                                     invalid_postcodes_as_null=True,
                                     include_distance_in_km_level=True,
                                     lat_col="lat",
                                     long_col="long",
                                     km_thresholds=[10, 100]
                                     )
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 Basic Postcode Comparison
                 ``` python
                 import splink.athena.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
@@ -1473,15 +1474,15 @@
                 for the thresholds specified. Defaults to None.
             m_probability_domain_match (float, optional): Starting m probability
                 for domain only match level. Defaults to None.
             m_probability_else (float, optional): Starting m probability for
                 the 'everything else' level. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Basic email Comparison
                 ``` python
                 import splink.duckdb.duckdb_comparison_template_library as ctl
                 ctl.email_comparison("email")
                 ```
                 Bespoke email Comparison
                 ``` python
@@ -1490,15 +1491,15 @@
                                     levenshtein_thresholds = [2],
                                     damerau_levenshtein_thresholds = [2],
                                     invalid_emails_as_null = True,
                                     include_username_match_level = True,
                                     include_domain_match_level = True,
                                     )
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Basic email Comparison
                 ``` python
                 import splink.spark.spark_comparison_template_library as ctl
                 ctl.email_comparison(col_name = "email")
                 ```
                 Bespoke email Comparison
                 ``` python
```

### Comparing `splink-3.9.2/splink/comparison_vector_distribution.py` & `splink-3.9.3/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/comparison_vector_values.py` & `splink-3.9.3/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/connected_components.py` & `splink-3.9.3/splink/connected_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,42 +483,35 @@
         )
         linker._enqueue_sql(sql, "r")
         # Update our rep_match column in the representatives table.
         sql = _cc_update_representatives_loop_cond(
             prev_representatives_table.physical_name
         )
 
-        # To allow debug mode to work with our recursive loop, add
-        # the iteration number as a suffix
-        if linker.debug_mode:
-            repr_name = "__splink__df_representatives"
-        else:
-            repr_name = f"__splink__df_representatives_{iteration}"
+        repr_name = f"__splink__df_representatives_{iteration}"
 
         representatives = linker._enqueue_sql(
             sql,
             repr_name,
         )
 
         representatives = linker._execute_sql_pipeline([neighbours])
         # Update table reference
-        prev_representatives_table.drop_table_from_database()
+        prev_representatives_table.drop_table_from_database_and_remove_from_cache()
         prev_representatives_table = representatives
 
         # Check if our exit condition has been met...
         sql = _cc_assess_exit_condition(representatives.physical_name)
 
         linker._enqueue_sql(sql, "__splink__df_root_rows")
 
-        root_rows_df = linker._execute_sql_pipeline(
-            materialise_as_hash=False, use_cache=False
-        )
+        root_rows_df = linker._execute_sql_pipeline(use_cache=False)
 
         root_rows = root_rows_df.as_record_dict()
-        root_rows_df.drop_table_from_database()
+        root_rows_df.drop_table_from_database_and_remove_from_cache()
         root_rows = root_rows[0]["count"]
         logger.info(f"Completed iteration {iteration}, root rows count {root_rows}")
         end_time = time.time()
         logger.log(15, f"    Iteration time: {end_time - start_time} seconds")
 
     # Create our final representatives table
     # Need to edit how we export the table based on whether we are
```

### Comparing `splink-3.9.2/splink/convert_v2_to_v3.py` & `splink-3.9.3/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/databricks/enable_splink.py` & `splink-3.9.3/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/default_from_jsonschema.py` & `splink-3.9.3/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/dialect_base.py` & `splink-3.9.3/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_base.py` & `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     date_format=None,
 ):
     if date_format is None:
         date_format = "%Y-%m-%d"
 
     if cast_str:
         return f"""
-            abs(date_diff('{date_metric}',strptime({col_name_l},
-              '{date_format}'),strptime({col_name_r},
-              '{date_format}'))) <= {date_threshold}
+            abs(date_diff('{date_metric}',
+                strptime({col_name_l}, '{date_format}'),
+                strptime({col_name_r}, '{date_format}'))
+                ) <= {date_threshold}
         """
     else:
         return f"""
             abs(date_diff('{date_metric}', {col_name_l},
               {col_name_r})) <= {date_threshold}
         """
```

### Comparing `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py` & `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
     DamerauLevenshteinLevelBase,
-    DateDiffLevelBase,
+    DatediffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     JaccardLevelBase,
     JaroLevelBase,
     JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
-    ArrayIntersectAtSizesComparisonBase,
-    DamerauLevenshteinAtThresholdsComparisonBase,
-    DateDiffAtThresholdsComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
-    DistanceInKMAtThresholdsComparisonBase,
+    ArrayIntersectAtSizesBase,
+    DamerauLevenshteinAtThresholdsBase,
+    DatediffAtThresholdsBase,
+    DistanceFunctionAtThresholdsBase,
+    DistanceInKMAtThresholdsBase,
     ExactMatchBase,
-    JaccardAtThresholdsComparisonBase,
-    JaroAtThresholdsComparisonBase,
-    JaroWinklerAtThresholdsComparisonBase,
-    LevenshteinAtThresholdsComparisonBase,
+    JaccardAtThresholdsBase,
+    JaroAtThresholdsBase,
+    JaroWinklerAtThresholdsBase,
+    LevenshteinAtThresholdsBase,
 )
 from ...comparison_template_library import (
     DateComparisonBase,
     EmailComparisonBase,
     ForenameSurnameComparisonBase,
     NameComparisonBase,
     PostcodeComparisonBase,
@@ -144,85 +144,79 @@
     pass
 
 
 class distance_in_km_level(DuckDBBase, DistanceInKMLevelBase):
     pass
 
 
-class datediff_level(DuckDBBase, DateDiffLevelBase):
+class datediff_level(DuckDBBase, DatediffLevelBase):
     pass
 
 
 ##########################
 ### COMPARISON LIBRARY ###
 ##########################
 class exact_match(DuckDBComparisonProperties, ExactMatchBase):
     pass
 
 
 class distance_function_at_thresholds(
-    DuckDBComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+    DuckDBComparisonProperties, DistanceFunctionAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._distance_function_level
 
 
 class levenshtein_at_thresholds(
-    DuckDBComparisonProperties, LevenshteinAtThresholdsComparisonBase
+    DuckDBComparisonProperties, LevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._levenshtein_level
 
 
 class damerau_levenshtein_at_thresholds(
-    DuckDBComparisonProperties, DamerauLevenshteinAtThresholdsComparisonBase
+    DuckDBComparisonProperties, DamerauLevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._damerau_levenshtein_level
 
 
-class jaro_at_thresholds(DuckDBComparisonProperties, JaroAtThresholdsComparisonBase):
+class jaro_at_thresholds(DuckDBComparisonProperties, JaroAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._jaro_level
 
 
 class jaro_winkler_at_thresholds(
-    DuckDBComparisonProperties, JaroWinklerAtThresholdsComparisonBase
+    DuckDBComparisonProperties, JaroWinklerAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._jaro_winkler_level
 
 
-class jaccard_at_thresholds(
-    DuckDBComparisonProperties, JaccardAtThresholdsComparisonBase
-):
+class jaccard_at_thresholds(DuckDBComparisonProperties, JaccardAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._jaccard_level
 
 
-class array_intersect_at_sizes(
-    DuckDBComparisonProperties, ArrayIntersectAtSizesComparisonBase
-):
+class array_intersect_at_sizes(DuckDBComparisonProperties, ArrayIntersectAtSizesBase):
     pass
 
 
-class datediff_at_thresholds(
-    DuckDBComparisonProperties, DateDiffAtThresholdsComparisonBase
-):
+class datediff_at_thresholds(DuckDBComparisonProperties, DatediffAtThresholdsBase):
     pass
 
 
 class distance_in_km_at_thresholds(
-    DuckDBComparisonProperties, DistanceInKMAtThresholdsComparisonBase
+    DuckDBComparisonProperties, DistanceInKMAtThresholdsBase
 ):
     pass
 
 
 ###################################
 ### COMPARISON TEMPLATE LIBRARY ###
 ###################################
```

### Comparing `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/duckdb/linker.py` & `splink-3.9.3/splink/duckdb/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         col_strings = list(d.keys())
         return [InputColumn(c, sql_dialect="duckdb") for c in col_strings]
 
     def validate(self):
         pass
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         self._check_drop_table_created_by_splink(force_non_splink_table)
 
         self.linker._delete_table_from_database(self.physical_name)
 
     def as_record_dict(self, limit=None):
         sql = f"select * from {self.physical_name}"
         if limit:
@@ -101,14 +101,15 @@
         self,
         input_table_or_tables: str | list,
         settings_dict: dict | str = None,
         connection: str | DuckDBPyConnection = ":memory:",
         set_up_basic_logging: bool = True,
         output_schema: str = None,
         input_table_aliases: str | list = None,
+        validate_settings: bool = True,
     ):
         """The Linker object manages the data linkage process and holds the data linkage
         model.
 
         Most of Splink's functionality can  be accessed by calling functions (methods)
         on the linker, such as `linker.predict()`, `linker.profile_columns()` etc.
 
@@ -130,14 +131,16 @@
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             output_schema (str, optional): Set the schema along which all tables
                 will be created.
             input_table_aliases (Union[str, list], optional): Labels assigned to
                 input tables in Splink outputs.  If the names of the tables in the
                 input database are long or unspecific, this argument can be used
                 to attach more easily readable/interpretable names. Defaults to None.
+            validate_settings (bool, optional): When True, check your settings
+                dictionary for any potential errors that may cause splink to fail.
         """
 
         self._sql_dialect_ = "duckdb"
 
         validate_duckdb_connection(connection, logger)
 
         if isinstance(connection, str):
@@ -176,14 +179,15 @@
 
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
+            validate_settings=validate_settings,
         )
 
         # Quickly check for casting error in duckdb/pandas
         for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
             if isinstance(table, pd.DataFrame):
                 if isinstance(alias, pd.DataFrame):
                     alias = f"__splink__input_table_{i}"
```

### Comparing `splink-3.9.2/splink/em_training_session.py` & `splink-3.9.3/splink/em_training_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         linker: Linker,
         blocking_rule_for_training: str,
         fix_u_probabilities: bool = False,
         fix_m_probabilities: bool = False,
         fix_probability_two_random_records_match: bool = False,
         comparisons_to_deactivate: list[Comparison] = None,
         comparison_levels_to_reverse_blocking_rule: list[ComparisonLevel] = None,
+        estimate_without_term_frequencies: bool = False,
     ):
         logger.info("\n----- Starting EM training session -----\n")
 
         self._original_settings_obj = linker._settings_obj
         self._original_linker = linker
         self._training_linker = deepcopy(linker)
 
@@ -53,14 +54,17 @@
         self._settings_obj._training_mode = True
 
         if not isinstance(blocking_rule_for_training, BlockingRule):
             blocking_rule = BlockingRule(blocking_rule_for_training)
 
         self._settings_obj._blocking_rule_for_training = blocking_rule
         self._blocking_rule_for_training = blocking_rule
+        self._settings_obj._estimate_without_term_frequencies = (
+            estimate_without_term_frequencies
+        )
 
         if comparison_levels_to_reverse_blocking_rule:
             self._comparison_levels_to_reverse_blocking_rule = (
                 comparison_levels_to_reverse_blocking_rule
             )
         else:
             self._comparison_levels_to_reverse_blocking_rule = self._original_settings_obj._get_comparison_levels_corresponding_to_training_blocking_rule(  # noqa
```

### Comparing `splink-3.9.2/splink/estimate_u.py` & `splink-3.9.3/splink/estimate_u.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,29 +56,29 @@
         from __splink__df_concat_with_tf
         """
 
         training_linker._enqueue_sql(sql, "__splink__df_concat_count")
         dataframe = training_linker._execute_sql_pipeline([nodes_with_tf])
 
         result = dataframe.as_record_dict()
-        dataframe.drop_table_from_database()
+        dataframe.drop_table_from_database_and_remove_from_cache()
         total_nodes = result[0]["count"]
         sample_size = _rows_needed_for_n_pairs(max_pairs)
         proportion = sample_size / total_nodes
 
     if settings_obj._link_type == "link_only":
         sql = """
         select count(source_dataset) as count
         from __splink__df_concat_with_tf
         group by source_dataset
         """
         training_linker._enqueue_sql(sql, "__splink__df_concat_count")
         dataframe = training_linker._execute_sql_pipeline([nodes_with_tf])
         result = dataframe.as_record_dict()
-        dataframe.drop_table_from_database()
+        dataframe.drop_table_from_database_and_remove_from_cache()
         frame_counts = [res["count"] for res in result]
         # total valid links is sum of pairwise product of individual row counts
         # i.e. if frame_counts are [a, b, c, d, ...],
         # total_links = a*b + a*c + a*d + ... + b*c + b*d + ... + c*d + ...
         total_links = (
             sum(frame_counts) ** 2 - sum([count**2 for count in frame_counts])
         ) / 2
@@ -132,16 +132,16 @@
 
     sql = compute_new_parameters_sql(settings_obj)
     linker._enqueue_sql(sql, "__splink__m_u_counts")
     df_params = training_linker._execute_sql_pipeline(sample_dataframe)
 
     param_records = df_params.as_pandas_dataframe()
     param_records = compute_proportions_for_new_parameters(param_records)
-    df_params.drop_table_from_database()
-    df_sample.drop_table_from_database()
+    df_params.drop_table_from_database_and_remove_from_cache()
+    df_sample.drop_table_from_database_and_remove_from_cache()
 
     m_u_records = [
         r
         for r in param_records
         if r["output_column_name"] != "_probability_two_random_records_match"
     ]
```

### Comparing `splink-3.9.2/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/comparator_score_chart.json` & `splink-3.9.3/splink/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-3.9.3/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/completeness.json` & `splink-3.9.3/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.3/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.3/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.3/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.3/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/missingness.json` & `splink-3.9.3/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.3/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/phonetic_match_chart.json` & `splink-3.9.3/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/precision_recall.json` & `splink-3.9.3/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.9.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/profile_data.json` & `splink-3.9.3/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/roc.json` & `splink-3.9.3/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-3.9.3/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.3/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.3/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.3/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/external_js/vega@5.21.0` & `splink-3.9.3/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/settings_jsonschema.json` & `splink-3.9.3/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.3/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.3/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.3/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.3/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.3/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/input_column.py` & `splink-3.9.3/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/linker.py` & `splink-3.9.3/splink/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import hashlib
 import json
 import logging
 import os
 import re
+import time
 import warnings
-from collections import UserDict
 from copy import copy, deepcopy
 from pathlib import Path
 from statistics import median
 
 import sqlglot
 
 from splink.input_column import InputColumn, remove_quotes_from_identifiers
@@ -22,14 +22,15 @@
     truth_space_table_from_labels_table,
 )
 from .analyse_blocking import (
     cumulative_comparisons_generated_by_blocking_rules,
     number_of_comparisons_generated_by_blocking_rule_sql,
 )
 from .blocking import BlockingRule, block_using_rules_sql
+from .cache_dict_with_logging import CacheDictWithLogging
 from .charts import (
     completeness_chart,
     cumulative_blocking_rule_comparisons_generated,
     match_weights_histogram,
     missingness_chart,
     parameter_estimate_comparisons,
     precision_recall_chart,
@@ -47,34 +48,40 @@
 from .connected_components import (
     _cc_create_unique_id_cols,
     solve_connected_components,
 )
 from .em_training_session import EMTrainingSession
 from .estimate_u import estimate_u_values
 from .exceptions import SplinkException
+from .labelling_tool import (
+    generate_labelling_tool_comparisons,
+    render_labelling_tool_html,
+)
 from .logging_messages import execute_sql_logging_message_info, log_sql
 from .m_from_labels import estimate_m_from_pairwise_labels
 from .m_training import estimate_m_values_from_label_column
 from .match_key_analysis import (
     count_num_comparisons_from_blocking_rules_for_prediction_sql,
 )
 from .match_weights_histogram import histogram_data
 from .misc import (
     ascii_uid,
     bayes_factor_to_prob,
     ensure_is_list,
     ensure_is_tuple,
     find_unique_source_dataset,
+    parse_duration,
     prob_to_bayes_factor,
 )
 from .missingness import completeness_data, missingness_data
 from .pipeline import SQLPipeline
 from .predict import predict_from_comparison_vectors_sqls
 from .profile_data import profile_columns
 from .settings import Settings
+from .settings_validator import InvalidSettingsLogger
 from .splink_comparison_viewer import (
     comparison_viewer_table_sqls,
     render_splink_comparison_viewer_html,
 )
 from .splink_dataframe import SplinkDataFrame
 from .term_frequencies import (
     _join_tf_to_input_df_sql,
@@ -92,40 +99,14 @@
 from .vertically_concatenate import vertically_concatenate_sql
 
 logger = logging.getLogger(__name__)
 
 warnings.simplefilter("always", DeprecationWarning)
 
 
-class CacheDictWithLogging(UserDict):
-    def __getitem__(self, key) -> SplinkDataFrame:
-        splink_dataframe = super().__getitem__(key)
-        phy_name = splink_dataframe.physical_name
-        logger.debug(
-            f"Using cache for template name {key}" f" with physical name {phy_name}"
-        )
-        splink_dataframe.templated_name = key
-        # Return a copy so that user can modify physical or templated name
-        # without modifying the version in the cache
-        return copy(splink_dataframe)
-
-    def __setitem__(self, key, value):
-        if not isinstance(value, SplinkDataFrame):
-            raise TypeError("Cached items must be of type SplinkDataFrame")
-
-        super().__setitem__(key, value)
-
-        logger.log(
-            1, f"Setting cache for template name {key}" f" with physical name {value}"
-        )
-
-    def invalidate_cache(self):
-        self.data = dict()
-
-
 class Linker:
     """The Linker object manages the data linkage process and holds the data linkage
     model.
 
     Most of Splink's functionality can  be accessed by calling methods (functions)
     on the linker, such as `linker.predict()`, `linker.profile_columns()` etc.
 
@@ -136,20 +117,21 @@
     def __init__(
         self,
         input_table_or_tables: str | list,
         settings_dict: dict | Path,
         accepted_df_dtypes,
         set_up_basic_logging: bool = True,
         input_table_aliases: str | list = None,
+        validate_settings: bool = True,
     ):
         """Initialise the linker object, which manages the data linkage process and
         holds the data linkage model.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Dedupe
                 ```py
                 df = pd.read_csv("data_to_dedupe.csv")
                 linker = DuckDBLinker(df, settings_dict)
                 ```
                 Link
                 ```py
@@ -162,15 +144,15 @@
                     )
                 ```
                 Dedupe with a pre-trained model read from a json file
                 ```py
                 df = pd.read_csv("data_to_dedupe.csv")
                 linker = DuckDBLinker(df, "model.json")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Dedupe
                 ```py
                 df = spark.read.csv("data_to_dedupe.csv")
                 linker = SparkLinker(df, settings_dict)
                 ```
                 Link
                 ```py
@@ -201,14 +183,16 @@
                 `linker.load_settings()` or `linker.load_model()` Defaults to None.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             input_table_aliases (Union[str, list], optional): Labels assigned to
                 input tables in Splink outputs.  If the names of the tables in the
                 input database are long or unspecific, this argument can be used
                 to attach more easily readable/interpretable names. Defaults to None.
+            validate_settings (bool, optional): When True, check your settings
+                dictionary for any potential errors that may cause splink to fail.
         """
         self._db_schema = "splink"
         if set_up_basic_logging:
             logging.basicConfig(
                 format="%(message)s",
             )
             splink_logger = logging.getLogger("splink")
@@ -235,16 +219,19 @@
         )
 
         self._input_tables_dict = self._get_input_tables_dict(
             homogenised_tables, homogenised_aliases
         )
 
         self._validate_input_dfs()
+        self._validate_settings(validate_settings)
         self._em_training_sessions = []
 
+        self._intermediate_table_cache: CacheDictWithLogging = CacheDictWithLogging()
+
         self._find_new_matches_mode = False
         self._train_u_using_random_sample_mode = False
         self._compare_two_records_mode = False
         self._self_link_mode = False
         self._analyse_blocking_mode = False
         self._deterministic_link_mode = False
 
@@ -283,15 +270,18 @@
         if self._self_link_mode:
             return "__splink__df_concat_with_tf"
 
         if self._compare_two_records_mode:
             return "__splink__compare_two_records_left_with_tf"
 
         if self._train_u_using_random_sample_mode:
-            return "__splink__df_concat_with_tf_sample"
+            if self._two_dataset_link_only:
+                return "__splink__df_concat_with_tf_sample_left"
+            else:
+                return "__splink__df_concat_with_tf_sample"
 
         if self._analyse_blocking_mode:
             return "__splink__df_concat"
 
         if self._two_dataset_link_only:
             return "__splink__df_concat_with_tf_left"
 
@@ -305,21 +295,24 @@
         if self._self_link_mode:
             return "__splink__df_concat_with_tf"
 
         if self._compare_two_records_mode:
             return "__splink__compare_two_records_right_with_tf"
 
         if self._train_u_using_random_sample_mode:
-            return "__splink__df_concat_with_tf_sample"
+            if self._two_dataset_link_only:
+                return "__splink__df_concat_with_tf_sample_right"
+            else:
+                return "__splink__df_concat_with_tf_sample"
 
         if self._analyse_blocking_mode:
             return "__splink__df_concat"
 
         if self._two_dataset_link_only:
-            return "__splink_df_concat_with_tf_right"
+            return "__splink__df_concat_with_tf_right"
         return "__splink__df_concat_with_tf"
 
     @property
     def _source_dataset_column_name(self):
         if self._settings_obj_ is None:
             return None
 
@@ -340,20 +333,14 @@
         # concatenation of all input datasets
         if self._find_new_matches_mode:
             return True
 
         if self._compare_two_records_mode:
             return True
 
-        # in u-train sample mode we are joining the concatenated table mixing
-        # both data sets - hence if we inner join on True we will end up with
-        # samples which both originate from the same dataset
-        if self._train_u_using_random_sample_mode:
-            return False
-
         if self._analyse_blocking_mode:
             return False
 
         if (
             len(self._input_tables_dict) == 2
             and self._settings_obj._link_type == "link_only"
         ):
@@ -460,23 +447,37 @@
             settings_dict["linker_uid"] = uid
 
         if settings_dict is None:
             self._settings_obj_ = None
         else:
             self._settings_obj_ = Settings(settings_dict)
 
-            self._validate_dialect()
+    def _validate_settings(self, validate_settings):
+        if (
+            # no settings to check
+            self._settings_obj_ is None
+            or
+            # raw tables don't yet exist in db
+            not hasattr(self, "_input_tables_dict")
+        ):
+            return
+
+        self.settings_validator = InvalidSettingsLogger(self)
+        self.settings_validator._validate_dialect()
+        # Constructs output logs for our various settings inputs
+        if validate_settings:
+            self.settings_validator.construct_output_logs()
 
     def _initialise_df_concat(self, materialise=False):
         cache = self._intermediate_table_cache
         concat_df = None
         if "__splink__df_concat" in cache:
-            concat_df = cache["__splink__df_concat"]
+            concat_df = cache.get_with_logging("__splink__df_concat")
         elif "__splink__df_concat_with_tf" in cache:
-            concat_df = cache["__splink__df_concat_with_tf"]
+            concat_df = cache.get_with_logging("__splink__df_concat_with_tf")
             concat_df.templated_name = "__splink__df_concat"
         else:
             if materialise:
                 # Clear the pipeline if we are materialising
                 # There's no reason not to do this, since when
                 # we execute the pipeline, it'll get cleared anyway
                 self._pipeline.reset()
@@ -488,15 +489,15 @@
 
         return concat_df
 
     def _initialise_df_concat_with_tf(self, materialise=True):
         cache = self._intermediate_table_cache
         nodes_with_tf = None
         if "__splink__df_concat_with_tf" in cache:
-            nodes_with_tf = cache["__splink__df_concat_with_tf"]
+            nodes_with_tf = cache.get_with_logging("__splink__df_concat_with_tf")
 
         else:
             if materialise:
                 # Clear the pipeline if we are materialising
                 # There's no reason not to do this, since when
                 # we execute the pipeline, it'll get cleared anyway
                 self._pipeline.reset()
@@ -538,26 +539,23 @@
     def _enqueue_sql(self, sql, output_table_name):
         """Add sql to the current pipeline, but do not execute the pipeline."""
         self._pipeline.enqueue_sql(sql, output_table_name)
 
     def _execute_sql_pipeline(
         self,
         input_dataframes: list[SplinkDataFrame] = [],
-        materialise_as_hash=True,
         use_cache=True,
     ) -> SplinkDataFrame:
         """Execute the SQL queued in the current pipeline as a single statement
         e.g. `with a as (), b as , c as (), select ... from c`, then execute the
         pipeline, returning the resultant table as a SplinkDataFrame
 
         Args:
             input_dataframes (List[SplinkDataFrame], optional): A 'starting point' of
                 SplinkDataFrames if needed. Defaults to [].
-            materialise_as_hash (bool, optional): If true, the output tablename will end
-                in a unique identifer. Defaults to True.
             use_cache (bool, optional): If true, look at whether the SQL pipeline has
                 been executed before, and if so, use the existing result. Defaults to
                 True.
 
         Returns:
             SplinkDataFrame: An abstraction representing the table created by the sql
                 pipeline
@@ -568,38 +566,41 @@
 
             output_tablename_templated = self._pipeline.queue[-1].output_table_name
 
             try:
                 dataframe = self._sql_to_splink_dataframe_checking_cache(
                     sql_gen,
                     output_tablename_templated,
-                    materialise_as_hash,
                     use_cache,
                 )
             except Exception as e:
                 raise e
             finally:
                 self._pipeline.reset()
 
             return dataframe
         else:
             # In debug mode, we do not pipeline the sql and print the
             # results of each part of the pipeline
             for task in self._pipeline._generate_pipeline_parts(input_dataframes):
+                start_time = time.time()
                 output_tablename = task.output_table_name
                 sql = task.sql
-                print("------")
-                print(f"--------Creating table: {output_tablename}--------")
+                print("------")  # noqa: T201
+                print(  # noqa: T201
+                    f"--------Creating table: {output_tablename}--------"
+                )
 
                 dataframe = self._sql_to_splink_dataframe_checking_cache(
                     sql,
                     output_tablename,
-                    materialise_as_hash=False,
                     use_cache=False,
                 )
+                run_time = parse_duration(time.time() - start_time)
+                print(f"Step ran in: {run_time}")  # noqa: T201
             self._pipeline.reset()
             return dataframe
 
     def _execute_sql_against_backend(
         self, sql: str, templated_name: str, physical_name: str
     ) -> SplinkDataFrame:
         """Execute a single sql SELECT statement, returning a SplinkDataFrame.
@@ -707,33 +708,33 @@
 
     def query_sql(self, sql, output_type="pandas"):
         """
         Run a SQL query against your backend database and return
         the resulting output.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ```py
                 linker = DuckDBLinker(df, settings)
                 df_predict = linker.predict()
                 linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ```py
                 linker = SparkLinker(df, settings)
                 df_predict = linker.predict()
                 linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ```py
                 linker = AthenaLinker(df, settings)
                 df_predict = linker.predict()
                 linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 ```py
                 linker = SQLiteLinker(df, settings)
                 df_predict = linker.predict()
                 linker.query_sql(f"select * from {df_predict.physical_name} limit 10")
             ```
 
         Args:
@@ -743,36 +744,34 @@
         """
 
         output_tablename_templated = "__splink__df_sql_query"
 
         splink_dataframe = self._sql_to_splink_dataframe_checking_cache(
             sql,
             output_tablename_templated,
-            materialise_as_hash=False,
             use_cache=False,
         )
 
         if output_type in ("splink_df", "splinkdf"):
             return splink_dataframe
         elif output_type == "pandas":
             out = splink_dataframe.as_pandas_dataframe()
             # If pandas, drop the table to cleanup the db
-            splink_dataframe.drop_table_from_database()
+            splink_dataframe.drop_table_from_database_and_remove_from_cache()
             return out
         else:
             raise ValueError(
                 f"output_type '{output_type}' is not supported.",
                 "Must be one of 'splink_df'/'splinkdf' or 'pandas'",
             )
 
     def _sql_to_splink_dataframe_checking_cache(
         self,
         sql,
         output_tablename_templated,
-        materialise_as_hash=True,
         use_cache=True,
     ) -> SplinkDataFrame:
         """Execute sql, or if identical sql has been run before, return cached results.
 
         This function
             - is used by _execute_sql_pipeline to to execute SQL
             - or can be used directly if you have a single SQL statement that's
@@ -783,53 +782,72 @@
 
         to_hash = (sql + self._cache_uid).encode("utf-8")
         hash = hashlib.sha256(to_hash).hexdigest()[:9]
         # Ensure hash is valid sql table name
         table_name_hash = f"{output_tablename_templated}_{hash}"
 
         if use_cache:
-            if self._table_exists_in_database(output_tablename_templated):
-                logger.debug(f"Using existing table {output_tablename_templated}")
-                return self._table_to_splink_dataframe(
-                    output_tablename_templated, output_tablename_templated
+            # Certain tables are put in the cache using their templated_name
+            # An example is __splink__df_concat_with_tf
+            # These tables are put in the cache when they are first calculated
+            # e.g. with _initialise_df_concat_with_tf()
+            # But they can also be put in the cache manually using
+            # e.g. register_table_input_nodes_concat_with_tf()
+
+            # Look for these 'named' tables in the cache prior
+            # to looking for the hashed version
+
+            if output_tablename_templated in self._intermediate_table_cache:
+                return self._intermediate_table_cache.get_with_logging(
+                    output_tablename_templated
                 )
 
+            if table_name_hash in self._intermediate_table_cache:
+                return self._intermediate_table_cache.get_with_logging(table_name_hash)
+
+            # If not in cache, fall back on checking the database
             if self._table_exists_in_database(table_name_hash):
                 logger.debug(
-                    f"Using cache for {output_tablename_templated}"
-                    f" with physical name {table_name_hash}"
+                    f"Found cache for {output_tablename_templated} "
+                    f"in database using table name with physical name {table_name_hash}"
                 )
                 return self._table_to_splink_dataframe(
                     output_tablename_templated, table_name_hash
                 )
 
         if self.debug_mode:
-            print(sql)
-
-        if materialise_as_hash:
-            splink_dataframe = self._execute_sql_against_backend(
-                sql, output_tablename_templated, table_name_hash
-            )
-        else:
+            print(sql)  # noqa: T201
             splink_dataframe = self._execute_sql_against_backend(
                 sql,
                 output_tablename_templated,
                 output_tablename_templated,
             )
 
-        self._names_of_tables_created_by_splink.add(splink_dataframe.physical_name)
+            self._intermediate_table_cache.executed_queries.append(splink_dataframe)
 
-        if self.debug_mode:
             df_pd = splink_dataframe.as_pandas_dataframe()
             try:
                 from IPython.display import display
 
                 display(df_pd)
             except ModuleNotFoundError:
-                print(df_pd)
+                print(df_pd)  # noqa: T201
+
+        else:
+            splink_dataframe = self._execute_sql_against_backend(
+                sql, output_tablename_templated, table_name_hash
+            )
+            self._intermediate_table_cache.executed_queries.append(splink_dataframe)
+
+        splink_dataframe.created_by_splink = True
+        splink_dataframe.sql_used_to_create = sql
+
+        physical_name = splink_dataframe.physical_name
+
+        self._intermediate_table_cache[physical_name] = splink_dataframe
 
         return splink_dataframe
 
     def __deepcopy__(self, memo):
         """When we do EM training, we need a copy of the linker which is independent
         of the main linker e.g. setting parameters on the copy will not affect the
         main linker.  This method implements ensures linker can be deepcopied.
@@ -902,23 +920,14 @@
             if self._settings_obj._link_type == "dedupe_only":
                 if len(self._input_tables_dict) > 1:
                     raise ValueError(
                         'If link_type = "dedupe only" then input tables must contain '
                         "only a single input table",
                     )
 
-    def _validate_dialect(self):
-        settings_dialect = self._settings_obj._sql_dialect
-        if settings_dialect != self._sql_dialect:
-            raise ValueError(
-                f"Incompatible SQL dialect! `settings` dictionary uses "
-                f"dialect {settings_dialect}, but expecting "
-                f"'{self._sql_dialect}' for Linker of type {type(self)}"
-            )
-
     def _populate_probability_two_random_records_match_from_trained_values(self):
         recip_prop_matches_estimates = []
 
         logger.log(
             15,
             (
                 "---- Using training sessions to compute "
@@ -996,37 +1005,18 @@
         for cc in ccs:
             for cl in cc._comparison_levels_excluding_null:
                 if cl._has_estimated_u_values:
                     cl.u_probability = cl._trained_u_median
                 if cl._has_estimated_m_values:
                     cl.m_probability = cl._trained_m_median
 
-    def _delete_tables_created_by_splink_from_db(
-        self, retain_term_frequency=True, retain_df_concat_with_tf=True
-    ):
-        to_remove = set()
-        for name in self._names_of_tables_created_by_splink:
-            # Only delete tables explicitly marked as having been created by splink
-            if "__splink__" not in name:
-                continue
-            if name == "__splink__df_concat_with_tf":
-                if not retain_df_concat_with_tf:
-                    self._delete_table_from_database(name)
-                    to_remove.add(name)
-            elif name.startswith("__splink__df_tf_"):
-                if not retain_term_frequency:
-                    self._delete_table_from_database(name)
-                    to_remove.add(name)
-            else:
-                self._delete_table_from_database(name)
-                to_remove.add(name)
-
-        self._names_of_tables_created_by_splink = (
-            self._names_of_tables_created_by_splink - to_remove
-        )
+    def delete_tables_created_by_splink_from_db(self):
+        for splink_df in list(self._intermediate_table_cache.values()):
+            if splink_df.created_by_splink:
+                splink_df.drop_table_from_database_and_remove_from_cache()
 
     def _raise_error_if_necessary_waterfall_columns_not_computed(self):
         ricc = self._settings_obj._retain_intermediate_calculation_columns
         rmc = self._settings_obj._retain_matching_columns
         if not (ricc and rmc):
             raise ValueError(
                 "retain_intermediate_calculation_columns and "
@@ -1044,30 +1034,36 @@
                 "retain_matching_columns must be set to True in your settings"
                 " dictionary to use this function, because otherwise the necessary "
                 "columns will not be available in the input records."
                 f" Its current value is {rmc}. "
                 "Please re-run your linkage with it set to True."
             )
 
-    def load_settings(self, settings_dict: dict | str | Path):
+    def load_settings(
+        self,
+        settings_dict: dict | str | Path,
+        validate_settings: str = True,
+    ):
         """Initialise settings for the linker.  To be used if settings were
         not passed to the linker on creation. This can either be in the form
         of a settings dictionary or a filepath to a json file containing a
         valid settings dictionary.
 
         Examples:
             ```py
             linker = DuckDBLinker(df)
             linker.profile_columns(["first_name", "surname"])
-            linker.load_settings(settings_dict)
+            linker.load_settings(settings_dict, validate_settings=True)
             ```
 
         Args:
             settings_dict (dict | str | Path): A Splink settings dictionary or
                 the path to your settings json file.
+            validate_settings (bool, optional): When True, check your settings
+                dictionary for any potential errors that may cause splink to fail.
         """
 
         if not isinstance(settings_dict, dict):
             p = Path(settings_dict)
             if not p.is_file():  # check if it's a valid file/filepath
                 raise FileNotFoundError(
                     "The filepath you have provided is either not a valid file "
@@ -1093,15 +1089,15 @@
         settings_dict["linker_uid"] = settings_dict.get("linker_uid", cache_id)
         settings_dict["sql_dialect"] = settings_dict.get(
             "sql_dialect", self._sql_dialect
         )
         self._settings_dict = settings_dict
         self._settings_obj_ = Settings(settings_dict)
         self._validate_input_dfs()
-        self._validate_dialect()
+        self._validate_settings(validate_settings)
 
     def load_model(self, model_path: Path):
         """
         Load a pre-defined model from a json file into the linker.
         This is intended to be used with the output of
         `save_model_to_json()`.
 
@@ -1120,33 +1116,33 @@
         """*This method is now deprecated. Please use `load_settings`
         when loading existing settings or `load_model` when loading
          a pre-trained model.*
 
         Initialise settings for the linker.  To be used if settings were
         not passed to the linker on creation.
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ```py
                 linker = DuckDBLinker(df")
                 linker.profile_columns(["first_name", "surname"])
                 linker.initialise_settings(settings_dict)
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ```py
                 linker = SparkLinker(df")
                 linker.profile_columns(["first_name", "surname"])
                 linker.initialise_settings(settings_dict)
                 ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
                 ```py
                 linker = AthenaLinker(df")
                 linker.profile_columns(["first_name", "surname"])
                 linker.initialise_settings(settings_dict)
                 ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
                 ```py
                 linker = SQLiteLinker(df")
                 linker.profile_columns(["first_name", "surname"])
                 linker.initialise_settings(settings_dict)
                 ```
         Args:
             settings_dict (dict): A Splink settings dictionary
@@ -1198,15 +1194,15 @@
         """Compute a term frequency table for a given column and persist to the database
 
         This method is useful if you want to pre-compute term frequency tables e.g.
         so that real time linkage executes faster, or so that you can estimate
         various models without having to recompute term frequency tables each time
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 Real time linkage
                 ```py
                 linker = DuckDBLinker(df)
                 linker.load_settings("saved_settings.json")
                 linker.compute_tf_table("surname")
                 linker.compare_two_records(record_left, record_right)
                 ```
@@ -1216,15 +1212,15 @@
                 df_first_name_tf = linker.compute_tf_table("first_name")
                 df_first_name_tf.write.parquet("folder/first_name_tf")
                 >>>
                 # On subsequent data linking job, read this table rather than recompute
                 df_first_name_tf = pd.read_parquet("folder/first_name_tf")
                 df_first_name_tf.createOrReplaceTempView("__splink__df_tf_first_name")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 Real time linkage
                 ```py
                 linker = SparkLinker(df)
                 linker.load_settings("saved_settings.json")
                 linker.compute_tf_table("surname")
                 linker.compare_two_records(record_left, record_right)
                 ```
@@ -1251,36 +1247,34 @@
         cache = self._intermediate_table_cache
         concat_tf_tables = [
             remove_quotes_from_identifiers(tf_col.input_name_as_tree).sql()
             for tf_col in self._settings_obj._term_frequency_columns
         ]
 
         if tf_tablename in cache:
-            tf_df = cache[tf_tablename]
+            tf_df = cache.get_with_logging(tf_tablename)
         elif "__splink__df_concat_with_tf" in cache and column_name in concat_tf_tables:
             self._pipeline.reset()
             # If our df_concat_with_tf table already exists, use backwards inference to
             # find a given tf table
             colname = InputColumn(column_name)
             sql = term_frequencies_from_concat_with_tf(colname)
             self._enqueue_sql(sql, colname_to_tf_tablename(colname))
-            tf_df = self._execute_sql_pipeline(
-                [cache["__splink__df_concat_with_tf"]], materialise_as_hash=True
-            )
+            tf_df = self._execute_sql_pipeline([cache["__splink__df_concat_with_tf"]])
             self._intermediate_table_cache[tf_tablename] = tf_df
         else:
             # Clear the pipeline if we are materialising
             self._pipeline.reset()
             df_concat = self._initialise_df_concat()
             input_dfs = []
             if df_concat:
                 input_dfs.append(df_concat)
             sql = term_frequencies_for_single_column_sql(input_col)
             self._enqueue_sql(sql, tf_tablename)
-            tf_df = self._execute_sql_pipeline(input_dfs, materialise_as_hash=True)
+            tf_df = self._execute_sql_pipeline(input_dfs)
             self._intermediate_table_cache[tf_tablename] = tf_df
 
         return tf_df
 
     def deterministic_link(self) -> SplinkDataFrame:
         """Uses the blocking rules specified by
         `blocking_rules_to_generate_predictions` in the settings dictionary to
@@ -1289,15 +1283,15 @@
         For deterministic linkage, this should be a list of blocking rules which
         are strict enough to generate only true links.
 
         Deterministic linkage, however, is likely to result in missed links
         (false negatives).
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
             ```py
             from splink.duckdb.linker import DuckDBLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
@@ -1305,15 +1299,15 @@
                 ],
                 "comparisons": []
             }
             >>>
             linker = DuckDBLinker(df, settings)
             df = linker.deterministic_link()
             ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
             ```py
             from splink.spark.linker import SparkLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
@@ -1321,15 +1315,15 @@
                 ],
                 "comparisons": []
             }
             >>>
             linker = SparkLinker(df, settings)
             df = linker.deterministic_link()
             ```
-            === "Athena"
+            === ":simple-amazonaws: Athena"
             ```py
             from splink.athena.linker import AthenaLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
@@ -1337,15 +1331,15 @@
                 ],
                 "comparisons": []
             }
             >>>
             linker = AthenaLinker(df, settings)
             df = linker.deterministic_link()
             ```
-            === "SQLite"
+            === ":simple-sqlite: SQLite"
             ```py
             from splink.sqlite.linker import SQLiteLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
@@ -1481,14 +1475,15 @@
         self._settings_obj._columns_without_estimated_parameters_message()
 
     def estimate_parameters_using_expectation_maximisation(
         self,
         blocking_rule: str,
         comparisons_to_deactivate: list[str | Comparison] = None,
         comparison_levels_to_reverse_blocking_rule: list[ComparisonLevel] = None,
+        estimate_without_term_frequencies: bool = False,
         fix_probability_two_random_records_match: bool = False,
         fix_m_probabilities=False,
         fix_u_probabilities=True,
         populate_probability_two_random_records_match_from_trained_values=False,
     ) -> EMTrainingSession:
         """Estimate the parameters of the linkage model using expectation maximisation.
 
@@ -1551,14 +1546,18 @@
                 objects.  Defaults to None.
             comparison_levels_to_reverse_blocking_rule (list, optional): By default,
                 splink will analyse the blocking rule provided and adjust the
                 global probability two random records match to account for the matches
                 specified in the blocking rule. If provided, this argument will overrule
                 this default behaviour. The user must provide a list of ComparisonLevel
                 objects.  Defaults to None.
+            estimate_without_term_frequencies (bool, optional): If True, the iterations
+                of the EM algorithm ignore any term frequency adjustments and only
+                depend on the comparison vectors. This allows the EM algorithm to run
+                much faster, but the estimation of the parameters will change slightly.
             fix_probability_two_random_records_match (bool, optional): If True, do not
                 update the probability two random records match after each iteration.
                 Defaults to False.
             fix_m_probabilities (bool, optional): If True, do not update the m
                 probabilities after each iteration. Defaults to False.
             fix_u_probabilities (bool, optional): If True, do not update the u
                 probabilities after each iteration. Defaults to True.
@@ -1605,14 +1604,15 @@
             self,
             blocking_rule,
             fix_u_probabilities=fix_u_probabilities,
             fix_m_probabilities=fix_m_probabilities,
             fix_probability_two_random_records_match=fix_probability_two_random_records_match,  # noqa 501
             comparisons_to_deactivate=comparisons_to_deactivate,
             comparison_levels_to_reverse_blocking_rule=comparison_levels_to_reverse_blocking_rule,  # noqa 501
+            estimate_without_term_frequencies=estimate_without_term_frequencies,
         )
 
         em_training_session._train()
 
         self._populate_m_u_from_trained_values()
 
         if populate_probability_two_random_records_match_from_trained_values:
@@ -1749,18 +1749,19 @@
         original_blocking_rules = (
             self._settings_obj._blocking_rules_to_generate_predictions
         )
         original_link_type = self._settings_obj._link_type
 
         if not isinstance(records_or_tablename, str):
             uid = ascii_uid(8)
+            new_records_tablename = f"__splink__df_new_records_{uid}"
             self.register_table(
-                records_or_tablename, f"__splink__df_new_records_{uid}", overwrite=True
+                records_or_tablename, new_records_tablename, overwrite=True
             )
-            new_records_tablename = f"__splink__df_new_records_{uid}"
+
         else:
             new_records_tablename = records_or_tablename
 
         cache = self._intermediate_table_cache
         input_dfs = []
         # If our df_concat_with_tf table already exists, use backwards inference to
         # find all underlying term frequency tables.
@@ -1786,15 +1787,14 @@
             br_as_obj = BlockingRule(r) if not isinstance(r, BlockingRule) else r
             br_as_obj.preceding_rules = rules.copy()
             rules.append(br_as_obj)
         blocking_rules = rules
 
         self._settings_obj._blocking_rules_to_generate_predictions = blocking_rules
 
-        self._settings_obj._link_type = "link_only_find_matches_to_new_records"
         self._find_new_matches_mode = True
 
         sql = _join_tf_to_input_df_sql(self)
         sql = sql.replace("__splink__df_concat", new_records_tablename)
         self._enqueue_sql(sql, "__splink__df_new_records_with_tf")
 
         sql = block_using_rules_sql(self)
@@ -2108,21 +2108,21 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ```py
                 labels = pd.read_csv("my_labels.csv")
                 linker.register_table(labels, "labels")
                 linker.truth_space_table_from_labels_table("labels")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ```py
                 labels = spark.read.csv("my_labels.csv", header=True)
                 labels.createDataFrame("labels")
                 linker.truth_space_table_from_labels_table("labels")
                 ```
         Returns:
             SplinkDataFrame:  Table of truth statistics
@@ -2170,21 +2170,21 @@
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
 
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ```py
                 labels = pd.read_csv("my_labels.csv")
                 linker.register_table(labels, "labels")
                 linker.roc_chart_from_labels_table("labels")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ```py
                 labels = spark.read.csv("my_labels.csv", header=True)
                 labels.createDataFrame("labels")
                 linker.roc_chart_from_labels_table("labels")
                 ```
 
         Returns:
@@ -2234,21 +2234,21 @@
                 is used as the threshold to classify `clerical_match_score`s as binary
                 matches or non matches. Defaults to 0.5.
             match_weight_round_to_nearest (float, optional): When provided, thresholds
                 are rounded.  When large numbers of labels are provided, this is
                 sometimes necessary to reduce the size of the ROC table, and therefore
                 the number of points plotted on the ROC chart. Defaults to None.
         Examples:
-            === "DuckDB"
+            === ":simple-duckdb: DuckDB"
                 ```py
                 labels = pd.read_csv("my_labels.csv")
                 linker.register_table(labels, "labels")
                 linker.precision_recall_chart_from_labels_table("labels")
                 ```
-            === "Spark"
+            === ":simple-apachespark: Spark"
                 ```py
                 labels = spark.read.csv("my_labels.csv", header=True)
                 labels.createDataFrame("labels")
                 linker.precision_recall_chart_from_labels_table("labels")
                 ```
 
         Returns:
@@ -3154,17 +3154,17 @@
 
         # As a result, any previously cached tables will not be found
         self._cache_uid = ascii_uid(8)
 
         # As a result, any previously cached tables will not be found
         self._intermediate_table_cache.invalidate_cache()
 
-        # Also drop any existing splink tables from the database
+        # Drop any existing splink tables from the database
         # Note, this is not actually necessary, it's just good housekeeping
-        self._delete_tables_created_by_splink_from_db()
+        self.delete_tables_created_by_splink_from_db()
 
     def register_table_input_nodes_concat_with_tf(self, input_data, overwrite=False):
         """Register a pre-computed version of the input_nodes_concat_with_tf table that
         you want to re-use e.g. that you created in a previous run
 
         This method allowed you to register this table in the Splink cache
         so it will be used rather than Splink computing this table anew.
@@ -3176,34 +3176,97 @@
                 exists
         """
 
         table_name_physical = "__splink__df_concat_with_tf_" + self._cache_uid
         splink_dataframe = self.register_table(
             input_data, table_name_physical, overwrite=overwrite
         )
+        splink_dataframe.templated_name = "__splink__df_concat_with_tf"
+
         self._intermediate_table_cache["__splink__df_concat_with_tf"] = splink_dataframe
         return splink_dataframe
 
     def register_table_predict(self, input_data, overwrite=False):
         table_name_physical = "__splink__df_predict_" + self._cache_uid
         splink_dataframe = self.register_table(
             input_data, table_name_physical, overwrite=overwrite
         )
         self._intermediate_table_cache["__splink__df_predict"] = splink_dataframe
+        splink_dataframe.templated_name = "__splink__df_predict"
         return splink_dataframe
 
     def register_term_frequency_lookup(self, input_data, col_name, overwrite=False):
         input_col = InputColumn(col_name, settings_obj=self._settings_obj)
         table_name_templated = colname_to_tf_tablename(input_col)
         table_name_physical = f"{table_name_templated}_{self._cache_uid}"
         splink_dataframe = self.register_table(
             input_data, table_name_physical, overwrite=overwrite
         )
         self._intermediate_table_cache[table_name_templated] = splink_dataframe
+        splink_dataframe.templated_name = table_name_templated
         return splink_dataframe
 
     def register_labels_table(self, input_data, overwrite=False):
         table_name_physical = "__splink__df_labels_" + ascii_uid(8)
         splink_dataframe = self.register_table(
             input_data, table_name_physical, overwrite=overwrite
         )
+        splink_dataframe.templated_name = "__splink__df_labels"
         return splink_dataframe
+
+    def labelling_tool_for_specific_record(
+        self,
+        unique_id,
+        source_dataset=None,
+        out_path="labelling_tool.html",
+        overwrite=False,
+        match_weight_threshold=-4,
+        view_in_jupyter=False,
+        show_splink_predictions_in_interface=True,
+    ):
+        """Create a standalone, offline labelling dashboard for a specific record
+        as identified by its unique id
+
+        Args:
+            unique_id (str): The unique id of the record for which to create the
+                labelling tool
+            source_dataset (str, optional): If there are multiple datasets, to
+                identify the record you must also specify the source_dataset. Defaults
+                to None.
+            out_path (str, optional): The output path for the labelling tool. Defaults
+                to "labelling_tool.html".
+            overwrite (bool, optional): If true, overwrite files at the output
+                path if they exist. Defaults to False.
+            match_weight_threshold (int, optional): Include possible matches in the
+                output which score above this threshold. Defaults to -4.
+            view_in_jupyter (bool, optional): If you're viewing in the Jupyter
+                html viewer, set this to True to extract your labels. Defaults to False.
+            show_splink_predictions_in_interface (bool, optional): Whether to
+                show information about the Splink model's predictions that could
+                potentially bias the decision of the clerical labeller. Defaults to
+                True.
+        """
+
+        df_comparisons = generate_labelling_tool_comparisons(
+            self,
+            unique_id,
+            source_dataset,
+            match_weight_threshold=match_weight_threshold,
+        )
+
+        render_labelling_tool_html(
+            self,
+            df_comparisons,
+            show_splink_predictions_in_interface=show_splink_predictions_in_interface,
+            out_path=out_path,
+            view_in_jupyter=view_in_jupyter,
+            overwrite=overwrite,
+        )
+
+    def _remove_splinkdataframe_from_cache(self, splink_dataframe: SplinkDataFrame):
+        keys_to_delete = set()
+        for key, df in self._intermediate_table_cache.items():
+            if df.physical_name == splink_dataframe.physical_name:
+                keys_to_delete.add(key)
+
+        for k in keys_to_delete:
+            del self._intermediate_table_cache[k]
```

### Comparing `splink-3.9.2/splink/lower_id_on_lhs.py` & `splink-3.9.3/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/m_from_labels.py` & `splink-3.9.3/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/m_training.py` & `splink-3.9.3/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/m_u_records_to_parameters.py` & `splink-3.9.3/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/match_key_analysis.py` & `splink-3.9.3/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/match_weights_histogram.py` & `splink-3.9.3/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/misc.py` & `splink-3.9.3/splink/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import random
 import string
-from math import inf, log2
+from collections import namedtuple
+from datetime import datetime, timedelta
+from math import ceil, inf, log2
 from typing import Iterable
 
 import numpy as np
 import pkg_resources
 
 
 def dedupe_preserving_order(list_of_items):
@@ -70,14 +72,17 @@
     Without this, json.dumps errors if given an a column of class int32, int64
     np.array, datetime.date etc.
 
     Thanks to:
     https://github.com/mpld3/mpld3/issues/434#issuecomment-340255689
     """
 
+    # Note that the default method is only called for data types that are
+    # NOT natively serializable.  The 'encode' method can be used
+    # for natively serializable data
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
             return float(obj)
         elif isinstance(obj, np.bool_):
             return bool(obj)
@@ -157,17 +162,54 @@
     base_version = base_comparison_version.split(".")[:2]
     base_version = [v.zfill(10) for v in base_version]
 
     return this_version >= base_version
 
 
 def ascii_uid(len):
-    return "".join(random.choices(string.ascii_letters + string.digits, k=len))
+    # use only lowercase as case-sensitivity is an issue in e.g. postgres
+    return "".join(random.choices(string.ascii_lowercase + string.digits, k=len))
 
 
 def find_unique_source_dataset(src_ds):
     sql = f"""
         select distinct {src_ds} as src
         from __splink__df_concat_with_tf
     """
 
     return sql
+
+
+def parse_duration(duration: int):
+    # math.ceil so <1 second gets reported
+    d = datetime(1, 1, 1) + timedelta(seconds=int(ceil(duration)))
+    time_index = namedtuple("Time", ["Days", "Hours", "Minutes", "Seconds"])
+    duration = time_index(d.day - 1, d.hour, d.minute, d.second)
+    txt_duration = [
+        f"{t} {duration._fields[n]}" for n, t in enumerate(duration) if t > 0
+    ]
+    if len(txt_duration) > 1:
+        txt_duration[-1] = "and " + txt_duration[-1]
+
+    return ", ".join(txt_duration)
+
+
+class colour:
+    """A class to beautify your text. Simply import and then use this class's
+    attributes to adjust how the text is formatted. For example:
+
+    `f"{colour.BOLD}Send help{colour.END}`
+
+    will print your text to the console in bold.
+    """
+
+    PURPLE = "\033[95m"
+    CYAN = "\033[96m"
+    DARKCYAN = "\033[36m"
+    BLUE = "\033[94m"
+    GREEN = "\033[92m"
+    YELLOW = "\033[93m"
+    RED = "\033[91m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+    ITALICS = "\033[3m"
+    END = "\033[0m"
```

### Comparing `splink-3.9.2/splink/missingness.py` & `splink-3.9.3/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/parse_sql.py` & `splink-3.9.3/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/pipeline.py` & `splink-3.9.3/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/postgres/linker.py` & `splink-3.9.3/splink/postgres/linker.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             raise ValueError(
                 f"{self.physical_name} does not exist in the postgres db provided.\n"
                 "Postgres Linker requires input data"
                 " to be a string containing the name of a"
                 " postgres table that exists in the provided db."
             )
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         self._check_drop_table_created_by_splink(force_non_splink_table)
         self.linker._delete_table_from_database(self.physical_name)
 
     def as_record_dict(self, limit=None):
         sql = f"""
         SELECT *
         FROM {self.physical_name}
@@ -79,14 +79,15 @@
     def __init__(
         self,
         input_table_or_tables,
         settings_dict=None,
         engine: Engine = None,
         set_up_basic_logging=True,
         input_table_aliases: str | list = None,
+        validate_settings: bool = True,
         schema="splink",
     ):
         self._sql_dialect_ = "postgres"
         if not isinstance(engine, Engine):
             raise ValueError(
                 "You must supply a sqlalchemy engine " "to create a PostgresLinker."
             )
@@ -109,14 +110,15 @@
 
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
+            validate_settings=validate_settings,
         )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
         return PostgresDataFrame(templated_name, physical_name, self)
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         # In the case of a table already existing in the database,
@@ -220,14 +222,24 @@
         CREATE OR REPLACE FUNCTION log2(n float8)
         RETURNS float8 AS $$
         SELECT log(2.0, n::numeric)::float8;
         $$ LANGUAGE SQL IMMUTABLE;
         """
         self._run_sql_execution(sql)
 
+    def _extend_round_function(self):
+        # extension of round to double
+        sql = """
+        CREATE OR REPLACE FUNCTION round(n float8, dp integer)
+        RETURNS numeric AS $$
+        SELECT round(n::numeric, dp);
+        $$ LANGUAGE SQL IMMUTABLE;
+        """
+        self._run_sql_execution(sql)
+
     def _create_datediff_function(self):
         sql = """
         CREATE OR REPLACE FUNCTION datediff(x date, y date)
         RETURNS integer AS $$
         SELECT x - y;
         $$ LANGUAGE SQL IMMUTABLE;
         """
@@ -281,14 +293,16 @@
         # need for predict_from_comparison_vectors_sql (could adjust)
         self._create_log2_function()
         # need for datediff levels
         self._create_datediff_function()
         self._create_months_between_function()
         # need for array_intersect levels
         self._create_array_intersect_function()
+        # extension of round to handle doubles - used in unlinkables
+        self._extend_round_function()
 
     def _register_extensions(self):
         sql = """
         CREATE EXTENSION IF NOT EXISTS fuzzystrmatch;
         """
         self._run_sql_execution(sql)
```

### Comparing `splink-3.9.2/splink/postgres/postgres_helpers/postgres_base.py` & `splink-3.9.3/splink/postgres/postgres_helpers/postgres_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/postgres/postgres_helpers/postgres_comparison_imports.py` & `splink-3.9.3/splink/postgres/postgres_helpers/postgres_comparison_imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
-    DateDiffLevelBase,
+    DatediffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
-    ArrayIntersectAtSizesComparisonBase,
-    DateDiffAtThresholdsComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
-    DistanceInKMAtThresholdsComparisonBase,
+    ArrayIntersectAtSizesBase,
+    DatediffAtThresholdsBase,
+    DistanceFunctionAtThresholdsBase,
+    DistanceInKMAtThresholdsBase,
     ExactMatchBase,
-    LevenshteinAtThresholdsComparisonBase,
+    LevenshteinAtThresholdsBase,
 )
 from .postgres_base import (
     PostgresBase,
 )
 
 
 # Class used to feed our comparison_library classes
@@ -89,55 +89,51 @@
     pass
 
 
 class distance_in_km_level(PostgresBase, DistanceInKMLevelBase):
     pass
 
 
-class datediff_level(PostgresBase, DateDiffLevelBase):
+class datediff_level(PostgresBase, DatediffLevelBase):
     pass
 
 
 ##########################
 ### COMPARISON LIBRARY ###
 ##########################
 class exact_match(PostgresComparisonProperties, ExactMatchBase):
     pass
 
 
 class distance_function_at_thresholds(
-    PostgresComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+    PostgresComparisonProperties, DistanceFunctionAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return distance_function_level
 
 
 class levenshtein_at_thresholds(
-    PostgresComparisonProperties, LevenshteinAtThresholdsComparisonBase
+    PostgresComparisonProperties, LevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return levenshtein_level
 
 
-class array_intersect_at_sizes(
-    PostgresComparisonProperties, ArrayIntersectAtSizesComparisonBase
-):
+class array_intersect_at_sizes(PostgresComparisonProperties, ArrayIntersectAtSizesBase):
     pass
 
 
-class datediff_at_thresholds(
-    PostgresComparisonProperties, DateDiffAtThresholdsComparisonBase
-):
+class datediff_at_thresholds(PostgresComparisonProperties, DatediffAtThresholdsBase):
     pass
 
 
 class distance_in_km_at_thresholds(
-    PostgresComparisonProperties, DistanceInKMAtThresholdsComparisonBase
+    PostgresComparisonProperties, DistanceInKMAtThresholdsBase
 ):
     pass
 
 
 ###################################
 ### COMPARISON TEMPLATE LIBRARY ###
 ###################################
```

### Comparing `splink-3.9.2/splink/profile_data.py` & `splink-3.9.3/splink/profile_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 def _get_df_top_bottom_n(expressions, limit=20, value_order="desc"):
     sql = """
     select * from
     (select *
     from __splink__df_all_column_value_frequencies
     where group_name = '{gn}'
     order by value_count {value_order}
-    limit {limit})
+    limit {limit}) top_bottom_freqs
     """
 
     to_union = [
         sql.format(gn=_group_name(g), limit=limit, value_order=value_order)
         for g in expressions
     ]
 
@@ -168,15 +168,15 @@
             (select count({col_or_expr}) from {table_name}) as total_non_null_rows,
             (select count(*) from {table_name}) as total_rows_inc_nulls,
             (select count(distinct {col_or_expr}) from {table_name})
                 as distinct_value_count
         from {table_name}
         where {col_or_expr} is not null
         group by {col_or_expr}
-        order by count(*) desc)
+        order by count(*) desc) column_stats
         """
         sqls.append(sql)
 
     return " union all ".join(sqls)
 
 
 def _add_100_percentile_to_df_percentiles(percentile_rows):
@@ -201,15 +201,15 @@
     column_expressions = expressions_to_sql(column_expressions_raw)
 
     sql = _col_or_expr_frequencies_raw_data_sql(
         column_expressions_raw, "__splink__df_concat"
     )
 
     linker._enqueue_sql(sql, "__splink__df_all_column_value_frequencies")
-    df_raw = linker._execute_sql_pipeline(input_dataframes, materialise_as_hash=True)
+    df_raw = linker._execute_sql_pipeline(input_dataframes)
 
     sqls = _get_df_percentiles()
     for sql in sqls:
         linker._enqueue_sql(sql["sql"], sql["output_table_name"])
 
     df_percentiles = linker._execute_sql_pipeline([df_raw])
     percentile_rows_all = df_percentiles.as_record_dict()
```

### Comparing `splink-3.9.2/splink/settings.py` & `splink-3.9.3/splink/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self._bf_prefix = s_else_d("bayes_factor_column_prefix")
         self._tf_prefix = s_else_d("term_frequency_adjustment_column_prefix")
         self._blocking_rule_for_training = None
         self._training_mode = False
 
         self._warn_if_no_null_level_in_comparisons()
 
+        self._additional_cols_to_retain = self._get_raw_additional_cols_to_retain
         self._additional_columns_to_retain_list = (
             self._get_additional_columns_to_retain()
         )
 
     def __deepcopy__(self, memo) -> Settings:
         """When we do EM training, we need a copy of the Settings which is independent
         of the original e.g. modifying the copy will not affect the original.
@@ -105,14 +106,22 @@
                     " with the case that one or both sides of the comparison are null."
                     "\nThis comparison level should have the `is_null_level` flag to "
                     "True in the settings for that comparison level"
                     "\nIf the column does not contain null values, or you know what "
                     "you're doing, you can ignore this warning"
                 )
 
+    @property
+    def _get_raw_additional_cols_to_retain(self):
+        a_cols = self._from_settings_dict_else_default("additional_columns_to_retain")
+
+        # Add any columns used in blocking rules but not model
+        if a_cols:
+            return [InputColumn(c) for c in a_cols]
+
     def _get_additional_columns_to_retain(self):
         a_cols = self._from_settings_dict_else_default("additional_columns_to_retain")
 
         # Add any columns used in blocking rules but not model
         if self._retain_matching_columns:
             # Want to add any columns not already by the model
             used_by_brs = []
@@ -143,18 +152,15 @@
     @property
     def _additional_columns_to_retain(self):
         cols = self._additional_columns_to_retain_list
         return [InputColumn(c, settings_obj=self) for c in cols]
 
     @property
     def _source_dataset_column_name_is_required(self):
-        return self._link_type not in [
-            "dedupe_only",
-            "link_only_find_matches_to_new_records",
-        ]
+        return self._link_type not in ["dedupe_only"]
 
     @property
     def _source_dataset_input_column(self):
         if self._source_dataset_column_name_is_required:
             s_else_d = self._from_settings_dict_else_default
             return s_else_d("source_dataset_column_name")
         else:
```

### Comparing `splink-3.9.2/splink/spark/linker.py` & `splink-3.9.3/splink/spark/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import os
 import re
 from itertools import compress
 
 import pandas as pd
 import sqlglot
+from numpy import nan
 from pyspark.sql.dataframe import DataFrame as spark_df
 from pyspark.sql.types import DoubleType, StringType
 from pyspark.sql.utils import AnalysisException
 
 from ..databricks.enable_splink import enable_splink
 from ..input_column import InputColumn
 from ..linker import Linker
@@ -42,15 +43,15 @@
     def as_record_dict(self, limit=None):
         sql = f"select * from {self.physical_name}"
         if limit:
             sql += f" limit {limit}"
 
         return self.linker.spark.sql(sql).toPandas().to_dict(orient="records")
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         # Spark, in general, does not persist its results to disk
         # There is a whitelist of dataframes to either perist() or checkpoint()
         # But there's no real need to clean these up, so we'll just do nothing
         pass
 
     def as_pandas_dataframe(self, limit=None):
         sql = f"select * from {self.physical_name}"
@@ -77,47 +78,51 @@
         spark_df.write.format("csv").option("header", "true").save(filepath)
 
 
 class SparkLinker(Linker):
     def __init__(
         self,
         input_table_or_tables,
-        settings_dict=None,
+        settings_dict: dict | str = None,
         break_lineage_method=None,
         set_up_basic_logging=True,
         input_table_aliases: str | list = None,
         spark=None,
+        validate_settings: bool = True,
         catalog=None,
         database=None,
         repartition_after_blocking=False,
         num_partitions_on_repartition=None,
     ):
         """Initialise the linker object, which manages the data linkage process and
                 holds the data linkage model.
 
         Args:
             input_table_or_tables: Input data into the linkage model.  Either a
                 single table or a list of tables.  Tables can be provided either as
                 a Spark DataFrame, or as the name of the table as a string, as
                 registered in the Spark catalog
-            settings_dict (dict, optional): A Splink settings dictionary. If not
-                provided when the object is created, can later be added using
-                `linker.load_settings()` Defaults to None.
+            settings_dict (dict | Path, optional): A Splink settings dictionary, or
+                 a path to a json defining a settingss dictionary or pre-trained model.
+                  If not provided when the object is created, can later be added using
+                `linker.load_settings()` or `linker.load_model()` Defaults to None.
             break_lineage_method (str, optional): Method to use to cache intermediate
                 results.  Can be "checkpoint", "persist", "parquet", "delta_lake_files",
                 "delta_lake_table". Defaults to "parquet".
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             input_table_aliases (Union[str, list], optional): Labels assigned to
                 input tables in Splink outputs.  If the names of the tables in the
                 input database are long or unspecific, this argument can be used
                 to attach more easily readable/interpretable names. Defaults to None.
             spark: The SparkSession. Required only if `input_table_or_tables` are
                 provided as string - otherwise will be inferred from the provided
                 Spark Dataframes.
+            validate_settings (bool, optional): When True, check your settings
+                dictionary for any potential errors that may cause splink to fail.
             repartition_after_blocking (bool, optional): In some cases, especially when
                 the comparisons are very computationally intensive, performance may be
                 improved by repartitioning after blocking to distribute the workload of
                 computing the comparison vectors more evenly and reduce the number of
                 tasks. Defaults to False.
             num_partitions_on_repartition (int, optional): When saving out intermediate
                 results, how many partitions to use?  This should be set so that
@@ -166,14 +171,15 @@
 
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
+            validate_settings=validate_settings,
         )
         self._check_ansi_enabled_if_converting_dates()
 
         self.in_databricks = "DATABRICKS_RUNTIME_VERSION" in os.environ
         if self.in_databricks:
             enable_splink(spark)
 
@@ -461,23 +467,26 @@
 
         self._table_registration(input, table_name)
         return self._table_to_splink_dataframe(table_name, table_name)
 
     def _table_registration(self, input, table_name):
         if isinstance(input, dict):
             input = pd.DataFrame(input)
-            input = self.spark.createDataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
-            input = self.spark.createDataFrame(input)
-        elif isinstance(input, pd.DataFrame):
+
+        if isinstance(input, pd.DataFrame):
+            input = self._clean_pandas_df(input)
             input = self.spark.createDataFrame(input)
 
         input.createOrReplaceTempView(table_name)
 
+    def _clean_pandas_df(self, df):
+        return df.fillna(nan).replace([nan, pd.NA], [None, None])
+
     def _random_sample_sql(
         self, proportion, sample_size, seed=None, table=None, unique_id=None
     ):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         if seed:
```

### Comparing `splink-3.9.2/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-3.9.3/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/spark/spark_helpers/spark_base.py` & `splink-3.9.3/splink/spark/spark_helpers/spark_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/spark/spark_helpers/spark_comparison_imports.py` & `splink-3.9.3/splink/spark/spark_helpers/spark_comparison_imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
     DamerauLevenshteinLevelBase,
-    DateDiffLevelBase,
+    DatediffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     JaccardLevelBase,
     JaroLevelBase,
     JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
-    ArrayIntersectAtSizesComparisonBase,
-    DamerauLevenshteinAtThresholdsComparisonBase,
-    DateDiffAtThresholdsComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
-    DistanceInKMAtThresholdsComparisonBase,
+    ArrayIntersectAtSizesBase,
+    DamerauLevenshteinAtThresholdsBase,
+    DatediffAtThresholdsBase,
+    DistanceFunctionAtThresholdsBase,
+    DistanceInKMAtThresholdsBase,
     ExactMatchBase,
-    JaccardAtThresholdsComparisonBase,
-    JaroAtThresholdsComparisonBase,
-    JaroWinklerAtThresholdsComparisonBase,
-    LevenshteinAtThresholdsComparisonBase,
+    JaccardAtThresholdsBase,
+    JaroAtThresholdsBase,
+    JaroWinklerAtThresholdsBase,
+    LevenshteinAtThresholdsBase,
 )
 from ...comparison_template_library import (
     DateComparisonBase,
     EmailComparisonBase,
     ForenameSurnameComparisonBase,
     NameComparisonBase,
     PostcodeComparisonBase,
@@ -144,85 +144,77 @@
     pass
 
 
 class distance_in_km_level(SparkBase, DistanceInKMLevelBase):
     pass
 
 
-class datediff_level(SparkBase, DateDiffLevelBase):
+class datediff_level(SparkBase, DatediffLevelBase):
     pass
 
 
 ##########################
 ### COMPARISON LIBRARY ###
 ##########################
 class exact_match(SparkComparisonProperties, ExactMatchBase):
     pass
 
 
 class distance_function_at_thresholds(
-    SparkComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+    SparkComparisonProperties, DistanceFunctionAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._distance_function_level
 
 
-class levenshtein_at_thresholds(
-    SparkComparisonProperties, LevenshteinAtThresholdsComparisonBase
-):
+class levenshtein_at_thresholds(SparkComparisonProperties, LevenshteinAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._levenshtein_level
 
 
 class damerau_levenshtein_at_thresholds(
-    SparkComparisonProperties, DamerauLevenshteinAtThresholdsComparisonBase
+    SparkComparisonProperties, DamerauLevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._damerau_levenshtein_level
 
 
-class jaro_at_thresholds(SparkComparisonProperties, JaroAtThresholdsComparisonBase):
+class jaro_at_thresholds(SparkComparisonProperties, JaroAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._jaro_level
 
 
 class jaro_winkler_at_thresholds(
-    SparkComparisonProperties, JaroWinklerAtThresholdsComparisonBase
+    SparkComparisonProperties, JaroWinklerAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._jaro_winkler_level
 
 
-class jaccard_at_thresholds(
-    SparkComparisonProperties, JaccardAtThresholdsComparisonBase
-):
+class jaccard_at_thresholds(SparkComparisonProperties, JaccardAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._jaccard_level
 
 
-class array_intersect_at_sizes(
-    SparkComparisonProperties, ArrayIntersectAtSizesComparisonBase
-):
+class array_intersect_at_sizes(SparkComparisonProperties, ArrayIntersectAtSizesBase):
     pass
 
 
-class datediff_at_thresholds(
-    SparkComparisonProperties, DateDiffAtThresholdsComparisonBase
-):
+class datediff_at_thresholds(SparkComparisonProperties, DatediffAtThresholdsBase):
     pass
 
 
 class distance_in_km_at_thresholds(
-    SparkComparisonProperties, DistanceInKMAtThresholdsComparisonBase
+    SparkComparisonProperties, DistanceInKMAtThresholdsBase
 ):
     pass
 
 
 ###################################
 ### COMPARISON TEMPLATE LIBRARY ###
 ###################################
```

### Comparing `splink-3.9.2/splink/splink_comparison_viewer.py` & `splink-3.9.3/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/splink_dataframe.py` & `splink-3.9.3/splink/splink_dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     """
 
     def __init__(self, templated_name: str, physical_name: str, linker: Linker):
         self.templated_name = templated_name
         self.physical_name = physical_name
         self.linker = linker
         self._target_schema = "splink"
+        self.created_by_splink = False
+        self.sql_used_to_create = None
 
     @property
     def columns(self):
         pass
 
     @property
     def columns_escaped(self):
@@ -37,34 +39,41 @@
         pass
 
     @property
     def physical_and_template_names_equal(self):
         return self.templated_name == self.physical_name
 
     def _check_drop_table_created_by_splink(self, force_non_splink_table=False):
-        if not self.physical_name.startswith("__splink__"):
+
+        if not self.created_by_splink:
             if not force_non_splink_table:
                 raise ValueError(
                     f"You've asked to drop table {self.physical_name} from your "
                     "database which is not a table created by Splink.  If you really "
                     "want to drop this table, you can do so by setting "
                     "force_non_splink_table=True"
                 )
         logger.debug(
             f"Dropping table with templated name {self.templated_name} and "
             f"physical name {self.physical_name}"
         )
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         raise NotImplementedError(
-            "Drop table from database not implemented for this linker"
+            "_drop_table_from_database from database not " "implemented for this linker"
         )
 
+    def drop_table_from_database_and_remove_from_cache(
+        self, force_non_splink_table=False
+    ):
+        self._drop_table_from_database(force_non_splink_table=force_non_splink_table)
+        self.linker._remove_splinkdataframe_from_cache(self)
+
     def as_record_dict(self, limit=None):
-        pass
+        raise NotImplementedError("as_record_dict not implemented for this linker")
 
     def as_pandas_dataframe(self, limit=None):
         """Return the dataframe as a pandas dataframe.
 
         This can be computationally expensive if the dataframe is large.
 
         Args:
```

### Comparing `splink-3.9.2/splink/sql_transform.py` & `splink-3.9.3/splink/sql_transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sqlglot
 import sqlglot.expressions as exp
 
 
-def sqlglot_transform_sql(sql, func):
-    syntax_tree = sqlglot.parse_one(sql, read=None)
+def sqlglot_transform_sql(sql, func, dialect=None):
+    syntax_tree = sqlglot.parse_one(sql, read=dialect)
     transformed_tree = syntax_tree.transform(func)
-    return transformed_tree.sql()
+    return transformed_tree.sql(dialect)
 
 
 def _add_l_or_r_to_identifier(node: exp.Expression):
     if not isinstance(node, exp.Identifier):
         return node
 
     p = node.parent
```

### Comparing `splink-3.9.2/splink/sqlite/linker.py` & `splink-3.9.3/splink/sqlite/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             raise ValueError(
                 f"{self.physical_name} does not exist in the sqlite db provided.\n"
                 "SQLite Linker requires input data"
                 " to be a string containing the name of a "
                 " sqlite table that exists in the provided db."
             )
 
-    def drop_table_from_database(self, force_non_splink_table=False):
+    def _drop_table_from_database(self, force_non_splink_table=False):
         self._check_drop_table_created_by_splink(force_non_splink_table)
 
         drop_sql = f"""
         DROP TABLE IF EXISTS {self.physical_name}"""
         cur = self.linker.con.cursor()
         cur.execute(drop_sql)
 
@@ -85,14 +85,15 @@
     def __init__(
         self,
         input_table_or_tables,
         settings_dict: dict | str = None,
         connection=":memory:",
         set_up_basic_logging=True,
         input_table_aliases: str | list = None,
+        validate_settings: bool = True,
         register_udfs=True,
     ):
         self._sql_dialect_ = "sqlite"
 
         if isinstance(connection, str):
             connection = sqlite3.connect(connection)
         self.con = connection
@@ -112,14 +113,15 @@
 
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
+            validate_settings=validate_settings,
         )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
         return SQLiteDataFrame(templated_name, physical_name, self)
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         # In the case of a table already existing in the database,
```

### Comparing `splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py` & `splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     JaroLevelBase,
     JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
-    DamerauLevenshteinAtThresholdsComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
+    DamerauLevenshteinAtThresholdsBase,
+    DistanceFunctionAtThresholdsBase,
     ExactMatchBase,
-    JaroAtThresholdsComparisonBase,
-    JaroWinklerAtThresholdsComparisonBase,
-    LevenshteinAtThresholdsComparisonBase,
+    JaroAtThresholdsBase,
+    JaroWinklerAtThresholdsBase,
+    LevenshteinAtThresholdsBase,
 )
 from ...comparison_template_library import (
     ForenameSurnameComparisonBase,
     NameComparisonBase,
 )
 from .sqlite_base import (
     SqliteBase,
@@ -113,43 +113,43 @@
 ### COMPARISON LIBRARY ###
 ##########################
 class exact_match(SqliteComparisonProperties, ExactMatchBase):
     pass
 
 
 class distance_function_at_thresholds(
-    SqliteComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+    SqliteComparisonProperties, DistanceFunctionAtThresholdsBase
 ):
     pass
 
 
 class levenshtein_at_thresholds(
-    SqliteComparisonProperties, LevenshteinAtThresholdsComparisonBase
+    SqliteComparisonProperties, LevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._levenshtein_level
 
 
 class damerau_levenshtein_at_thresholds(
-    SqliteComparisonProperties, DamerauLevenshteinAtThresholdsComparisonBase
+    SqliteComparisonProperties, DamerauLevenshteinAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._damerau_levenshtein_level
 
 
-class jaro_at_thresholds(SqliteComparisonProperties, JaroAtThresholdsComparisonBase):
+class jaro_at_thresholds(SqliteComparisonProperties, JaroAtThresholdsBase):
     @property
     def _distance_level(self):
         return self._jaro_level
 
 
 class jaro_winkler_at_thresholds(
-    SqliteComparisonProperties, JaroWinklerAtThresholdsComparisonBase
+    SqliteComparisonProperties, JaroWinklerAtThresholdsBase
 ):
     @property
     def _distance_level(self):
         return self._jaro_winkler_level
 
 
 ###################################
```

### Comparing `splink-3.9.2/splink/term_frequencies.py` & `splink-3.9.3/splink/term_frequencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,21 +231,19 @@
             },
         )
         for cl in c
     ]
 
     c = [comparison_level_to_tf_chart_data(cl) for cl in c]
     df = concat([cl["df_out"] for cl in c])
-    # print(df.to_dict"records")
     # Filter values
     selected = False if not vals_to_include else df["value"].isin(vals_to_include)
     least_freq = True if not n_least_freq else df["least_freq_rank"] < n_least_freq
     most_freq = True if not n_most_freq else df["most_freq_rank"] < n_most_freq
     mask = selected | least_freq | most_freq
-    # df = df[mask]
 
     vals_not_included = [val for val in vals_to_include if val not in df["value"]]
     if vals_not_included:
         warnings.warn(
             f"Values {vals_not_included} from `vals_to_include` were not found in "
             f"the dataset so are not included in the chart.",
             stacklevel=2,
```

### Comparing `splink-3.9.2/splink/unique_id_concat.py` & `splink-3.9.3/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/unlinkables.py` & `splink-3.9.3/splink/unlinkables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-def unlinkables_data(linker):
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+# https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
+if TYPE_CHECKING:
+    from .linker import Linker
+
+
+def unlinkables_data(linker: Linker):
     """Generate data displaying the proportion of records that are "unlinkable"
     for a given splink score threshold and model parameters. These are records that,
     even when compared with themselves, do not contain enough information to confirm
     a match.
 
     Args:
         linker (Splink): A Splink data linker
@@ -34,12 +43,12 @@
     sql = """
         select *,
         sum(prop) over(order by match_probability) as cum_prop
         from __splink__df_unlinkables_proportions
         where match_probability < 1
     """
     linker._enqueue_sql(sql, "__splink__df_unlinkables_proportions_cumulative")
-    data = linker._execute_sql_pipeline(materialise_as_hash=False, use_cache=False)
+    data = linker._execute_sql_pipeline(use_cache=False)
 
     unlinkables_dict = data.as_record_dict()
-
+    data.drop_table_from_database_and_remove_from_cache()
     return unlinkables_dict
```

### Comparing `splink-3.9.2/splink/validate_jsonschema.py` & `splink-3.9.3/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/vertically_concatenate.py` & `splink-3.9.3/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/splink/waterfall_chart.py` & `splink-3.9.3/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.2/PKG-INFO` & `splink-3.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.9.2
+Version: 3.9.3
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -30,25 +30,25 @@
 
 [![pypi](https://img.shields.io/github/v/release/moj-analytical-services/splink?include_prereleases)](https://pypi.org/project/splink/#history)
 [![Downloads](https://pepy.tech/badge/splink/month)](https://pepy.tech/project/splink)
 [![Documentation](https://img.shields.io/badge/API-documentation-blue)](https://moj-analytical-services.github.io/splink/)
 
 # Fast, accurate and scalable probabilistic data linkage
 
-Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
+Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets that lack unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
-📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.  
+⚡ **Speed:** Capable of linking a million records on a laptop in around a minute.  
+🎯 **Accuracy:** Support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required for model training.  
+📊 **Interactive Outputs:** Multiple interactive visualisations help users understand their model and diagnose problems.  
 
-Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
+Splink's linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
 
 ![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_1.drawio.png)
 
@@ -72,15 +72,15 @@
 
 ## Documentation
 
 The homepage for the Splink documentation can be found [here](https://moj-analytical-services.github.io/splink/). Interactive demos can be found [here](https://github.com/moj-analytical-services/splink_demos/tree/splink3_demos), or by clicking the following Binder link:
 
 [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/moj-analytical-services/splink_demos/master?urlpath=lab)
 
-The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. A [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
+The specification of the Fellegi Sunter statistical model behind `splink` is similar as that used in the R [fastLink package](https://github.com/kosukeimai/fastLink). Accompanying the fastLink package is an [academic paper](http://imai.fas.harvard.edu/research/files/linkage.pdf) that describes this model. The [Splink documentation site](https://moj-analytical-services.github.io/splink/topic_guides/fellegi_sunter.html) and a [series of interactive articles](https://www.robinlinacre.com/probabilistic_linkage/) also explores the theory behind Splink.
 
 The Office for National Statistics have written a [case study about using Splink](https://github.com/Data-Linkage/Splink-census-linkage/blob/main/SplinkCaseStudy.pdf) to link 2021 Census data to itself.
 
 ## Installation
 
 Splink supports python 3.7+. To obtain the latest released version of splink you can install from PyPI using pip:
 
@@ -97,24 +97,23 @@
 Should you require a more bare-bones version of Splink **without DuckDB**, please see the following area of the docs:
 > [DuckDBless Splink Installation](https://moj-analytical-services.github.io/splink/installations.html#duckdb-less-installation)
 
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
-For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
+For more detailed tutorial, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.linker import DuckDBLinker
 import splink.duckdb.comparison_library as cl
 import splink.duckdb.comparison_template_library as ctl
+from splink.datasets import splink_datasets
 
-import pandas as pd
-
-df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
+df = splink_datasets.fake_1000
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
         "l.first_name = r.first_name",
         "l.surname = r.surname",
     ],
@@ -145,15 +144,15 @@
 ## Videos
 
 - [A introductory presentation on Splink](https://www.youtube.com/watch?v=msz3T741KQI)
 - [An introduction to the Splink Comparison Viewer dashboard](https://www.youtube.com/watch?v=DNvCMqjipis)
 
 ## Support
 
-Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, pleaase raise an [issue](https://github.com/moj-analytical-services/splink/issues).
+Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, please raise an [issue](https://github.com/moj-analytical-services/splink/issues).
 
 ## Awards
 
 🥇 Analysis in Government Awards 2020: Innovative Methods: [Winner](https://www.gov.uk/government/news/launch-of-the-analysis-in-government-awards)
 
 🥇 MoJ DASD Awards 2020: Innovation and Impact - Winner
```

