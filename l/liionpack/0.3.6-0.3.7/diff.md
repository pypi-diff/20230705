# Comparing `tmp/liionpack-0.3.6.tar.gz` & `tmp/liionpack-0.3.7.tar.gz`

## Comparing `liionpack-0.3.6.tar` & `liionpack-0.3.7.tar`

### file list

```diff
@@ -1,89 +1,90 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.6/.git-blame-ignore-revs
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 liionpack-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.6/.readthedocs.yaml
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 liionpack-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.6/asv.conf.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 liionpack-0.3.6/environment.yml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.6/mkdocs.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/codecov.yml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/periodic_benchmarks.yml
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/run_benchmarks_over_history.yml
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/test_on_push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/benchmarks/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.6/benchmarks/benchmarks.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/about.md
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/conduct.md
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/contributing.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/index.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/install.md
--rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/liionpack.png
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/mathjax-config.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/reference.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/requirements.txt
--rw-r--r--   0        0        0   428208 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/01 Getting Started.ipynb
--rw-r--r--   0        0        0   258064 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/02 Using inputs.ipynb
--rw-r--r--   0        0        0   115177 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/03 Experiments.ipynb
--rw-r--r--   0        0        0   320758 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/04 Initial SoC.ipynb
--rw-r--r--   0        0        0   939974 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/05 Drive cycles.ipynb
--rw-r--r--   0        0        0   894028 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/06 Changing a model.ipynb
--rw-r--r--   0        0        0   131502 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/07 Visualizing larger packs.ipynb
--rw-r--r--   0        0        0  1291981 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/08 SEI degradation model.ipynb
--rw-r--r--   0        0        0   322325 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/09 Terminal locations.ipynb
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/basic_16p2s.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/big_circuit.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/different_initial_soc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/draw_circuit.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/draw_terminals.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/drive_cycle.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/drive_cycle_comparison.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/load_4p1s.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/mixed_terminals.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/paper_example.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/save_output.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/step_external_variable.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/thermal_external.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/definitions.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/logger.py
--rw-r--r--   0        0        0    25031 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/netlist_utils.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/plots.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/protocols.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/sim_utils.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/simulations.py
--rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/solver_utils.py
--rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/solvers.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/utils.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.asc
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.cir
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.txt
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper.bib
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper.md
--rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_0.png
--rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_1.png
--rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_2.png
--rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_3.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/test_1p1s.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/test_all_solvers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_logger.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_netlist_utils.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_notebooks.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_plots.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_protocols.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_sim_utils.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_simulations.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_solver_utils.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_solvers.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 liionpack-0.3.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.6/LICENSE
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.6/README.md
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 liionpack-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 liionpack-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.7/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 liionpack-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.7/.readthedocs.yaml
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 liionpack-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.7/asv.conf.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 liionpack-0.3.7/environment.yml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.7/mkdocs.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/codecov.yml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/workflows/periodic_benchmarks.yml
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/workflows/run_benchmarks_over_history.yml
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 liionpack-0.3.7/.github/workflows/test_on_push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.7/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.7/benchmarks/benchmarks.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/about.md
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/conduct.md
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/contributing.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/index.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/install.md
+-rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/liionpack.png
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/mathjax-config.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/reference.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/requirements.txt
+-rw-r--r--   0        0        0   428208 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/01 Getting Started.ipynb
+-rw-r--r--   0        0        0   258064 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/02 Using inputs.ipynb
+-rw-r--r--   0        0        0   129217 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/03 Experiments.ipynb
+-rw-r--r--   0        0        0   320758 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/04 Initial SoC.ipynb
+-rw-r--r--   0        0        0  1413983 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/05 Drive cycles.ipynb
+-rw-r--r--   0        0        0   894028 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/06 Changing a model.ipynb
+-rw-r--r--   0        0        0   131502 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/07 Visualizing larger packs.ipynb
+-rw-r--r--   0        0        0  1291981 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/08 SEI degradation model.ipynb
+-rw-r--r--   0        0        0   322325 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/examples/09 Terminal locations.ipynb
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.7/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/basic_16p2s.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/big_circuit.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/different_initial_soc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/draw_circuit.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/draw_terminals.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/drive_cycle.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/drive_cycle_comparison.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/load_4p1s.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/mixed_capacity.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/mixed_terminals.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/paper_example.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/save_output.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/step_external_variable.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.7/examples/thermal_external.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/definitions.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/logger.py
+-rw-r--r--   0        0        0    25031 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/netlist_utils.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/plots.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/protocols.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/sim_utils.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/simulations.py
+-rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/solver_utils.py
+-rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/solvers.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/utils.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/circuits/4p1s.asc
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/circuits/4p1s.cir
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.7/liionpack/circuits/4p1s.txt
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper.bib
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper.md
+-rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper_figures/Figure_0.png
+-rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper_figures/Figure_1.png
+-rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper_figures/Figure_2.png
+-rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.7/paper/paper_figures/Figure_3.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/integration/test_1p1s.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/integration/test_all_solvers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_logger.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_netlist_utils.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_notebooks.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_plots.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_protocols.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_sim_utils.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_simulations.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_solver_utils.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_solvers.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.7/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 liionpack-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.7/README.md
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 liionpack-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 liionpack-0.3.7/PKG-INFO
```

