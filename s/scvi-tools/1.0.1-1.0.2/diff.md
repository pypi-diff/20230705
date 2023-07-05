# Comparing `tmp/scvi_tools-1.0.1.tar.gz` & `tmp/scvi_tools-1.0.2.tar.gz`

## Comparing `scvi_tools-1.0.1.tar` & `scvi_tools-1.0.2.tar`

### file list

```diff
@@ -1,351 +1,351 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.editorconfig
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitattributes
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitmodules
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/codecov.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/readthedocs.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/setup.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/conf.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/index.md
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/installation.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/make.bat
--rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/references.bib
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/references.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/code-24px.svg
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/computer-24px.svg
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/library_books-24px.svg
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/logo.png
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/logo.svg
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/old_logo.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/play_circle_outline-24px.svg
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/scvi-tools-horizontal.svg
--rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/scvi_team.jpg
--rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks-01.png
--rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks.png
--rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tasks.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/css/override.css
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/ldvae.svg
--rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/overview.svg
--rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/scanvi_alt.svg
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_static/tutorials/totalvi_cell.svg
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/class_no_inherited.rst
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/layout.html
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/datasets.md
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/developer.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/index.md
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/api/user.md
--rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/contributing/index.md
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/extensions/edit_colab_url.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    78407 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/index.md
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/figures/anndata_manager_schematic.svg
--rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/release_notes/figures/setup_anndata_before_after.svg
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_atac.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_dev.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_hub.md
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_multimodal.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_quick_start.md
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_scrna.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_spatial.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/tutorials/index_tuning.md
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/codebase_overview.md
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/counterfactual_prediction.md
--rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/differential_expression.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/transfer_learning.md
--rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/variational_inference.md
--rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/codebase_overview.svg
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/fdr_control.png
--rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/background/figures/vi_projection.svg
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/amortizedlda.md
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/autozi.md
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/cellassign.md
--rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/destvi.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/gimvi.md
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/linearscvi.md
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/multivi.md
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/peakvi.md
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scanvi.md
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scar.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scbasset.md
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/scvi.md
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/solo.md
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/stereoscope.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/tangram.md
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/totalvi.md
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/fdr_control.png
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scLVM_graphical_model.svg
--rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scanvi_pgm.png
--rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stLVM_graphical_model.svg
--rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
--rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
--rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/docs/user_guide/models/figures/totalvi_graphical_model.svg
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_compat.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_constants.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_decorators.py
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_settings.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/_types.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_callbacks.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_defaults.py
--rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_manager.py
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_tuner.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_types.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/autotune/_utils.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/_constants.py
--rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/criticism/_ppc.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/__init__.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_anntorchdataset.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_constants.py
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_datasets.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_download.py
--rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_manager.py
--rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_preprocessing.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_read.py
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/__init__.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_brain_large.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cellxgene.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cite_seq.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_cortex.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_csv.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_dataset_10x.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_heartcellatlas.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_loom.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_pbmc.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_smfish.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/_built_in_data/_synthetic.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/__init__.py
--rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_arraylike_field.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_base_field.py
--rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_dataframe_field.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_layer_field.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_mudata.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_protein.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_scanvi.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/data/fields/_uns_field.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_ann_dataloader.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_concat_dataloader.py
--rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_data_splitting.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/dataloaders/_semi_dataloader.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/__init__.py
--rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/_negative_binomial.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/distributions/_utils.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/_model.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/cellassign/_module.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/__init__.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_model.py
--rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_module.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_task.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/gimvi/_utils.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/__init__.py
--rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/_model.py
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scar/_module.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/__init__.py
--rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/_model.py
--rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/scbasset/_module.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/solo/__init__.py
--rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/solo/_model.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/__init__.py
--rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/_model.py
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/stereoscope/_module.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/__init__.py
--rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/_model.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/external/tangram/_module.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/_constants.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/_url.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/hub_metadata.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/hub_model.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/hub/model_card_template.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_amortizedlda.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_autozi.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_condscvi.py
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_destvi.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_jaxscvi.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_linear_scvi.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_metrics.py
--rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_multivi.py
--rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_peakvi.py
--rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_scanvi.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_scvi.py
--rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_totalvi.py
--rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/_utils.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/__init__.py
--rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_archesmixin.py
--rw-r--r--   0        0        0    33943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_base_model.py
--rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_differential.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_jaxmixin.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_log_likelihood.py
--rwxr-xr-x   0        0        0    20650 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_pyromixin.py
--rw-r--r--   0        0        0    29147 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_rnamixin.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_training_mixin.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_utils.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/base/_vaemixin.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/_mde.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/model/utils/_minification.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/__init__.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_amortizedlda.py
--rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_autozivae.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_classifier.py
--rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_jaxvae.py
--rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_mrdeconv.py
--rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_multivae.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_peakvae.py
--rw-r--r--   0        0        0    13210 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_scanvae.py
--rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_totalvae.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_utils.py
--rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_vae.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/_vaec.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/__init__.py
--rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_base_module.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_decorators.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/module/base/_pyro.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/__init__.py
--rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/_base_components.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/nn/_utils.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/__init__.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_callbacks.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_logger.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_metrics.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_progress.py
--rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainer.py
--rw-r--r--   0        0        0    51888 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainingplans.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/train/_trainrunner.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_attrdict.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_decorators.py
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_docstrings.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_exceptions.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_jax.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/scvi/utils/_track.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_defaults.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_manager.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_tuner.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_types.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/autotune/test_utils.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/core/test_differential.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/core/test_distributions.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/criticism/test_criticism.py
--rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Cortex.loom
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
--rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Layer2_BC_count_matrix-1.tsv
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/Rep11_MOB_count_matrix-1.tsv
--rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/SeqFISH.xlsx
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/TM_droplet_mat.h5ad
--rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brain_large.h5
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brain_small_metadata.pickle
--rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/brainlarge_dataset_test.h5ad
--rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/expression.bin
--rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/fc-dropseq.loom
--rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/immune_control_expression_matrix.txt
--rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/immune_stimulated_expression_matrix.txt
--rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/mpfc-starmap.loom
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/osmFISH_SScortex_mouse_all_cell.loom
--rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/pbmc_10k_protein_v3.h5ad
--rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/pbmc_5k_protein_v3.h5ad
--rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/random_metadata.pickle
--rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/retina.loom
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus.zip
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/gene_info_pbmc.csv
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc_metadata.pickle
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/bBM.spring_and_pba.csv
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/HEMATO/data.zip
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/seqfishplus/sourcedata/ob_counts.csv
--rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_1.loom
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_2.loom
--rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/simulation/simulation_3.loom
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa.fai
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.fa.sizes
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/data/test_genome/test_genome.gaps.bed
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataloaders/test_dataloaders.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataloaders/test_datasplitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/conftest.py
--rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_anndata.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_built_in_data.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_dataset10X.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_mudata.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/test_preprocessing.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/dataset/utils.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_cellassign.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_gimvi.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_scar.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_scbasset.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_solo.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_stereoscope.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/external/test_tangram.py
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_hub_metadata.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_hub_model.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/hub/test_url.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/model/base/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_lightning.py
--rw-r--r--   0        0        0    57068 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_models.py
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_models_with_minified_data.py
--rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_mudata_models.py
--rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_pyro.py
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/models/test_scarches.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/notebooks/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/train/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/tests/train/test_trainingplans.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/.gitignore
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/LICENSE
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/README.md
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 scvi_tools-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.editorconfig
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.gitattributes
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.gitmodules
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/codecov.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/readthedocs.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/setup.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/index.md
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/installation.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/references.bib
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/references.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/code-24px.svg
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/computer-24px.svg
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/library_books-24px.svg
+-rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/logo.png
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/old_logo.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/scvi-tools-horizontal.svg
+-rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/scvi_team.jpg
+-rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tasks-01.png
+-rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tasks.png
+-rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tasks.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/css/override.css
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tutorials/ldvae.svg
+-rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tutorials/overview.svg
+-rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tutorials/scanvi_alt.svg
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_static/tutorials/totalvi_cell.svg
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_templates/class_no_inherited.rst
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_templates/layout.html
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/api/datasets.md
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/api/developer.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/api/index.md
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/api/user.md
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/contributing/index.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/extensions/edit_colab_url.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    78586 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/release_notes/index.md
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/release_notes/figures/anndata_manager_schematic.svg
+-rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/release_notes/figures/setup_anndata_before_after.svg
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_atac.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_dev.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_hub.md
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_multimodal.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_quick_start.md
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_scrna.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_spatial.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/tutorials/index_tuning.md
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/codebase_overview.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/counterfactual_prediction.md
+-rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/differential_expression.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/transfer_learning.md
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/variational_inference.md
+-rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/figures/codebase_overview.svg
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/figures/fdr_control.png
+-rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/background/figures/vi_projection.svg
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/amortizedlda.md
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/autozi.md
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/cellassign.md
+-rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/destvi.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/gimvi.md
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/linearscvi.md
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/multivi.md
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/peakvi.md
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/scanvi.md
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/scar.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/scbasset.md
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/scvi.md
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/solo.md
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/stereoscope.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/tangram.md
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/totalvi.md
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/fdr_control.png
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/scLVM_graphical_model.svg
+-rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/scanvi_pgm.png
+-rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
+-rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
+-rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/docs/user_guide/models/figures/totalvi_graphical_model.svg
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/_compat.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/_constants.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/_decorators.py
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/_settings.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/_types.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_callbacks.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_defaults.py
+-rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_manager.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_tuner.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_types.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/autotune/_utils.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/criticism/__init__.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/criticism/_constants.py
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/criticism/_ppc.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/__init__.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_anntorchdataset.py
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_compat.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_constants.py
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_datasets.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_download.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_manager.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_preprocessing.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_read.py
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/__init__.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_brain_large.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_cellxgene.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_cite_seq.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_cortex.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_csv.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_dataset_10x.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_heartcellatlas.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_loom.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_pbmc.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_smfish.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/_built_in_data/_synthetic.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/__init__.py
+-rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_arraylike_field.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_base_field.py
+-rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_dataframe_field.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_layer_field.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_mudata.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_protein.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_scanvi.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/data/fields/_uns_field.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/dataloaders/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/dataloaders/_ann_dataloader.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/dataloaders/_concat_dataloader.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/dataloaders/_data_splitting.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/dataloaders/_semi_dataloader.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/distributions/__init__.py
+-rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/distributions/_negative_binomial.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/distributions/_utils.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/cellassign/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/cellassign/_model.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/cellassign/_module.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/gimvi/__init__.py
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/gimvi/_model.py
+-rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/gimvi/_module.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/gimvi/_task.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/gimvi/_utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scar/__init__.py
+-rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scar/_model.py
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scar/_module.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scbasset/__init__.py
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scbasset/_model.py
+-rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/scbasset/_module.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/solo/__init__.py
+-rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/solo/_model.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/stereoscope/__init__.py
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/stereoscope/_model.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/stereoscope/_module.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/tangram/__init__.py
+-rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/tangram/_model.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/external/tangram/_module.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/_constants.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/_url.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/hub_metadata.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/hub_model.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/hub/model_card_template.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/__init__.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_amortizedlda.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_autozi.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_condscvi.py
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_destvi.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_jaxscvi.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_linear_scvi.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_metrics.py
+-rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_multivi.py
+-rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_peakvi.py
+-rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_scanvi.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_scvi.py
+-rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_totalvi.py
+-rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/_utils.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/__init__.py
+-rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_archesmixin.py
+-rw-r--r--   0        0        0    33943 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_base_model.py
+-rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_differential.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_jaxmixin.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_log_likelihood.py
+-rwxr-xr-x   0        0        0    20650 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_pyromixin.py
+-rw-r--r--   0        0        0    29147 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_rnamixin.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_training_mixin.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_utils.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/base/_vaemixin.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/utils/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/utils/_mde.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/model/utils/_minification.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/__init__.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_amortizedlda.py
+-rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_autozivae.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_classifier.py
+-rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_jaxvae.py
+-rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_mrdeconv.py
+-rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_multivae.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_peakvae.py
+-rw-r--r--   0        0        0    13210 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_scanvae.py
+-rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_totalvae.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_utils.py
+-rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_vae.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/_vaec.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/base/__init__.py
+-rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/base/_base_module.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/base/_decorators.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/module/base/_pyro.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/nn/__init__.py
+-rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/nn/_base_components.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/nn/_utils.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/__init__.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_callbacks.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_logger.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_metrics.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_progress.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_trainer.py
+-rw-r--r--   0        0        0    51888 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_trainingplans.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/train/_trainrunner.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_attrdict.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_decorators.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_docstrings.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_exceptions.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_jax.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/scvi/utils/_track.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/autotune/test_defaults.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/autotune/test_manager.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/autotune/test_tuner.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/autotune/test_types.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/autotune/test_utils.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/core/test_differential.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/core/test_distributions.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/criticism/test_criticism.py
+-rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/Cortex.loom
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
+-rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/Layer2_BC_count_matrix-1.tsv
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/Rep11_MOB_count_matrix-1.tsv
+-rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/SeqFISH.xlsx
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/TM_droplet_mat.h5ad
+-rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/brain_large.h5
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/brain_small_metadata.pickle
+-rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/brainlarge_dataset_test.h5ad
+-rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/expression.bin
+-rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/fc-dropseq.loom
+-rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/immune_control_expression_matrix.txt
+-rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/immune_stimulated_expression_matrix.txt
+-rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/mpfc-starmap.loom
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/osmFISH_SScortex_mouse_all_cell.loom
+-rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/pbmc_10k_protein_v3.h5ad
+-rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/pbmc_5k_protein_v3.h5ad
+-rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/random_metadata.pickle
+-rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/retina.loom
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/seqfishplus.zip
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/gene_info_pbmc.csv
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/pbmc_metadata.pickle
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/HEMATO/bBM.spring_and_pba.csv
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/HEMATO/data.zip
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/seqfishplus/sourcedata/ob_counts.csv
+-rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/simulation/simulation_1.loom
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/simulation/simulation_2.loom
+-rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/simulation/simulation_3.loom
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/test_genome/test_genome.fa
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/test_genome/test_genome.fa.fai
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/test_genome/test_genome.fa.sizes
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/data/test_genome/test_genome.gaps.bed
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataloaders/test_dataloaders.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataloaders/test_datasplitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/conftest.py
+-rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/test_anndata.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/test_built_in_data.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/test_dataset10X.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/test_mudata.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/test_preprocessing.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/dataset/utils.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_cellassign.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_gimvi.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_scar.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_scbasset.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_solo.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_stereoscope.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/external/test_tangram.py
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/hub/test_hub_metadata.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/hub/test_hub_model.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/hub/test_url.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/model/base/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_lightning.py
+-rw-r--r--   0        0        0    57068 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_models.py
+-rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_models_with_minified_data.py
+-rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_mudata_models.py
+-rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_pyro.py
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/models/test_scarches.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/notebooks/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/train/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/tests/train/test_trainingplans.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/README.md
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 scvi_tools-1.0.2/PKG-INFO
```

