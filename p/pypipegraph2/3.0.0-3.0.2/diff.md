# Comparing `tmp/pypipegraph2-3.0.0.tar.gz` & `tmp/pypipegraph2-3.0.2.tar.gz`

## Comparing `pypipegraph2-3.0.0.tar` & `pypipegraph2-3.0.2.tar`

### file list

```diff
@@ -1,123 +1,122 @@
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.0/Cargo.toml
--rw-r--r--   0     1001      123      595 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.coveragerc
--rw-r--r--   0     1001      123     1963 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1231 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.github/workflows/pytest.yml
--rw-r--r--   0     1001      123      754 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.gitignore
--rw-r--r--   0     1001      123      754 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.gitignore.orig
--rw-r--r--   0     1001      123      106 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.hgignore
--rw-r--r--   0     1001      123       30 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/.ppg/logs/runtimes.tsv
--rw-r--r--   0     1001      123       95 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/AUTHORS.rst
--rw-r--r--   0     1001      123      128 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/CHANGELOG.rst
--rw-r--r--   0     1001      123    13831 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/Cargo.lock
--rw-r--r--   0     1001      123     9569 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/README.md
--rwxr-xr-x   0     1001      123       55 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/bacon.sh
--rw-r--r--   0     1001      123      700 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benches/bench1.rs
--rwxr-xr-x   0     1001      123      841 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benchmarks/bench_disjoint.py
--rwxr-xr-x   0     1001      123      802 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benchmarks/bench_kilo_jobs.py
--rwxr-xr-x   0     1001      123     1133 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benchmarks/bench_simple.py
--rwxr-xr-x   0     1001      123      985 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benchmarks/bench_tall.py
--rwxr-xr-x   0     1001      123      947 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/benchmarks/bench_wide.py
--rw-r--r--   0     1001      123     6315 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/designgoals.md
--rw-r--r--   0     1001      123     7618 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/Makefile
--rw-r--r--   0     1001      123       18 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/_static/.gitignore
--rw-r--r--   0     1001      123       41 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/authors.rst
--rw-r--r--   0     1001      123       43 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/changelog.rst
--rw-r--r--   0     1001      123     9264 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/conf.py
--rw-r--r--   0     1001      123     2241 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/index.rst
--rw-r--r--   0     1001      123       67 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/docs/license.rst
--rw-r--r--   0     1001      123    21307 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/Basic_notebook.ipynb
--rw-r--r--   0     1001      123     1409 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/abort_when_stalled.py
--rw-r--r--   0     1001      123     1120 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/call_externals.py
--rw-r--r--   0     1001      123     1126 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/long_for_interactive.py
--rw-r--r--   0     1001      123      260 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/massive_exception.py
--rw-r--r--   0     1001      123      501 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/nested_exception.py
--rw-r--r--   0     1001      123      563 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/pandas_exception.py
--rw-r--r--   0     1001      123      506 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/runtimes.py
--rw-r--r--   0     1001      123     5790 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/simplest/simplest.py
--rw-r--r--   0     1001      123     1148 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/slow_for_interactive.py
--rw-r--r--   0     1001      123     1241 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/stall.py
--rw-r--r--   0     1001      123     1458 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/stop_then_abort_when_stalled.py
--rw-r--r--   0     1001      123     1554 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/examples/stop_when_stalled.py
--rw-r--r--   0     1001      123     2533 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/flake.lock
--rw-r--r--   0     1001      123     6109 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/flake.nix
--rw-r--r--   0     1001      123  1650094 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/flame.svg
--rwxr-xr-x   0     1001      123      121 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/loop_cargo_test.sh
--rwxr-xr-x   0     1001      123      151 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/loop_main.sh
--rwxr-xr-x   0     1001      123      162 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/loop_ppg2_iterations_with_fail.sh
--rwxr-xr-x   0     1001      123      165 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/loop_ppg2_iterations_without_fail.sh
--rwxr-xr-x   0     1001      123       64 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/loop_pytest.sh
--rwxr-xr-x   0     1001      123      171 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/prep_for_tests.sh
--rw-r--r--   0     1001      123     1972 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/pyproject.toml
--rw-r--r--   0     1001      123     6089 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/__init__.py
--rw-r--r--   0     1001      123     3224 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/entry_points.py
--rw-r--r--   0     1001      123     1831 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/enums.py
--rw-r--r--   0     1001      123     1899 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/exceptions.py
--rwxr-xr-x   0     1001      123    28025 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/graph.py
--rw-r--r--   0     1001      123     1528 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/hashers.py
--rwxr-xr-x   0     1001      123     1466 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/history_comparisons.py
--rw-r--r--   0     1001      123    10730 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/interactive.py
--rwxr-xr-x   0     1001      123      843 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/job_status.py
--rwxr-xr-x   0     1001      123   110639 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/jobs.py
--rw-r--r--   0     1001      123     3408 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/parallel.py
--rw-r--r--   0     1001      123    18402 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/ppg1_compatibility.py
--rw-r--r--   0     1001      123     8513 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/ppg_traceback.py
--rwxr-xr-x   0     1001      123    39990 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/runner.py
--rw-r--r--   0     1001      123     2551 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/testing/__init__.py
--rw-r--r--   0     1001      123     9557 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/testing/fixtures.py
--rw-r--r--   0     1001      123     5217 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/python/pypipegraph2/util.py
--rwxr-xr-x   0     1001      123      806 2023-05-17 07:52:01.000000 pypipegraph2-3.0.0/run-maturin-action.sh
--rwxr-xr-x   0     1001      123      167 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/run_pytest.sh
--rw-r--r--   0     1001      123     1645 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/setup.cfg
--rw-r--r--   0     1001      123      557 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/setup.py
--rwxr-xr-x   0     1001      123    97038 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/engine.rs
--rwxr-xr-x   0     1001      123    19910 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/lib.rs
--rw-r--r--   0     1001      123     1009 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/main.rs
--rw-r--r--   0     1001      123    15543 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/main_iterations_with_fail.rs
--rw-r--r--   0     1001      123    10553 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/main_iterations_without_fail.rs
--rwxr-xr-x   0     1001      123    79221 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/src/tests.rs
--rw-r--r--   0     1001      123      209 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/t.py
--rw-r--r--   0     1001      123        0 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/__init__.py
--rw-r--r--   0     1001      123      282 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/_import_does_not_hang.py
--rw-r--r--   0     1001      123     4975 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/conftest.py
--rw-r--r--   0     1001      123      677 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/old_history_for_conversion_test.gz
--rw-r--r--   0     1001      123        0 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/__init__.py
--rw-r--r--   0     1001      123      965 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/shared.py
--rw-r--r--   0     1001      123    27757 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_cache_jobs.py
--rw-r--r--   0     1001      123     5840 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_compatibility_layer.py
--rw-r--r--   0     1001      123     3050 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_cycles.py
--rw-r--r--   0     1001      123    75082 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
--rw-r--r--   0     1001      123    23004 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
--rw-r--r--   0     1001      123    17831 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_other.py
--rw-r--r--   0     1001      123    21651 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_plotjobs.py
--rw-r--r--   0     1001      123     4365 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_prune.py
--rw-r--r--   0     1001      123     3196 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_simple.py
--rw-r--r--   0     1001      123     4792 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_util.py
--rw-r--r--   0     1001      123      927 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/shared.py
--rw-r--r--   0     1001      123    69648 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_basics.py
--rw-r--r--   0     1001      123     7374 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_bootstrap.py
--rw-r--r--   0     1001      123    14235 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_cache_jobs.py
--rw-r--r--   0     1001      123     1636 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_cycles.py
--rw-r--r--   0     1001      123      558 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_flake8.py
--rw-r--r--   0     1001      123     3366 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_function_invariants.py
--rw-r--r--   0     1001      123     2499 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_interactive.py
--rw-r--r--   0     1001      123    47281 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_invariants_and_dependencies.py
--rw-r--r--   0     1001      123    11292 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_job_generating_jobs.py
--rwxr-xr-x   0     1001      123    67423 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_jobs.py
--rw-r--r--   0     1001      123    21848 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_other.py
--rw-r--r--   0     1001      123     2616 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_parallel.py
--rw-r--r--   0     1001      123        2 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/A
--rw-r--r--   0     1001      123      743 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/manual.py
--rwxr-xr-x   0     1001      123       46 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/sleeper.sh
--rw-r--r--   0     1001      123      954 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/stage2.py
--rw-r--r--   0     1001      123    16239 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_plotjobs.py
--rw-r--r--   0     1001      123     2736 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_prune.py
--rw-r--r--   0     1001      123     1914 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_rust_conversion.py
--rw-r--r--   0     1001      123    23688 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_shared_jobs.py
--rw-r--r--   0     1001      123     1846 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_simple.py
--rw-r--r--   0     1001      123     3691 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_util.py
--rw-r--r--   0     1001      123      508 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/test_version.py
--rw-r--r--   0     1001      123    61338 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/tests_from_the_field.py
--rw-r--r--   0     1001      123    61629 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tests/tests_from_the_field.py.orig
--rw-r--r--   0     1001      123     5453 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/todo.md
--rw-r--r--   0     1001      123      154 2023-05-17 07:51:31.000000 pypipegraph2-3.0.0/tox.ini
--rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 pypipegraph2-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.2/Cargo.toml
+-rw-r--r--   0     1001      123      595 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.coveragerc
+-rw-r--r--   0     1001      123     1231 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.github/workflows/pytest.yml
+-rw-r--r--   0     1001      123     1876 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      754 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.gitignore
+-rw-r--r--   0     1001      123      754 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.gitignore.orig
+-rw-r--r--   0     1001      123      106 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.hgignore
+-rw-r--r--   0     1001      123       30 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.ppg/logs/runtimes.tsv
+-rw-r--r--   0     1001      123       95 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/AUTHORS.rst
+-rw-r--r--   0     1001      123      128 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/CHANGELOG.rst
+-rw-r--r--   0     1001      123    13831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/Cargo.lock
+-rw-r--r--   0     1001      123     9569 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/README.md
+-rwxr-xr-x   0     1001      123       55 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/bacon.sh
+-rw-r--r--   0     1001      123      700 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benches/bench1.rs
+-rwxr-xr-x   0     1001      123      841 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_disjoint.py
+-rwxr-xr-x   0     1001      123      802 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_kilo_jobs.py
+-rwxr-xr-x   0     1001      123     1133 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_simple.py
+-rwxr-xr-x   0     1001      123      985 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_tall.py
+-rwxr-xr-x   0     1001      123      947 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_wide.py
+-rw-r--r--   0     1001      123     6315 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/designgoals.md
+-rw-r--r--   0     1001      123     7618 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/Makefile
+-rw-r--r--   0     1001      123       18 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/_static/.gitignore
+-rw-r--r--   0     1001      123       41 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/authors.rst
+-rw-r--r--   0     1001      123       43 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/changelog.rst
+-rw-r--r--   0     1001      123     9264 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/conf.py
+-rw-r--r--   0     1001      123     2241 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/index.rst
+-rw-r--r--   0     1001      123       67 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/license.rst
+-rw-r--r--   0     1001      123    21307 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/Basic_notebook.ipynb
+-rw-r--r--   0     1001      123     1409 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/abort_when_stalled.py
+-rw-r--r--   0     1001      123     1120 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/call_externals.py
+-rw-r--r--   0     1001      123     1126 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/long_for_interactive.py
+-rw-r--r--   0     1001      123      260 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/massive_exception.py
+-rw-r--r--   0     1001      123      501 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/nested_exception.py
+-rw-r--r--   0     1001      123      563 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/pandas_exception.py
+-rw-r--r--   0     1001      123      506 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/runtimes.py
+-rw-r--r--   0     1001      123     5790 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/simplest/simplest.py
+-rw-r--r--   0     1001      123     1148 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/slow_for_interactive.py
+-rw-r--r--   0     1001      123     1241 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stall.py
+-rw-r--r--   0     1001      123     1458 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stop_then_abort_when_stalled.py
+-rw-r--r--   0     1001      123     1554 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stop_when_stalled.py
+-rw-r--r--   0     1001      123     2533 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flake.lock
+-rw-r--r--   0     1001      123     6109 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flake.nix
+-rw-r--r--   0     1001      123  1650094 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flame.svg
+-rwxr-xr-x   0     1001      123      121 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_cargo_test.sh
+-rwxr-xr-x   0     1001      123      151 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_main.sh
+-rwxr-xr-x   0     1001      123      162 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_ppg2_iterations_with_fail.sh
+-rwxr-xr-x   0     1001      123      165 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_ppg2_iterations_without_fail.sh
+-rwxr-xr-x   0     1001      123       64 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_pytest.sh
+-rwxr-xr-x   0     1001      123      171 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/prep_for_tests.sh
+-rw-r--r--   0     1001      123     1972 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/pyproject.toml
+-rwxr-xr-x   0     1001      123     6124 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/__init__.py
+-rw-r--r--   0     1001      123     3224 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/entry_points.py
+-rw-r--r--   0     1001      123     1831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/enums.py
+-rw-r--r--   0     1001      123     1899 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/exceptions.py
+-rwxr-xr-x   0     1001      123    28025 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/graph.py
+-rw-r--r--   0     1001      123     1528 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/hashers.py
+-rwxr-xr-x   0     1001      123     1466 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/history_comparisons.py
+-rw-r--r--   0     1001      123    10730 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/interactive.py
+-rwxr-xr-x   0     1001      123      843 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/job_status.py
+-rwxr-xr-x   0     1001      123   112223 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/jobs.py
+-rw-r--r--   0     1001      123     3408 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/parallel.py
+-rw-r--r--   0     1001      123    18439 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/ppg1_compatibility.py
+-rw-r--r--   0     1001      123     8513 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/ppg_traceback.py
+-rwxr-xr-x   0     1001      123    40775 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/runner.py
+-rw-r--r--   0     1001      123     2551 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/testing/__init__.py
+-rw-r--r--   0     1001      123     9557 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/testing/fixtures.py
+-rw-r--r--   0     1001      123     5217 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/util.py
+-rwxr-xr-x   0     1001      123      806 2023-07-05 09:25:40.000000 pypipegraph2-3.0.2/run-maturin-action.sh
+-rwxr-xr-x   0     1001      123      167 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/run_pytest.sh
+-rw-r--r--   0     1001      123     1645 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/setup.cfg
+-rw-r--r--   0     1001      123      557 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/setup.py
+-rwxr-xr-x   0     1001      123    97038 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/engine.rs
+-rwxr-xr-x   0     1001      123    19910 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     1009 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main.rs
+-rw-r--r--   0     1001      123    15543 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main_iterations_with_fail.rs
+-rw-r--r--   0     1001      123    10553 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main_iterations_without_fail.rs
+-rwxr-xr-x   0     1001      123    79221 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/tests.rs
+-rw-r--r--   0     1001      123      209 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/t.py
+-rw-r--r--   0     1001      123        0 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/__init__.py
+-rw-r--r--   0     1001      123      282 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/_import_does_not_hang.py
+-rw-r--r--   0     1001      123     4975 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/conftest.py
+-rw-r--r--   0     1001      123      677 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/old_history_for_conversion_test.gz
+-rw-r--r--   0     1001      123        0 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/__init__.py
+-rw-r--r--   0     1001      123      965 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/shared.py
+-rw-r--r--   0     1001      123    27757 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cache_jobs.py
+-rw-r--r--   0     1001      123     5840 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_compatibility_layer.py
+-rw-r--r--   0     1001      123     3050 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cycles.py
+-rw-r--r--   0     1001      123    75082 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
+-rw-r--r--   0     1001      123    23004 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
+-rw-r--r--   0     1001      123    17831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_other.py
+-rw-r--r--   0     1001      123    21651 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_plotjobs.py
+-rw-r--r--   0     1001      123     4365 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_prune.py
+-rw-r--r--   0     1001      123     3196 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_simple.py
+-rw-r--r--   0     1001      123     4792 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_util.py
+-rw-r--r--   0     1001      123      927 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/shared.py
+-rw-r--r--   0     1001      123    69648 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_basics.py
+-rw-r--r--   0     1001      123     7374 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_bootstrap.py
+-rw-r--r--   0     1001      123    14235 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_cache_jobs.py
+-rw-r--r--   0     1001      123     1636 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_cycles.py
+-rw-r--r--   0     1001      123      558 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_flake8.py
+-rw-r--r--   0     1001      123     3366 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_function_invariants.py
+-rw-r--r--   0     1001      123     2499 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_interactive.py
+-rw-r--r--   0     1001      123    47281 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_invariants_and_dependencies.py
+-rw-r--r--   0     1001      123    11292 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_job_generating_jobs.py
+-rwxr-xr-x   0     1001      123    67423 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_jobs.py
+-rw-r--r--   0     1001      123    21959 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_other.py
+-rw-r--r--   0     1001      123     2616 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parallel.py
+-rw-r--r--   0     1001      123        2 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/A
+-rw-r--r--   0     1001      123      759 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/manual.py
+-rwxr-xr-x   0     1001      123       52 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/sleeper.sh
+-rw-r--r--   0     1001      123      977 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/stage2.py
+-rw-r--r--   0     1001      123    16239 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_plotjobs.py
+-rw-r--r--   0     1001      123     2736 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_prune.py
+-rw-r--r--   0     1001      123     1914 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_rust_conversion.py
+-rw-r--r--   0     1001      123    23688 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_shared_jobs.py
+-rw-r--r--   0     1001      123     1846 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_simple.py
+-rw-r--r--   0     1001      123     3691 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_util.py
+-rw-r--r--   0     1001      123      508 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_version.py
+-rw-r--r--   0     1001      123    61338 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/tests_from_the_field.py
+-rw-r--r--   0     1001      123     5453 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/todo.md
+-rw-r--r--   0     1001      123      154 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tox.ini
+-rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 pypipegraph2-3.0.2/PKG-INFO
```