### Comparing `liionpack-0.3.6/CHANGELOG.md` & `liionpack-0.3.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,31 @@
 
 - ([#PR](link))
 
 ## Breaking changes
 
 - ([#PR](link))
 
-# [v0.3.6](https://github.com/pybamm-team/liionpack/)
+# [v0.3.7](https://github.com/pybamm-team/liionpack/tree/v0.3.7) - 2023-07-05
+
+
+## Bug fixes
+
+- Update to PyBaMM 23.5 with small chages to protocols ([#265](https://github.com/pybamm-team/liionpack/pull/265))
+
+
+# [v0.3.6](https://github.com/pybamm-team/liionpack/tree/v0.3.6) - 2023-05-26
 
 
 ## Bug fixes
 
 - Fix a RunTimeError introduced by change to latest version of casadi that PyBaMM now supports. Solution returned by casadi no longer contains initial state. ([#259](https://github.com/pybamm-team/liionpack/pull/259))
 
 
-# [v0.3.5](https://github.com/pybamm-team/liionpack/) - 2023-04-05
+# [v0.3.5](https://github.com/pybamm-team/liionpack/tree/v0.3.5) - 2023-04-05
 
 ## Features
 
 - Add pre commit and migrate to ruff ([#232](https://github.com/pybamm-team/liionpack/pull/232))
 
 ## Bug fixes
```

### Comparing `liionpack-0.3.6/asv.conf.json` & `liionpack-0.3.7/asv.conf.json`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/environment.yml` & `liionpack-0.3.7/environment.yml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   - matplotlib
   - pandas
   - ipython
   - jupyter
   - sympy
   - pip
   - pip:
-    - pybamm>=23.3
+    - pybamm>=23.5
     - ipdb
     - ruff
     - mkdocstrings-python-legacy
     - mkdocs-material
     - mkdocs-jupyter
     - nbconvert
     - -e .
```

### Comparing `liionpack-0.3.6/mkdocs.yml` & `liionpack-0.3.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/ISSUE_TEMPLATE/bug_report.yml` & `liionpack-0.3.7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/ISSUE_TEMPLATE/feature_request.yml` & `liionpack-0.3.7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/workflows/periodic_benchmarks.yml` & `liionpack-0.3.7/.github/workflows/periodic_benchmarks.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/workflows/publish_pypi.yml` & `liionpack-0.3.7/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/workflows/run_benchmarks_over_history.yml` & `liionpack-0.3.7/.github/workflows/run_benchmarks_over_history.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.github/workflows/test_on_push.yml` & `liionpack-0.3.7/.github/workflows/test_on_push.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/benchmarks/benchmarks.py` & `liionpack-0.3.7/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/conduct.md` & `liionpack-0.3.7/docs/conduct.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/contributing.md` & `liionpack-0.3.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/index.md` & `liionpack-0.3.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/install.md` & `liionpack-0.3.7/docs/install.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/liionpack.png` & `liionpack-0.3.7/docs/liionpack.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/mathjax-config.js` & `liionpack-0.3.7/docs/mathjax-config.js`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/01 Getting Started.ipynb` & `liionpack-0.3.7/docs/examples/01 Getting Started.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/02 Using inputs.ipynb` & `liionpack-0.3.7/docs/examples/02 Using inputs.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/03 Experiments.ipynb` & `liionpack-0.3.7/docs/examples/03 Experiments.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9932105654761905%*

 * *Differences: {"'cells'": "{10: {'execution_count': 7, 'outputs': {0: {'data': {'text/plain': ['[_Step(current, "*

 * *            '5.0, duration=1000 s, termination=3.3 V, description=Discharge at 5 A for 1000 s or '*

 * *            "until 3.3 V),\\n', ' _Step(current, 0, duration=1000 s, description=Rest for 1000 "*

 * *            "s),\\n', ' _Step(current, -5.0, duration=1000 s, termination=4.1 V, "*

 * *            "description=Charge at 5 A for 1000 s or until 4.1 V),\\n', ' _Step(current, 0, "*

 * *            "duration=1000 s, descripti […]*

```diff
@@ -116,149 +116,53 @@
             "metadata": {},
             "source": [
                 "Now we have out experiment we can take a look at the steps involved"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[{'Current input [A]': 5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Discharge at 5 A for 1000 s or until 3.3 V',\n",
-                            "  'events': {'Voltage input [V]': 3.3, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': -5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Charge at 5 A for 1000 s or until 4.1 V',\n",
-                            "  'events': {'Voltage input [V]': 4.1, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Discharge at 5 A for 1000 s or until 3.3 V',\n",
-                            "  'events': {'Voltage input [V]': 3.3, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': -5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Charge at 5 A for 1000 s or until 4.1 V',\n",
-                            "  'events': {'Voltage input [V]': 4.1, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Discharge at 5 A for 1000 s or until 3.3 V',\n",
-                            "  'events': {'Voltage input [V]': 3.3, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': -5.0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Charge at 5 A for 1000 s or until 4.1 V',\n",
-                            "  'events': {'Voltage input [V]': 4.1, 'type': 'voltage'},\n",
-                            "  'tags': None},\n",
-                            " {'Current input [A]': 0,\n",
-                            "  'type': 'current',\n",
-                            "  'time': 1000.0,\n",
-                            "  'period': 10.0,\n",
-                            "  'temperature': None,\n",
-                            "  'dc_data': None,\n",
-                            "  'string': 'Rest for 1000 s',\n",
-                            "  'events': None,\n",
-                            "  'tags': None}]"
+                            "[_Step(current, 5.0, duration=1000 s, termination=3.3 V, description=Discharge at 5 A for 1000 s or until 3.3 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s),\n",
+                            " _Step(current, -5.0, duration=1000 s, termination=4.1 V, description=Charge at 5 A for 1000 s or until 4.1 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s),\n",
+                            " _Step(current, 5.0, duration=1000 s, termination=3.3 V, description=Discharge at 5 A for 1000 s or until 3.3 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s),\n",
+                            " _Step(current, -5.0, duration=1000 s, termination=4.1 V, description=Charge at 5 A for 1000 s or until 4.1 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s),\n",
+                            " _Step(current, 5.0, duration=1000 s, termination=3.3 V, description=Discharge at 5 A for 1000 s or until 3.3 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s),\n",
+                            " _Step(current, -5.0, duration=1000 s, termination=4.1 V, description=Charge at 5 A for 1000 s or until 4.1 V),\n",
+                            " _Step(current, 0, duration=1000 s, description=Rest for 1000 s)]"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "experiment.operating_conditions"
+                "experiment.operating_conditions_steps"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Currently, this is the only information used by liionpack and voltage limits are ignored. There is also some additional checks that take place behind the scenes. The current must be specified in [A] and not in [C] and the time for each step must be an integer multiple of the period."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Cycling experiment\n",
                 "bad_exp_1 = pybamm.Experiment([(\"Discharge at 5 C for 1000 s\",)] * 3, period=\"10 s\")\n",
                 "\n",
                 "bad_exp_2 = pybamm.Experiment([(\"Discharge at 5 A for 999 s\",)] * 3, period=\"10 s\")"
@@ -269,26 +173,26 @@
             "metadata": {},
             "source": [
                 "These bad experiments will be acceptable to PyBaMM and there is no error thrown but the liionpack solver will not like them. We can check what the protocol looks like using the `generate_protocol_from_experiment` function, and this will return a list of currents that are applied at each timestep."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, -5.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "protocol = lp.generate_protocol_from_experiment(experiment)\n",
                 "protocol"
@@ -299,22 +203,22 @@
             "metadata": {},
             "source": [
                 "Let's solve the problem and view the results"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Stepping simulation: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1201/1201 [00:13<00:00, 86.84it/s]\n"
+                        "Stepping simulation: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1201/1201 [00:14<00:00, 84.34it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "# Solve pack\n",
                 "output = lp.solve(\n",
                 "    netlist=netlist,\n",
@@ -323,22 +227,22 @@
                 "    output_variables=output_variables,\n",
                 "    initial_soc=0.5\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAxUAAAJOCAYAAADBIyqKAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy88F64QAAAACXBIWXMAAA9hAAAPYQGoP6dpAACqFklEQVR4nOzdd5wdZb0/8M8zM6dsz5b0CgQIJZREpF1BQLkWimJAgnAhQlTateG9FvwZxF6AK4oCV4MFEL3kUryAAiISOoEQAoF0kkDqbjabLafMzPP747TdbDtlzpl5nvN5v14h2d2z53yHme88852njJgzZ44EERERERFRkQy/AyAiIiIiIrWxqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopKwqCAiIiIiopJYfgdARKSDM888E4sWLcp+bds22tvb8fzzz+OWW27Bzp07Pf/MW2+9FWPGjMEnP/nJon7/9NNPx3nnnYfp06ejrq4OnZ2dWL9+PR577DHcd9993gZLRERaY1FBROShRYsWYcOGDYhGozj66KOxYMECzJkzB5/85CcRi8X8Di/r6quvxiWXXIIlS5bgd7/7HXp7ezFx4kS85z3vwcknn8yigoiICsKigojIQ2vXrsWqVasAAC+99BJM08TChQtxyimn4OGHH/Y5upRIJIL58+fjL3/5C7773e8O+NmDDz4IIYRPkfkrEokgHo/7HQYRkZI4p4KIqIxee+01AMCECRMAAAsXLsRvf/tb/P3vf8eTTz6JO++8E2efffaQv/uhD30IixcvxlNPPYWnnnoKd91117CvzTjllFPw9NNP45vf/CZM0xzyNTU1NYhEIti1a9eQP5dSZv89d+5cLFu2DHPnzh3wmokTJ2LZsmU488wzs99btGgRnnrqKcyYMQM///nPsXTpUvz1r3/FJZdcAgA4/PDD8etf/xpLly7FkiVLcMYZZwx4zzPPPBPLli3DMcccg2uvvRaPP/44nnzySVx33XWIRqNobW3FD37wA/zjH//AX//6V3zhC1+AZQ28N5bv/98HH3wQN910E0455RTceeedeOaZZ/CZz3wGv/zlL3HvvfcO+f/lvvvuw3/9138N+TMiomrHngoiojKaOnUqAKCzsxMAMGnSJNx7773Ytm0bAGD27Nn4j//4D4wbNw6333579vc+97nPYeHChXj88cfxhz/8Ad3d3TjggAMwceLEYT/rggsuwOc//3ncdttt+PWvfz3s6zo7O7Fp0ybMmzcPHR0dePrpp7Fx48bSNxaAZVn48Y9/jHvvvRe/+93v8KEPfQhXX3016urqcOqpp+K3v/0tduzYgU9+8pO47rrrsHbtWrz55psD3uPaa6/FE088ga9//es4+OCDceWVV8KyLEyfPh1///vfsWTJEhx77LG45JJLsHPnTtx5553Z3833/y8AzJo1C/vttx/++7//G++++y76+vrw6quv4sYbb8R73/tevPDCC9nXnnjiiZg6dSp+/OMfe/L/iYhINywqiIg8ZJomTNNEOBzG3Llzcemll6K7uxtPPvkkAOC6667LvlYIgWXLlkEIgfnz52cveidNmoQFCxbgoYcewje/+c3s659//vkhP1MIgWuuuQbnnHMOFi1alNcwq2984xv40Y9+hC996Uv40pe+hO7ubrz88st49NFH8dBDDxW9/eFwGLfccgueeOIJAMCyZcvwvve9D5/+9KdxwQUX4K233gIAvPHGG3j00Ufx4Q9/eFBRsXTpUtx0003ZbT7iiCPwoQ99CD/96U9x1113AQBeeOEFHHfccfjwhz88oKjI5/9vRnNzM84991xs2rRpwO9s2bIFn/zkJwcUFeeddx42b96Mp59+uuj/N0REOmNRQUTkod/+9rcDvl6zZg2+//3vo6OjAwBwzDHHYMGCBTjssMNQX18/4LUtLS3o6OjAscceC8uy8Kc//WnUz4tEIvjpT3+Ko446CldeeSVefvnlvOJ844038LGPfQzHHHMMjj76aBx66KF473vfi5NOOgkf/OAH8cUvfjHPLR7Idd0BF96O42Dz5s1wHCdbUABAV1cXdu/enR0W1t9TTz014OsNGzbglFNOwdKlSwd8f+PGjTjuuOMGfC+f/78Za9euHVBQAKmhX/fccw8+//nPY8KECdi2bRumTJmCE044IVvoEBHRYCwqiIg89M1vfhMbNmyA4zjo6OgYMG/hsMMOw89//nMsW7YM3/nOd7B9+3Ykk0m8//3vx2WXXYZIJAIgdQcdAHbs2DHq5zU3N+P444/HCy+8gBUrVhQUq23bePbZZ/Hss88CAJqamvCjH/0IJ510Ek488cSi7srHYjEkEokB30smk9izZ8+g1yaTyew297fva5PJJIBUIbLv98PhcPbrfP//Zgw3p+SBBx7A5z73OXziE5/AL37xC5x77rmIx+O4//77R9hyIqLqxonaREQe2rBhA1atWoXVq1cPumg9/fTTYds2vvCFL+DRRx/FihUrsitF9bd7924AwLhx40b9vG3btuGLX/wi5s6dix//+McDLrILtWfPnuzwogMOOAAAsqsh7fu+Y8aMKfpzyiXf/78Z/Sek99fd3Y2//OUv+NjHPobGxkacddZZeOSRR9Dd3V2u0ImIlMeigoioghzHgeu62a8jkQg++tGPDnjNc889B9u2MW/evLze87nnnsNVV12FOXPm4KabbkI0Gh3x9ZZloampacif7bfffgCQfVjf1q1bAQAzZ84c8LqTTz45r9gqLZ//v/n44x//iDFjxuBHP/oRGhsbcc8993gZJhGRdjj8iYioQpYuXYoLL7wQ3/3ud7FkyRI0NTXhoosuGjRcaOvWrVi8eDEWLlyIaDSavUu+//77Y8yYMbj11lsHvffy5cvxuc99Dj//+c/xi1/8Ap///OeHvbNeX1+PBx98EI899hheeOEFbNu2DbW1tZg7dy7mz5+P9evXZydat7e347nnnsOCBQuwd+9ebN26Fe9973txyimneP8/qET5/v/Nx6ZNm/DMM8/gX/7lX/DKK69gzZo1ZYiYiEgf7KkgIqqQF198EYsWLcLMmTNx44034sorr8Tjjz+OO+64Y9Brf/WrX+Gb3/wmJkyYgO985zv46U9/irPOOgvvvvvusO+/atUqLFy4EFOmTMGvfvWrYYcodXd349Zbb0VLSwuuvPJK/OIXv8CPfvQjvO9978Ndd92FSy+9dMDTv//f//t/ePHFF3H11Vfjhz/8IcaOHYuvf/3rpf7v8Fwh/3/z8eijjwIAeymIiPIg5syZM/SgUiIioir2ox/9CLNnz8aZZ54J27b9DoeIKNA4/ImIiCgtFAph1qxZOPzww3HKKafghhtuYEFBRJQHFhVERERpbW1tuOOOO9Dd3Y0lS5Zw6BMRUZ44/ImIiIiIiErCidpERERERFQSFhVERERERFQSFhVERERERFQSTtQexqxZs9De3u53GERERESkqNbWVrz55pt+h1ERLCqGMGvWLNx5551+h0FEREREivvUpz5VFYUFi4ohZHooPvWpT7G3goiIiIgK1tra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\n",
                         "text/plain": [
-                            "<Figure size 576x432 with 2 Axes>"
+                            "<Figure size 800x600 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
@@ -358,13 +262,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.6/docs/examples/04 Initial SoC.ipynb` & `liionpack-0.3.7/docs/examples/04 Initial SoC.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/06 Changing a model.ipynb` & `liionpack-0.3.7/docs/examples/06 Changing a model.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/07 Visualizing larger packs.ipynb` & `liionpack-0.3.7/docs/examples/07 Visualizing larger packs.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/08 SEI degradation model.ipynb` & `liionpack-0.3.7/docs/examples/08 SEI degradation model.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/docs/examples/09 Terminal locations.ipynb` & `liionpack-0.3.7/docs/examples/09 Terminal locations.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/basic_16p2s.py` & `liionpack-0.3.7/examples/basic_16p2s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/big_circuit.py` & `liionpack-0.3.7/examples/big_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/different_initial_soc.py` & `liionpack-0.3.7/examples/different_initial_soc.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/draw_circuit.py` & `liionpack-0.3.7/examples/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/draw_terminals.py` & `liionpack-0.3.7/examples/draw_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/drive_cycle.py` & `liionpack-0.3.7/examples/drive_cycle.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/drive_cycle_comparison.py` & `liionpack-0.3.7/examples/drive_cycle_comparison.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/load_4p1s.py` & `liionpack-0.3.7/examples/load_4p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/mixed_terminals.py` & `liionpack-0.3.7/examples/mixed_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/paper_example.py` & `liionpack-0.3.7/examples/paper_example.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/save_output.py` & `liionpack-0.3.7/examples/save_output.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/step_external_variable.py` & `liionpack-0.3.7/examples/step_external_variable.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/examples/thermal_external.py` & `liionpack-0.3.7/examples/thermal_external.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/__init__.py` & `liionpack-0.3.7/liionpack/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 from .definitions import MODULE_DIR
 from .definitions import CIRCUIT_DIR
 from .solvers import CasadiManager
 from .solvers import RayManager
 from .solvers import GenericActor
 from .solvers import RayActor
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

### Comparing `liionpack-0.3.6/liionpack/logger.py` & `liionpack-0.3.7/liionpack/logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/netlist_utils.py` & `liionpack-0.3.7/liionpack/netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/plots.py` & `liionpack-0.3.7/liionpack/plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/sim_utils.py` & `liionpack-0.3.7/liionpack/sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/simulations.py` & `liionpack-0.3.7/liionpack/simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/solver_utils.py` & `liionpack-0.3.7/liionpack/solver_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/solvers.py` & `liionpack-0.3.7/liionpack/solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/utils.py` & `liionpack-0.3.7/liionpack/utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/circuits/4p1s.asc` & `liionpack-0.3.7/liionpack/circuits/4p1s.asc`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/liionpack/circuits/4p1s.cir` & `liionpack-0.3.7/liionpack/circuits/4p1s.cir`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper.bib` & `liionpack-0.3.7/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper.md` & `liionpack-0.3.7/paper/paper.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper_figures/Figure_0.png` & `liionpack-0.3.7/paper/paper_figures/Figure_0.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper_figures/Figure_1.png` & `liionpack-0.3.7/paper/paper_figures/Figure_1.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper_figures/Figure_2.png` & `liionpack-0.3.7/paper/paper_figures/Figure_2.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/paper/paper_figures/Figure_3.png` & `liionpack-0.3.7/paper/paper_figures/Figure_3.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/integration/test_1p1s.py` & `liionpack-0.3.7/tests/integration/test_1p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/integration/test_all_solvers.py` & `liionpack-0.3.7/tests/integration/test_all_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_logger.py` & `liionpack-0.3.7/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_netlist_utils.py` & `liionpack-0.3.7/tests/unit/test_netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_notebooks.py` & `liionpack-0.3.7/tests/unit/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_plots.py` & `liionpack-0.3.7/tests/unit/test_plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_protocols.py` & `liionpack-0.3.7/tests/unit/test_protocols.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,15 @@
     def test_generate_protocol_from_drive_cycle(self):
         os.chdir(pybamm.__path__[0] + "/..")
         drive_cycle = pd.read_csv(
             "pybamm/input/drive_cycles/US06.csv", comment="#", header=None
         ).to_numpy()
 
         experiment = pybamm.Experiment(
-            operating_conditions=["Run US06 (A)"],
-            period="1 minute",
-            drive_cycles={"US06": drive_cycle},
+            [pybamm.step.current(drive_cycle)], period="1 second"
         )
         p = lp.generate_protocol_from_experiment(experiment)
         assert len(p) == 601
         assert np.allclose(np.mean(p), 0.8404807891846922)
 
     def test_time_exception(self):
         def bad_timing():
```

### Comparing `liionpack-0.3.6/tests/unit/test_sim_utils.py` & `liionpack-0.3.7/tests/unit/test_sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_simulations.py` & `liionpack-0.3.7/tests/unit/test_simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_solver_utils.py` & `liionpack-0.3.7/tests/unit/test_solver_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_solvers.py` & `liionpack-0.3.7/tests/unit/test_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/tests/unit/test_utils.py` & `liionpack-0.3.7/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/.gitignore` & `liionpack-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/LICENSE` & `liionpack-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/README.md` & `liionpack-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.6/pyproject.toml` & `liionpack-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "lcapy",
     "matplotlib",
     "networkx",
     "numpy",
     "openpyxl",
     "pandas",
     "plotly",
-    "pybamm>=23.3",
+    "pybamm>=23.5",
     "ray",
     "redis",
     "scikit-spatial",
     "scipy",
     "textwrapper",
     "tqdm",
     "nbconvert",
```

### Comparing `liionpack-0.3.6/PKG-INFO` & `liionpack-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liionpack
-Version: 0.3.6
+Version: 0.3.7
 Summary: A battery pack simulator for PyBaMM
 Project-URL: Bug Tracker, https://github.com/pybamm-team/liionpack/issues
 Project-URL: Changelog, https://github.com/pybamm-team/liionpack/blob/develop/CHANGELOG.md
 Project-URL: Documentation, https://liionpack.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/pybamm-team/liionpack
 Author-email: Tom Tranter <t.g.tranter@gmail.com>
 License-Expression: MIT
@@ -25,15 +25,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: plotly
-Requires-Dist: pybamm>=23.3
+Requires-Dist: pybamm>=23.5
 Requires-Dist: ray
 Requires-Dist: redis
 Requires-Dist: scikit-spatial
 Requires-Dist: scipy
 Requires-Dist: textwrapper
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
```