### Comparing `scvi_tools-1.0.1/.pre-commit-config.yaml` & `scvi_tools-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/CODE_OF_CONDUCT.md` & `scvi_tools-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/.devcontainer/devcontainer.json` & `scvi_tools-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/.github/workflows/build.yml` & `scvi_tools-1.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/.github/workflows/release.yml` & `scvi_tools-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/.github/workflows/test.yml` & `scvi_tools-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/Makefile` & `scvi_tools-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/conf.py` & `scvi_tools-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/index.md` & `scvi_tools-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/installation.md` & `scvi_tools-1.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/make.bat` & `scvi_tools-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/references.bib` & `scvi_tools-1.0.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/logo.png` & `scvi_tools-1.0.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/logo.svg` & `scvi_tools-1.0.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/old_logo.png` & `scvi_tools-1.0.2/docs/_static/old_logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/scvi-tools-horizontal.svg` & `scvi_tools-1.0.2/docs/_static/scvi-tools-horizontal.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/scvi_team.jpg` & `scvi_tools-1.0.2/docs/_static/scvi_team.jpg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tasks-01.png` & `scvi_tools-1.0.2/docs/_static/tasks-01.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tasks.png` & `scvi_tools-1.0.2/docs/_static/tasks.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tasks.svg` & `scvi_tools-1.0.2/docs/_static/tasks.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tutorials/ldvae.svg` & `scvi_tools-1.0.2/docs/_static/tutorials/ldvae.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tutorials/overview.svg` & `scvi_tools-1.0.2/docs/_static/tutorials/overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tutorials/scanvi_alt.svg` & `scvi_tools-1.0.2/docs/_static/tutorials/scanvi_alt.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_static/tutorials/totalvi_cell.svg` & `scvi_tools-1.0.2/docs/_static/tutorials/totalvi_cell.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_templates/class_no_inherited.rst` & `scvi_tools-1.0.2/docs/_templates/class_no_inherited.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_templates/layout.html` & `scvi_tools-1.0.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/_templates/autosummary/class.rst` & `scvi_tools-1.0.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/api/datasets.md` & `scvi_tools-1.0.2/docs/api/datasets.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/api/developer.md` & `scvi_tools-1.0.2/docs/api/developer.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/api/user.md` & `scvi_tools-1.0.2/docs/api/user.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/contributing/index.md` & `scvi_tools-1.0.2/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/extensions/edit_colab_url.py` & `scvi_tools-1.0.2/docs/extensions/edit_colab_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/extensions/typed_returns.py` & `scvi_tools-1.0.2/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/release_notes/index.md` & `scvi_tools-1.0.2/docs/release_notes/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
 #### Removed
 
 -   Remove deprecated `use_gpu` in favor of PyTorch Lightning arguments `accelerator` and `devices` {pr}`xxxx`.
 
 ## Version 1.0
 