### Comparing `pypipegraph2-3.0.0/Cargo.toml` & `pypipegraph2-3.0.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pypipegraph2"
-version = "3.0.0"
+version = "3.0.2"
 edition = "2018"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pypipegraph2"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `pypipegraph2-3.0.0/.coveragerc` & `pypipegraph2-3.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/.github/workflows/CI.yml` & `pypipegraph2-3.0.2/.github/workflows/release.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-name: CI
+name: release
 
 on:
-  push:
-  pull_request:
+  release:
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: PyO3/maturin-action@v1
@@ -58,15 +57,14 @@
   #     with:
   #       name: wheels
   #       path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    # if: github.event_name == 'release' && github.event.action == 'published'
     needs: [ linux ]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: messense/maturin-action@v1
```

### Comparing `pypipegraph2-3.0.0/.github/workflows/pytest.yml` & `pypipegraph2-3.0.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/.gitignore` & `pypipegraph2-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/.gitignore.orig` & `pypipegraph2-3.0.2/.gitignore.orig`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/Cargo.lock` & `pypipegraph2-3.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pypipegraph2"
-version = "3.0.0"
+version = "3.0.2"
 dependencies = [
  "backtrace",
  "colored",
  "env_logger",
  "itertools",
  "log",
  "num_cpus",
```

