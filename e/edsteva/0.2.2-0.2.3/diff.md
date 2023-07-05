# Comparing `tmp/edsteva-0.2.2.tar.gz` & `tmp/edsteva-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsteva-0.2.2.tar", max compression
+gzip compressed data, was "edsteva-0.2.3.tar", max compression
```

## Comparing `edsteva-0.2.2.tar` & `edsteva-0.2.3.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1485 2023-07-03 16:24:44.940304 edsteva-0.2.2/LICENSE
--rw-r--r--   0        0        0     3030 2023-07-03 16:24:44.940304 edsteva-0.2.2/README.md
--rw-r--r--   0        0        0     3083 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/__init__.py
--rw-r--r--   0        0        0      138 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/__init__.py
--rw-r--r--   0        0        0     2345 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/files.py
--rw-r--r--   0        0        0    11701 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/hive.py
--rw-r--r--   0        0        0     6221 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/i2b2_mapping.py
--rw-r--r--   0        0        0     2957 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/postgres.py
--rw-r--r--   0        0        0     9050 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/settings.py
--rw-r--r--   0        0        0       37 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/__init__.py
--rw-r--r--   0        0        0     4044 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/biology.py
--rw-r--r--   0        0        0     1053 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/care_site.py
--rw-r--r--   0        0        0     4169 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/note.py
--rw-r--r--   0        0        0    27017 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/synthetic.py
--rw-r--r--   0        0        0     2997 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/utils.py
--rw-r--r--   0        0        0     3835 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/io/synthetic/visit.py
--rw-r--r--   0        0        0      395 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/metrics/__init__.py
--rw-r--r--   0        0        0     2169 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/metrics/error.py
--rw-r--r--   0        0        0     2558 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/metrics/error_after_t0.py
--rw-r--r--   0        0        0     2718 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/metrics/error_between_t0_t1.py
--rw-r--r--   0        0        0       42 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/__init__.py
--rw-r--r--   0        0        0    10800 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/base.py
--rw-r--r--   0        0        0       83 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/__init__.py
--rw-r--r--   0        0        0      239 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/algos/__init__.py
--rw-r--r--   0        0        0     3329 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     5590 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/rectangle_function.py
--rw-r--r--   0        0        0     1450 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     5197 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/defaults.py
--rw-r--r--   0        0        0     1207 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0     1036 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      284 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      165 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0       68 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/__init__.py
--rw-r--r--   0        0        0      336 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/algos/__init__.py
--rw-r--r--   0        0        0     2670 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     2488 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/algos/quantile.py
--rw-r--r--   0        0        0     5292 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/step_function.py
--rw-r--r--   0        0        0     1395 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     4315 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/defaults.py
--rw-r--r--   0        0        0      960 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      789 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      284 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      165 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/models/step_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0      257 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/__init__.py
--rw-r--r--   0        0        0    14067 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/base.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/biology/__init__.py
--rw-r--r--   0        0        0     9091 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/biology/biology.py
--rw-r--r--   0        0        0      488 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/biology/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     5645 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/biology/completeness_predictors/per_measurement.py
--rw-r--r--   0        0        0     6468 2023-07-03 16:24:44.956304 edsteva-0.2.2/edsteva/probes/biology/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     2595 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
--rw-r--r--   0        0        0     5642 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
--rw-r--r--   0        0        0      417 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
--rw-r--r--   0        0        0     5941 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
--rw-r--r--   0        0        0      417 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5963 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      417 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/__init__.py
--rw-r--r--   0        0        0      483 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7900 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/completeness_predictors/per_condition.py
--rw-r--r--   0        0        0     8932 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6392 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/condition.py
--rw-r--r--   0        0        0     2437 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/__init__.py
--rw-r--r--   0        0        0     5701 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/__init__.py
--rw-r--r--   0        0        0     5933 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     6549 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/__init__.py
--rw-r--r--   0        0        0      457 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7222 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/completeness_predictors/per_note.py
--rw-r--r--   0        0        0     8556 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6418 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/note.py
--rw-r--r--   0        0        0     2278 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/__init__.py
--rw-r--r--   0        0        0     5218 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/__init__.py
--rw-r--r--   0        0        0     5475 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     6185 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/utils/__init__.py
--rw-r--r--   0        0        0    10772 2023-07-03 16:24:44.960304 edsteva-0.2.2/edsteva/probes/utils/filter_df.py
--rw-r--r--   0        0        0    22314 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/utils/prepare_df.py
--rw-r--r--   0        0        0     6672 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/utils/utils.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/__init__.py
--rw-r--r--   0        0        0      291 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     8230 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     5326 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/visit.py
--rw-r--r--   0        0        0     1795 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/__init__.py
--rw-r--r--   0        0        0     4982 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5237 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/__init__.py
--rw-r--r--   0        0        0     2498 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/checks.py
--rw-r--r--   0        0        0     1155 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/file_management.py
--rw-r--r--   0        0        0     1970 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/framework.py
--rw-r--r--   0        0        0      176 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/loss_functions.py
--rw-r--r--   0        0        0      344 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/utils/typing.py
--rw-r--r--   0        0        0       52 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/__init__.py
--rw-r--r--   0        0        0      242 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/normalized_probe/__init__.py
--rw-r--r--   0        0        0    11510 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/probe/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/probe/fitted_probe.py
--rw-r--r--   0        0        0     3477 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/probe/probe.py
--rw-r--r--   0        0        0     7686 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/dashboards/probe/wrapper.py
--rw-r--r--   0        0        0      339 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/estimates_densities/__init__.py
--rw-r--r--   0        0        0     8510 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/estimates_densities/estimates_densities.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/normalized_probe/__init__.py
--rw-r--r--   0        0        0     7448 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/probe/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/probe/fitted_probe.py
--rw-r--r--   0        0        0     1483 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/probe/probe.py
--rw-r--r--   0        0        0     5473 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/plots/probe/wrapper.py
--rw-r--r--   0        0        0    15945 2023-07-03 16:24:44.964304 edsteva-0.2.2/edsteva/viz/utils.py
--rw-r--r--   0        0        0     3492 2023-07-03 16:24:44.968304 edsteva-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5759 1970-01-01 00:00:00.000000 edsteva-0.2.2/setup.py
--rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 edsteva-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-07-05 07:04:21.350945 edsteva-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3030 2023-07-05 07:04:21.350945 edsteva-0.2.3/README.md
+-rw-r--r--   0        0        0     3083 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/files.py
+-rw-r--r--   0        0        0    11701 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/hive.py
+-rw-r--r--   0        0        0     6221 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/i2b2_mapping.py
+-rw-r--r--   0        0        0     2957 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/postgres.py
+-rw-r--r--   0        0        0     9050 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/settings.py
+-rw-r--r--   0        0        0       37 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/__init__.py
+-rw-r--r--   0        0        0     4044 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/biology.py
+-rw-r--r--   0        0        0     1053 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/care_site.py
+-rw-r--r--   0        0        0     4169 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/note.py
+-rw-r--r--   0        0        0    27017 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/synthetic.py
+-rw-r--r--   0        0        0     2997 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/utils.py
+-rw-r--r--   0        0        0     3835 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/visit.py
+-rw-r--r--   0        0        0      395 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error.py
+-rw-r--r--   0        0        0     2558 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error_after_t0.py
+-rw-r--r--   0        0        0     2718 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error_between_t0_t1.py
+-rw-r--r--   0        0        0       42 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/base.py
+-rw-r--r--   0        0        0       83 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/__init__.py
+-rw-r--r--   0        0        0      239 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/algos/__init__.py
+-rw-r--r--   0        0        0     3329 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     5590 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/rectangle_function.py
+-rw-r--r--   0        0        0     1450 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     5197 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1207 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0     1036 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0       68 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/__init__.py
+-rw-r--r--   0        0        0     2670 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     2488 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/quantile.py
+-rw-r--r--   0        0        0     5292 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/step_function.py
+-rw-r--r--   0        0        0     1395 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     4315 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0      960 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      789 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0      257 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/__init__.py
+-rw-r--r--   0        0        0    14067 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/base.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/__init__.py
+-rw-r--r--   0        0        0     9091 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/biology.py
+-rw-r--r--   0        0        0      488 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     5645 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_measurement.py
+-rw-r--r--   0        0        0     6468 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     2595 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
+-rw-r--r--   0        0        0     5239 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
+-rw-r--r--   0        0        0     5538 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5539 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/condition/__init__.py
+-rw-r--r--   0        0        0      483 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7900 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_condition.py
+-rw-r--r--   0        0        0     8932 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6392 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/condition.py
+-rw-r--r--   0        0        0     2437 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/__init__.py
+-rw-r--r--   0        0        0     5310 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/__init__.py
+-rw-r--r--   0        0        0     5542 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6131 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7222 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_note.py
+-rw-r--r--   0        0        0     8556 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6418 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/note.py
+-rw-r--r--   0        0        0     2278 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/__init__.py
+-rw-r--r--   0        0        0     5148 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5782 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/__init__.py
+-rw-r--r--   0        0        0    10772 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/filter_df.py
+-rw-r--r--   0        0        0    22314 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/prepare_df.py
+-rw-r--r--   0        0        0     6672 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     8230 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     5326 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/visit.py
+-rw-r--r--   0        0        0     1795 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/__init__.py
+-rw-r--r--   0        0        0     4649 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     4904 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/__init__.py
+-rw-r--r--   0        0        0     2498 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/checks.py
+-rw-r--r--   0        0        0     1155 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/file_management.py
+-rw-r--r--   0        0        0     1970 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/framework.py
+-rw-r--r--   0        0        0      176 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/utils/loss_functions.py
+-rw-r--r--   0        0        0      344 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/utils/typing.py
+-rw-r--r--   0        0        0       52 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/__init__.py
+-rw-r--r--   0        0        0    11909 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/fitted_probe.py
+-rw-r--r--   0        0        0     3477 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/probe.py
+-rw-r--r--   0        0        0     7686 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/wrapper.py
+-rw-r--r--   0        0        0      339 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/estimates_densities/__init__.py
+-rw-r--r--   0        0        0     8510 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/estimates_densities/estimates_densities.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/normalized_probe/__init__.py
+-rw-r--r--   0        0        0     7621 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/fitted_probe.py
+-rw-r--r--   0        0        0     1483 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/probe.py
+-rw-r--r--   0        0        0     5453 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/wrapper.py
+-rw-r--r--   0        0        0    16408 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/utils.py
+-rw-r--r--   0        0        0     3492 2023-07-05 07:04:21.374945 edsteva-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5759 1970-01-01 00:00:00.000000 edsteva-0.2.3/setup.py
+-rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 edsteva-0.2.3/PKG-INFO
```

### Comparing `edsteva-0.2.2/LICENSE` & `edsteva-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/README.md` & `edsteva-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.2
+pip install edsteva==0.2.3
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -8,14 +8,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.2 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.3 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