+### 1.0.2 (2023-07-05)
+
+### Fixed
+
+-   Fix link to Scanpy preprocessing in introduction tutorial {pr}`2154`.
+-   Fix link to Ray Tune search API in autotune tutorial {pr}`2154`.
+
 ### 1.0.1 (2023-07-04)
 
 #### Added
 
 -   Add support for Python 3.11 {pr}`1977`.
 
 #### Changed
```

### Comparing `scvi_tools-1.0.1/docs/release_notes/figures/anndata_manager_schematic.svg` & `scvi_tools-1.0.2/docs/release_notes/figures/anndata_manager_schematic.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/release_notes/figures/setup_anndata_before_after.svg` & `scvi_tools-1.0.2/docs/release_notes/figures/setup_anndata_before_after.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/tutorials/index.md` & `scvi_tools-1.0.2/docs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/tutorials/index_dev.md` & `scvi_tools-1.0.2/docs/tutorials/index_dev.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/index.md` & `scvi_tools-1.0.2/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/differential_expression.md` & `scvi_tools-1.0.2/docs/user_guide/background/differential_expression.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/transfer_learning.md` & `scvi_tools-1.0.2/docs/user_guide/background/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/variational_inference.md` & `scvi_tools-1.0.2/docs/user_guide/background/variational_inference.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/figures/codebase_overview.svg` & `scvi_tools-1.0.2/docs/user_guide/background/figures/codebase_overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/figures/fdr_control.png` & `scvi_tools-1.0.2/docs/user_guide/background/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/background/figures/vi_projection.svg` & `scvi_tools-1.0.2/docs/user_guide/background/figures/vi_projection.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/amortizedlda.md` & `scvi_tools-1.0.2/docs/user_guide/models/amortizedlda.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/autozi.md` & `scvi_tools-1.0.2/docs/user_guide/models/autozi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/cellassign.md` & `scvi_tools-1.0.2/docs/user_guide/models/cellassign.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/destvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/destvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/linearscvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/linearscvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/multivi.md` & `scvi_tools-1.0.2/docs/user_guide/models/multivi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/peakvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/peakvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/scanvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/scanvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/scar.md` & `scvi_tools-1.0.2/docs/user_guide/models/scar.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/scbasset.md` & `scvi_tools-1.0.2/docs/user_guide/models/scbasset.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/scvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/scvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/solo.md` & `scvi_tools-1.0.2/docs/user_guide/models/solo.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/stereoscope.md` & `scvi_tools-1.0.2/docs/user_guide/models/stereoscope.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/tangram.md` & `scvi_tools-1.0.2/docs/user_guide/models/tangram.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/totalvi.md` & `scvi_tools-1.0.2/docs/user_guide/models/totalvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/fdr_control.png` & `scvi_tools-1.0.2/docs/user_guide/models/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/scLVM_graphical_model.svg` & `scvi_tools-1.0.2/docs/user_guide/models/figures/scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/scanvi_pgm.png` & `scvi_tools-1.0.2/docs/user_guide/models/figures/scanvi_pgm.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/scvi_annotated_graphical_model.png` & `scvi_tools-1.0.2/docs/user_guide/models/figures/scvi_annotated_graphical_model.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/stLVM_graphical_model.svg` & `scvi_tools-1.0.2/docs/user_guide/models/figures/stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg` & `scvi_tools-1.0.2/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg` & `scvi_tools-1.0.2/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/docs/user_guide/models/figures/totalvi_graphical_model.svg` & `scvi_tools-1.0.2/docs/user_guide/models/figures/totalvi_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/__init__.py` & `scvi_tools-1.0.2/scvi/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/_constants.py` & `scvi_tools-1.0.2/scvi/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/_decorators.py` & `scvi_tools-1.0.2/scvi/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/_settings.py` & `scvi_tools-1.0.2/scvi/_settings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_callbacks.py` & `scvi_tools-1.0.2/scvi/autotune/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_defaults.py` & `scvi_tools-1.0.2/scvi/autotune/_defaults.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_manager.py` & `scvi_tools-1.0.2/scvi/autotune/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_tuner.py` & `scvi_tools-1.0.2/scvi/autotune/_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_types.py` & `scvi_tools-1.0.2/scvi/autotune/_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/autotune/_utils.py` & `scvi_tools-1.0.2/scvi/autotune/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/criticism/_ppc.py` & `scvi_tools-1.0.2/scvi/criticism/_ppc.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/__init__.py` & `scvi_tools-1.0.2/scvi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_anntorchdataset.py` & `scvi_tools-1.0.2/scvi/data/_anntorchdataset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_compat.py` & `scvi_tools-1.0.2/scvi/data/_compat.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_constants.py` & `scvi_tools-1.0.2/scvi/data/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_datasets.py` & `scvi_tools-1.0.2/scvi/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_download.py` & `scvi_tools-1.0.2/scvi/data/_download.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_manager.py` & `scvi_tools-1.0.2/scvi/data/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_preprocessing.py` & `scvi_tools-1.0.2/scvi/data/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_read.py` & `scvi_tools-1.0.2/scvi/data/_read.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_utils.py` & `scvi_tools-1.0.2/scvi/data/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_brain_large.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_brain_large.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_cellxgene.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_cellxgene.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_cite_seq.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_cite_seq.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_cortex.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_cortex.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_csv.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_csv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_dataset_10x.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_dataset_10x.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_heartcellatlas.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_heartcellatlas.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_loom.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_loom.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_pbmc.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_pbmc.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_smfish.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_smfish.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/_built_in_data/_synthetic.py` & `scvi_tools-1.0.2/scvi/data/_built_in_data/_synthetic.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/__init__.py` & `scvi_tools-1.0.2/scvi/data/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_arraylike_field.py` & `scvi_tools-1.0.2/scvi/data/fields/_arraylike_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_base_field.py` & `scvi_tools-1.0.2/scvi/data/fields/_base_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_dataframe_field.py` & `scvi_tools-1.0.2/scvi/data/fields/_dataframe_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_layer_field.py` & `scvi_tools-1.0.2/scvi/data/fields/_layer_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_mudata.py` & `scvi_tools-1.0.2/scvi/data/fields/_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_protein.py` & `scvi_tools-1.0.2/scvi/data/fields/_protein.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_scanvi.py` & `scvi_tools-1.0.2/scvi/data/fields/_scanvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/data/fields/_uns_field.py` & `scvi_tools-1.0.2/scvi/data/fields/_uns_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/dataloaders/__init__.py` & `scvi_tools-1.0.2/scvi/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/dataloaders/_ann_dataloader.py` & `scvi_tools-1.0.2/scvi/dataloaders/_ann_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/dataloaders/_concat_dataloader.py` & `scvi_tools-1.0.2/scvi/dataloaders/_concat_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/dataloaders/_data_splitting.py` & `scvi_tools-1.0.2/scvi/dataloaders/_data_splitting.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/dataloaders/_semi_dataloader.py` & `scvi_tools-1.0.2/scvi/dataloaders/_semi_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/distributions/_negative_binomial.py` & `scvi_tools-1.0.2/scvi/distributions/_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/distributions/_utils.py` & `scvi_tools-1.0.2/scvi/distributions/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/cellassign/_model.py` & `scvi_tools-1.0.2/scvi/external/cellassign/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/cellassign/_module.py` & `scvi_tools-1.0.2/scvi/external/cellassign/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/gimvi/_model.py` & `scvi_tools-1.0.2/scvi/external/gimvi/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/gimvi/_module.py` & `scvi_tools-1.0.2/scvi/external/gimvi/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/gimvi/_task.py` & `scvi_tools-1.0.2/scvi/external/gimvi/_task.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/gimvi/_utils.py` & `scvi_tools-1.0.2/scvi/external/gimvi/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/scar/_model.py` & `scvi_tools-1.0.2/scvi/external/scar/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/scar/_module.py` & `scvi_tools-1.0.2/scvi/external/scar/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/scbasset/_model.py` & `scvi_tools-1.0.2/scvi/external/scbasset/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/scbasset/_module.py` & `scvi_tools-1.0.2/scvi/external/scbasset/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/solo/_model.py` & `scvi_tools-1.0.2/scvi/external/solo/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/stereoscope/_model.py` & `scvi_tools-1.0.2/scvi/external/stereoscope/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/stereoscope/_module.py` & `scvi_tools-1.0.2/scvi/external/stereoscope/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/tangram/_model.py` & `scvi_tools-1.0.2/scvi/external/tangram/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/external/tangram/_module.py` & `scvi_tools-1.0.2/scvi/external/tangram/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/hub/_constants.py` & `scvi_tools-1.0.2/scvi/hub/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/hub/_url.py` & `scvi_tools-1.0.2/scvi/hub/_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/hub/hub_metadata.py` & `scvi_tools-1.0.2/scvi/hub/hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/hub/hub_model.py` & `scvi_tools-1.0.2/scvi/hub/hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/hub/model_card_template.py` & `scvi_tools-1.0.2/scvi/hub/model_card_template.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/__init__.py` & `scvi_tools-1.0.2/scvi/model/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_amortizedlda.py` & `scvi_tools-1.0.2/scvi/model/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_autozi.py` & `scvi_tools-1.0.2/scvi/model/_autozi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_condscvi.py` & `scvi_tools-1.0.2/scvi/model/_condscvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_destvi.py` & `scvi_tools-1.0.2/scvi/model/_destvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_jaxscvi.py` & `scvi_tools-1.0.2/scvi/model/_jaxscvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_linear_scvi.py` & `scvi_tools-1.0.2/scvi/model/_linear_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_metrics.py` & `scvi_tools-1.0.2/scvi/model/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_multivi.py` & `scvi_tools-1.0.2/scvi/model/_multivi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_peakvi.py` & `scvi_tools-1.0.2/scvi/model/_peakvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_scanvi.py` & `scvi_tools-1.0.2/scvi/model/_scanvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_scvi.py` & `scvi_tools-1.0.2/scvi/model/_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_totalvi.py` & `scvi_tools-1.0.2/scvi/model/_totalvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/_utils.py` & `scvi_tools-1.0.2/scvi/model/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/__init__.py` & `scvi_tools-1.0.2/scvi/model/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_archesmixin.py` & `scvi_tools-1.0.2/scvi/model/base/_archesmixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_base_model.py` & `scvi_tools-1.0.2/scvi/model/base/_base_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_differential.py` & `scvi_tools-1.0.2/scvi/model/base/_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_jaxmixin.py` & `scvi_tools-1.0.2/scvi/model/base/_jaxmixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_log_likelihood.py` & `scvi_tools-1.0.2/scvi/model/base/_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_pyromixin.py` & `scvi_tools-1.0.2/scvi/model/base/_pyromixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_rnamixin.py` & `scvi_tools-1.0.2/scvi/model/base/_rnamixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_training_mixin.py` & `scvi_tools-1.0.2/scvi/model/base/_training_mixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_utils.py` & `scvi_tools-1.0.2/scvi/model/base/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/base/_vaemixin.py` & `scvi_tools-1.0.2/scvi/model/base/_vaemixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/utils/_mde.py` & `scvi_tools-1.0.2/scvi/model/utils/_mde.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/model/utils/_minification.py` & `scvi_tools-1.0.2/scvi/model/utils/_minification.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/__init__.py` & `scvi_tools-1.0.2/scvi/module/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_amortizedlda.py` & `scvi_tools-1.0.2/scvi/module/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_autozivae.py` & `scvi_tools-1.0.2/scvi/module/_autozivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_classifier.py` & `scvi_tools-1.0.2/scvi/module/_classifier.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_jaxvae.py` & `scvi_tools-1.0.2/scvi/module/_jaxvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_mrdeconv.py` & `scvi_tools-1.0.2/scvi/module/_mrdeconv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_multivae.py` & `scvi_tools-1.0.2/scvi/module/_multivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_peakvae.py` & `scvi_tools-1.0.2/scvi/module/_peakvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_scanvae.py` & `scvi_tools-1.0.2/scvi/module/_scanvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_totalvae.py` & `scvi_tools-1.0.2/scvi/module/_totalvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_utils.py` & `scvi_tools-1.0.2/scvi/module/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_vae.py` & `scvi_tools-1.0.2/scvi/module/_vae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/_vaec.py` & `scvi_tools-1.0.2/scvi/module/_vaec.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/base/_base_module.py` & `scvi_tools-1.0.2/scvi/module/base/_base_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/module/base/_decorators.py` & `scvi_tools-1.0.2/scvi/module/base/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/nn/_base_components.py` & `scvi_tools-1.0.2/scvi/nn/_base_components.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/__init__.py` & `scvi_tools-1.0.2/scvi/train/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_callbacks.py` & `scvi_tools-1.0.2/scvi/train/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_logger.py` & `scvi_tools-1.0.2/scvi/train/_logger.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_metrics.py` & `scvi_tools-1.0.2/scvi/train/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_progress.py` & `scvi_tools-1.0.2/scvi/train/_progress.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_trainer.py` & `scvi_tools-1.0.2/scvi/train/_trainer.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_trainingplans.py` & `scvi_tools-1.0.2/scvi/train/_trainingplans.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/train/_trainrunner.py` & `scvi_tools-1.0.2/scvi/train/_trainrunner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/utils/_decorators.py` & `scvi_tools-1.0.2/scvi/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/utils/_docstrings.py` & `scvi_tools-1.0.2/scvi/utils/_docstrings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/utils/_exceptions.py` & `scvi_tools-1.0.2/scvi/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/scvi/utils/_track.py` & `scvi_tools-1.0.2/scvi/utils/_track.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/conftest.py` & `scvi_tools-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/autotune/test_manager.py` & `scvi_tools-1.0.2/tests/autotune/test_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/autotune/test_tuner.py` & `scvi_tools-1.0.2/tests/autotune/test_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/autotune/test_types.py` & `scvi_tools-1.0.2/tests/autotune/test_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/core/test_differential.py` & `scvi_tools-1.0.2/tests/core/test_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/core/test_distributions.py` & `scvi_tools-1.0.2/tests/core/test_distributions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/criticism/test_criticism.py` & `scvi_tools-1.0.2/tests/criticism/test_criticism.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/Cortex.loom` & `scvi_tools-1.0.2/tests/data/Cortex.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz` & `scvi_tools-1.0.2/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/Layer2_BC_count_matrix-1.tsv` & `scvi_tools-1.0.2/tests/data/Layer2_BC_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/Rep11_MOB_count_matrix-1.tsv` & `scvi_tools-1.0.2/tests/data/Rep11_MOB_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/SeqFISH.xlsx` & `scvi_tools-1.0.2/tests/data/SeqFISH.xlsx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/TM_droplet_mat.h5ad` & `scvi_tools-1.0.2/tests/data/TM_droplet_mat.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/brain_large.h5` & `scvi_tools-1.0.2/tests/data/brain_large.h5`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/brain_small_metadata.pickle` & `scvi_tools-1.0.2/tests/data/brain_small_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/brainlarge_dataset_test.h5ad` & `scvi_tools-1.0.2/tests/data/brainlarge_dataset_test.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/expression.bin` & `scvi_tools-1.0.2/tests/data/expression.bin`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/fc-dropseq.loom` & `scvi_tools-1.0.2/tests/data/fc-dropseq.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/immune_control_expression_matrix.txt` & `scvi_tools-1.0.2/tests/data/immune_control_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/immune_stimulated_expression_matrix.txt` & `scvi_tools-1.0.2/tests/data/immune_stimulated_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/mpfc-starmap.loom` & `scvi_tools-1.0.2/tests/data/mpfc-starmap.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/osmFISH_SScortex_mouse_all_cell.loom` & `scvi_tools-1.0.2/tests/data/osmFISH_SScortex_mouse_all_cell.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/pbmc_10k_protein_v3.h5ad` & `scvi_tools-1.0.2/tests/data/pbmc_10k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/pbmc_5k_protein_v3.h5ad` & `scvi_tools-1.0.2/tests/data/pbmc_5k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/random_metadata.pickle` & `scvi_tools-1.0.2/tests/data/random_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/retina.loom` & `scvi_tools-1.0.2/tests/data/retina.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/seqfishplus.zip` & `scvi_tools-1.0.2/tests/data/seqfishplus.zip`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/gene_info_pbmc.csv` & `scvi_tools-1.0.2/tests/data/10X/gene_info_pbmc.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/pbmc_metadata.pickle` & `scvi_tools-1.0.2/tests/data/10X/pbmc_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv` & `scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx` & `scvi_tools-1.0.2/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.2/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz` & `scvi_tools-1.0.2/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/HEMATO/bBM.spring_and_pba.csv` & `scvi_tools-1.0.2/tests/data/HEMATO/bBM.spring_and_pba.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz` & `scvi_tools-1.0.2/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz` & `scvi_tools-1.0.2/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv` & `scvi_tools-1.0.2/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx` & `scvi_tools-1.0.2/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/simulation/simulation_1.loom` & `scvi_tools-1.0.2/tests/data/simulation/simulation_1.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/simulation/simulation_2.loom` & `scvi_tools-1.0.2/tests/data/simulation/simulation_2.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/data/simulation/simulation_3.loom` & `scvi_tools-1.0.2/tests/data/simulation/simulation_3.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataloaders/test_dataloaders.py` & `scvi_tools-1.0.2/tests/dataloaders/test_dataloaders.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataloaders/test_datasplitter.py` & `scvi_tools-1.0.2/tests/dataloaders/test_datasplitter.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/conftest.py` & `scvi_tools-1.0.2/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/test_anndata.py` & `scvi_tools-1.0.2/tests/dataset/test_anndata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/test_built_in_data.py` & `scvi_tools-1.0.2/tests/dataset/test_built_in_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/test_dataset10X.py` & `scvi_tools-1.0.2/tests/dataset/test_dataset10X.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/test_mudata.py` & `scvi_tools-1.0.2/tests/dataset/test_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/test_preprocessing.py` & `scvi_tools-1.0.2/tests/dataset/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/dataset/utils.py` & `scvi_tools-1.0.2/tests/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_cellassign.py` & `scvi_tools-1.0.2/tests/external/test_cellassign.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_gimvi.py` & `scvi_tools-1.0.2/tests/external/test_gimvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_scar.py` & `scvi_tools-1.0.2/tests/external/test_scar.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_scbasset.py` & `scvi_tools-1.0.2/tests/external/test_scbasset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_solo.py` & `scvi_tools-1.0.2/tests/external/test_solo.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_stereoscope.py` & `scvi_tools-1.0.2/tests/external/test_stereoscope.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/external/test_tangram.py` & `scvi_tools-1.0.2/tests/external/test_tangram.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/hub/test_hub_metadata.py` & `scvi_tools-1.0.2/tests/hub/test_hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/hub/test_hub_model.py` & `scvi_tools-1.0.2/tests/hub/test_hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/model/base/test_base_model.py` & `scvi_tools-1.0.2/tests/model/base/test_base_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_lightning.py` & `scvi_tools-1.0.2/tests/models/test_lightning.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_models.py` & `scvi_tools-1.0.2/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_models_with_minified_data.py` & `scvi_tools-1.0.2/tests/models/test_models_with_minified_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_mudata_models.py` & `scvi_tools-1.0.2/tests/models/test_mudata_models.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_pyro.py` & `scvi_tools-1.0.2/tests/models/test_pyro.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/models/test_scarches.py` & `scvi_tools-1.0.2/tests/models/test_scarches.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/tests/train/test_trainingplans.py` & `scvi_tools-1.0.2/tests/train/test_trainingplans.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/.gitignore` & `scvi_tools-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/LICENSE` & `scvi_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/README.md` & `scvi_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.1/pyproject.toml` & `scvi_tools-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 
 [project]
 name = "scvi-tools"
-version = "1.0.1"
+version = "1.0.2"
 description = "Deep probabilistic analysis of single-cell omics data."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "The scvi-tools development team"},
 ]
```

### Comparing `scvi_tools-1.0.1/PKG-INFO` & `scvi_tools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scvi-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Deep probabilistic analysis of single-cell omics data.
 Project-URL: Documentation, https://scvi-tools.org
 Project-URL: Source, https://github.com/scverse/scvi-tools
 Project-URL: Home-page, https://scvi-tools.org
 Author: The scvi-tools development team
 Maintainer-email: The scvi-tools development team <adamgayoso@berkeley.edu>
 License: BSD 3-Clause License
```