### Comparing `pypipegraph2-3.0.0/README.md` & `pypipegraph2-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benches/bench1.rs` & `pypipegraph2-3.0.2/benches/bench1.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benchmarks/bench_disjoint.py` & `pypipegraph2-3.0.2/benchmarks/bench_disjoint.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benchmarks/bench_kilo_jobs.py` & `pypipegraph2-3.0.2/benchmarks/bench_kilo_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benchmarks/bench_simple.py` & `pypipegraph2-3.0.2/benchmarks/bench_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benchmarks/bench_tall.py` & `pypipegraph2-3.0.2/benchmarks/bench_tall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/benchmarks/bench_wide.py` & `pypipegraph2-3.0.2/benchmarks/bench_wide.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/designgoals.md` & `pypipegraph2-3.0.2/designgoals.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/docs/Makefile` & `pypipegraph2-3.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/docs/conf.py` & `pypipegraph2-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/docs/index.rst` & `pypipegraph2-3.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/Basic_notebook.ipynb` & `pypipegraph2-3.0.2/examples/Basic_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/abort_when_stalled.py` & `pypipegraph2-3.0.2/examples/abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/call_externals.py` & `pypipegraph2-3.0.2/examples/call_externals.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/long_for_interactive.py` & `pypipegraph2-3.0.2/examples/long_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/pandas_exception.py` & `pypipegraph2-3.0.2/examples/pandas_exception.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/simplest/simplest.py` & `pypipegraph2-3.0.2/examples/simplest/simplest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/slow_for_interactive.py` & `pypipegraph2-3.0.2/examples/slow_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/stall.py` & `pypipegraph2-3.0.2/examples/stall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/stop_then_abort_when_stalled.py` & `pypipegraph2-3.0.2/examples/stop_then_abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/examples/stop_when_stalled.py` & `pypipegraph2-3.0.2/examples/stop_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/flake.lock` & `pypipegraph2-3.0.2/flake.lock`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/flake.nix` & `pypipegraph2-3.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/flame.svg` & `pypipegraph2-3.0.2/flame.svg`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/pyproject.toml` & `pypipegraph2-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.12,<0.13"]
 build-backend = "maturin"
 
 [project]
 name = "pypipegraph2"