### Comparing `edsteva-0.2.2/edsteva/__init__.py` & `edsteva-0.2.3/edsteva/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 
 import importlib
 import os
 import sys
 import time
 from distutils.version import LooseVersion
```

### Comparing `edsteva-0.2.2/edsteva/io/files.py` & `edsteva-0.2.3/edsteva/io/files.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/hive.py` & `edsteva-0.2.3/edsteva/io/hive.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/i2b2_mapping.py` & `edsteva-0.2.3/edsteva/io/i2b2_mapping.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/postgres.py` & `edsteva-0.2.3/edsteva/io/postgres.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/settings.py` & `edsteva-0.2.3/edsteva/io/settings.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/biology.py` & `edsteva-0.2.3/edsteva/io/synthetic/biology.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/care_site.py` & `edsteva-0.2.3/edsteva/io/synthetic/care_site.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/note.py` & `edsteva-0.2.3/edsteva/io/synthetic/note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/synthetic.py` & `edsteva-0.2.3/edsteva/io/synthetic/synthetic.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/utils.py` & `edsteva-0.2.3/edsteva/io/synthetic/utils.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/io/synthetic/visit.py` & `edsteva-0.2.3/edsteva/io/synthetic/visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/metrics/error.py` & `edsteva-0.2.3/edsteva/metrics/error.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/metrics/error_after_t0.py` & `edsteva-0.2.3/edsteva/metrics/error_after_t0.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/metrics/error_between_t0_t1.py` & `edsteva-0.2.3/edsteva/metrics/error_between_t0_t1.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/base.py` & `edsteva-0.2.3/edsteva/models/base.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/algos/loss_minimization.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/algos/loss_minimization.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/rectangle_function.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/rectangle_function.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/defaults.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py` & `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/algos/loss_minimization.py` & `edsteva-0.2.3/edsteva/models/step_function/algos/loss_minimization.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/algos/quantile.py` & `edsteva-0.2.3/edsteva/models/step_function/algos/quantile.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/step_function.py` & `edsteva-0.2.3/edsteva/models/step_function/step_function.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/models/step_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/viz_configs/defaults.py` & `edsteva-0.2.3/edsteva/models/step_function/viz_configs/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py` & `edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/models/step_function/viz_configs/normalized_probe_plot.py` & `edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_plot.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/base.py` & `edsteva-0.2.3/edsteva/probes/base.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/biology.py` & `edsteva-0.2.3/edsteva/probes/biology/biology.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/completeness_predictors/per_measurement.py` & `edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_measurement.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/completeness_predictors/per_visit.py` & `edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/defaults.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,30 +120,14 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_measurement="sum(n_measurement)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_measurement="max(sum_measurement)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_measurement / alt.datum.max_measurement)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
```

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/defaults.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,30 +131,14 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_measurement="sum(n_measurement)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_measurement="max(sum_measurement)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_measurement / alt.datum.max_measurement)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
```

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/defaults.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,30 +131,14 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            sum_visit_with_measurement="sum(n_visit_with_measurement)",
-            groupby=["value", "date"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_visit_with_measurement / alt.datum.sum_visit)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
```

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py` & `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/condition/completeness_predictors/per_condition.py` & `edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_condition.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/condition/completeness_predictors/per_visit.py` & `edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/condition/condition.py` & `edsteva-0.2.3/edsteva/probes/condition/condition.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/condition/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/probes/condition/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/condition/viz_configs/n_condition/defaults.py` & `edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,30 +94,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_condition="sum(n_condition)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_condition="max(sum_condition)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_condition / alt.datum.max_condition)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -139,42 +123,51 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
+    aggregates=[
+        dict(
+            sum_condition="sum(n_condition)",
+            groupby=["value", "date"],
+        ),
+        dict(
+            max_condition="max(sum_condition)",
+            groupby=["value"],
+        ),
+    ],
+    calculates=[
+        dict(completeness=alt.datum.sum_condition / alt.datum.max_condition),
+    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "sum(n_condition):Q",
-            title="Number of recorded diagnostic codes",
+            "completeness:Q",
+            title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_condition",
                 "op": "sum",
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip(
-                "sum(n_condition):Q",
-                title="Number of recorded diagnostic codes",
-                format=",",
-            ),
+            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_condition/defaults.py` & `edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,30 +94,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_condition="sum(n_condition)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_condition="max(sum_condition)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_condition / alt.datum.max_condition)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -139,51 +123,42 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
-    aggregates=[
-        dict(
-            sum_condition="sum(n_condition)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_condition="max(sum_condition)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(completeness=alt.datum.sum_condition / alt.datum.max_condition),
-    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
-            title="Completeness predictor c(t)",
+            "sum(n_condition):Q",
+            title="Number of recorded diagnostic codes",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_condition",
                 "op": "sum",
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip(
+                "sum(n_condition):Q",
+                title="Number of recorded diagnostic codes",
+                format=",",
+            ),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/probes/condition/viz_configs/per_visit/defaults.py` & `edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,30 +110,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            sum_visit_with_condition="sum(n_visit_with_condition)",
-            groupby=["value", "date"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_visit_with_condition / alt.datum.sum_visit)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
```

### Comparing `edsteva-0.2.2/edsteva/probes/note/completeness_predictors/per_note.py` & `edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/note/completeness_predictors/per_visit.py` & `edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/note/note.py` & `edsteva-0.2.3/edsteva/probes/note/note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/note/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/probes/note/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/note/viz_configs/n_note/defaults.py` & `edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,27 +82,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_note="sum(n_note)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_note="max(sum_note)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(normalized_c=(alt.datum.sum_note / alt.datum.max_note) / alt.datum.c_0)
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -124,40 +111,51 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
+    aggregates=[
+        dict(
+            sum_note="sum(n_note)",
+            groupby=["value", "date"],
+        ),
+        dict(
+            max_note="max(sum_note)",
+            groupby=["value"],
+        ),
+    ],
+    calculates=[
+        dict(completeness=alt.datum.sum_note / alt.datum.max_note),
+    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "sum(n_note):Q",
-            title="Number of discharge summaries",
+            "completeness:Q",
+            title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_note",
                 "op": "sum",
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip(
-                "sum(n_note):Q", title="Number of discharge summaries", format=","
-            ),
+            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/probes/note/viz_configs/per_note/defaults.py` & `edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,27 +82,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_note="sum(n_note)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_note="max(sum_note)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(normalized_c=(alt.datum.sum_note / alt.datum.max_note) / alt.datum.c_0)
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -124,51 +111,40 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
-    aggregates=[
-        dict(
-            sum_note="sum(n_note)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_note="max(sum_note)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(completeness=alt.datum.sum_note / alt.datum.max_note),
-    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
-            title="Completeness predictor c(t)",
+            "sum(n_note):Q",
+            title="Number of discharge summaries",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_note",
                 "op": "sum",
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip(
+                "sum(n_note):Q", title="Number of discharge summaries", format=","
+            ),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/probes/note/viz_configs/per_visit/defaults.py` & `edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,30 +98,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            sum_visit_with_note="sum(n_visit_with_note)",
-            groupby=["value", "date"],
-        ),
-    ],
-    calculates=[
-        dict(
-            normalized_c=(alt.datum.sum_visit_with_note / alt.datum.sum_visit)
-            / alt.datum.c_0
-        )
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
```

### Comparing `edsteva-0.2.2/edsteva/probes/utils/filter_df.py` & `edsteva-0.2.3/edsteva/probes/utils/filter_df.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/utils/prepare_df.py` & `edsteva-0.2.3/edsteva/probes/utils/prepare_df.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/utils/utils.py` & `edsteva-0.2.3/edsteva/probes/utils/utils.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/visit/completeness_predictors/per_visit.py` & `edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/visit/visit.py` & `edsteva-0.2.3/edsteva/probes/visit/visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/visit/viz_configs/__init__.py` & `edsteva-0.2.3/edsteva/probes/visit/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/probes/visit/viz_configs/n_visit/defaults.py` & `edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,27 +76,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_visit="max(sum_visit)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(normalized_c=(alt.datum.sum_visit / alt.datum.max_visit) / alt.datum.c_0)
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -114,36 +101,47 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
+    aggregates=[
+        dict(
+            sum_visit="sum(n_visit)",
+            groupby=["value", "date"],
+        ),
+        dict(
+            max_visit="max(sum_visit)",
+            groupby=["value"],
+        ),
+    ],
+    calculates=[
+        dict(completeness=alt.datum.sum_visit / alt.datum.max_visit),
+    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "sum(n_visit):Q",
-            title="Number of administrative records",
+            "completeness:Q",
+            title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={"field": "n_visit", "op": "sum", "order": "descending"},
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip(
-                "sum(n_visit):Q", title="Number of administrative records", format=","
-            ),
+            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/probes/visit/viz_configs/per_visit/defaults.py` & `edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/defaults.py`

 * *Files 17% similar despite different names*

```diff
@@ -76,27 +76,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_visit="max(sum_visit)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(normalized_c=(alt.datum.sum_visit / alt.datum.max_visit) / alt.datum.c_0)
-    ],
     legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
@@ -114,47 +101,36 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 main_chart = dict(
-    aggregates=[
-        dict(
-            sum_visit="sum(n_visit)",
-            groupby=["value", "date"],
-        ),
-        dict(
-            max_visit="max(sum_visit)",
-            groupby=["value"],
-        ),
-    ],
-    calculates=[
-        dict(completeness=alt.datum.sum_visit / alt.datum.max_visit),
-    ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
-            title="Completeness predictor c(t)",
+            "sum(n_visit):Q",
+            title="Number of administrative records",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={"field": "n_visit", "op": "sum", "order": "descending"},
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip(
+                "sum(n_visit):Q", title="Number of administrative records", format=","
+            ),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.2/edsteva/utils/checks.py` & `edsteva-0.2.3/edsteva/utils/checks.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/utils/file_management.py` & `edsteva-0.2.3/edsteva/utils/file_management.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/utils/framework.py` & `edsteva-0.2.3/edsteva/utils/framework.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/dashboards/normalized_probe/normalized_probe.py` & `edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/normalized_probe.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from copy import deepcopy
-from typing import Dict
+from typing import Dict, List
 
 import altair as alt
 import pandas as pd
 from IPython.display import HTML, display
 
 from edsteva.models.base import BaseModel
 from edsteva.probes.base import BaseProbe
@@ -19,14 +19,15 @@
     generate_error_line,
     generate_horizontal_bar_charts,
     generate_main_chart,
     generate_model_line,
     generate_probe_line,
     generate_time_line,
     generate_vertical_bar_charts,
+    get_indexes_to_groupby,
     month_diff,
     save_html,
 )
 
 
 def normalized_probe_dashboard(
     probe: BaseProbe,
@@ -41,14 +42,15 @@
     probe_line_config: Dict[str, str] = None,
     estimates_selections: Dict[str, str] = None,
     estimates_filters: Dict[str, str] = None,
     vertical_bar_charts_config: Dict[str, str] = None,
     horizontal_bar_charts_config: Dict[str, str] = None,
     time_line_config: Dict[str, str] = None,
     chart_style: Dict[str, float] = None,
+    indexes_to_remove: List[str] = ["care_site_id", "care_site_level"],
     **kwargs,
 ):
     r"""Displays an interactive chart with:
 
     - On the top, the aggregated normalized completeness predictor $\frac{c(\Delta t)}{c_0}$ over normalized time $\Delta t = t - t_0$. It represents the overall deviation from the Model.
     - On the bottom, interactive filters including all the columns in the [Probe][probe] (such as time, care site, number of visits...etc.) and all the estimates (coefficients and metrics) in the [Model][model].
 
@@ -85,32 +87,47 @@
     horizontal_bar_charts_config: Dict[str, str], optional
         If not None, configuration used to construct the horizontal bar charts.
     time_line_config: Dict[str, str], optional
         If not None, configuration used to construct the time line.
     chart_style: Dict[str, float], optional
         If not None, configuration used to configure the chart style.
         **EXAMPLE**: `{"labelFontSize": 13, "titleFontSize": 14}`
+    indexes_to_remove: List[str], optional
+        indexes to remove from the groupby selection.
     """
     alt.data_transformers.disable_max_rows()
 
+    # Pre-processing
     predictor = probe.predictor.copy()
     estimates = fitted_model.estimates.copy()
+    predictor_metrics = probe._metrics.copy()
+    indexes = get_indexes_to_groupby(
+        predictor_columns=predictor.columns,
+        predictor_metrics=predictor_metrics,
+        indexes_to_remove=indexes_to_remove,
+    )
     predictor = predictor.merge(estimates, on=probe._index)
-
     predictor["normalized_date"] = month_diff(
         predictor["date"], predictor["t_0"]
     ).astype(int)
-    predictor["normalized_c_0"] = predictor["c_0"].mask(
-        (predictor["normalized_date"] < 0) | (predictor["c_0"] == 0), 1
+    for estimate in fitted_model._coefs + fitted_model._metrics:
+        if pd.api.types.is_datetime64_any_dtype(predictor[estimate]):
+            predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
+    predictor["normalized_c"] = predictor["c"].where(
+        (predictor["normalized_date"] < 0) | (predictor["c_0"] == 0),
+        predictor["c"] / predictor["c_0"],
     )
-
     predictor["model"] = 1
     predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
+    predictor["legend_model"] = type(fitted_model).__name__
+    predictor = filter_predictor(
+        predictor=predictor, care_site_level=care_site_level, **kwargs
+    )
 
-    predictor.t_0 = predictor.t_0.dt.strftime("%Y-%m")
+    # Get viz config
     probe_config = deepcopy(probe.get_viz_config("normalized_probe_dashboard"))
     model_config = deepcopy(
         fitted_model.get_viz_config("normalized_probe_dashboard", predictor=predictor)
     )
     if not main_chart_config:
         main_chart_config = probe_config["main_chart"]
     if not time_line_config:
@@ -135,24 +152,17 @@
     if not model_line_config:
         model_line_config = model_config["model_line"]
     if not estimates_selections:
         estimates_selections = model_config["estimates_selections"]
     if not estimates_filters:
         estimates_filters = model_config["estimates_filters"]
 
+    # Viz
     predictor["legend_predictor"] = main_chart_config["legend_title"]
     predictor["legend_error_band"] = error_line_config["legend_title"]
-    predictor["legend_model"] = type(fitted_model).__name__
-    predictor = filter_predictor(
-        predictor=predictor, care_site_level=care_site_level, **kwargs
-    )
-    for estimate in fitted_model._coefs + fitted_model._metrics:
-        if pd.api.types.is_datetime64_any_dtype(predictor[estimate]):
-            predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
-
     base = alt.Chart(predictor)
     time_line, time_selection = generate_time_line(
         base=base,
         time_line_config=time_line_config,
     )
 
     horizontal_bar_charts, y_variables_selections = generate_horizontal_bar_charts(
@@ -161,15 +171,14 @@
         predictor=predictor,
     )
     vertical_bar_charts, x_variables_selections = generate_vertical_bar_charts(
         base=base,
         vertical_bar_charts_config=vertical_bar_charts_config,
         predictor=predictor,
     )
-
     selections = dict(
         date=time_selection,
         **y_variables_selections,
         **x_variables_selections,
     )
     selection_charts = dict(
         horizontal_bar_charts,
@@ -182,15 +191,15 @@
     )
     base = add_estimates_filters(
         base=base,
         selection_charts=selection_charts,
         estimates_filters=estimates_filters,
     )
     index_selection, index_fields = create_groupby_selection(
-        indexes=vertical_bar_charts_config["x"] + horizontal_bar_charts_config["y"],
+        indexes=indexes,
         predictor=predictor,
     )
     main_chart = generate_main_chart(
         base=base,
         main_chart_config=main_chart_config,
         index_selection=index_selection,
         index_fields=index_fields,
```

### Comparing `edsteva-0.2.2/edsteva/viz/dashboards/probe/fitted_probe.py` & `edsteva-0.2.3/edsteva/viz/dashboards/probe/fitted_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/dashboards/probe/probe.py` & `edsteva-0.2.3/edsteva/viz/dashboards/probe/probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/dashboards/probe/wrapper.py` & `edsteva-0.2.3/edsteva/viz/dashboards/probe/wrapper.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/plots/estimates_densities/estimates_densities.py` & `edsteva-0.2.3/edsteva/viz/plots/estimates_densities/estimates_densities.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/plots/normalized_probe/normalized_probe.py` & `edsteva-0.2.3/edsteva/viz/plots/normalized_probe/normalized_probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     configure_style,
     create_groupby_selection,
     filter_predictor,
     generate_error_line,
     generate_main_chart,
     generate_model_line,
     generate_probe_line,
+    get_indexes_to_groupby,
     month_diff,
     save_html,
 )
 
 
 def normalized_probe_plot(
     probe: BaseProbe,
@@ -38,15 +39,15 @@
     main_chart_config: Dict[str, float] = None,
     model_line_config: Dict[str, str] = None,
     probe_line_config: Dict[str, str] = None,
     error_line_config: Dict[str, str] = None,
     estimates_selections: Dict[str, str] = None,
     estimates_filters: Dict[str, str] = None,
     chart_style: Dict[str, float] = None,
-    remove_care_site_id: bool = True,
+    indexes_to_remove: List[str] = ["care_site_id"],
     **kwargs,
 ):
     r"""Displays a chart with the aggregated normalized completeness predictor $\frac{c(\Delta t)}{c_0}$ over normalized time $\Delta t = t - t_0$. It represents the overall deviation from the Model.
 
     Is is possible to save the chart in HTML with the "save_path" optional input.
 
     Parameters
@@ -90,81 +91,81 @@
     estimates_selections: Dict[str, str], optional
         If not None, configuration used to construct the estimates selections.
     estimates_filters: Dict[str, str], optional
         If not None, configuration used to construct the estimates filters.
     chart_style: Dict[str, float], optional
         If not None, configuration used to configure the chart style.
         **EXAMPLE**: `{"labelFontSize": 13, "titleFontSize": 14}`
-    remove_care_site_id: bool, optional
-        If False, it will display care site id and care site name, else only care site name.
+    indexes_to_remove: List[str], optional
+        indexes to remove from the groupby selection.
     """
 
+    alt.data_transformers.disable_max_rows()
+
+    # Pre-processing
     predictor = probe.predictor.copy()
+    predictor_metrics = probe._metrics.copy()
     estimates = fitted_model.estimates.copy()
-
-    cols_to_remove = ["date", *probe._metrics]
-    if remove_care_site_id:
-        cols_to_remove.append("care_site_id")
-    indexes = list(set(predictor.columns).difference(cols_to_remove))
-    predictor = predictor.merge(estimates, on=probe._index)
-
-    probe_config = deepcopy(probe.get_viz_config("normalized_probe_plot"))
-    model_config = deepcopy(
-        fitted_model.get_viz_config("normalized_probe_plot", predictor=predictor)
+    indexes = get_indexes_to_groupby(
+        predictor_columns=predictor.columns,
+        predictor_metrics=predictor_metrics,
+        indexes_to_remove=indexes_to_remove,
     )
-    if not probe_line_config:
-        probe_line_config = model_config["probe_line"]
-    if not model_line_config:
-        model_line_config = model_config["model_line"]
-    if not estimates_selections:
-        estimates_selections = model_config["estimates_selections"]
-    if not estimates_filters:
-        estimates_filters = model_config["estimates_filters"]
-    if not main_chart_config:
-        main_chart_config = probe_config["main_chart"]
-    if not error_line_config:
-        error_line_config = probe_config["error_line"]
-    if not chart_style:
-        chart_style = probe_config["chart_style"]
-
+    predictor = predictor.merge(estimates, on=probe._index)
     predictor["normalized_date"] = month_diff(
         predictor["date"], predictor["t_0"]
     ).astype(int)
-    predictor["legend_predictor"] = "Mean"
-    predictor["legend_error_band"] = "Standard deviation"
-    predictor["legend_model"] = type(fitted_model).__name__
-
+    for estimate in fitted_model._coefs + fitted_model._metrics:
+        if pd.api.types.is_datetime64_any_dtype(predictor[estimate]):
+            predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
+    predictor["normalized_c"] = predictor["c"].where(
+        (predictor["normalized_date"] < 0) | (predictor["c_0"] == 0),
+        predictor["c"] / predictor["c_0"],
+    )
     predictor["model"] = 1
     predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
-
+    predictor["legend_model"] = type(fitted_model).__name__
     predictor = filter_predictor(
         predictor=predictor,
         care_site_level=care_site_level,
         stay_type=stay_type,
         care_site_id=care_site_id,
         care_site_short_name=care_site_short_name,
         start_date=start_date,
         end_date=end_date,
         **kwargs,
     )
-    for estimate in fitted_model._coefs + fitted_model._metrics:
-        if pd.api.types.is_datetime64_any_dtype(predictor[estimate]):
-            predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
-
     if t_min:
         predictor = predictor[predictor.normalized_date >= t_min]
     if t_max:
         predictor = predictor[predictor.normalized_date <= t_max]
 
-    indexes = [
-        {"field": variable, "title": variable.replace("_", " ").capitalize()}
-        for variable in indexes
-        if variable in predictor.columns
-    ]
+    # Get viz config
+    probe_config = deepcopy(probe.get_viz_config("normalized_probe_plot"))
+    model_config = deepcopy(
+        fitted_model.get_viz_config("normalized_probe_plot", predictor=predictor)
+    )
+    if not probe_line_config:
+        probe_line_config = model_config["probe_line"]
+    if not model_line_config:
+        model_line_config = model_config["model_line"]
+    if not estimates_selections:
+        estimates_selections = model_config["estimates_selections"]
+    if not estimates_filters:
+        estimates_filters = model_config["estimates_filters"]
+    if not main_chart_config:
+        main_chart_config = probe_config["main_chart"]
+    if not error_line_config:
+        error_line_config = probe_config["error_line"]
+    if not chart_style:
+        chart_style = probe_config["chart_style"]
 
+    # Viz
+    predictor["legend_predictor"] = main_chart_config["legend_title"]
+    predictor["legend_error_band"] = error_line_config["legend_title"]
     index_selection, index_fields = create_groupby_selection(
         indexes=indexes,
         predictor=predictor,
     )
     base = alt.Chart(predictor)
     base = add_estimates_filters(
         base=base,
```

### Comparing `edsteva-0.2.2/edsteva/viz/plots/probe/fitted_probe.py` & `edsteva-0.2.3/edsteva/viz/plots/probe/fitted_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/plots/probe/probe.py` & `edsteva-0.2.3/edsteva/viz/plots/probe/probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.2/edsteva/viz/plots/probe/wrapper.py` & `edsteva-0.2.3/edsteva/viz/plots/probe/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     legend_model: str = "Model f(t)",
     x_axis_title: str = None,
     y_axis_title: str = None,
     main_chart_config: Dict[str, float] = None,
     model_line_config: Dict[str, str] = None,
     probe_line_config: Dict[str, str] = None,
     chart_style: Dict[str, float] = None,
-    remove_care_site_id: bool = True,
+    indexes_to_remove: List[str] = ["care_site_id"],
     **kwargs,
 ):
     r"""
     Displays a chart with the average completeness predictor $c(t)$ over time $t$ with the fitted model $\hat{c}(t)$ if specified.
     The chart is exportable in png or svg format and easy to integrate into a report. Is also possible to save the chart in HTML with the "save_path" optional input.
 
     Parameters
@@ -70,29 +70,29 @@
     model_line_config: Dict[str, str], optional
         If not None, configuration used to construct the model line.
     probe_line_config: Dict[str, str], optional
         If not None, configuration used to construct the probe line.
     chart_style: Dict[str, float], optional
         If not None, configuration used to configure the chart style.
         **EXAMPLE**: `{"labelFontSize": 13, "titleFontSize": 14}`
-    remove_care_site_id: bool, optional
-        If False, it will display care site id and care site name, else only care site name.
+    indexes_to_remove: List[str], optional
+        indexes to remove from the groupby selection.
     """
     alt.data_transformers.enable("default")
     alt.data_transformers.disable_max_rows()
 
     probe_config = deepcopy(probe.get_viz_config("probe_plot"))
     if not main_chart_config:
         main_chart_config = probe_config["main_chart"]
     if not chart_style:
         chart_style = probe_config["chart_style"]
     predictor = probe.predictor.copy()
     cols_to_remove = ["date", *probe._metrics]
-    if remove_care_site_id:
-        cols_to_remove.append("care_site_id")
+    if indexes_to_remove:
+        cols_to_remove.extend(indexes_to_remove)
     indexes = list(set(predictor.columns).difference(cols_to_remove))
 
     if fitted_model:
         predictor = fitted_model.predict(probe).copy()
     else:
         predictor = probe.predictor.copy()
```

### Comparing `edsteva-0.2.2/edsteva/viz/utils.py` & `edsteva-0.2.3/edsteva/viz/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,18 +176,16 @@
         vertical_bar_charts[x_variable["field"]] = x_variable_bar_charts
     return vertical_bar_charts, x_variables_selections
 
 
 def add_interactive_selection(
     base: alt.Chart,
     selections: Dict[str, alt.SelectionParameter],
-    selection_charts: Dict[str, List[alt.Chart]] = None,
+    selection_charts: Dict[str, List[alt.Chart]],
 ):
-    if selection_charts is None:
-        selection_charts = {}
     for selection_variable, selection in selections.items():
         base = base.transform_filter(selection)
         for chart_variable in selection_charts.keys():
             if chart_variable != selection_variable:
                 for i in range(len(selection_charts[chart_variable])):
                     selection_charts[chart_variable][i] = selection_charts[
                         chart_variable
@@ -220,14 +218,29 @@
                 selection_charts[chart_variable][i] = selection_charts[chart_variable][
                     i
                 ].transform_filter(estimate_filter)
 
     return base
 
 
+def get_indexes_to_groupby(
+    predictor_columns: List[str],
+    predictor_metrics: List[str],
+    indexes_to_remove: List[str],
+):
+    cols_to_remove = ["date", *predictor_metrics]
+    if indexes_to_remove:
+        cols_to_remove.extend(indexes_to_remove)
+    indexes = list(set(predictor_columns).difference(cols_to_remove))
+    return [
+        {"field": variable, "title": variable.replace("_", " ").capitalize()}
+        for variable in indexes
+    ]
+
+
 def create_groupby_selection(
     indexes: List[Dict[str, str]],
     predictor: pd.DataFrame,
 ):
     index_fields = [
         index["field"] for index in indexes if index["field"] in predictor.columns
     ]
@@ -247,23 +260,25 @@
     return index_selection, index_fields
 
 
 def configure_style(
     chart: alt.Chart,
     chart_style: Dict[str, float],
 ):
-    return chart.configure_axis(
-        labelFontSize=chart_style["labelFontSize"],
-        titleFontSize=chart_style["titleFontSize"],
-        labelLimit=500,
-    ).configure_legend(
-        labelFontSize=chart_style["labelFontSize"],
-        titleFontSize=chart_style["titleFontSize"],
-        labelLimit=500,
-    )
+    if chart_style:
+        chart = chart.configure_axis(
+            labelFontSize=chart_style["labelFontSize"],
+            titleFontSize=chart_style["titleFontSize"],
+            labelLimit=500,
+        ).configure_legend(
+            labelFontSize=chart_style["labelFontSize"],
+            titleFontSize=chart_style["titleFontSize"],
+            labelLimit=500,
+        )
+    return chart
 
 
 def concatenate_charts(
     main_chart: alt.Chart,
     horizontal_bar_charts: Dict[str, List[alt.Chart]],
     vertical_bar_charts: Dict[str, List[alt.Chart]],
     time_line: alt.Chart = None,
```

### Comparing `edsteva-0.2.2/pyproject.toml` & `edsteva-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edsteva"
-version = "0.2.2"
+version = "0.2.3"
 description = "EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records."
 authors = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Benoit Playe <benoit.playe@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>", "Paul Bernard <paul.bernard@aphp.fr>"]
 keywords = ["OMOP", "Data Analysis", "Electronic health record"]
 readme = "README.md"
 maintainers = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Thomas Petit-Jean <thomas.petitjean@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>"]
 homepage = "https://github.com/aphp/edsteva"
 repository = "https://github.com/aphp/edsteva"
```

### Comparing `edsteva-0.2.2/setup.py` & `edsteva-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
  'pgpasslib>=1.1.0,<2.0.0',
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyarrow>=0.15,<0.17.0',
  'pyspark>=2.4.3,<2.5.0']
 
 setup_kwargs = {
     'name': 'edsteva',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.',
-    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n<a href="https://github.com/astral-sh/ruff" target="_blank">\n    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.2\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
+    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n<a href="https://github.com/astral-sh/ruff" target="_blank">\n    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.3\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
     'author': 'Adam Remaki',
     'author_email': 'adam.remaki@aphp.fr',
     'maintainer': 'Adam Remaki',
     'maintainer_email': 'adam.remaki@aphp.fr',
     'url': 'https://github.com/aphp/edsteva',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 'edsteva.viz.dashboards.probe', 'edsteva.viz.plots',
 'edsteva.viz.plots.estimates_densities', 'edsteva.viz.plots.normalized_probe',
 'edsteva.viz.plots.probe'] package_data = \ {'': ['*']} install_requires = \
 ['altair>=5.0,<6.0', 'catalogue>=2.0.8,<3.0.0', 'ipython>=7.31.0,<8.0.0',
 'koalas>=1.8.2,<2.0.0', 'loguru==0.7.0', 'numpy<1.20.0', 'pandas>=1.3,<2.0',
 'pgpasslib>=1.1.0,<2.0.0', 'psycopg2-binary>=2.9.3,<3.0.0',
 'pyarrow>=0.15,<0.17.0', 'pyspark>=2.4.3,<2.5.0'] setup_kwargs = { 'name':
-'edsteva', 'version': '0.2.2', 'description': 'EDS-TeVa provides a set of tools
+'edsteva', 'version': '0.2.3', 'description': 'EDS-TeVa provides a set of tools
 that aims at modeling the adoption over time and across space of the Electronic
 Health Records.', 'long_description': '
        \nDISCLAIMER:EDS-TeVa is intended to be a module of EDS-Scikit\n
 \n\n
                                      \n\n
                                 \n [EDS-TeVa]\n
    \n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://
@@ -47,15 +47,15 @@
 tools that aims at modeling the adoption over time and across space of the
 Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders
 of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:
 \n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa
 through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning
 the library version in your projects, or use a strict package manager like
 [Poetry](https://python-poetry.org/).\n\n```\npip install
-edsteva==0.2.2\n```\n## Example\n\nA scientific paper is currently being
+edsteva==0.2.3\n```\n## Example\n\nA scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given.\n\n## Acknowledgement\n\nWe would like to thank
 [Assistance Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP
 Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
 'author': 'Adam Remaki', 'author_email': 'adam.remaki@aphp.fr', 'maintainer':
```

### Comparing `edsteva-0.2.2/PKG-INFO` & `edsteva-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsteva
-Version: 0.2.2
+Version: 0.2.3
 Summary: EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.
 Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause
 Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki
 Author-email: adam.remaki@aphp.fr
 Maintainer: Adam Remaki
@@ -92,15 +92,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.2
+pip install edsteva==0.2.3
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edsteva Version: 0.2.2 Summary: EDS-TeVa provides a
+Metadata-Version: 2.1 Name: edsteva Version: 0.2.3 Summary: EDS-TeVa provides a
 set of tools that aims at modeling the adoption over time and across space of
 the Electronic Health Records. Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki Author-email: adam.remaki@aphp.fr Maintainer: Adam Remaki
 Maintainer-email: adam.remaki@aphp.fr Requires-Python: >=3.7.1,<3.8.0
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
@@ -29,14 +29,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.2 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.3 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