-version = "3.0.0"
+version = "3.0.2"
 description = "Advanced python 'what changed and what do we need to do' tracking"
 long-description = "README.md"
 authors = [
  {"name" = "Florian Finkernagel", "email" = "finkernagel@imt.uni-marburg.de"}
 ]
 classifiers = [
 	"Development Status :: 4 - Beta",
```

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/__init__.py` & `pypipegraph2-3.0.2/python/pypipegraph2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "3.0.0"
+__version__ = "3.0.2"
 
 from pathlib import Path
 import logging
 import contextlib
 from .graph import PyPipeGraph, ALL_CORES
 from .jobs import (
     FileGeneratingJob,
@@ -20,14 +20,15 @@
     FileInvariant,
     ParameterInvariant,
     JobGeneratingJob,
     Job,
     JobList,
     SharedMultiFileGeneratingJob,
     NotebookInvariant,
+    NotebookJob
 )
 from .exceptions import (
     PPGException,
     NotADag,
     FatalGraphException,
     JobOutputConflict,
     JobContractError,
@@ -208,14 +209,15 @@
     "CachedDataLoadingJob",
     "CachedAttributeLoadingJob",
     "PlotJob",
     "FunctionInvariant",
     "FileInvariant",
     "ParameterInvariant",
     "NotebookInvariant",
+    "NotebookJob",
     "JobGeneratingJob",
     "SharedMultiFileGeneratingJob",
     "PPGException",
     "NotADag",
     "FatalGraphException",
     "JobOutputConflict",
     "JobContractError",
```

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/entry_points.py` & `pypipegraph2-3.0.2/python/pypipegraph2/entry_points.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/enums.py` & `pypipegraph2-3.0.2/python/pypipegraph2/enums.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/exceptions.py` & `pypipegraph2-3.0.2/python/pypipegraph2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/graph.py` & `pypipegraph2-3.0.2/python/pypipegraph2/graph.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/hashers.py` & `pypipegraph2-3.0.2/python/pypipegraph2/hashers.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/history_comparisons.py` & `pypipegraph2-3.0.2/python/pypipegraph2/history_comparisons.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/interactive.py` & `pypipegraph2-3.0.2/python/pypipegraph2/interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/job_status.py` & `pypipegraph2-3.0.2/python/pypipegraph2/job_status.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/jobs.py` & `pypipegraph2-3.0.2/python/pypipegraph2/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,14 @@
         files: List[Path],  # todo: extend type attribute to allow mapping
         generating_function: Callable[List[Path]],
         resources: Resources = Resources.SingleCore,
         depend_on_function: bool = True,
         empty_ok=True,
         always_capture_output=True,
     ):
-
         self.generating_function = self._validate_func_argument(generating_function)
         self.depend_on_function = depend_on_function
         self.files, self._lookup = self._validate_files_argument(files)
         if len(self.files) != len(set(self.files)):
             raise ValueError(
                 "Paths were present multiple times in files argument. Fix your input"
             )
@@ -838,15 +837,17 @@
                     try:
                         while wp1 == 0 and waitstatus == 0:
                             sleep_time *= 2
                             if sleep_time > 1:
                                 sleep_time = 1
                             time.sleep(sleep_time)
                             wp1, waitstatus = os.waitpid(self.pid, os.WNOHANG)
-                    except KeyboardInterrupt:  # pragma: no cover  todo: interactive testing
+                    except (
+                        KeyboardInterrupt
+                    ):  # pragma: no cover  todo: interactive testing
                         log_trace(
                             f"Keyboard interrupt in {self.job_id} - sigbreak spawned process"
                         )
                         os.kill(self.pid, signal.SIGUSR1)
                         time.sleep(1)
                         log_trace(
                             f"Keyboard interrupt in {self.job_id} - checking spawned process"
@@ -1136,15 +1137,14 @@
         )
 
 
 class _FileInvariantMixin:
     def calculate(
         self, file, stat, runner=None
     ):  # so that FileInvariant and FunctionInvariant can reuse it
-
         # ppg1 had the option of using an external .md5sum file for the hash
         # provided the filetime was exactly the same as the files'
         # it would accept it instead of calculating it's own.
         # todo:  decide wether we want to keep this here,
         # or move it into it's own class?
         # the pro argument is basically, ppg1. compatibility.
         # the draw back is the complexity for the common case,
@@ -2111,15 +2111,15 @@
     if (
         not hasattr(plot, "render")
         and not hasattr(plot, "save")
         and not hasattr(plot, "savefig")
     ):
         raise exceptions.JobContractError(
             f"{output_filename}.plot_function did not return a plot object "
-            f"(needs to have as render/save/save_fig function). Was {type(plot)}"
+            f"(needs to have as render/save/savefig function). Was {type(plot)}"
         )
     if hasattr(plot, "pd"):  # dppd special..
         plot = plot.pd
     render_args = {}
     if "width" not in render_args and hasattr(plot, "width"):
         render_args["width"] = plot.width
     if "height" not in render_args and hasattr(plot, "height"):
@@ -2224,15 +2224,14 @@
             do_cache,
             depend_on_function=depend_on_function,
         )
         Job.depends_on(
             plot_job, cache_job.load
         )  # necessary because the ppg1 compatibility layer messes with this
     else:
-
         cache_job = None
         if str(cache_filename) in global_pipegraph.jobs:
             raise ValueError(
                 "Redefining PlotJob and removing caching in the process "
                 "not supported. Once cached, always cached. "
                 "At least until somebody fixes job deletion "
                 "or makes this a warning instead"
@@ -2496,15 +2495,17 @@
 
             try:
                 symlink.symlink_to(
                     Path("..")
                     / self.output_dir.relative_to(self.output_dir_prefix)
                     / output_key,
                 )
-            except FileExistsError as e:  # existed, or race condition... symlink.exist()   is lying.
+            except (
+                FileExistsError
+            ) as e:  # existed, or race condition... symlink.exist()   is lying.
                 if not symlink.is_symlink():  # pragma: no cover
                     # can only happen in race condition, other wise captured in output_needed
                     # we really expect this to be a symlink to be a symlink,k?
                     raise ValueError(
                         f"{symlink.absolute()} was not a symlink. Fubared output directory."
                     )
                 if symlink.resolve().absolute() != store_folder.absolute():
@@ -2608,15 +2609,18 @@
         fn = global_pipegraph.history_dir / SharedMultiFileGeneratingJob.log_filename
         with _SharedMultiFileGeneratingJob_log_local_lock:
             if fn.exists():
                 keys = json.loads(fn.read_text())
             else:
                 keys = {}
             keys[str(self.output_dir_prefix)] = key
-            fn.write_text(json.dumps(keys))
+            # safe write to temp, rename temp
+            tf = fn.with_suffix(".temp")
+            tf.write_text(json.dumps(keys))
+            os.rename(tf, fn)
 
     def _raise_partial_result_exception(self):
         raise exceptions.JobContractError(
             f"{self.job_id} some result files existed, some didn't. "
             "In the normal operation of SharedMultiFileGeneratingJob this is impossible."
             " This means your callback is not deterministic "
             ", ie your input does not define your output "
@@ -2700,15 +2704,15 @@
         e.g. size/mtime for FileInvariants or
         per-python-version-bytecodes for FunctionInvariants.
 
         We have to extract just the relevant data,
         and for that we need to lookup the actual jobs.
         """
         hasher = hashlib.sha512()
-        for (key, value) in sorted(hashes.items()):
+        for key, value in sorted(hashes.items()):
             job_id = runner.job_graph.outputs_to_job_ids[key]
             job = runner.jobs[job_id]
             if isinstance(job, SharedMultiFileGeneratingJob) and key == str(
                 job.output_dir_prefix
             ):
                 continue
             hasher.update(key.encode("utf-8"))
@@ -2778,15 +2782,14 @@
 
 class NotebookInvariant(FileInvariant):
     """An invariant that checks only the code and markdown from a notebook (not the results)"""
 
     def calculate(
         self, file, stat, runner=None
     ):  # so that FileInvariant and FunctionInvariant can reuse it
-
         # ppg1 had the option of using an external .md5sum file for the hash
         # provided the filetime was exactly the same as the files'
         # it would accept it instead of calculating it's own.
         # todo:  decide wether we want to keep this here,
         # or move it into it's own class?
         # the pro argument is basically, ppg1. compatibility.
         # the draw back is the complexity for the common case,
@@ -2798,17 +2801,61 @@
             if file in runner._hash_file_cache:
                 return runner._hash_file_cache[file]
             else:
                 h = hashers.hash_file(file)
                 runner._hash_file_cache[file] = h
                 return h
         else:
-            return hashers.hash_str(NotebookInvariant.extract_notebook_content(file))
+            stat = file.stat()
+            return {
+                "hash": hashers.hash_str(
+                    NotebookInvariant.extract_notebook_content(file)
+                ),
+                "mtime": int(stat.st_mtime),
+                "size": stat.st_size,
+            }
 
     @staticmethod
     def extract_notebook_content(file):
         cells = json.loads(file.read_text())["cells"]
         out = ""
         for cell in cells:
             if cell["cell_type"] in ("markdown", "code"):
-                out += "--\n" + cell["source"][0] + "\n\n"
+                out += "--\n" + "\n".join(cell["source"]) + "\n\n"
         return out
+
+
+def NotebookJob(notebook_file, input_files, output_files, html_output_folder):
+    """Run a jupyter notebook, tracking input and output files.
+    Then notebook is rendered into an html file in html_output_folder
+    Reruns whenever the *code* of the notebook changes,
+    not the output results.
+    """
+    notebook_file = Path(notebook_file)
+    html_output_folder = Path(html_output_folder)
+    html_filename = html_output_folder / notebook_file.with_suffix(".html").name
+    output_files = [Path(x) for x in output_files]
+    output_files.append(html_filename)
+
+    def run(output_files):
+        import subprocess
+
+        Path(html_filename.parent).mkdir(exist_ok=True, parents=True)
+        subprocess.check_call(
+            [
+                "jupyter",
+                "nbconvert",
+                "--execute",
+                "--to",
+                "html",
+                notebook_file,
+                "--output",
+                html_filename,
+            ]
+        )
+
+    job = MultiFileGeneratingJob(output_files, run)
+    job.depends_on(
+        NotebookInvariant(notebook_file)
+    )  # todo: replace with 'code in notebook'
+    job.depends_on(input_files)
+    return job
```

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/parallel.py` & `pypipegraph2-3.0.2/python/pypipegraph2/parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/ppg1_compatibility.py` & `pypipegraph2-3.0.2/python/pypipegraph2/ppg1_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import logging
 import pypipegraph as ppg1
 import pypipegraph.testing
 import pypipegraph.testing.fixtures
 import pypipegraph2 as ppg2
 import pypipegraph2.testing
+import pypipegraph2.testing.fixtures
 import wrapt
 import importlib
 from .util import (
     # log_info, log_error, log_warning, log_debug,
     log_job_trace,
 )
```

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/ppg_traceback.py` & `pypipegraph2-3.0.2/python/pypipegraph2/ppg_traceback.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/runner.py` & `pypipegraph2-3.0.2/python/pypipegraph2/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,25 @@
 watcher_parent_pid = None
 watcher_ignored_processes = None
 watcher_session_id = None
 
 
 def get_same_session_id_processes():
     for proc in psutil.process_iter():
-        proc_sid = os.getsid(proc.pid)
+        proc_sid = os.getpgid(proc.pid)
         if proc_sid == watcher_session_id:
             yield proc
 
 
 def kill_process_group_but_ppg_runner():
+    log_info("kill_process_group_but_ppg_runner")
     children_to_reap = []
     my_pid = os.getpid()
     for proc in get_same_session_id_processes():
+        log_info(f"{proc} ignored: {proc in watcher_ignored_processes}")
         if not proc in watcher_ignored_processes:
             children_to_reap.append(proc)
     for p in children_to_reap:
         try:
             log_info(
                 f"Abort: Watcher is terminating child processes {p.pid} {p.name()} {p.status()}"
             )
@@ -75,15 +77,15 @@
 def watcher_unexpected_death_of_parent(_signum, _frame):
     log_error(f"Watcher discovered parent process died unexpectedly {os.getpid()}")
     kill_process_group_but_ppg_runner()
     os._exit(0)
 
 
 def watcher_expected_death_of_parent(_signum, _frame):
-    log_error("Watcher discovered parent process ended regularly")
+    log_info("Watcher discovered parent process ended regularly")
     kill_process_group_but_ppg_runner()
     os._exit(0)
 
 
 def spawn_watcher():
     """The watcher registers to be informed when the parent process dies.
     It then goes and kills the process group,
@@ -93,38 +95,46 @@
 
     The watcher also get's a sig_int when the graph execution ends,
     which also signals it to go and terminate all stragglers.
 
     """
     global watcher_parent_pid, watcher_ignored_processes, watcher_session_id
     if watcher_session_id is None:
-        log_info("setting watcher sid")
-        already_a_session = True
-        os.setsid()
-        watcher_session_id = os.getsid(0)
+        log_info("Capturing watcher process group id")
+        my_pid = os.getpid()
+        my_pgid = os.getpgid(my_pid)
+        # ok, the shell gives us a group id, right?
+        # we do not mess with that, or the session id, we are not a shell,
+        # and we don't fork for the top level managment process.
+        # (messing with setgrp and so on has only lead to pain...)
+        watcher_session_id = my_pgid
+        log_info(f"Watcher identifies process by process group id {watcher_session_id}")
     recv, send = multiprocessing.Pipe()
+    log_info("Collecting already running process that will be ignored by teh watcher")
+    log_info("%s" % (watcher_ignored_processes,))
     pid = os.fork()
     if pid == 0:
-        log_info(f"watcher_session_id {watcher_session_id}")
+        watcher_ignored_processes = list(get_same_session_id_processes())
         watcher_parent_pid = os.getppid()
         parent_process = psutil.Process(watcher_parent_pid)
         # these guys were around before, so we don't kill tehm.
-        watcher_ignored_processes = list(get_same_session_id_processes())
 
         signal.signal(signal.SIGTERM, watcher_unexpected_death_of_parent)
         signal.signal(signal.SIGINT, watcher_expected_death_of_parent)
+        # get watcher to detect parent's death
         prtcl = ctypes.CDLL("libc.so.6")["prctl"]
         PR_SET_PDEATHSIG = 1
         prtcl(PR_SET_PDEATHSIG, signal.SIGTERM)  # 1 =
         log_info("entering watcher loop")
         send.send_bytes(b"go")
         send.close()
+        sys.stdin.close()
         while True:
-            time.sleep(100)
-        log_info("watcher done")
+            time.sleep(100)  # we Live by signal from here on
+        log_info("watcher loop exit - should be unreachable?")
         os._exit(0)
     else:
         recv.recv_bytes()
         recv.close()
         return pid
 
 
@@ -281,15 +291,17 @@
         for job_id in new_jobs:
             _recurse_unpruning(job_id)
 
         for job_id in pruned:
             log_job_trace(f"pruned {job_id}")
             try:
                 dag.remove_node(job_id)
-            except networkx.exception.NetworkXError:  # happens with cleanup nodes that we  omitted
+            except (
+                networkx.exception.NetworkXError
+            ):  # happens with cleanup nodes that we  omitted
                 pass
             # del self.jobs[job_id]
         return pruned
 
     def modify_dag(  # noqa: C901
         self,
         job_graph,
@@ -794,23 +806,24 @@
                                     )
                                     error = exceptions.JobContractError(
                                         f"{job_id} changed current_working_directory. Since ppg2 is multithreaded, you must not do this in jobs that RunHere"
                                     )
                                     outputs = None
                                     raise error
 
-                    except SystemExit as e:  # pragma: no cover - happens in spawned process, and we don't get coverage logging for it thanks to os._exit
+                    except (
+                        SystemExit
+                    ) as e:  # pragma: no cover - happens in spawned process, and we don't get coverage logging for it thanks to os._exit
                         log_trace(
                             "SystemExit in spawned process -> converting to hard exit"
                         )
                         if os.getpid() != self.pid:
                             os._exit(e.args[0])
                     except Exception as e:
                         if isinstance(e, KeyboardInterrupt):  # happens on abort
-
                             raise
                         elif isinstance(e, exceptions.JobError):
                             pass  # take it at face value
                         else:
                             exception_type, exception_value, tb = sys.exc_info()
                             captured_tb = ppg_traceback.Trace(
                                 exception_type, exception_value, tb
@@ -846,15 +859,14 @@
                                     error = exceptions.JobContractError(
                                         f"\t{job_id} returned the wrong set of outputs. "
                                         f"Should be {escape_logging(str(set((self.jobs[job_id].outputs))))}, was {escape_logging(str(set(outputs.keys())))}",
                                     )
                                     outputs = None
 
                                 if outputs is not None:
-
                                     self.job_outcomes[job_id] = RecordedJobOutcome(
                                         job_id, JobOutcome.Success, outputs
                                     )
                                     str_history = json.dumps(
                                         outputs, sort_keys=True, indent=1
                                     )
                                     ljt(f"success {job_id} str_history {str_history}")
```

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/testing/__init__.py` & `pypipegraph2-3.0.2/python/pypipegraph2/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/testing/fixtures.py` & `pypipegraph2-3.0.2/python/pypipegraph2/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/python/pypipegraph2/util.py` & `pypipegraph2-3.0.2/python/pypipegraph2/util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/run-maturin-action.sh` & `pypipegraph2-3.0.2/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/setup.cfg` & `pypipegraph2-3.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [metadata]
 name = pypipegraph2
 description = Advanced python 'what changed and what do we need to do' tracking
-version = 3.0.0
+version = 3.0.2
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
 license = mit
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8
 url = https://github.com/pyscaffold/pyscaffold/
 project-urls =
```

### Comparing `pypipegraph2-3.0.0/setup.py` & `pypipegraph2-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/engine.rs` & `pypipegraph2-3.0.2/src/engine.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/lib.rs` & `pypipegraph2-3.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/main.rs` & `pypipegraph2-3.0.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/main_iterations_with_fail.rs` & `pypipegraph2-3.0.2/src/main_iterations_with_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/main_iterations_without_fail.rs` & `pypipegraph2-3.0.2/src/main_iterations_without_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/src/tests.rs` & `pypipegraph2-3.0.2/src/tests.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/conftest.py` & `pypipegraph2-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/old_history_for_conversion_test.gz` & `pypipegraph2-3.0.2/tests/old_history_for_conversion_test.gz`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/shared.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_cache_jobs.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_compatibility_layer.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_compatibility_layer.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_cycles.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_job_gen_jobs.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_job_gen_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_other.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_other.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_plotjobs.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_prune.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_simple.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/ppg1_compatibility_layer/test_util.py` & `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/shared.py` & `pypipegraph2-3.0.2/tests/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_basics.py` & `pypipegraph2-3.0.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_bootstrap.py` & `pypipegraph2-3.0.2/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_cache_jobs.py` & `pypipegraph2-3.0.2/tests/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_cycles.py` & `pypipegraph2-3.0.2/tests/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_flake8.py` & `pypipegraph2-3.0.2/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_function_invariants.py` & `pypipegraph2-3.0.2/tests/test_function_invariants.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_interactive.py` & `pypipegraph2-3.0.2/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_invariants_and_dependencies.py` & `pypipegraph2-3.0.2/tests/test_invariants_and_dependencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_job_generating_jobs.py` & `pypipegraph2-3.0.2/tests/test_job_generating_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_jobs.py` & `pypipegraph2-3.0.2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_other.py` & `pypipegraph2-3.0.2/tests/test_other.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,14 +640,15 @@
     pid = int(Path("pid").read_text())
     ok = False
     try:
         ok = psutil.Process(pid).status() == "zombie"
     except psutil.NoSuchProcess:
         ok = True
     if not ok:
+        # subprocess.check_call(["ps", "xf", "-o", "pid,ppid,pgid,cmd"])
         raise ValueError("Process was neither zombie (since parent is dead), nor gone.")
 
     p.communicate()
 
 
 def test_spawned_processes_get_killed_on_catastrophic_process_failure(
     ppg2_per_test, job_trace_log
@@ -663,15 +664,15 @@
             raise ValueError(
                 "children not killed, found a ppg2_test_parallel_sentinel",
                 "pid",
                 proc.pid,
                 "ppid",
                 proc.ppid(),
             )
-        if "sleep" in proc.info["cmdline"]:
+        if "sleep" in proc.info["cmdline"] and "5.51234" in proc.info["cmdline"]:
             raise ValueError(
                 "children not killed, found a sleep",
                 "pid",
                 proc.pid,
                 "ppid",
                 proc.ppid(),
             )
```

### Comparing `pypipegraph2-3.0.0/tests/test_parallel.py` & `pypipegraph2-3.0.2/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/manual.py` & `pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/manual.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import psutil
 
 import setproctitle
 
 setproctitle.setproctitle("stage1")
 
 
-p = subprocess.Popen(["python", Path(__file__).parent / "stage2.py"])
+p = subprocess.Popen(["python", Path(__file__).parent / "stage2.py"], env=os.environ)
 p.communicate()
 print("stage 2 ended, ", os.getpid())
 subprocess.check_call(["ps", "--forest", "-o", "%p %r %c"])
 
 for proc in psutil.process_iter(["cmdline"]):
     if "ppg2_test_parallel_sentinel" in proc.info["cmdline"]:
         print(
```

### Comparing `pypipegraph2-3.0.0/tests/test_parent_termination_kills_children/stage2.py` & `pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/stage2.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     )
 
 
 def kill_us():
     time.sleep(1)
 
     p = psutil.Process(os.getpid())
-    ppg.util.log_error(f"killing {os.getpid()}")
+    ppg.util.log_error(f"now killing this jobs process. {os.getpid()}")
     p.kill()
 
 
 jobA = ppg.FileGeneratingJob("A", do_a)
 jobB = ppg.JobGeneratingJob("B", kill_us)
 
 try:
```

### Comparing `pypipegraph2-3.0.0/tests/test_plotjobs.py` & `pypipegraph2-3.0.2/tests/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_prune.py` & `pypipegraph2-3.0.2/tests/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_rust_conversion.py` & `pypipegraph2-3.0.2/tests/test_rust_conversion.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_shared_jobs.py` & `pypipegraph2-3.0.2/tests/test_shared_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_simple.py` & `pypipegraph2-3.0.2/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/test_util.py` & `pypipegraph2-3.0.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/tests/tests_from_the_field.py` & `pypipegraph2-3.0.2/tests/tests_from_the_field.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/todo.md` & `pypipegraph2-3.0.2/todo.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.0/PKG-INFO` & `pypipegraph2-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipegraph2
-Version: 3.0.0
+Version: 3.0.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: loguru
 Requires-Dist: rich
 Requires-Dist: xxhash
 Requires-Dist: wrapt
```

