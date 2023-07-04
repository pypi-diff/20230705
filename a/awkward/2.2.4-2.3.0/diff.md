# Comparing `tmp/awkward-2.2.4.tar.gz` & `tmp/awkward-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jun 15 15:47:29 2023, max compression
+gzip compressed data, last modified: Tue Jul  4 08:50:40 2023, max compression
```

## Comparing `awkward-2.2.4.tar` & `awkward-2.3.0.tar`

### file list

```diff
@@ -1,865 +1,874 @@
--rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.4/CITATION.cff
--rw-r--r--   0        0        0    13855 2023-06-15 15:47:29.000000 awkward-2.2.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-06-15 15:47:29.000000 awkward-2.2.4/README.md
--rw-r--r--   0        0        0      241 2023-06-15 15:47:29.000000 awkward-2.2.4/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/conf.py
--rw-r--r--   0        0        0      346 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/index.md
--rw-r--r--   0        0        0    11642 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/redirects.json
--rw-r--r--   0        0        0       22 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/requirements-wasm.txt
--rw-r--r--   0        0        0      574 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/requirements.txt
--rw-r--r--   0        0        0      460 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24165 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/ak.behavior.md
--rw-r--r--   0        0        0     1426 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/index.md
--rw-r--r--   0        0        0     7349 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1325 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/__init__.py
--rw-r--r--   0        0        0     4626 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_behavior.py
--rw-r--r--   0        0        0    38827 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0     2221 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_dispatch.py
--rw-r--r--   0        0        0    13672 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_do.py
--rw-r--r--   0        0        0    14536 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_errors.py
--rw-r--r--   0        0        0     5727 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5860 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_lookup.py
--rw-r--r--   0        0        0     8456 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_operators.py
--rw-r--r--   0        0        0     5454 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    28974 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_reducers.py
--rw-r--r--   0        0        0     1492 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_typing.py
--rw-r--r--   0        0        0     2263 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forth.py
--rw-r--r--   0        0        0   102730 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8044 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/jax.py
--rw-r--r--   0        0        0     6052 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/numba.py
--rw-r--r--   0        0        0     8272 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/record.py
--rw-r--r--   0        0        0     1679 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     2082 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3763 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1425 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53532 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4491 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    11582 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    38024 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      806 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0      789 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0    11085 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35828 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31510 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49133 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1111 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    16149 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     5365 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2276 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     3149 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    14154 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/placeholder.py
--rw-r--r--   0        0        0     2379 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    48309 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     7884 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    28289 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    41835 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    44583 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13853 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    41644 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    64475 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    62401 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    84953 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    48679 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    46696 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    56591 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    61396 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    19483 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6413 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5668 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     4443 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    21398 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/form.py
--rw-r--r--   0        0        0     6020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5416 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5904 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     5127 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6350 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8967 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     8125 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4478 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4828 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3332 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     8301 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     3335 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5019 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3513 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5561 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5518 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     2998 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      943 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9540 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6499 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15528 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1418 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     7815 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12728 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2737 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5151 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4560 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3359 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     4503 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4544 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50327 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5203 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3433 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7767 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     2975 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      748 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2417 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14159 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1809 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1446 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     3872 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1522 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    29428 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2036 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11457 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     2960 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8680 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      890 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2478 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      728 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      929 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2396 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8760 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3219 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4627 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     5926 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     7760 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3552 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12363 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3078 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     5948 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4237 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2009 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     4922 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3878 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1800 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4211 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1807 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5037 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4118 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2256 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9532 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     2741 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2513 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     6788 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10397 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4573 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6361 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2267 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6144 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11167 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4357 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2636 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2115 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3331 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    17406 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2797 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3344 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23334 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4428 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9335 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2465 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2511 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     8016 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5505 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6008 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2563 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1709 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3713 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1477 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     1982 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8602 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     2168 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     3007 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6171 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4886 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8774 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3928 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1341 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0    10063 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/type.py
--rw-r--r--   0        0        0     4593 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     2489 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6321 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2335 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115270 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28454 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26468 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33243 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18848 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     4372 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4607 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2845 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     1716 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2085_empty_if_typetracer.py
--rw-r--r--   0        0        0     2765 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     6369 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2192_union_absorb_indexed.py
--rw-r--r--   0        0        0     6059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4104 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      315 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0      720 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2296_duplicate_field.py
--rw-r--r--   0        0        0     2262 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      648 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2929 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15615 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0      934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2364_empty_list_of_string.py
--rw-r--r--   0        0        0    37200 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5250 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5848 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      956 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      212 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0     1070 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      800 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      704 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      351 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1563 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1211 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      495 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      857 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2471_flatten_string.py
--rw-r--r--   0        0        0     1032 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2484_reduce_starts_empty.py
--rw-r--r--   0        0        0      659 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2487_broadcast_list_offsets.py
--rw-r--r--   0        0        0     1319 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2490_reduce_regulararray_positional.py
--rw-r--r--   0        0        0     1816 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2495_concatenate_typetracer.py
--rw-r--r--   0        0        0     3800 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2501_positional_record_reducer.py
--rw-r--r--   0        0        0      603 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2503_deprecate_to_numpyform.py
--rw-r--r--   0        0        0     4942 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2512_record_array_carry.py
--rw-r--r--   0        0        0     1014 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2518_datetime_units_as_parameter.py
--rw-r--r--   0        0        0     5946 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2536_select_columns.py
--rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1629 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-06-15 15:47:29.000000 awkward-2.2.4/.gitignore
--rw-r--r--   0        0        0     1520 2023-06-15 15:47:29.000000 awkward-2.2.4/LICENSE
--rw-r--r--   0        0        0     8520 2023-06-15 15:47:29.000000 awkward-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-06-15 15:47:29.000000 awkward-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-07-04 08:50:40.000000 awkward-2.3.0/CITATION.cff
+-rw-r--r--   0        0        0    13855 2023-07-04 08:50:40.000000 awkward-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-07-04 08:50:40.000000 awkward-2.3.0/README.md
+-rw-r--r--   0        0        0      241 2023-07-04 08:50:40.000000 awkward-2.3.0/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/redirects.json
+-rw-r--r--   0        0        0       32 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/requirements-wasm.txt
+-rw-r--r--   0        0        0      566 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0      460 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24368 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/index.md
+-rw-r--r--   0        0        0     7349 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18472 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36902 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11694 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1232 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/__init__.py
+-rw-r--r--   0        0        0     4728 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    37966 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0     1259 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_categorical.py
+-rw-r--r--   0        0        0     2221 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_dispatch.py
+-rw-r--r--   0        0        0    13571 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_do.py
+-rw-r--r--   0        0        0    14543 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5727 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     8456 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_operators.py
+-rw-r--r--   0        0        0     4861 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    28974 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     1492 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1162 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2263 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forth.py
+-rw-r--r--   0        0        0   101292 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8044 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/jax.py
+-rw-r--r--   0        0        0     8346 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/record.py
+-rw-r--r--   0        0        0     1679 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     2082 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1453 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1425 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32612 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53532 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4491 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    16494 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    38024 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      806 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0      789 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    71373 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0    11085 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35828 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31510 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9698 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    52212 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0    43059 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/layoutbuilder.py
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1118 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    16149 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     5365 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2276 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     1833 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14154 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     3579 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/placeholder.py
+-rw-r--r--   0        0        0     2379 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    48309 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0      542 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     1642 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    28289 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    41835 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45406 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13361 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    41911 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    64744 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    62401 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    84928 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    48395 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    46696 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    56591 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    60368 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    19483 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      962 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6499 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5754 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     4104 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    21520 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     6106 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5502 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5990 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     5213 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6412 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     9175 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5425 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     8237 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4564 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     9508 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/numba/__init__.py
+-rw-r--r--   0        0        0    23907 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/numba/layoutbuilder.py
+-rw-r--r--   0        0        0     4828 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3332 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8301 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     3335 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5019 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3513 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5561 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5518 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     2998 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      943 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9540 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6499 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15528 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1418 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     7815 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12773 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2737 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5151 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4560 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3359 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     4503 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4544 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50327 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5203 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3433 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7767 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     2975 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      748 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2417 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14159 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1809 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1446 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     3872 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1522 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    29428 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2036 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11457 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     2960 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8680 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      890 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2478 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      728 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      929 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2396 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8760 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3219 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4627 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     5926 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     7760 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3552 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12363 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3078 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     5948 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4237 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2009 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     4922 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3878 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1800 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4211 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1807 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5037 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4118 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2256 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9532 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     2741 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2513 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     6788 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3020 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10397 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4573 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6361 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2267 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6144 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6041 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13339 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11167 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4357 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2693 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2115 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3331 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    17406 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2797 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3344 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23334 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4428 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9335 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2465 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2511 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     8016 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5544 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6008 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2563 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1709 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3713 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1477 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     1982 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8602 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2168 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     3434 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6523 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4886 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8774 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     4355 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1341 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10177 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4593 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1908 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     9772 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3786 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     5796 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12215 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12177 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9151 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2335 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    25853 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   109110 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28350 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26468 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33092 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18752 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4372 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11759 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      513 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4607 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2845 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1716 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2765 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     6369 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2192_union_absorb_indexed.py
+-rw-r--r--   0        0        0     6063 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4104 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      315 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      720 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2262 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37200 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5250 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5848 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      956 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0    34463 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2408_layoutbuilder_in_numba.py
+-rw-r--r--   0        0        0      854 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1211 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      545 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      495 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      857 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2471_flatten_string.py
+-rw-r--r--   0        0        0     1032 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2484_reduce_starts_empty.py
+-rw-r--r--   0        0        0      659 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2487_broadcast_list_offsets.py
+-rw-r--r--   0        0        0     1319 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2490_reduce_regulararray_positional.py
+-rw-r--r--   0        0        0     1816 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2495_concatenate_typetracer.py
+-rw-r--r--   0        0        0     3800 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2501_positional_record_reducer.py
+-rw-r--r--   0        0        0      603 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2503_deprecate_to_numpyform.py
+-rw-r--r--   0        0        0     4942 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2512_record_array_carry.py
+-rw-r--r--   0        0        0     1014 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2518_datetime_units_as_parameter.py
+-rw-r--r--   0        0        0     5946 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2536_select_columns.py
+-rw-r--r--   0        0        0      735 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2548_record_form_fields.py
+-rw-r--r--   0        0        0     3629 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2549_list_nominal_type.py
+-rw-r--r--   0        0        0      670 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2550_validity_error_recursive.py
+-rw-r--r--   0        0        0      443 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2560_minimal_listarray.py
+-rw-r--r--   0        0        0     1451 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2564_string_broadcast_regular.py
+-rw-r--r--   0        0        0      128 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1629 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-07-04 08:50:40.000000 awkward-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1520 2023-07-04 08:50:40.000000 awkward-2.3.0/LICENSE
+-rw-r--r--   0        0        0     8580 2023-07-04 08:50:40.000000 awkward-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-07-04 08:50:40.000000 awkward-2.3.0/PKG-INFO
```

### Comparing `awkward-2.2.4/CITATION.cff` & `awkward-2.3.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/CONTRIBUTING.md` & `awkward-2.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/README.md` & `awkward-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/_toc.yml` & `awkward-2.3.0/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/conf.py` & `awkward-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/index.md` & `awkward-2.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/prepare_docstrings.py` & `awkward-2.3.0/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/redirects-user-guide.json` & `awkward-2.3.0/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/redirects.json` & `awkward-2.3.0/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/requirements.txt` & `awkward-2.3.0/docs/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 sphinx-design
 sphinx-sitemap
 pydata-sphinx-theme
 myst-nb
 sphinx-external-toc
 ipyleaflet
 
-numpy>=1.13.1
+numpy
 numba>=0.50.0;python_version<"3.11"
 pandas>=0.24.0
 numexpr
 pyarrow>=7.0.0
 fsspec
 s3fs
 h5py
```

### Comparing `awkward-2.2.4/docs/_static/css/awkward.css` & `awkward-2.3.0/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/getting-started/community-tutorials.md` & `awkward-2.3.0/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/getting-started/index.md` & `awkward-2.3.0/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/getting-started/papers-and-talks.md` & `awkward-2.3.0/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.3.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/image/example-hierarchy.svg` & `awkward-2.3.0/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/reference/ak.behavior.md` & `awkward-2.3.0/docs/reference/ak.behavior.md`

 * *Files 4% similar despite different names*

```diff
@@ -506,72 +506,74 @@
 
 A footnote: in this implementation, adding a WeightedPoint and a Point returns a Point.
 One may wish to disable this by type-checking, since the functionalities are rather different.
 
 ## Adding behavior to arrays
 
 Occasionally, you may want to add behavior to an array that does not contain
-records. A good example of this is to implement strings: strings are not a
-special data type in Awkward Array as they are in many other libraries, they
-are a behavior overlaid on arrays.
+records. Historically, this mechanism was used to help implement strings (although)
+strings have since been made a part of Awkward's internals, alongside categorical types.
 
-There are four predefined string behaviors:
-
-- {class}`ak.CharBehavior`: an array of UTF-8 encoded characters;
-- {class}`ak.ByteBehavior`: an array of unencoded characters;
-- {class}`ak.StringBehavior`: an array of variable-length UTF-8 encoded strings;
-- {class}`ak.ByteStringBehavior`: an array of variable-length unencoded bytestrings.
-
-All four override the string representations (`__str__` and `__repr__`),
-but the string behaviors additionally override equality:
+Awkward Array supports adding behaviors to the list-types in an array. Let's suppose that 
+one wishes to define a special list that defines a `reversed()` method, equivalent to `array[..., ::-1]`.
 
+First, one must define the behavior class
 ```python
->>> ak.Array(["one", "two", "three"]) == ak.Array(["1", "TWO", "three"])
-<Array [False, False, True] type='3 * bool'>
+class ReversibleArray(ak.Array):
+    def reversed(self):
+        return self[..., ::-1]
+```
+To make this behavior class available to new arrays, it must be associated with its name
+```python
+ak.behavior["reversible"] = ReversibleArray
+```
+One can then add the `__list__` parameter to a list-type array to request this behavior class
+```pycon
+>>> reversible_list = ak.with_parameter([[1, 2, 3], [4], [5, 6, 7]], "__list__", "reversible")
+>>> reversible_list.reversed()
+[[3, 2, 1], [4], [7, 6, 5]]
+```
+If this list is nested within another list, the array class will not be found:
+```pycon
+>>> nested_list = ak.unflatten(reversible_list, [2, 1])
+>>> nested_list.reversed()
+Traceback (most recent call last):
+  File "<stdin>", line 1, in <module>
+...
+AttributeError: no field named 'reversed'
 ```
 
-The only difference here is the parameter: instead of setting `"__record__"`,
-we set `"__array__"`.
-
+Just like with records, we can register a "deep" array class that will be found for all levels of list-depth, using `"*"`:
 ```python
->>> ak.Array(["one", "two", "three"]).layout
-<ListOffsetArray64>
-    <parameters>
-        <param key="__array__">"string"</param>
-    </parameters>
-    <offsets><Index64 i="[0 3 6 11]" offset="0" length="4""/></offsets>
-    <content><NumpyArray format="B" shape="11" data="0x 6f6e6574 776f7468 726565">
-        <parameters>
-            <param key="__array__">"char"</param>
-        </parameters>
-    </NumpyArray></content>
-</ListOffsetArray64>
+>>> ak.behavior["*", "reversible"] = ReversibleArray
+>>> nested_list = ak.unflatten(reversible_list, [2, 1])
+>>> nested_list.reversed()
+[[[3, 2, 1], [4]], [[7, 6, 5]]]
 ```
 
 In `ak.behaviors.string`, string behaviors are assigned with lines like
 
 ```python
 ak.behavior["string"] = StringBehavior
 ak.behavior[np.equal, "string", "string"] = _string_equal
 ```
 
 ## Custom type names
 
-To make the string type appear as `string` in type representations, a
-`"__typestr__"` behavior is overriden (in `ak.behaviors.string`):
-
+To change the type-string representation of our custom list, a
+`"__typestr__"` behavior can be registered:
 ```python
-ak.behavior["__typestr__", "string"] = "string"
+ak.behavior["__typestr__", "reversible"] = "a-reversible-list"
 ```
 
 so that
 
 ```python
->>> ak.type(ak.Array(["one", "two", "three"]))
-3 * string
+>>> ak.type(ak.with_parameter([[1, 2, 3], [4], [5, 6, 7]], "__list__", "reversible"))
+3 * a-reversible-list
 ```
 
 ## Overriding behavior in Numba
 
 Awkward Arrays can be arguments and return values of functions compiled with
 [Numba](http://numba.pydata.org). Since these functions run on low-level
 objects, most functionality must be reimplemented, including behavioral
@@ -652,17 +654,17 @@
 ak.behavior["__numba_typer__", ".", record_name] = typer
 ak.behavior["__numba_lower__", ".", record_name] = lower
 
 # for an array any number of levels deep
 ak.behavior["__numba_typer__", "*", record_name] = typer
 ak.behavior["__numba_lower__", "*", record_name] = lower
 
-# parameters["__array__"] = array_name
-ak.behavior["__numba_typer__", array_name] = typer
-ak.behavior["__numba_lower__", array_name] = lower
+# parameters["__list__"] = list_name
+ak.behavior["__numba_typer__", list_name] = typer
+ak.behavior["__numba_lower__", list_name] = lower
 ```
 
 The `typer` function takes an
 {func}`ak._connect._numba.arrayview.ArrayViewType` as its only argument
 and returns the Numba type of its replacement, while the `lower`
 function takes
```

### Comparing `awkward-2.2.4/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.3.0/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/reference/awkwardforth.rst` & `awkward-2.3.0/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/reference/toctree.txt` & `awkward-2.3.0/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.3.0/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.3.0/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.3.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-json.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-python.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-python.md`

 * *Files 3% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 ak.Array([b"one", b"two", b"three", b"four"]).to_list()
 ```
 
 ```{note}
 Advanced topic: the rest of this section may be skipped if you don't care about internal representations.
 ```
 
-Awkward's strings and bytestrings are not distinct types, but specializations of variable-length lists. Whereas a list might be internally represented by a {class}`ak.contents.ListArray` or a {class}`ak.contents.ListOffsetArray`,
+Awkward's strings and bytestrings are _specializations_ of variable-length lists. Whereas a list might be internally represented by a {class}`ak.contents.ListArray` or a {class}`ak.contents.ListOffsetArray`,
 
 ```{code-cell} ipython3
 ak.Array([[1.1, 2.2, 3.3], [], [4.4, 5.5]]).layout
 ```
 
 Strings and bytestrings are just {class}`ak.contents.ListArray`s and {class}`ak.contents.ListOffsetArray`s of one-byte integers with special parameters:
 
@@ -336,27 +336,14 @@
 ak.Array(["one", "two", "three", "four"]) == ak.Array(
     ["one", "TWO", "thirty three", "four"]
 )
 ```
 
 (Without this overloaded behavior, the string comparison would yield `[True, True, True]` for `"one" == "one"` and would fail to broadcast `"three"` and `"thirty three"`.)
 
-Special behaviors for strings are implemented using the same {data}`ak.behavior` mechanism that you might use to give special behaviors to Arrays and Records.
-
-```{code-cell} ipython3
-ak.behavior["string"]
-```
-
-```{code-cell} ipython3
-ak.behavior["bytestring"]
-```
-
-```{code-cell} ipython3
-ak.behavior[np.equal, "string", "string"]
-```
 
 The fact that strings are really just variable-length lists is worth keeping in mind, since they might behave in unexpectedly list-like ways. If you notice any behavior that ought to be overloded for strings, recommend it as a [feature request](https://github.com/scikit-hep/awkward-1.0/issues/new?assignees=&labels=feature&template=feature-request.md&title=).
 
 +++
 
 Conversion of dicts and tuples
 ------------------------------
```

### Comparing `awkward-2.2.4/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.3.0/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.3.0/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-constructors.md` & `awkward-2.3.0/docs/user-guide/how-to-create-constructors.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,17 @@
 Sections in this document about a subclass of Content are named "`Content >: XYZ`" (using the "[is superclass of](https://stackoverflow.com/q/7759361/1623645)" operator).
 
 +++
 
 Parameters
 ----------
 
-Each layout node can have arbitrary metadata, called "parameters." Some parameters have built-in meanings, which are described below, and others can be given meanings by defining functions in {data}`ak.behavior`.
+Each layout node can have arbitrary metadata[^foot], called "parameters." Some parameters have built-in meanings, which are described below, and others can be given meanings by defining functions in {data}`ak.behavior`.
+
+[^foot]: Except for `ak.contents.EmptyArray`, which is an identity type.
 
 +++
 
 Index classes
 -------------
 
 {class}`ak.index.Index` instances are buffers of integers that are used to give structure to an array. For instance, the `offsets` in the ListOffsetArrays, above, are Indexes, but the NumpyArray of _y_ list contents are not. {class}`ak.contents.NumpyArray` is a subclass of {class}`ak.contents.Content`, and {class}`ak.index.Index` is not. Indexes are more restricted than general NumPy arrays (must be one-dimensional, C-contiguous integers; dtypes are also prescribed) because they are frequently manipulated by Awkward Array operations, such as slicing.
@@ -120,32 +122,24 @@
 +++
 
 Content >: EmptyArray
 ---------------------
 
 {class}`ak.contents.EmptyArray` is one of the two possible leaf types of a layout tree; the other is {class}`ak.contents.NumpyArray` (A third, corner-case "leaf type" is a {class}`ak.contents.RecordArray` with zero fields).
 
-EmptyArray is a trivial node type: it can only represent empty arrays with unknown type.
+EmptyArray is a trivial node type: it can only represent empty arrays with unknown type. It is an identity — when merging an array against an empty array, the empty array has no effect upon the result type. As such, this node cannot have user-defined parameters; {attr}`ak.contents.EmptyArray.parameters` is always empty.
 
 ```{code-cell} ipython3
 ak.contents.EmptyArray()
 ```
 
 ```{code-cell} ipython3
 ak.Array(ak.contents.EmptyArray())
 ```
 
-Since this is such a simple node type, let's use it to show examples of adding parameters.
-
-```{code-cell} ipython3
-ak.contents.EmptyArray(
-    parameters={"name1": "value1", "name2": {"more": ["complex", "value"]}}
-)
-```
-
 Content >: NumpyArray
 ---------------------
 
 {class}`ak.contents.NumpyArray` is one of the two possible leaf types of a layout tree; the other is {class}`ak.contents.EmptyArray`. (A third, corner-case "leaf type" is a {class}`ak.contents.RecordArray` with zero fields)
 
 NumpyArray represents data the same way as a NumPy [np.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html). That is, it can be multidimensional, but only rectilinear arrays.
 
@@ -191,14 +185,25 @@
 ak.Array(
     ak.contents.RegularArray(ak.contents.NumpyArray(np.array([1, 2, 3, 4, 5, 6])), 3)
 )
 ```
 
 If you are _producing_ arrays, you can pick any representation that is convenient. If you are _consuming_ arrays, you need to be aware of the different representations.
 
+Since this is such a simple node type, let's use it to show examples of adding parameters.
+
+```{code-cell} ipython3
+ak.Array(
+    ak.contents.NumpyArray(
+        np.array([[1, 2, 3], [4, 5, 6]]),
+        parameters={"name1": "value1", "name2": {"more": ["complex", "value"]}}
+    )
+)
+```
+
 +++
 
 Content >: RegularArray
 -----------------------
 
 {class}`ak.contents.RegularArray` represents regular-length lists (lists with all the same length). This was shown above as being equivalent to dimensions in a {class}`ak.contents.NumpyArray`, but it can also contain irregular data.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-lists.md` & `awkward-2.3.0/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-missing.md` & `awkward-2.3.0/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-records.md` & `awkward-2.3.0/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-strings.md` & `awkward-2.3.0/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.3.0/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.3.0/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.3.0/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.3.0/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.3.0/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-examine-type.md` & `awkward-2.3.0/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.3.0/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-filter-masked.md` & `awkward-2.3.0/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-filter-num.md` & `awkward-2.3.0/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.3.0/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.3.0/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.3.0/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-gpu.md` & `awkward-2.3.0/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-numpy.md` & `awkward-2.3.0/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-reducing.md` & `awkward-2.3.0/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-math-statistics.md` & `awkward-2.3.0/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.3.0/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.3.0/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.3.0/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.3.0/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.3.0/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.3.0/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.3.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     {Field::one, "one"},
     {Field::two, "two"}
 });
 ```
 
 ```{code-cell}
 template<class... BUILDERS>
-using RecordBuilder = awkward::LayoutBuilder::Record<UserDefinedMap, BUILDERS...>; 
+using RecordBuilder = awkward::LayoutBuilder::Record<UserDefinedMap, BUILDERS...>;
 
 template<std::size_t field_name, class BUILDER>
 using RecordField = awkward::LayoutBuilder::Field<field_name, BUILDER>;
 ```
 
 In the ListOffset Builder, there is an option to use 64-bit signed integers `int64`, 32-bit signed integers `int32` or 32-bit unsigned integers `uint32` as the type for list offsets.
 
@@ -132,34 +132,34 @@
 RecordBuilder<
   RecordField<Field::one, NumpyBuilder<double>>,
   RecordField<Field::two, ListOffsetBuilder<int64_t,
       NumpyBuilder<int32_t>>>
 > builder(fields_map);
 ```
 
-Second Method: The user-defined `fields_map` can be passed a parameter in `set_field_names()`.
+Second Method: The user-defined `fields_map` can be passed a parameter in `set_fields()`.
 
 ```{code-cell}
-builder.set_field_names(fields_map);
+builder.set_fields(fields_map);
 ```
 
-The `field_names()` method can be used to check if field names are set correctly in the Record Builder or not.
+The `fields()` method can be used to check if field names are set correctly in the Record Builder or not.
 
 ```{code-cell}
 std::vector<std::string> fields {"one", "two"};
 
-auto names = builder.field_names();
+auto names = builder.fields();
 names
 ```
 
 Assign each field content to a `fieldname_builder` builder which will be used to fill the Builder buffers.
 
 ```{code-cell}
-auto& one_builder = builder.field<Field::one>();
-auto& two_builder = builder.field<Field::two>();
+auto& one_builder = builder.content<Field::one>();
+auto& two_builder = builder.content<Field::two>();
 ```
 
 Append the data in the fields using `append()`. In case of ListOffsetArray, append the data between `begin_list()` and `end_list()`.
 
 ```{code-cell}
 one_builder.append(1.1);
 auto& two_subbuilder = two_builder.begin_list();
@@ -261,35 +261,35 @@
     auto from_buffers = py::module::import("awkward").attr("from_buffers");
 
     // Build Python dictionary containing arrays
     // dtypes not important here as long as they match the underlying buffer
     // as Awkward Array calls `frombuffer` to convert to the correct type
     py::dict container;
     for (auto it: buffers) {
-        
+
         // Create capsule that frees the allocated data when out of scope
         py::capsule free_when_done(it.second, [](void *data) {
             uint8_t* dataPtr = reinterpret_cast<uint8_t*>(data);
             delete[] dataPtr;
         });
 
         // Adopt the memory filled by `to_buffers` as a NumPy array
         // We only need to return a "buffer" here, but py::array_t let's
-        // us associate a capsule for destruction, which means that 
+        // us associate a capsule for destruction, which means that
         // Python can own this memory. Therefore, we use py::array_t
         uint8_t* data = reinterpret_cast<uint8_t*>(it.second);
         container[py::str(it.first)] = py::array_t<uint8_t>(
             {names_nbytes[it.first]},
             {sizeof(uint8_t)},
             data,
             free_when_done
         );
     }
     return from_buffers(builder.form(), builder.length(), container);
-    
+
 }
 ```
 
 
 More Examples
 -------------
 Examples for other LayoutBuilders can be found [here](https://github.com/scikit-hep/awkward/blob/main/header-only/tests/test_1494-layout-builder.cpp).
```

### Comparing `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-data-analysts.png` & `awkward-2.3.0/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-data-analysts.svg` & `awkward-2.3.0/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-developers.png` & `awkward-2.3.0/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-developers.svg` & `awkward-2.3.0/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-doxygen.png` & `awkward-2.3.0/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-sphinx.png` & `awkward-2.3.0/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-tutorials-alternate.png` & `awkward-2.3.0/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/panel-tutorials.png` & `awkward-2.3.0/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.3.0/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-timeline.png` & `awkward-2.3.0/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.3.0/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.3.0/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.3.0/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.3.0/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.3.0/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-array.svg` & `awkward-2.3.0/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-hierarchy.png` & `awkward-2.3.0/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.3.0/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.3.0/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.3.0/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-reduction.png` & `awkward-2.3.0/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/example-reduction.svg` & `awkward-2.3.0/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/git-strategy.pdf` & `awkward-2.3.0/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/git-strategy.png` & `awkward-2.3.0/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/git-strategy.svg` & `awkward-2.3.0/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.3.0/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.3.0/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/how-it-works.svg` & `awkward-2.3.0/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/sorting-axis.svg` & `awkward-2.3.0/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/all.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/any.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/count.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/max.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/min.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/product.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/diagrams/reducers/sum.svg` & `awkward-2.3.0/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/logo/favicon.ico` & `awkward-2.3.0/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/logo/logo-300px-white.png` & `awkward-2.3.0/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/logo/logo-300px.png` & `awkward-2.3.0/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/logo/logo-600px.png` & `awkward-2.3.0/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/logo/logo.svg` & `awkward-2.3.0/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/photos/desire-path.jpg` & `awkward-2.3.0/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.3.0/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/plots/awkward-0-popularity.png` & `awkward-2.3.0/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.3.0/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.3.0/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.3.0/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/__init__.py` & `awkward-2.3.0/src/awkward/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,16 +41,14 @@
 from awkward.behaviors.mixins import *
 
 # exports
 import awkward.builder
 import awkward.forth
 
 behavior: dict = {}
-awkward.behaviors.string.register(behavior)
-awkward.behaviors.categorical.register(behavior)
 
 # operations
 from awkward.operations import *
 
 # version
 __all__ = [x for x in globals() if not x.startswith("_")]
```

### Comparing `awkward-2.2.4/src/awkward/_behavior.py` & `awkward-2.3.0/src/awkward/_behavior.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     return ChainMap(behavior, ak.behavior)
 
 
 def get_array_class(layout, behavior):
     from awkward.highlevel import Array
 
     behavior = overlay_behavior(behavior)
-    arr = layout.parameter("__array__")
-    if isinstance(arr, str):
-        cls = behavior.get(arr)
+    list_name = layout.parameter("__list__")
+    if isinstance(list_name, str):
+        cls = behavior.get(list_name)
         if isinstance(cls, type) and issubclass(cls, Array):
             return cls
-    deeprec = layout.purelist_parameter("__record__")
-    if isinstance(deeprec, str):
-        cls = behavior.get(("*", deeprec))
+    deep_list_record_name = layout.purelist_parameters("__record__", "__list__")
+    if isinstance(deep_list_record_name, str):
+        cls = behavior.get(("*", deep_list_record_name))
         if isinstance(cls, type) and issubclass(cls, Array):
             return cls
     return Array
 
 
 def get_record_class(layout, behavior):
     from awkward.highlevel import Record
@@ -65,15 +65,15 @@
         if fcn is not None:
             return fcn
     return None
 
 
 def find_ufunc_generic(ufunc, layout, behavior):
     behavior = overlay_behavior(behavior)
-    custom = layout.parameter("__array__")
+    custom = layout.parameter("__list__")
     if custom is None:
         custom = layout.parameter("__record__")
     if isinstance(custom, str):
         fcn = behavior.get((ufunc, custom))
         if fcn is None:
             fcn = behavior.get((ufuncs.ufunc, custom))
         return fcn
@@ -104,29 +104,33 @@
                         for k, s in zip(key[1:], signature[1:])
                     )
                 ):
                     return custom
 
 
 def find_record_typestr(
-    behavior: None | Mapping, parameters: None | Mapping[str, Any], default: str = None
+    behavior: None | Mapping,
+    parameters: None | Mapping[str, Any],
+    default: str | None = None,
 ):
     if parameters is None:
         return default
     behavior = overlay_behavior(behavior)
     return behavior.get(("__typestr__", parameters.get("__record__")), default)
 
 
 def find_array_typestr(
-    behavior: None | Mapping, parameters: None | Mapping[str, Any], default: str = None
+    behavior: None | Mapping,
+    parameters: None | Mapping[str, Any],
+    default: str | None = None,
 ):
     if parameters is None:
         return default
     behavior = overlay_behavior(behavior)
-    return behavior.get(("__typestr__", parameters.get("__array__")), default)
+    return behavior.get(("__typestr__", parameters.get("__list__")), default)
 
 
 def behavior_of(*arrays, **kwargs):
     from awkward.highlevel import Array, ArrayBuilder, Record
 
     behavior = kwargs.get("behavior")
     if behavior is not None:
```

### Comparing `awkward-2.2.4/src/awkward/_broadcasting.py` & `awkward-2.3.0/src/awkward/_broadcasting.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from collections.abc import Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import backend_of
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._parameters import (
     parameters_are_empty,
     parameters_are_equal,
     parameters_intersect,
 )
-from awkward._typing import Any, Callable, Dict, List, TypeAlias, Union
+from awkward._typing import Any, JSONMapping, List, TypedDict
 from awkward._util import UNSET, Sentinel
 from awkward.contents.bitmaskedarray import BitMaskedArray
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.contents.emptyarray import EmptyArray
 from awkward.contents.indexedarray import IndexedArray
 from awkward.contents.indexedoptionarray import IndexedOptionArray
@@ -30,41 +30,51 @@
 from awkward.contents.listoffsetarray import ListOffsetArray
 from awkward.contents.numpyarray import NumpyArray
 from awkward.contents.recordarray import RecordArray
 from awkward.contents.regulararray import RegularArray
 from awkward.contents.unionarray import UnionArray
 from awkward.contents.unmaskedarray import UnmaskedArray
 from awkward.index import (  # IndexU8,  ; Index32,  ; IndexU32,  ; noqa: F401
-    Index,
     Index8,
     Index64,
 )
 from awkward.record import Record
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 optiontypes = (IndexedOptionArray, ByteMaskedArray, BitMaskedArray, UnmaskedArray)
 listtypes = (ListOffsetArray, ListArray, RegularArray)
 
 
+class BroadcastOptions(TypedDict):
+    allow_records: bool
+    left_broadcast: bool
+    right_broadcast: bool
+    numpy_to_regular: bool
+    regular_to_jagged: bool
+    function_name: str | None
+    broadcast_parameters_rule: BroadcastParameterRule
+
+
 def length_of_broadcast(inputs: Sequence) -> int | type[unknown_length]:
-    maxlen = -1
+    maxlen = 1
 
+    has_seen_unknown_length: bool = False
     for x in inputs:
         if isinstance(x, Content):
             if x.length is unknown_length:
-                return x.length
-
+                has_seen_unknown_length = True
+                continue
             maxlen = max(maxlen, x.length)
 
-    if maxlen < 0:
-        maxlen = 1
-
-    return maxlen
+    if has_seen_unknown_length:
+        return unknown_length
+    else:
+        return maxlen
 
 
 def broadcast_pack(inputs: Sequence, isscalar: list[bool]) -> list:
     maxlen = length_of_broadcast(inputs)
     nextinputs = []
 
     for x in inputs:
@@ -105,17 +115,17 @@
 def in_function(options):
     if options["function_name"] is None:
         return ""
     else:
         return " in " + options["function_name"]
 
 
-def checklength(inputs, options):
+def ensure_common_length(inputs, options: BroadcastOptions) -> ShapeItem:
     it = iter(inputs)
-    length: int
+    length: ShapeItem = unknown_length
     for content in it:
         if content.length is not unknown_length:
             length = content.length
             break
 
     for other_content in it:
         if other_content.length is unknown_length:
@@ -126,84 +136,39 @@
                     type(content).__name__,
                     length,
                     type(other_content).__name__,
                     other_content.length,
                     in_function(options),
                 )
             )
+    return length
 
 
-def all_same_offsets(backend: Backend, inputs: list) -> bool:
-    index_nplike = backend.index_nplike
-
-    offsets = None
-    for x in inputs:
-        if isinstance(x, ListOffsetArray):
-            if offsets is None:
-                offsets = x.offsets.raw(index_nplike)
-            elif not index_nplike.array_equal(offsets, x.offsets.raw(index_nplike)):
-                return False
-
-        elif isinstance(x, ListArray):
-            starts = x.starts.raw(index_nplike)
-            stops = x.stops.raw(index_nplike)
-
-            if not index_nplike.array_equal(starts[1:], stops[:-1]):
-                return False
-
-            elif offsets is None:
-                offsets = index_nplike.empty(starts.shape[0] + 1, dtype=starts.dtype)
-                if offsets.shape[0] == 1:
-                    offsets[0] = 0
-                else:
-                    offsets[:-1] = starts
-                    offsets[-1] = stops[-1]
-
-            elif not index_nplike.array_equal(offsets[:-1], starts) or (
-                stops.shape[0] != 0 and offsets[-1] != stops[-1]
-            ):
-                return False
-
-        elif isinstance(x, RegularArray):
-            if x.size == 0:
-                my_offsets = index_nplike.empty(0, dtype=np.int64)
-            else:
-                my_offsets = index_nplike.arange(
-                    0, x.content.length + 1, x.size, dtype=np.int64
-                )
-
-            if offsets is None:
-                offsets = my_offsets
-            elif not index_nplike.array_equal(offsets, my_offsets):
-                return False
-
-        elif isinstance(x, Content):
-            return False
-
-    return True
+def offset_source_rank(list_content: ak.contents.Content) -> int:
+    if isinstance(list_content, ak.contents.ListOffsetArray):
+        return 0
+    elif isinstance(list_content, ak.contents.ListArray):
+        return 1
+    else:
+        raise AssertionError
 
 
 NO_PARAMETERS = Sentinel("NO_PARAMETERS", __name__)
 
 
 class BroadcastParameterRule(str, enum.Enum):
     """Behaviour for parameter coalescence during broadcasting."""
 
     INTERSECT = "intersect"
     ONE_TO_ONE = "one_to_one"
     ALL_OR_NOTHING = "all_or_nothing"
     NONE = "none"
 
 
-BroadcastParameterFactory: TypeAlias = Callable[
-    [int], List[Union[Dict[str, Any], None]]
-]
-
-
-def _parameters_of(obj: Any, default: Any = NO_PARAMETERS) -> Any:
+def parameters_of(obj: Any, default: Any = NO_PARAMETERS) -> JSONMapping | None:
     """
     Args:
         obj: #ak.contents.Content that holds parameters, or object
         default: value to return if obj is not an #ak.contents.Content
 
     Return the parameters of an object if it is a #ak.contents.Content;
     otherwise, return a default value.
@@ -211,141 +176,139 @@
     if isinstance(obj, ak.contents.Content):
         return obj._parameters
     else:
         return default
 
 
 def all_or_nothing_parameters_factory(
-    inputs: Sequence,
-) -> BroadcastParameterFactory:
+    parameters: Sequence[JSONMapping | None], n_outputs: int
+) -> List[JSONMapping | None]:
     """
     Args:
-        inputs: sequence of #ak.contents.Content or other objects
+        parameters: sequence of #ak.contents.Content or other objects
+        n_outputs: required number of outputs
 
     Return a callable that creates an appropriately sized list of parameter objects.
     The parameter objects within this list are built using an "all or nothing rule":
 
     If the parameters of all the given contents are equal, then the first content's
     parameters are repeated, i.e. `[parameters, parameters, ...]`. Otherwise, a list
     of Nones is returned, i.e. `[None, None, ...]`.
     """
-    input_parameters = [
-        p for p in (_parameters_of(c) for c in inputs) if p is not NO_PARAMETERS
-    ]
+    input_parameters = [p for p in parameters if p is not NO_PARAMETERS]
 
-    parameters = None
+    result = None
     if len(input_parameters) > 0:
         # All parameters must match this first layout's parameters
         first_parameters = input_parameters[0]
         # Ensure all parameters match, or set parameters to None
         for other_parameters in input_parameters[1:]:
             if not parameters_are_equal(first_parameters, other_parameters):
                 break
         else:
-            parameters = first_parameters
+            result = first_parameters
 
-    def apply(n_outputs: int) -> list[dict[str, Any] | None]:
-        # NB: we don't make unique copies here, so let's hope everyone
-        # is well-behaved downstream!
-        return [parameters] * n_outputs
-
-    return apply
+    # NB: we don't make unique copies here, so let's hope everyone
+    # is well-behaved downstream!
+    return [result] * n_outputs
 
 
 def intersection_parameters_factory(
-    inputs: Sequence,
-) -> BroadcastParameterFactory:
+    parameters: Sequence[JSONMapping | None],
+    n_outputs: int,
+) -> List[JSONMapping | None]:
     """
     Args:
-        inputs: sequence of #ak.contents.Content or other objects
+        parameters: sequence of #ak.contents.Content or other objects
+        n_outputs: required number of outputs
 
     Return a callable that creates an appropriately sized list of parameter objects.
     The parameter objects within this list are built using an "intersection rule":
 
     The intersection of `content._parameters.items()` for each content is computed.
     If any parameter dictionaries are None, then a list of Nones is returned, i.e.
     `[None, None, ...]`; otherwise, the computed parameter dictionary is repeated,
     i.e. `[parameters, parameters, ...]`.
     """
-    input_parameters = [
-        p for p in (_parameters_of(c) for c in inputs) if p is not NO_PARAMETERS
-    ]
+    input_parameters = [p for p in parameters if p is not NO_PARAMETERS]
 
     intersected_parameters = None
     parameters_to_intersect = []
     # Build a list of set-like dict.items() views.
     # If we encounter None-parameters, then we stop early
     # as there can be no intersection.
-    for parameters in input_parameters:
-        if parameters_are_empty(parameters):
+    for params in input_parameters:
+        if parameters_are_empty(params):
             break
         else:
-            parameters_to_intersect.append(parameters)
+            parameters_to_intersect.append(params)
     # Otherwise, build the intersected parameter dict
     else:
-        intersected_parameters = functools.reduce(
-            parameters_intersect, parameters_to_intersect
-        )
-
-    def apply(n_outputs: int) -> list[dict[str, Any] | None]:
-        # NB: we don't make unique copies here, so let's hope everyone
-        # is well-behaved downstream!
-        return [intersected_parameters] * n_outputs
+        if len(parameters_to_intersect):
+            intersected_parameters = functools.reduce(
+                parameters_intersect, parameters_to_intersect
+            )
+        else:
+            intersected_parameters = None
 
-    return apply
+    # NB: we don't make unique copies here, so let's hope everyone
+    # is well-behaved downstream!
+    return [intersected_parameters] * n_outputs
 
 
 def one_to_one_parameters_factory(
-    inputs: Sequence,
-) -> BroadcastParameterFactory:
+    parameters: Sequence[JSONMapping | None],
+    n_outputs: int,
+) -> List[JSONMapping | None]:
     """
     Args:
-        inputs: sequence of #ak.contents.Content or other objects
+        parameters: sequence of #ak.contents.Content or other objects
+        n_outputs: required number of outputs
 
     Return a callable that creates an appropriately sized list of parameter objects.
     The parameter objects within this list are built using a "one-to-one rule":
 
     The requested number of outputs is compared against the length of the given
     `inputs`. If the two values match, then a list of parameter objects is returned,
     where each element of the returned list corresponds to the parameters of the
     content at the same position in the `inputs` sequence. If the length of the
-    given contents does not match the requested list length, a ValueError is raised.
+    given contents does not match the requested list length, the intersection of the parameters
+    is returned instead.
     """
-    # Find the parameters of the inputs, with None values for non-Contents
-    input_parameters = [_parameters_of(c, default=None) for c in inputs]
-
-    def apply(n_outputs) -> list[dict[str, Any] | None]:
-        if n_outputs != len(inputs):
-            raise ValueError(
-                "cannot follow one-to-one parameter broadcasting rule for actions "
-                "which change the number of outputs."
-            )
-        return input_parameters
-
-    return apply
+    if n_outputs == len(parameters):
+        return [p if p is not NO_PARAMETERS else None for p in parameters]
+    else:
+        return intersection_parameters_factory(parameters, n_outputs)
 
 
 def none_parameters_factory(
-    inputs: Sequence,
-) -> BroadcastParameterFactory:
+    parameters: Sequence[JSONMapping | None],
+    n_outputs: int,
+) -> List[JSONMapping | None]:
     """
     Args:
-        inputs: sequence of #ak.contents.Content or other objects
+        parameters: sequence of #ak.contents.Content or other objects
+        n_outputs: required number of outputs
 
     Return a callable that creates an appropriately sized list of parameter objects.
     The parameter objects within this list are built using an "all or nothing rule":
 
     A list of Nones is returned, with a length corresponding to the requested number of
     outputs, i.e. `[None, None, ...]`.
     """
 
-    def apply(n_outputs: int) -> list[dict[str, Any] | None]:
-        return [None] * n_outputs
+    return [None] * n_outputs
+
 
-    return apply
+def is_string_like(obj) -> bool:
+    return (
+        isinstance(obj, ak.contents.Content)
+        and obj.is_list
+        and obj.parameter("__array__") in {"string", "bytestring"}
+    )
 
 
 # Mapping from rule enum values to factory implementations
 BROADCAST_RULE_TO_FACTORY_IMPL = {
     BroadcastParameterRule.INTERSECT: intersection_parameters_factory,
     BroadcastParameterRule.ALL_OR_NOTHING: all_or_nothing_parameters_factory,
     BroadcastParameterRule.ONE_TO_ONE: one_to_one_parameters_factory,
@@ -355,23 +318,98 @@
 
 def left_broadcast_to(content: Content, depth: int) -> Content:
     for _ in range(content.purelist_depth, depth):
         content = RegularArray(content, 1, content.length)
     return content
 
 
+def broadcast_regular_dim_size(contents: Sequence[ak.contents.Content]) -> ShapeItem:
+    # Find known size out of our contents
+    dim_size: ShapeItem
+    it_non_string_regular_contents = iter(
+        c for c in contents if c.is_regular and not is_string_like(c)
+    )
+    for x in it_non_string_regular_contents:
+        if x.size is not unknown_length:
+            dim_size = x.size
+            break
+    else:
+        # We should only be here if we didn't find any regular arrays with known lengths;
+        # there is guaranteed to be at least one non-string list
+        dim_size = unknown_length
+    # Now we know that we have at least one layout with concrete size, let's check the remainder
+    # dim_size=0 should win, though, so we require that dim_size != 0
+    if dim_size is not unknown_length and dim_size > 0:
+        for x in it_non_string_regular_contents:
+            # Any unknown lengths can't be compared
+            if x.size is unknown_length:
+                continue
+            # Any zero-length column triggers zero broadcasting
+            if x.size == 0:
+                return 0
+            else:
+                dim_size = max(dim_size, x.size)
+    return dim_size
+
+
+def broadcast_to_offsets_avoiding_carry(
+    list_content: ak.contents.Content,
+    offsets: ak.index.Index,
+) -> ak.contents.Content:
+    index_nplike = list_content.backend.index_nplike
+
+    # Without known data, we can't perform these optimisations
+    if not index_nplike.known_data:
+        return list_content._broadcast_tooffsets64(offsets).content
+
+    elif isinstance(list_content, ListOffsetArray):
+        if index_nplike.array_equal(offsets.data, list_content.offsets.data):
+            next_length = index_nplike.index_as_shape_item(offsets[-1])
+            return list_content.content[:next_length]
+        else:
+            return list_content._broadcast_tooffsets64(offsets).content
+    elif isinstance(list_content, ListArray):
+        # Is this list contiguous?
+        if index_nplike.array_equal(
+            list_content.starts.data[1:], list_content.stops.data[:-1]
+        ):
+            # Does this list match the offsets?
+            if index_nplike.array_equal(
+                offsets.data[:-1], list_content.starts.data
+            ) and not (
+                list_content.stops.data.shape[0] != 0
+                and offsets[-1] != list_content.stops[-1]
+            ):
+                next_length = index_nplike.index_as_shape_item(offsets[-1])
+                return list_content.content[:next_length]
+            else:
+                return list_content._broadcast_tooffsets64(offsets).content
+        else:
+            return list_content._broadcast_tooffsets64(offsets).content
+
+    elif isinstance(list_content, RegularArray):
+        my_offsets = list_content._compact_offsets64(True)
+        if index_nplike.array_equal(offsets.data, my_offsets.data):
+            return list_content.content[: list_content.size * list_content.length]
+        else:
+            return list_content._broadcast_tooffsets64(offsets).content
+
+    else:
+        raise AssertionError
+
+
 def apply_step(
     backend: Backend,
     inputs: Sequence,
     action,
     depth: int,
     depth_context,
     lateral_context,
     behavior,
-    options,
+    options: BroadcastOptions,
 ):
     # This happens when descending anyway, but setting the option does it before action.
     if options["numpy_to_regular"] and any(
         isinstance(x, NumpyArray) and x.data.ndim != 1 for x in inputs
     ):
         inputs = [
             x.to_RegularArray() if isinstance(x, NumpyArray) else x for x in inputs
@@ -406,349 +444,262 @@
                     depth,
                     depth_context,
                     lateral_context,
                     behavior,
                     options,
                 )
 
-    # Now all lengths must agree.
-    checklength(contents, options)
+    # Now all lengths must agree
+    length = ensure_common_length(contents, options)
 
     # Load the parameter broadcasting rule implementation
     rule = options["broadcast_parameters_rule"]
     try:
-        parameters_factory_impl = BROADCAST_RULE_TO_FACTORY_IMPL[rule]
+        parameters_factory = BROADCAST_RULE_TO_FACTORY_IMPL[rule]
     except KeyError:
         raise ValueError(
             f"`broadcast_parameters_rule` should be one of {[str(x) for x in BroadcastParameterRule]}, "
             f"but this routine received `{rule}`"
         ) from None
-    parameters_factory = parameters_factory_impl(inputs)
 
     # This whole function is one big switch statement.
     def broadcast_any_record():
         if not options["allow_records"]:
-            raise ValueError(f"cannot broadcast records {in_function(options)}")
+            raise ValueError(f"cannot broadcast records{in_function(options)}")
+
+        fields: list[str] | None = UNSET
+        frozen_fields: frozenset[str] | None = UNSET
+
+        is_tuple: bool = True
+        nextparameters = []
 
-        fields, length, istuple = UNSET, UNSET, UNSET
         for x in contents:
             if x.is_record:
+                nextparameters.append(x._parameters)
+
+                if x.is_tuple:
+                    continue
+
+                # Check fields match
                 if fields is UNSET:
-                    fields = x.fields
-                elif set(fields) != set(x.fields):
+                    fields = x._fields
+                    frozen_fields = frozenset(x._fields)
+                elif frozen_fields != frozenset(x.fields):
                     raise ValueError(
                         "cannot broadcast records because fields don't "
                         "match{}:\n    {}\n    {}".format(
                             in_function(options),
                             ", ".join(sorted(fields)),
                             ", ".join(sorted(x.fields)),
                         )
                     )
-                if length is UNSET:
-                    length = x.length
-                elif length != x.length:
-                    raise ValueError(
-                        "cannot broadcast RecordArray of length {} "
-                        "with RecordArray of length {}{}".format(
-                            length, x.length, in_function(options)
-                        )
-                    )
                 # Records win over tuples
-                if istuple is UNSET or not x.is_tuple:
-                    istuple = False
+                is_tuple = False
+            else:
+                nextparameters.append(NO_PARAMETERS)
 
-        outcontents, numoutputs = [], None
+        numoutputs = None
+        outcontents = []
         for field in fields:
             outcontents.append(
                 apply_step(
                     backend,
                     [x[field] if isinstance(x, RecordArray) else x for x in inputs],
                     action,
                     depth,
                     copy.copy(depth_context),
                     lateral_context,
                     behavior,
                     options,
                 )
             )
             assert isinstance(outcontents[-1], tuple)
-            if numoutputs is not None:
+            if numoutputs is None:
+                numoutputs = len(outcontents[-1])
+            else:
                 assert numoutputs == len(outcontents[-1])
-            numoutputs = len(outcontents[-1])
+
+        parameters = parameters_factory(nextparameters, numoutputs)
 
         return tuple(
             RecordArray(
                 [x[i] for x in outcontents],
-                None if istuple else fields,
+                None if is_tuple else fields,
                 length,
                 parameters=p,
             )
-            for i, p in enumerate(parameters_factory(numoutputs))
+            for i, p in enumerate(parameters)
         )
 
     def broadcast_any_list():
         index_nplike = backend.index_nplike
-        # All regular?
-        if all(x.is_regular or not x.is_list for x in contents):
-            # Ensure all layouts have same length
-            length = None
-            for x in contents:
-                if length is None:
-                    length = x.length
-                elif length is not unknown_length and x.length is not unknown_length:
-                    assert length == x.length
-            assert length is not None
+        # Under the category of "is_list", we have both strings and non-strings
+        # The strings should behave like non-lists within these routines.
 
-            # Determine the size of the broadcast result
-            dim_size = None
-            for x in contents:
-                if not x.is_regular:
-                    continue
+        # Are the non-string list types exclusively regular?
+        if all(x.is_regular or (is_string_like(x) or not x.is_list) for x in contents):
+            # Compute the expected dim size
+            dim_size = broadcast_regular_dim_size(contents)
+            dimsize_maybe_broadcastable = dim_size is unknown_length or dim_size > 1
+            dimsize_is_zero = dim_size is not unknown_length and dim_size == 0
 
-                # Any unknown length sets max_size to unknown
-                if x.size is unknown_length:
-                    dim_size = unknown_length
-                # Any zero-length column triggers zero broadcasting
-                elif x.size == 0:
-                    dim_size = 0
-                    break
-                # Take first size as dim_size
-                elif dim_size is None:
-                    dim_size = x.size
-                # If the dim_size is unknown, we can't compare
-                elif dim_size is unknown_length:
-                    continue
-                else:
-                    dim_size = max(dim_size, x.size)
-
-            dimsize_greater_than_one_if_known = (
-                dim_size is unknown_length or dim_size > 1
-            )
-            dimsize_known_to_be_zero = dim_size is not unknown_length and dim_size == 0
-
-            # Build a broadcast index for size=1 contents
+            # Build a broadcast index for size=1 contents, and identify whether we have strings
+            inputs_are_strings = []
             size_one_carry_index = None
-            for x in contents:
-                if x.is_regular:
-                    x_size_known_to_be_one = (
-                        x.size is not unknown_length and x.size == 1
-                    )
-                    if dimsize_greater_than_one_if_known and x_size_known_to_be_one:
+            for x in inputs:
+                if isinstance(x, ak.contents.Content):
+                    content_is_string = is_string_like(x)
+                    inputs_are_strings.append(content_is_string)
+                    if (
+                        # Strings don't count as lists in this context
+                        not content_is_string
+                        # Is this layout known to be size==1?
+                        and x.is_regular
+                        and x.size is not unknown_length
+                        and x.size == 1
+                        # Does the computed dim_size support broadcasting
+                        and dimsize_maybe_broadcastable
+                        and size_one_carry_index is None
+                    ):
                         # For any (N, 1) array, we know we'll broadcast to (N, M) where M is maxsize
                         size_one_carry_index = Index64(
                             index_nplike.repeat(
                                 index_nplike.arange(
-                                    index_nplike.shape_item_as_index(x.length),
+                                    index_nplike.shape_item_as_index(length),
                                     dtype=np.int64,
                                 ),
                                 index_nplike.shape_item_as_index(dim_size),
                             ),
                             nplike=index_nplike,
                         )
-                        break
+                else:
+                    inputs_are_strings.append(False)
+
+            # W.r.t broadcasting against other lists, we have three possibilities
+            # a. any (exactly) size-0 content broadcasts all other regular dimensions to 0
+            # b. any (exactly) size-1 content broadcasts to the `size_one_carry_index``
+            # c. otherwise, the list size should equal the dimension; recurse into the content as-is
 
-            # Here we have three possible broadcasting outcomes (by precedence):
-            # 1. any (exactly) size-0 content trims all other contents
-            # 2. any (exactly) size-1 content broadcasts to the common length
-            # 3. otherwise, recurse into the content as-is
+            # If we have non-lists, these are just appended as-is. As we're dealing with regular layouts,
+            # we don't left-broadcast
             nextinputs = []
-            for x in inputs:
-                if isinstance(x, RegularArray):
-                    x_size_known_to_be_one = (
+            nextparameters = []
+            for x, x_is_string in zip(inputs, inputs_are_strings):
+                if isinstance(x, RegularArray) and not x_is_string:
+                    content_size_maybe_one = (
                         x.size is not unknown_length and x.size == 1
                     )
                     # If dimsize is known to be exactly zero, all contents are zero length
-                    if dimsize_known_to_be_zero:
+                    if dimsize_is_zero:
                         nextinputs.append(x.content[:0])
+                        nextparameters.append(x._parameters)
                     # If we have a known size=1 content, then broadcast it to the dimension size
-                    elif dimsize_greater_than_one_if_known and x_size_known_to_be_one:
+                    elif dimsize_maybe_broadcastable and content_size_maybe_one:
                         nextinputs.append(
                             x.content[: x.length * x.size]._carry(
                                 size_one_carry_index, allow_lazy=False
                             )
                         )
+                        nextparameters.append(x._parameters)
                     # Any unknown values or sizes are assumed to be correct as-is
                     elif (
                         dim_size is unknown_length
                         or x.size is unknown_length
                         or x.size == dim_size
                     ):
                         nextinputs.append(x.content[: x.length * x.size])
+                        nextparameters.append(x._parameters)
                     else:
                         raise ValueError(
                             "cannot broadcast RegularArray of size "
-                            "{} with RegularArray of size {} {}".format(
+                            "{} with RegularArray of size {}{}".format(
                                 x.size, dim_size, in_function(options)
                             )
                         )
                 else:
                     nextinputs.append(x)
+                    nextparameters.append(NO_PARAMETERS)
 
             outcontent = apply_step(
                 backend,
                 nextinputs,
                 action,
                 depth + 1,
                 copy.copy(depth_context),
                 lateral_context,
                 behavior,
                 options,
             )
             assert isinstance(outcontent, tuple)
-            parameters = parameters_factory(len(outcontent))
+            parameters = parameters_factory(nextparameters, len(outcontent))
+
             return tuple(
                 RegularArray(x, dim_size, length, parameters=p)
                 for x, p in zip(outcontent, parameters)
             )
-
-        # Not all regular, but all same offsets?
-        # Optimization: https://github.com/scikit-hep/awkward-1.0/issues/442
-        elif index_nplike.known_data and all_same_offsets(backend, inputs):
-            lencontent, offsets, starts, stops = None, None, None, None
-            nextinputs = []
-
-            for x in inputs:
-                if isinstance(x, ListOffsetArray):
-                    offsets = x.offsets
-                    lencontent = index_nplike.index_as_shape_item(offsets[-1])
-                    nextinputs.append(x.content[:lencontent])
-
-                elif isinstance(x, ListArray):
-                    starts, stops = x.starts, x.stops
-                    if (starts.length is not unknown_length and starts.length == 0) or (
-                        stops.length is not unknown_length and stops.length == 0
-                    ):
-                        nextinputs.append(x.content[:0])
-                    else:
-                        lencontent = index_nplike.index_as_shape_item(
-                            index_nplike.max(stops)
-                        )
-                        nextinputs.append(x.content[:lencontent])
-                elif isinstance(x, RegularArray):
-                    nextinputs.append(x.content[: x.size * x.length])
-                else:
-                    nextinputs.append(x)
-
-            outcontent = apply_step(
-                backend,
-                nextinputs,
-                action,
-                depth + 1,
-                copy.copy(depth_context),
-                lateral_context,
-                behavior,
-                options,
-            )
-            assert isinstance(outcontent, tuple)
-            parameters = parameters_factory(len(outcontent))
-
-            if isinstance(offsets, Index):
-                return tuple(
-                    ListOffsetArray(offsets, x, parameters=p).to_ListOffsetArray64(
-                        False
-                    )
-                    for x, p in zip(outcontent, parameters)
-                )
-            elif isinstance(starts, Index) and isinstance(stops, Index):
-                return tuple(
-                    ListArray(starts, stops, x, parameters=p).to_ListOffsetArray64(
-                        False
-                    )
-                    for x, p in zip(outcontent, parameters)
-                )
-            else:
-                raise AssertionError(
-                    "unexpected offsets, starts: {}, {}".format(
-                        type(offsets), type(starts)
-                    )
-                )
-
         # General list-handling case: the offsets of each list may be different.
         else:
-            # We have three possible cases here:
-            # 1. all-string (nothing to do)
-            # 2. mixed string-list (strings gain a dimension and broadcast to the non-string offsets)
-            # 3. no strings (all lists broadcast to a single offsets)
             offsets_content = None
-            all_content_strings = True
             input_is_string = []
+
+            # Find the offsets to broadcast to, taking the "best" list
             for x in inputs:
                 if isinstance(x, Content):
-                    content_is_string = x.parameter("__array__") in {
-                        "string",
-                        "bytestring",
-                    }
-                    # Don't try and take offsets from strings
-                    if not content_is_string:
-                        all_content_strings = False
-                        # Take the offsets from the first irregular list
-                        if x.is_list and not x.is_regular and offsets_content is None:
-                            offsets_content = x
+                    content_is_string = is_string_like(x)
                     input_is_string.append(content_is_string)
+                    if (
+                        x.is_list
+                        and not x.is_regular
+                        and not content_is_string
+                        and (
+                            offsets_content is None
+                            or (
+                                offset_source_rank(x)
+                                < offset_source_rank(offsets_content)
+                            )
+                        )
+                    ):
+                        offsets_content = x
                 else:
                     input_is_string.append(False)
 
-            # case (1): user getfunctions should exit before this gets called
-            if all_content_strings:
-                raise ValueError(
-                    "cannot broadcast all strings: {}{}".format(
-                        ", ".join(repr(type(x)) for x in inputs), in_function(options)
-                    )
-                )
-
-            # Didn't find a ragged list, try any list!
-            if offsets_content is None:
-                for content in contents:
-                    if content.is_list:
-                        offsets_content = content
-                        break
-                else:
-                    raise AssertionError("no list found in list branch!")
-
+            # Build the offsets of the lowest-ranking source
             offsets = offsets_content._compact_offsets64(True)
 
             nextinputs = []
+            nextparameters = []
             for x, x_is_string in zip(inputs, input_is_string):
-                if x_is_string:
-                    offsets_data = backend.index_nplike.asarray(offsets)
-                    counts = offsets_data[1:] - offsets_data[:-1]
-                    if ak._util.win or ak._util.bits32:
-                        counts = index_nplike.astype(counts, dtype=np.int32)
-                    parents = index_nplike.repeat(
-                        index_nplike.arange(counts.size, dtype=counts.dtype), counts
-                    )
-                    nextinputs.append(
-                        ak.contents.IndexedArray(
-                            ak.index.Index64(parents, nplike=index_nplike), x
-                        ).project()
-                    )
-                elif isinstance(x, listtypes):
-                    nextinputs.append(x._broadcast_tooffsets64(offsets).content)
+                if isinstance(x, listtypes) and not x_is_string:
+                    next_content = broadcast_to_offsets_avoiding_carry(x, offsets)
+                    nextinputs.append(next_content)
+                    nextparameters.append(x._parameters)
                 # Handle implicit left-broadcasting (non-NumPy-like broadcasting).
                 elif options["left_broadcast"] and isinstance(x, Content):
                     nextinputs.append(
                         RegularArray(x, 1, x.length)
                         ._broadcast_tooffsets64(offsets)
                         .content
                     )
+                    nextparameters.append(NO_PARAMETERS)
                 else:
                     nextinputs.append(x)
+                    nextparameters.append(NO_PARAMETERS)
 
             outcontent = apply_step(
                 backend,
                 nextinputs,
                 action,
                 depth + 1,
                 copy.copy(depth_context),
                 lateral_context,
                 behavior,
                 options,
             )
             assert isinstance(outcontent, tuple)
-            parameters = parameters_factory(len(outcontent))
+            parameters = parameters_factory(nextparameters, len(outcontent))
 
             return tuple(
                 ListOffsetArray(offsets, x, parameters=p)
                 for x, p in zip(outcontent, parameters)
             )
 
     def broadcast_any_option():
@@ -774,40 +725,53 @@
                 backend.index_nplike.shape_item_as_index(mask.shape[0]),
                 dtype=np.int64,
             )
             nextindex[mask] = -1
             nextindex = Index64(nextindex)
 
         nextinputs = []
+        nextparameters = []
         for x in inputs:
             if isinstance(x, optiontypes):
                 nextinputs.append(x.project(nextmask))
+                nextparameters.append(x._parameters)
             elif isinstance(x, Content):
                 nextinputs.append(IndexedOptionArray(nextindex, x).project(nextmask))
+                nextparameters.append(x._parameters)
             else:
                 nextinputs.append(x)
+                nextparameters.append(NO_PARAMETERS)
 
         outcontent = apply_step(
             backend,
             nextinputs,
             action,
             depth,
             copy.copy(depth_context),
             lateral_context,
             behavior,
             options,
         )
         assert isinstance(outcontent, tuple)
-        parameters = parameters_factory(len(outcontent))
+        parameters = parameters_factory(nextparameters, len(outcontent))
+
         return tuple(
             IndexedOptionArray.simplified(index, x, parameters=p)
             for x, p in zip(outcontent, parameters)
         )
 
     def broadcast_any_union():
+        nextparameters = []
+
+        for x in inputs:
+            if isinstance(x, UnionArray):
+                nextparameters.append(x._parameters)
+            else:
+                nextparameters.append(NO_PARAMETERS)
+
         if not backend.nplike.known_data:
             # assert False
             union_num_contents = []
             length = None
             for x in contents:
                 if x.is_union:
                     x._touch_data(recursive=False)
@@ -828,15 +792,15 @@
                 i = 0
                 for x in inputs:
                     if isinstance(x, UnionArray):
                         nextinputs.append(x._contents[combo[i]])
                         i += 1
                     else:
                         nextinputs.append(x)
-
+                assert len(nextinputs) == len(nextparameters)
                 outcontents.append(
                     apply_step(
                         backend,
                         nextinputs,
                         action,
                         depth,
                         copy.copy(depth_context),
@@ -918,15 +882,16 @@
                 if numoutputs is None:
                     numoutputs = len(outcontents[-1])
                 else:
                     assert numoutputs == len(outcontents[-1])
 
             assert numoutputs is not None
 
-        parameters = parameters_factory(numoutputs)
+        parameters = parameters_factory(nextparameters, numoutputs)
+
         return tuple(
             UnionArray.simplified(
                 Index8(tags),
                 Index64(index),
                 [x[i] for x in outcontents],
                 parameters=p,
             )
@@ -1000,16 +965,16 @@
         elif any(x.is_union for x in contents):
             return broadcast_any_union()
 
         # Any option-types?
         elif any(x.is_option for x in contents):
             return broadcast_any_option()
 
-        # Any list-types?
-        elif any(x.is_list for x in contents):
+        # Any non-string list-types?
+        elif any(x.is_list and not is_string_like(x) for x in contents):
             return broadcast_any_list()
 
         # Any RecordArrays?
         elif any(x.is_record for x in contents):
             return broadcast_any_record()
 
         else:
@@ -1040,20 +1005,20 @@
 
 def broadcast_and_apply(
     inputs,
     action,
     behavior,
     depth_context=None,
     lateral_context=None,
-    allow_records=True,
-    left_broadcast=True,
-    right_broadcast=True,
-    numpy_to_regular=False,
-    regular_to_jagged=False,
-    function_name=None,
+    allow_records: bool = True,
+    left_broadcast: bool = True,
+    right_broadcast: bool = True,
+    numpy_to_regular: bool = False,
+    regular_to_jagged: bool = False,
+    function_name: str | None = None,
     broadcast_parameters_rule=BroadcastParameterRule.INTERSECT,
 ):
     backend = backend_of(*inputs)
     isscalar = []
     out = apply_step(
         backend,
         broadcast_pack(inputs, isscalar),
```

### Comparing `awkward-2.2.4/src/awkward/_dispatch.py` & `awkward-2.3.0/src/awkward/_dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_do.py` & `awkward-2.3.0/src/awkward/_do.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 def to_buffers(
     content: Content,
     container: MutableMapping[str, Any] | None = None,
     buffer_key="{form_key}-{attribute}",
     form_key: str | None = "node{id}",
     id_start: Integral = 0,
-    backend: Backend = None,
+    backend: Backend | None = None,
     byteorder: Literal["<", ">"] = "<",
 ) -> tuple[form.Form, int, Mapping[str, Any]]:
     if container is None:
         container = {}
     if backend is None:
         backend = content._backend
     if not backend.nplike.known_data:
@@ -345,17 +345,14 @@
             behavior,
         )
 
         return next[0]
 
 
 def validity_error(layout: Content, path: str = "layout") -> str:
-    paramcheck = layout._validity_error_parameters(path)
-    if paramcheck != "":
-        return paramcheck
     return layout._validity_error(path)
 
 
 def argsort(
     layout: Content,
     axis: int = -1,
     ascending: bool = True,
```

### Comparing `awkward-2.2.4/src/awkward/_errors.py` & `awkward-2.3.0/src/awkward/_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
             except Exception:
                 return x._repr("    ", "", "")
 
         else:
             return repr(x)
 
 
-def index_error(subarray, slicer, details: str = None) -> IndexError:
+def index_error(subarray, slicer, details: str | None = None) -> IndexError:
     message = ""
     if details is not None:
         message = f": {details}"
 
     # Note: returns an error for the caller to raise!
     return IndexError(
         f"cannot slice {type(subarray).__name__} (of length {subarray.length}) with {SlicingErrorContext.format_slice(slicer)}{message}"
```

### Comparing `awkward-2.2.4/src/awkward/_kernels.py` & `awkward-2.3.0/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_layout.py` & `awkward-2.3.0/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_lookup.py` & `awkward-2.3.0/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_operators.py` & `awkward-2.3.0/src/awkward/_operators.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_prettyprint.py` & `awkward-2.3.0/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_reducers.py` & `awkward-2.3.0/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_regularize.py` & `awkward-2.3.0/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_slicing.py` & `awkward-2.3.0/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_typetracer.py` & `awkward-2.3.0/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_typing.py` & `awkward-2.3.0/src/awkward/_typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,24 @@
     }
 )
 
 
 AxisMaybeNone = TypeVar("AxisMaybeNone", int, None)  # noqa: F405
 
 if sys.version_info < (3, 11):
+    from typing import Final, SupportsIndex, runtime_checkable
+
     from typing_extensions import (
-        Final,
         Literal,
         Protocol,
         Self,
-        SupportsIndex,
         TypeAlias,
         TypedDict,
         Unpack,
         final,
-        runtime_checkable,
     )
 else:
     from typing import (
         Final,
         Literal,
         Protocol,
         Self,
```

### Comparing `awkward-2.2.4/src/awkward/_util.py` & `awkward-2.3.0/src/awkward/_util.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_v2.py` & `awkward-2.3.0/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/cppyy.py` & `awkward-2.3.0/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/highlevel.py` & `awkward-2.3.0/src/awkward/highlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+from __future__ import annotations
+
 __all__ = ("Array", "ArrayBuilder", "Record")
 
 import copy
 import html
 import io
 import itertools
 import keyword
@@ -18,21 +20,38 @@
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of, get_array_class, get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._operators import NDArrayOperatorsMixin
 from awkward._regularize import is_non_string_like_iterable
+from awkward._typing import TypeVar
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 _dir_pattern = re.compile(r"^[a-zA-Z_]\w*$")
 
 
+T = TypeVar("T", bound=ak.contents.Content)
+
+
+def prepare_layout(layout: T) -> T | str | bytes:
+    if isinstance(layout, ak.contents.NumpyArray):
+        array_param = layout.parameter("__array__")
+        if array_param == "byte":
+            return ak._util.tobytes(layout.data)
+        elif array_param == "char":
+            return ak._util.tobytes(layout.data).decode(errors="surrogateescape")
+        else:
+            return layout
+    else:
+        return layout
+
+
 class Array(NDArrayOperatorsMixin, Iterable, Sized):
     """
     Args:
         data (#ak.contents.Content, #ak.Array, `np.ndarray`, `cp.ndarray`, `pyarrow.*`, str, dict, or iterable):
             Data to wrap or convert into an array.
                - If a NumPy array, the regularity of its dimensions is preserved
                  and the data are viewed, not copied.
@@ -124,15 +143,15 @@
 
         np.concatenate
 
     can be used on an Awkward Array because
 
         ak.concatenate
 
-    exists. If your NumPy is older than 1.17, use `ak.concatenate` directly.
+    exists.
 
     Pandas
     ******
 
     Ragged arrays (list type) can be converted into Pandas
     [MultiIndex](https://pandas.pydata.org/pandas-docs/stable/user_guide/advanced.html)
     rows and nested records can be converted into MultiIndex columns. If the
@@ -486,40 +505,16 @@
             2.345207879911715
 
         Iteration over Arrays exists so that they can be more easily inspected
         as Python objects.
 
         See also #ak.to_list.
         """
-        if isinstance(self._layout, ak.contents.NumpyArray):
-            array = self._layout._raw(numpy)
-            array_param = self._layout.parameter("__array__")
-            if array_param == "byte":
-                for x in ak._util.tobytes(array):
-                    yield x
-            elif array_param == "char":
-                for x in ak._util.tobytes(array).decode(errors="surrogateescape"):
-                    yield x
-            else:
-                for x in array:
-                    yield x
-        else:
-            for x in self._layout:
-                if isinstance(x, ak.contents.NumpyArray):
-                    array_param = x.parameter("__array__")
-                    if array_param == "byte":
-                        yield ak._util.tobytes(x._raw(numpy))
-                    elif array_param == "char":
-                        yield ak._util.tobytes(x._raw(numpy)).decode(
-                            errors="surrogateescape"
-                        )
-                    else:
-                        yield wrap_layout(x, self._behavior)
-                else:
-                    yield wrap_layout(x, self._behavior, allow_other=True)
+        for item in self._layout:
+            yield wrap_layout(prepare_layout(item), self._behavior, allow_other=True)
 
     def __getitem__(self, where):
         """
         Args:
             where (many types supported; see below): Index of positions to
                 select from this Array.
 
@@ -943,27 +938,25 @@
              [[5.5]]]
 
         the sub-list at entry 0,0 is extended as the masked entries are
         acting at the last level, while the higher levels of the indexer all
         have the same dimension as the array being indexed.
         """
         with ak._errors.SlicingErrorContext(self, where):
-            out = self._layout[where]
-            if isinstance(out, ak.contents.NumpyArray):
-                array_param = out.parameter("__array__")
-                if array_param == "byte":
-                    return ak._util.tobytes(out._raw(numpy))
-                elif array_param == "char":
-                    return ak._util.tobytes(out._raw(numpy)).decode(
-                        errors="surrogateescape"
-                    )
-                else:
-                    return wrap_layout(out, self._behavior)
-            else:
-                return wrap_layout(out, self._behavior, allow_other=True)
+            return wrap_layout(
+                prepare_layout(self._layout[where]), self._behavior, allow_other=True
+            )
+
+    def __bytes__(self) -> bytes:
+        if isinstance(self._layout, ak.contents.NumpyArray) and self._layout.parameter(
+            "__array__"
+        ) in {"byte", "char"}:
+            return ak._util.tobytes(self._layout.data)
+        else:
+            return bytes(iter(self))
 
     def __setitem__(self, where, what):
         """
         Args:
             where (str or tuple of str): Field name to add to records in the array.
             what (#ak.Array): Array to add as the new field.
 
@@ -1362,17 +1355,14 @@
 
         This method conforms to NumPy's
         [NEP 18](https://numpy.org/neps/nep-0018-array-function-protocol.html)
         for overriding functions, which has been
         [available since NumPy 1.17](https://numpy.org/devdocs/release/1.17.0-notes.html#numpy-functions-now-always-support-overrides-with-array-function)
         (and
         [NumPy 1.16 with an experimental flag set](https://numpy.org/devdocs/release/1.16.0-notes.html#numpy-functions-now-support-overrides-with-array-function)).
-        This is not crucial for Awkward Array to work correctly, as NumPy
-        functions like np.concatenate can be manually replaced with
-        #ak.concatenate for early versions of NumPy.
 
         See also #__array_ufunc__.
         """
         return ak._connect.numpy.array_function(
             func, types, args, kwargs, behavior=self._behavior
         )
 
@@ -1741,27 +1731,17 @@
             3.3
             >>> record["y"]
             <Array [1, 2, 3] type='3 * int64'>
             >>> record["y", 1]
             2
         """
         with ak._errors.SlicingErrorContext(self, where):
-            out = self._layout[where]
-            if isinstance(out, ak.contents.NumpyArray):
-                array_param = out.parameter("__array__")
-                if array_param == "byte":
-                    return ak._util.tobytes(out._raw(numpy))
-                elif array_param == "char":
-                    return ak._util.tobytes(out._raw(numpy)).decode(
-                        errors="surrogateescape"
-                    )
-                else:
-                    return wrap_layout(out, self._behavior)
-            else:
-                return wrap_layout(out, self._behavior, allow_other=True)
+            return wrap_layout(
+                prepare_layout(self._layout[where]), self._behavior, allow_other=True
+            )
 
     def __setitem__(self, where, what):
         """
         Args:
             where (str or tuple of str): Field name to add data to the record.
             what: Data to add as the new field.
```

### Comparing `awkward-2.2.4/src/awkward/index.py` & `awkward-2.3.0/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/jax.py` & `awkward-2.3.0/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/record.py` & `awkward-2.3.0/src/awkward/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     regularize_backend,
 )
 from awkward._behavior import get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
-from awkward._typing import Self
+from awkward._typing import JSONSerializable, Self
 from awkward._util import UNSET
 from awkward.contents.content import Content
 
 np = NumpyMetadata.instance()
 
 
 class Record:
@@ -102,16 +102,19 @@
     @property
     def parameters(self):
         return self._array.parameters
 
     def parameter(self, key):
         return self._array.parameter(key)
 
-    def purelist_parameter(self, key):
-        return self._array.purelist_parameter(key)
+    def purelist_parameter(self, key) -> JSONSerializable:
+        return self._array.purelist_parameters(key)
+
+    def purelist_parameters(self, *keys):
+        return self._array.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._array.purelist_isregular
 
     @property
     def purelist_depth(self):
@@ -130,16 +133,15 @@
     def _touch_data(self, recursive):
         self._array._touch_data(recursive)
 
     def _touch_shape(self, recursive):
         self._array._touch_shape(recursive)
 
     def __getitem__(self, where):
-        with ak._errors.SlicingErrorContext(self, where):
-            return self._getitem(where)
+        return self._getitem(where)
 
     def _getitem(self, where):
         if is_integer(where):
             raise IndexError("scalar Record cannot be sliced by an integer")
 
         elif isinstance(where, slice):
             raise IndexError("scalar Record cannot be sliced by a range slice (`:`)")
```

### Comparing `awkward-2.2.4/src/awkward/typetracer.py` & `awkward-2.3.0/src/awkward/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/backend.py` & `awkward-2.3.0/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/cupy.py` & `awkward-2.3.0/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/dispatch.py` & `awkward-2.3.0/src/awkward/_backends/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/jax.py` & `awkward-2.3.0/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/numpy.py` & `awkward-2.3.0/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_backends/typetracer.py` & `awkward-2.3.0/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/avro.py` & `awkward-2.3.0/src/awkward/_connect/avro.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,15 @@
             aform = ak.forms.ListOffsetForm(
                 "i64",
                 ak.forms.NumpyForm(
                     "uint8",
                     parameters={"__array__": "char"},
                     form_key=f"node{form_next_id+1}",
                 ),
+                parameters={"__array__": "string"},
                 form_key=f"node{form_next_id}",
             )
             declarations.append(f"output node{form_next_id+1}-data uint8 \n")
             declarations.append(f"output node{form_next_id}-offsets int64 \n")
             form_keys.append(f"node{form_next_id+1}-data")
             form_keys.append(f"node{form_next_id}-offsets")
             init_code.append(f"0 node{form_next_id}-offsets <- stack\n")
@@ -789,14 +790,15 @@
                 ak.forms.ListOffsetForm(
                     "i64",
                     ak.forms.NumpyForm(
                         "uint8",
                         parameters={"__array__": "char"},
                         form_key=f"node{form_next_id+2}",
                     ),
+                    parameters={"__array__": "string"},
                     form_key=f"node{form_next_id+1}",
                 ),
                 parameters={"__array__": "categorical"},
                 form_key=f"node{form_next_id}",
             )
 
             form_keys.append(f"node{form_next_id}-index")
```

### Comparing `awkward-2.2.4/src/awkward/_connect/cling.py` & `awkward-2.3.0/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/hist.py` & `awkward-2.3.0/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/numexpr.py` & `awkward-2.3.0/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/pyarrow.py` & `awkward-2.3.0/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/__init__.py` & `awkward-2.3.0/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.3.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.3.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.3.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files 10% similar despite different names*

```diff
@@ -362,233 +362,27 @@
       /// @brief Form parameters.
       std::string parameters_;
 
       /// @brief Unique form ID.
       size_t id_;
     };
 
-    /// @class List
-    ///
-    /// @brief Builds a ListArray which generalizes ListOffsetArray.
-    /// Instead of a single offsets array, ListArray has -
-    /// starts which is the starting index of each list and
-    /// stops  which is the stopping index of each list.
-    ///
-    /// The starts and stops values can be 64-bit signed integers `int64`,
-    /// 32-bit signed integers `int32` or 32-bit unsigned integers `uint32`.
-    ///
-    /// @tparam PRIMITIVE The type of `starts` and `stops` buffer.
-    /// @tparam BUILDER The type of builder content.
-    template <typename PRIMITIVE, typename BUILDER>
-    class List {
-    public:
-      /// @brief Creates a new List layout builder by allocating new `starts`
-      /// and `stops` buffer, using `default_options` for initializing the buffer.
-      List()
-          : starts_(
-                awkward::GrowableBuffer<PRIMITIVE>(default_options)),
-            stops_(
-                awkward::GrowableBuffer<PRIMITIVE>(default_options)) {
-        size_t id = 0;
-        set_id(id);
-      }
-
-      /// @brief Creates a new List layout builder by allocating new `starts`
-      /// and `stops` buffer, taking `options` from
-      /// {@link BuilderOptions BuilderOptions} for initializing the buffer.
-      ///
-      /// @param options Initial size configuration of a buffer.
-      List(const awkward::BuilderOptions& options)
-          : starts_(awkward::GrowableBuffer<PRIMITIVE>(options)),
-            stops_(awkward::GrowableBuffer<PRIMITIVE>(options)) {
-        size_t id = 0;
-        set_id(id);
-      }
-
-      /// @brief Returns the reference to the builder content.
-      BUILDER&
-      content() noexcept {
-        return content_;
-      }
-
-      /// @brief Begins a list, appends the current length of the list
-      /// contents in the `starts` buffer and returns the reference to
-      /// the builder content.
-      BUILDER&
-      begin_list() noexcept {
-        starts_.append(content_.length());
-        return content_;
-      }
-
-      /// @brief Ends a list and appends the current length of the list
-      /// contents in the `stops` buffer.
-      void
-      end_list() noexcept {
-        stops_.append(content_.length());
-      }
-
-      /// @brief Parameters for the builder form.
-      const std::string&
-      parameters() const noexcept {
-        return parameters_;
-      }
-
-      /// @brief Sets the form parameters.
-      void
-      set_parameters(std::string parameter) noexcept {
-        parameters_ = parameter;
-      }
-
-      /// @brief Assigns a unique ID to each node.
-      void
-      set_id(size_t& id) noexcept {
-        id_ = id;
-        id++;
-        content_.set_id(id);
-      }
-
-      /// @brief Discards the accumulated starts and stops, and clears
-      /// the builder content.
-      void
-      clear() noexcept {
-        starts_.clear();
-        stops_.clear();
-        content_.clear();
-      }
-
-      /// @brief Current length of the content and `starts` buffer.
-      size_t
-      length() const noexcept {
-        return starts_.length();
-      }
-
-      /// @brief Checks for validity and consistency.
-      bool
-      is_valid(std::string& error) const noexcept {
-        if (starts_.length() != stops_.length()) {
-          std::stringstream out;
-          out << "List node" << id_ << " has starts length " << starts_.length()
-              << " but stops length " << stops_.length() << "\n";
-          error.append(out.str());
-
-          return false;
-        } else if (stops_.length() > 0 && content_.length() != stops_.last()) {
-          std::stringstream out;
-          out << "List node" << id_ << " has content length "
-              << content_.length() << " but last stops " << stops_.last()
-              << "\n";
-          error.append(out.str());
-
-          return false;
-        } else {
-          return content_.is_valid(error);
-        }
-      }
-
-      /// @brief Retrieves the names and sizes (in bytes) of the buffers used
-      /// in the builder and its contents.
-      void
-      buffer_nbytes(std::map<std::string, size_t>& names_nbytes) const
-          noexcept {
-        names_nbytes["node" + std::to_string(id_) + "-starts"] =
-            starts_.nbytes();
-        names_nbytes["node" + std::to_string(id_) + "-stops"] = stops_.nbytes();
-        content_.buffer_nbytes(names_nbytes);
-      }
-
-      /// @brief Copies and concatenates all the accumulated data in each of the
-      /// buffers of the builder and its contents to user-defined pointers.
-      ///
-      /// Used to fill the buffers map by allocating it with user-defined pointers
-      /// using the same names and sizes (in bytes) obtained from #buffer_nbytes.
-      void
-      to_buffers(std::map<std::string, void*>& buffers) const noexcept {
-        starts_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-starts"]));
-        stops_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-stops"]));
-        content_.to_buffers(buffers);
-      }
-
-      /// @brief Copies and concatenates all the accumulated data in the builder
-      /// to a map of user-allocated buffers.
-      ///
-      /// The map keys and the buffer sizes are obtained from #buffer_nbytes
-      void
-      to_char_buffers(std::map<std::string, uint8_t*>& buffers) const noexcept {
-        starts_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-starts"]));
-        stops_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-stops"]));
-        content_.to_char_buffers(buffers);
-      }
-
-      /// @brief Generates a unique description of the builder and its
-      /// contents in the form of a JSON-like string.
-      std::string
-      form() const noexcept {
-        std::stringstream form_key;
-        form_key << "node" << id_;
-        std::string params("");
-        if (parameters_ == "") {
-        } else {
-          params = std::string(", \"parameters\": { " + parameters_ + " }");
-        }
-        return "{ \"class\": \"ListArray\", \"starts\": \"" +
-               type_to_numpy_like<PRIMITIVE>() + "\", \"stops\": \"" +
-               type_to_numpy_like<PRIMITIVE>() +
-               "\", \"content\": " + content_.form() + params +
-               ", \"form_key\": \"" + form_key.str() + "\" }";
-      }
-
-    private:
-      /// @brief Buffer of `PRIMITIVE` type.
-      ///
-      /// It specifies the starting index of each list.
-      GrowableBuffer<PRIMITIVE> starts_;
-
-      /// @brief Buffer of `PRIMITIVE` type.
-      ///
-      /// It specifies the stopping index of each list.
-      GrowableBuffer<PRIMITIVE> stops_;
-
-      /// @brief The content of the ListArray.
-      BUILDER content_;
-
-      /// @brief Form parameters.
-      std::string parameters_;
-
-      /// @brief Unique form ID.
-      size_t id_;
-    };
 
     /// @class Empty
     ///
     /// @brief Builds an EmptyArray which has no content in it.
     /// It is used whenever an array's type is not known because it is empty.
     class Empty {
     public:
       /// @brief Creates a new Empty layout builder.
       Empty() {
         size_t id = 0;
         set_id(id);
       }
 
-      /// @brief Parameters for the builder form.
-      const std::string&
-      parameters() const noexcept {
-        return parameters_;
-      }
-
-      /// @brief Sets the form parameters.
-      void
-      set_parameters(std::string parameter) noexcept {
-        parameters_ = parameter;
-      }
-
       void
       set_id(size_t& /* id */) noexcept {}
 
       void
       clear() noexcept {}
 
       /// @brief Current length of the content.
@@ -617,149 +411,22 @@
       void
       to_char_buffers(std::map<std::string, uint8_t*>& /* buffers */) const noexcept {}
 
       /// @brief Generates a unique description of the builder and its
       /// contents in the form of a JSON-like string.
       std::string
       form() const noexcept {
-        std::string params("");
-        if (parameters_ == "") {
-        } else {
-          params = std::string(", \"parameters\": { " + parameters_ + " }");
-        }
-        return "{ \"class\": \"EmptyArray\"" + params + " }";
+        return "{ \"class\": \"EmptyArray\", \"parameters\": {} }";
       }
 
     private:
-      /// @brief Form parameters.
-      std::string parameters_;
-
       /// @brief Unique form ID.
       size_t id_;
     };
 
-    /// @class EmptyRecord
-    ///
-    /// @brief Builds an Empty RecordArray which has has `zero` contents.
-    /// It still represents a non-empty array. In this case, its length
-    /// is specified by #length.
-    ///
-    /// @tparam IS_TUPLE A boolean value which determines whether the builder
-    /// contains Tuples or Records.
-    template <bool IS_TUPLE>
-    class EmptyRecord {
-    public:
-      /// @brief Creates a new EmptyRecord layout builder.
-      EmptyRecord() : length_(0) {
-        size_t id = 0;
-        set_id(id);
-      }
-
-      /// @brief Inserts an empty record.
-      void
-      append() noexcept {
-        length_++;
-      }
-
-      /// @brief Inserts `size` number of empty records.
-      ///
-      /// Just an interface; not actually faster than calling append many times.
-      void
-      extend(size_t size) noexcept {
-        length_ += size;
-      }
-
-      /// @brief Parameters for the builder form.
-      const std::string&
-      parameters() const noexcept {
-        return parameters_;
-      }
-
-      /// @brief Sets the form parameters.
-      void
-      set_parameters(std::string parameter) noexcept {
-        parameters_ = parameter;
-      }
-
-      /// @brief Assigns a unique ID to each node.
-      void
-      set_id(size_t& id) noexcept {
-        id_ = id;
-        id++;
-      }
-
-      /// @brief Clears the builder contents, the #length returns to zero.
-      void
-      clear() noexcept {
-        length_ = 0;
-      }
-
-      /// @brief Current number of records.
-      size_t
-      length() const noexcept {
-        return length_;
-      }
-
-      /// @brief Checks for validity and consistency.
-      bool
-      is_valid(std::string& /* error */) const noexcept {
-        return true;
-      }
-
-      void
-      buffer_nbytes(std::map<std::string, size_t>& /* names_nbytes */) const
-          noexcept {}
-
-      void
-      to_buffers(std::map<std::string, void*>& /* buffers */) const noexcept {}
-
-      /// @brief Copies and concatenates all the accumulated data in the builder
-      /// to a map of user-allocated buffers.
-      ///
-      /// The map keys and the buffer sizes are obtained from #buffer_nbytes
-      void
-      to_char_buffers(std::map<std::string, uint8_t*>& buffers) const noexcept {}
-
-      /// @brief Generates a unique description of the builder and its
-      /// contents in the form of a JSON-like string.
-      std::string
-      form() const noexcept {
-        std::stringstream form_key;
-        form_key << "node" << id_;
-        std::string params("");
-        if (parameters_ == "") {
-        } else {
-          params = std::string(", \"parameters\": { " + parameters_ + " }");
-        }
-
-        if (is_tuple_) {
-          return "{ \"class\": \"RecordArray\", \"contents\": []" + params +
-                 ", \"form_key\": \"" + form_key.str() + "\" }";
-        } else {
-          return "{ \"class\": \"RecordArray\", \"contents\": {}" + params +
-                 ", \"form_key\": \"" + form_key.str() + "\" }";
-        }
-      }
-
-    private:
-      /// @brief Form parameters.
-      std::string parameters_;
-
-      /// @brief Unique form ID.
-      size_t id_;
-
-      /// @brief Current number of records.
-      size_t length_;
-
-      /// @brief Determines whether the builder contains Tuples or not.
-      ///
-      /// If the value is true, then the builder contains Tuples and if false,
-      /// it contains Records.
-      bool is_tuple_ = IS_TUPLE;
-    };
 
     /// @class Record
     ///
     /// @brief Builds a RecordArray which represents an array of records, which
     /// can be of same or different types. Its contents is an ordered list of arrays
     /// with the same length as the length of its shortest content; all are aligned
     /// element-by-element, associating a field name to every content.
@@ -794,39 +461,39 @@
         assert(content_names_.size() == fields_count_);
         size_t id = 0;
         set_id(id);
       }
 
       /// @brief Returns a vector of strings sontaining all the field names.
       const std::vector<std::string>
-      field_names() const noexcept {
+      fields() const noexcept {
         if (content_names_.empty()) {
-          return field_names_;
+          return fields_;
         } else {
           std::vector<std::string> result;
           for (auto it : content_names_) {
             result.emplace_back(it.second);
           }
           return result;
         }
       }
 
       /// @brief Sets the field names.
       ///
       /// Alternative method to set the field names besides passing the
       /// user-defined map as constructor parameter.
       void
-      set_field_names(MAP user_defined_field_id_to_name_map) noexcept {
+      set_fields(MAP user_defined_field_id_to_name_map) noexcept {
         content_names_ = user_defined_field_id_to_name_map;
       }
 
       /// @brief Returns the reference to the builder contents at `INDEX`.
       template <std::size_t INDEX>
       typename RecordFieldType<INDEX>::Builder&
-      field() noexcept {
+      content() noexcept {
         return std::get<INDEX>(contents).builder;
       }
 
       /// @brief Parameters for the builder form.
       const std::string&
       parameters() const noexcept {
         return parameters_;
@@ -878,15 +545,15 @@
         for (size_t i = 0; i < lengths.size(); i++) {
           if (length == -1) {
             length = lengths[i];
           }
           else if (length != (int64_t)lengths[i]) {
             std::stringstream out;
             out << "Record node" << id_ << " has field \""
-                << field_names().at(i) << "\" length " << lengths[i]
+                << fields().at(i) << "\" length " << lengths[i]
                 << " that differs from the first length " << length << "\n";
             error.append(out.str());
 
             return false;
           }
         }
 
@@ -968,15 +635,15 @@
 
     private:
       /// @brief Inserts the field names of all the record fields in a vector
       /// of strings.
       template <std::size_t... S>
       void
       map_fields(std::index_sequence<S...>) noexcept {
-        field_names_ = std::vector<std::string>(
+        fields_ = std::vector<std::string>(
             {std::string(std::get<S>(contents).index_as_field())...});
       }
 
       /// @brief Inserts the lengths of all the record fields in a vector and
       /// returns the vector.
       template <std::size_t... S>
       std::vector<size_t>
@@ -990,15 +657,15 @@
       field_is_valid(std::index_sequence<S...>, std::string& error) const
           noexcept {
         return std::vector<bool>(
             {std::get<S>(contents).builder.is_valid(error)...});
       }
 
       /// @brief Vector of strings of field names.
-      std::vector<std::string> field_names_;
+      std::vector<std::string> fields_;
 
       /// @brief User-defined map of record field names.
       UserDefinedMap content_names_;
 
       /// @brief Form parameters.
       std::string parameters_;
 
@@ -1028,15 +695,15 @@
         size_t id = 0;
         set_id(id);
       }
 
       /// @brief Returns the reference to the builder contents at `INDEX`.
       template <std::size_t INDEX>
       TupleContentType<INDEX>&
-      index() noexcept {
+      content() noexcept {
         return std::get<INDEX>(contents);
       }
 
       /// @brief Parameters for the builder form.
       const std::string&
       parameters() const noexcept {
         return parameters_;
@@ -1348,205 +1015,14 @@
       /// @brief Current number of lists of length `SIZE`.
       size_t length_;
 
       /// @brief Length of each list.
       size_t size_ = SIZE;
     };
 
-    /// @class Indexed
-    ///
-    /// @brief Builds an IndexedArray which consists of an `index` buffer. It is a
-    /// general-purpose tool for changing the order of and/or duplicating some content.
-    ///
-    /// The index values can be 64-bit signed integers `int64`, 32-bit signed integers
-    /// `int32` or 32-bit unsigned integers `uint32`.
-    ///
-    /// @tparam PRIMITIVE The type of `index` buffer.
-    /// @tparam BUILDER The type of builder content.
-    template <typename PRIMITIVE, typename BUILDER>
-    class Indexed {
-    public:
-      /// @brief Creates a new Indexed layout builder by allocating a new `index` buffer,
-      /// using `default_options` for initializing the buffer.
-      Indexed()
-          : index_(
-                awkward::GrowableBuffer<PRIMITIVE>(default_options)),
-            last_valid_(-1) {
-        size_t id = 0;
-        set_id(id);
-      }
-
-      /// @brief Creates a new Indexed layout builder by allocating a new `index`
-      /// buffer, taking `options` from {@link BuilderOptions BuilderOptions}
-      /// for initializing the buffer.
-      ///
-      /// @param options Initial size configuration of a buffer.
-      Indexed(const awkward::BuilderOptions& options)
-          : index_(awkward::GrowableBuffer<PRIMITIVE>(options)),
-            last_valid_(-1) {
-        size_t id = 0;
-        set_id(id);
-      }
-
-      /// @brief Returns the reference to the builder content.
-      BUILDER&
-      content() noexcept {
-        return content_;
-      }
-
-      /// @brief Inserts the last valid index in the `index` buffer and
-      /// returns the reference to the builder content.
-      BUILDER&
-      append_index() noexcept {
-        last_valid_ = content_.length();
-        index_.append(last_valid_);
-        return content_;
-      }
-
-      /// @brief Inserts `size` number of valid index in the `index` buffer
-      /// and returns the reference to the builder content.
-      ///
-      /// Just an interface; not actually faster than calling append many times.
-      BUILDER&
-      extend_index(size_t size) noexcept {
-        size_t start = content_.length();
-        size_t stop = start + size;
-        last_valid_ = stop - 1;
-        for (size_t i = start; i < stop; i++) {
-          index_.append(i);
-        }
-        return content_;
-      }
-
-      /// @brief Parameters for the builder form.
-      const std::string&
-      parameters() const noexcept {
-        return parameters_;
-      }
-
-      /// @brief Sets the form parameters.
-      void
-      set_parameters(std::string parameter) noexcept {
-        parameters_ = parameter;
-      }
-
-      /// @brief Assigns a unique ID to each node.
-      void
-      set_id(size_t& id) noexcept {
-        id_ = id;
-        id++;
-        content_.set_id(id);
-      }
-
-      /// @brief Discards the accumulated index and clears the content
-      /// of the builder. Also, last valid returns to `-1`.
-      void
-      clear() noexcept {
-        last_valid_ = -1;
-        index_.clear();
-        content_.clear();
-      }
-
-      /// @brief Current length of the content and the `index` buffer.
-      size_t
-      length() const noexcept {
-        return index_.length();
-      }
-
-      /// @brief Checks for validity and consistency.
-      bool
-      is_valid(std::string& error) const noexcept {
-        if (content_.length() != index_.length()) {
-          std::stringstream out;
-          out << "Indexed node" << id_ << " has content length "
-              << content_.length() << " but index length " << index_.length()
-              << "\n";
-          error.append(out.str());
-
-          return false;
-        } else if (content_.length() != last_valid_ + 1) {
-          std::stringstream out;
-          out << "Indexed node" << id_ << " has content length "
-              << content_.length() << " but last valid index is " << last_valid_
-              << "\n";
-          error.append(out.str());
-
-          return false;
-        } else {
-          return content_.is_valid(error);
-        }
-      }
-
-      /// @brief Retrieves the names and sizes (in bytes) of the buffers used
-      /// in the builder and its contents.
-      void
-      buffer_nbytes(std::map<std::string, size_t>& names_nbytes) const
-          noexcept {
-        names_nbytes["node" + std::to_string(id_) + "-index"] = index_.nbytes();
-        content_.buffer_nbytes(names_nbytes);
-      }
-
-      /// @brief Copies and concatenates all the accumulated data in each of the
-      /// buffers of the builder and its contents to user-defined pointers.
-      ///
-      /// Used to fill the buffers map by allocating it with user-defined pointers
-      /// using the same names and sizes (in bytes) obtained from #buffer_nbytes.
-      void
-      to_buffers(std::map<std::string, void*>& buffers) const noexcept {
-        index_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-index"]));
-        content_.to_buffers(buffers);
-      }
-
-      /// @brief Copies and concatenates all the accumulated data in the builder
-      /// to a map of user-allocated buffers.
-      ///
-      /// The map keys and the buffer sizes are obtained from #buffer_nbytes
-      void
-      to_char_buffers(std::map<std::string, uint8_t*>& buffers) const noexcept {
-        index_.concatenate(reinterpret_cast<PRIMITIVE*>(
-            buffers["node" + std::to_string(id_) + "-index"]));
-        content_.to_char_buffers(buffers);
-      }
-
-      /// @brief Generates a unique description of the builder and its
-      /// contents in the form of a JSON-like string.
-      std::string
-      form() const noexcept {
-        std::stringstream form_key;
-        form_key << "node" << id_;
-        std::string params("");
-        if (parameters_ == "") {
-        } else {
-          params = std::string(", \"parameters\": { " + parameters_ + " }");
-        }
-        return "{ \"class\": \"IndexedArray\", \"index\": \"" +
-               type_to_numpy_like<PRIMITIVE>() +
-               "\", \"content\": " + content_.form() + params +
-               ", \"form_key\": \"" + form_key.str() + "\" }";
-      }
-
-    private:
-      /// @brief Buffer of `PRIMITIVE` type.
-      ///
-      /// It specifies the index of each element.
-      GrowableBuffer<PRIMITIVE> index_;
-
-      /// @brief The content of the IndexedArray.
-      BUILDER content_;
-
-      /// @brief Form parameters.
-      std::string parameters_;
-
-      /// @brief Unique form ID.
-      size_t id_;
-
-      /// @brief Last valid index.
-      size_t last_valid_;
-    };
 
     /// @class IndexedOption
     ///
     /// @brief Builds an IndexedOptionArray which consists of an `index` buffer.
     /// The negative values in the index are interpreted as missing.
     ///
     /// The index values can be 64-bit signed integers `int64`, 32-bit signed
@@ -1584,46 +1060,46 @@
       content() noexcept {
         return content_;
       }
 
       /// @brief Inserts the last valid index in the `index` buffer and
       /// returns the reference to the builder content.
       BUILDER&
-      append_index() noexcept {
+      append_valid() noexcept {
         last_valid_ = content_.length();
         index_.append(last_valid_);
         return content_;
       }
 
       /// @brief Inserts `size` number of valid index in the `index` buffer
       /// and returns the reference to the builder content.
       ///
       /// Just an interface; not actually faster than calling append many times.
       BUILDER&
-      extend_index(size_t size) noexcept {
+      extend_valid(size_t size) noexcept {
         size_t start = content_.length();
         size_t stop = start + size;
         last_valid_ = stop - 1;
         for (size_t i = start; i < stop; i++) {
           index_.append(i);
         }
         return content_;
       }
 
       /// @brief Inserts `-1` in the `index` buffer.
       void
-      append_null() noexcept {
+      append_invalid() noexcept {
         index_.append(-1);
       }
 
       /// @brief Inserts `-1` in the `index` buffer `size` number of times
       ///
       /// Just an interface; not actually faster than calling append many times.
       void
-      extend_null(size_t size) noexcept {
+      extend_invalid(size_t size) noexcept {
         for (size_t i = 0; i < size; i++) {
           index_.append(-1);
         }
       }
 
       /// @brief Parameters for the builder form.
       const std::string&
@@ -1766,31 +1242,14 @@
 
       /// @brief Returns the reference to the builder content.
       BUILDER&
       content() noexcept {
         return content_;
       }
 
-      /// @brief Returns the reference to the builder content.
-      ///
-      /// After this, avalid element is inserted in the builder content.
-      BUILDER&
-      append_valid() noexcept {
-        return content_;
-      }
-      /// @brief Returns the reference to the builder content.
-      ///
-      /// After this, `size` number of valid elements are inserted in the builder content.
-      ///
-      /// Just an interface; not actually faster than calling append many times.
-      BUILDER&
-      extend_valid(size_t size) noexcept {
-        return content_;
-      }
-
       /// @brief Parameters for the builder form.
       const std::string&
       parameters() const noexcept {
         return parameters_;
       }
 
       /// @brief Sets the form parameters.
@@ -1951,26 +1410,26 @@
         return content_;
       }
 
       /// @brief Inserts !valid_when in the mask.
       ///
       /// After this, a dummy (invalid) value is inserted in the builder content.
       BUILDER&
-      append_null() noexcept {
+      append_invalid() noexcept {
         mask_.append(!valid_when_);
         return content_;
       }
 
       /// @brief Inserts `size` number of !valid_when in the mask.
       ///
       /// After this, `size` number of dummy (invalid) values are inserted in the builder content.
       ///
       /// Just an interface; not actually faster than calling append many times.
       BUILDER&
-      extend_null(size_t size) noexcept {
+      extend_invalid(size_t size) noexcept {
         for (size_t i = 0; i < size; i++) {
           mask_.append(!valid_when_);
         }
         return content_;
       }
 
       /// @brief Parameters for the builder form.
@@ -2199,29 +1658,29 @@
         return content_;
       }
 
       /// @brief Sets current_byte_ and cast_ default to null, no change in current_byte_.
       ///
       /// After this, a dummy (invalid) value is inserted in the builder content.
       BUILDER&
-      append_null() noexcept {
+      append_invalid() noexcept {
         append_begin();
         append_end();
         return content_;
       }
 
       /// @brief Sets current_byte_ and cast_ default to null, no change in current_byte_.
       ///
       /// After this, `size` number of dummy (invalid) values are inserted in the builder content.
       ///
       /// Just an interface; not actually faster than calling append many times.
       BUILDER&
-      extend_null(size_t size) noexcept {
+      extend_invalid(size_t size) noexcept {
         for (size_t i = 0; i < size; i++) {
-          append_null();
+          append_invalid();
         }
         return content_;
       }
 
       /// @brief Parameters for the builder form.
       const std::string&
       parameters() const noexcept {
@@ -2448,15 +1907,15 @@
         return std::get<I>(contents_);
       }
 
       /// @brief Inserts the current tag in the `tags` buffer and the next index in the
       /// `index` buffer and returns the reference to the content of the current builder.
       template <std::size_t TAG>
       ContentType<TAG>&
-      append_index() noexcept {
+      append_content() noexcept {
         auto& which_content = std::get<TAG>(contents_);
         INDEX next_index = which_content.length();
 
         TAGS tag = (TAGS)TAG;
         last_valid_index_[tag] = next_index;
         tags_.append(tag);
         index_.append(next_index);
```

### Comparing `awkward-2.2.4/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.3.0/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/jax/reducers.py` & `awkward-2.3.0/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/jax/trees.py` & `awkward-2.3.0/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/numba/arrayview.py` & `awkward-2.3.0/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.3.0/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/numba/builder.py` & `awkward-2.3.0/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.3.0/src/awkward/_connect/numba/growablebuffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     c.pyapi.decref(length_pos_obj)
     c.pyapi.decref(resize_obj)
 
     return out
 
 
 def _from_data():
-    ...
+    raise RuntimeError("_from_data Python function is only implemented in Numba")
 
 
 @numba.extending.type_callable(_from_data)
 def GrowableBuffer_from_data_typer(context):
     def typer(panels, length_pos, resize):
         if (
             isinstance(panels, numba.types.ListType)
```

### Comparing `awkward-2.2.4/src/awkward/_connect/numba/layout.py` & `awkward-2.3.0/src/awkward/_connect/numba/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,117 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import json
 
+import llvmlite.ir
 import numba
 
 import awkward as ak
 from awkward._behavior import overlay_behavior
 
 
+def string_numba_typer(viewtype):
+    if viewtype.type.parameters["__array__"] == "string":
+        return numba.types.string
+    else:
+        return numba.cpython.charseq.bytes_type
+
+
+def string_numba_lower(
+    context, builder, rettype, viewtype, viewval, viewproxy, attype, atval
+):
+    whichpos = ak._connect.numba.layout.posat(
+        context, builder, viewproxy.pos, viewtype.type.CONTENT
+    )
+    nextpos = ak._connect.numba.layout.getat(
+        context, builder, viewproxy.arrayptrs, whichpos
+    )
+
+    whichnextpos = ak._connect.numba.layout.posat(
+        context, builder, nextpos, viewtype.type.contenttype.ARRAY
+    )
+
+    startspos = ak._connect.numba.layout.posat(
+        context, builder, viewproxy.pos, viewtype.type.STARTS
+    )
+    startsptr = ak._connect.numba.layout.getat(
+        context, builder, viewproxy.arrayptrs, startspos
+    )
+    startsarraypos = builder.add(viewproxy.start, atval)
+    start = ak._connect.numba.layout.getat(
+        context, builder, startsptr, startsarraypos, viewtype.type.indextype.dtype
+    )
+
+    stopspos = ak._connect.numba.layout.posat(
+        context, builder, viewproxy.pos, viewtype.type.STOPS
+    )
+    stopsptr = ak._connect.numba.layout.getat(
+        context, builder, viewproxy.arrayptrs, stopspos
+    )
+    stopsarraypos = builder.add(viewproxy.start, atval)
+    stop = ak._connect.numba.layout.getat(
+        context, builder, stopsptr, stopsarraypos, viewtype.type.indextype.dtype
+    )
+
+    baseptr = ak._connect.numba.layout.getat(
+        context, builder, viewproxy.arrayptrs, whichnextpos
+    )
+    rawptr = builder.add(
+        baseptr,
+        ak._connect.numba.layout.castint(
+            context, builder, viewtype.type.indextype.dtype, numba.intp, start
+        ),
+    )
+    rawptr_cast = builder.inttoptr(
+        rawptr,
+        llvmlite.ir.PointerType(llvmlite.ir.IntType(numba.intp.bitwidth // 8)),
+    )
+    strsize = builder.sub(stop, start)
+    strsize_cast = ak._connect.numba.layout.castint(
+        context, builder, viewtype.type.indextype.dtype, numba.intp, strsize
+    )
+
+    pyapi = context.get_python_api(builder)
+    gil = pyapi.gil_ensure()
+
+    strptr = builder.bitcast(rawptr_cast, pyapi.cstring)
+
+    if viewtype.type.parameters["__array__"] == "string":
+        kind = context.get_constant(numba.types.int32, pyapi.py_unicode_1byte_kind)
+        pystr = pyapi.string_from_kind_and_data(kind, strptr, strsize_cast)
+    else:
+        pystr = pyapi.bytes_from_string_and_size(strptr, strsize_cast)
+
+    out = pyapi.to_native_value(rettype, pystr).value
+
+    pyapi.decref(pystr)
+
+    pyapi.gil_release(gil)
+
+    return out
+
+
 def find_numba_array_typer(layouttype, behavior):
     behavior = overlay_behavior(behavior)
-    arr = layouttype.parameters.get("__array__")
+    arr = layouttype.parameters.get("__list__")
     if isinstance(arr, str):
         typer = behavior.get(("__numba_typer__", arr))
         if callable(typer):
             return typer
     deeprec = layouttype.parameters.get("__record__")
     if isinstance(deeprec, str):
         typer = behavior.get(("__numba_typer__", "*", deeprec))
         if callable(typer):
             return typer
     return None
 
 
 def find_numba_array_lower(layouttype, behavior):
     behavior = overlay_behavior(behavior)
-    arr = layouttype.parameters.get("__array__")
+    arr = layouttype.parameters.get("__list__")
     if isinstance(arr, str):
         lower = behavior.get(("__numba_lower__", arr))
         if callable(lower):
             return lower
     deeprec = layouttype.parameters.get("__record__")
     if isinstance(deeprec, str):
         lower = behavior.get(("__numba_lower__", "*", deeprec))
@@ -98,14 +180,22 @@
         elif arraytype.dtype.bitwidth == 64:
             return ak.index.Index64
         else:
             raise AssertionError(f"no Index* type for array: {arraytype}")
 
     def getitem_at_check(self, viewtype):
         typer = find_numba_array_typer(viewtype.type, viewtype.behavior)
+
+        # Allow strings to override typer
+        if typer is None and viewtype.type.parameters.get("__array__") in {
+            "string",
+            "bytestring",
+        }:
+            typer = string_numba_typer
+
         if typer is None:
             return self.getitem_at(viewtype)
         else:
             return typer(viewtype)
 
     def getitem_range(self, viewtype):
         return ak._connect.numba.arrayview.wrap(self, viewtype, None)
@@ -128,34 +218,42 @@
         viewproxy,
         attype,
         atval,
         wrapneg,
         checkbounds,
     ):
         lower = find_numba_array_lower(viewtype.type, viewtype.behavior)
-        if lower is not None:
-            atval = regularize_atval(
-                context, builder, viewproxy, attype, atval, wrapneg, checkbounds
-            )
-            return lower(
-                context, builder, rettype, viewtype, viewval, viewproxy, attype, atval
-            )
-        else:
+
+        # Allow strings to override lower
+        if lower is None and viewtype.type.parameters.get("__array__") in {
+            "string",
+            "bytestring",
+        }:
+            lower = string_numba_lower
+
+        if lower is None:
             return self.lower_getitem_at(
                 context,
                 builder,
                 rettype,
                 viewtype,
                 viewval,
                 viewproxy,
                 attype,
                 atval,
                 wrapneg,
                 checkbounds,
             )
+        else:
+            atval = regularize_atval(
+                context, builder, viewproxy, attype, atval, wrapneg, checkbounds
+            )
+            return lower(
+                context, builder, rettype, viewtype, viewval, viewproxy, attype, atval
+            )
 
     def lower_getitem_range(
         self,
         context,
         builder,
         rettype,
         viewtype,
```

### Comparing `awkward-2.2.4/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.3.0/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.3.0/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.3.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/__init__.py` & `awkward-2.3.0/src/awkward/_nplikes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from awkward._typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from awkward._nplikes.numpylike import ArrayLike, NumpyLike
 
 
 def to_nplike(
-    array: ArrayLike, nplike: NumpyLike, *, from_nplike: NumpyLike = None
+    array: ArrayLike, nplike: NumpyLike, *, from_nplike: NumpyLike | None = None
 ) -> ArrayLike:
     if from_nplike is None:
         from_nplike = nplike_of(array, default=None)
         if from_nplike is None:
             raise TypeError(
                 f"internal error: expected an array supported by an existing nplike, got {type(array).__name__!r}"
             )
```

### Comparing `awkward-2.2.4/src/awkward/_nplikes/array_module.py` & `awkward-2.3.0/src/awkward/_nplikes/array_module.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/cupy.py` & `awkward-2.3.0/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/dispatch.py` & `awkward-2.3.0/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/jax.py` & `awkward-2.3.0/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/numpylike.py` & `awkward-2.3.0/src/awkward/_nplikes/numpylike.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/placeholder.py` & `awkward-2.3.0/src/awkward/_nplikes/placeholder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/shape.py` & `awkward-2.3.0/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/typetracer.py` & `awkward-2.3.0/src/awkward/_nplikes/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/_nplikes/ufuncs.py` & `awkward-2.3.0/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/behaviors/mixins.py` & `awkward-2.3.0/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/__init__.py` & `awkward-2.3.0/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/bitmaskedarray.py` & `awkward-2.3.0/src/awkward/contents/bitmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/bytemaskedarray.py` & `awkward-2.3.0/src/awkward/contents/bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/content.py` & `awkward-2.3.0/src/awkward/contents/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,18 @@
             pass
         elif not isinstance(parameters, dict):
             raise TypeError(
                 "{} 'parameters' must be a dict or None, not {}".format(
                     type(self).__name__, repr(parameters)
                 )
             )
-        else:
-            if not self.is_list and parameters.get("__array__") in (
+        # Validate built-in `__array__`
+        elif parameters.get("__array__") is not None:
+            array_name = parameters["__array__"]
+            if not self.is_list and array_name in (
                 "string",
                 "bytestring",
             ):
                 raise TypeError(
                     '{} is not allowed to have parameters["__array__"] = "{}"'.format(
                         type(self).__name__, parameters["__array__"]
                     )
@@ -115,26 +117,39 @@
                 "__array__"
             ) in ("char", "byte"):
                 raise TypeError(
                     '{} is not allowed to have parameters["__array__"] = "{}"'.format(
                         type(self).__name__, parameters["__array__"]
                     )
                 )
-            if not self.is_indexed and parameters.get("__array__") == "categorical":
+            if not self.is_indexed and array_name == "categorical":
                 raise TypeError(
                     '{} is not allowed to have parameters["__array__"] = "{}"'.format(
                         type(self).__name__, parameters["__array__"]
                     )
                 )
-            if not self.is_record and parameters.get("__array__") == "sorted_map":
+            if not self.is_record and array_name == "sorted_map":
                 raise TypeError(
                     '{} is not allowed to have parameters["__array__"] = "{}"'.format(
                         type(self).__name__, parameters["__array__"]
                     )
                 )
+        # TODO: enable this once we can guarantee this doesn't happen during broadcasting
+        # elif not (self.is_list or parameters.get("__list__") is None):
+        #     raise TypeError(
+        #         '{} is not allowed to have parameters["__list__"] = "{}"'.format(
+        #             type(self).__name__, parameters["__list__"]
+        #         )
+        #     )
+        # elif not (self.is_record or parameters.get("__record__") is None):
+        #     raise TypeError(
+        #         '{} is not allowed to have parameters["__record__"] = "{}"'.format(
+        #             type(self).__name__, parameters["__record__"]
+        #         )
+        #     )
 
         if not isinstance(backend, Backend):
             raise TypeError(
                 "{} 'backend' must be a Backend, not {}".format(
                     type(self).__name__, repr(backend)
                 )
             )
@@ -900,39 +915,41 @@
         recordlookup: list[str] | None,
         parameters: dict[str, Any] | None,
         axis: int,
         depth: int,
     ):
         raise NotImplementedError
 
-    def _validity_error_parameters(self, path: str) -> str:
-        if self.parameter("__array__") == "categorical":
-            if not ak._do.is_unique(self._content):
-                return 'at {} ("{}"): __array__ = "categorical" requires contents to be unique'.format(
-                    path, type(self)
-                )
-        return ""
-
     def _validity_error(self, path: str) -> str:
         raise NotImplementedError
 
     @property
     def nbytes(self) -> int:
         return self._nbytes_part()
 
     def purelist_parameter(self, key: str):
         """
         Return the value of the outermost parameter matching `key` in a sequence
         of nested lists, stopping at the first record or tuple layer.
 
-         If a layer has #ak.types.UnionType, the value is only returned if all
+        If a layer has #ak.types.UnionType, the value is only returned if all
         possibilities have the same value.
         """
         return self.form_cls.purelist_parameter(self, key)
 
+    def purelist_parameters(self, *keys: str):
+        """
+        Return the value of the outermost parameter matching one of `keys` in a sequence
+        of nested lists, stopping at the first record or tuple layer.
+
+        If a layer has #ak.types.UnionType, the value is only returned if all
+        possibilities have the same value.
+        """
+        return self.form_cls.purelist_parameters(self, *keys)
+
     def _is_unique(
         self,
         negaxis: AxisMaybeNone,
         starts: Index,
         parents: Index,
         outlength: int,
     ) -> bool:
```

### Comparing `awkward-2.2.4/src/awkward/contents/emptyarray.py` & `awkward-2.3.0/src/awkward/contents/emptyarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-import copy
 from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
-from awkward._errors import AxisError, deprecate
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
@@ -66,66 +65,60 @@
     """
 
     is_unknown = True
     is_leaf = True
 
     def __init__(self, *, parameters=None, backend=None):
         if not (parameters is None or len(parameters) == 0):
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
-            )
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         if backend is None:
             backend = NumpyBackend.instance()
         self._init(parameters, backend)
 
     form_cls: Final = EmptyForm
 
     def copy(
         self,
         *,
         parameters=UNSET,
         backend=UNSET,
     ):
         if not (parameters is UNSET or parameters is None or len(parameters) == 0):
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
-            )
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         return EmptyArray(
-            parameters=self._parameters if parameters is UNSET else parameters,
             backend=self._backend if backend is UNSET else backend,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
-        return self.copy(parameters=copy.deepcopy(self._parameters, memo))
+        return self.copy()
 
     @classmethod
     def simplified(cls, *, parameters=None, backend=None):
         if not (parameters is None or len(parameters) == 0):
-            deprecate(f"{cls.__name__} cannot contain parameters", version="2.2.0")
-        return cls(parameters=parameters, backend=backend)
+            raise TypeError(f"{cls.__name__} cannot contain parameters")
+        return cls(backend=backend)
 
     def _form_with_key(self, getkey: Callable[[Content], str | None]) -> EmptyForm:
-        return self.form_cls(parameters=self._parameters, form_key=getkey(self))
+        return self.form_cls(form_key=getkey(self))
 
     def _to_buffers(
         self,
         form: Form,
         getkey: Callable[[Content, Form, str], str],
         container: MutableMapping[str, ArrayLike],
         backend: Backend,
         byteorder: str,
     ):
         assert isinstance(form, self.form_cls)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         return EmptyArray(
-            parameters=self._parameters,
             backend=TypeTracerBackend.instance(),
         )
 
     def _touch_data(self, recursive: bool):
         pass
 
     def _touch_shape(self, recursive: bool):
@@ -249,30 +242,30 @@
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError(self, "axis=0 not allowed for flatten")
         else:
             offsets = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
             return (
                 offsets,
-                EmptyArray(parameters=self._parameters, backend=self._backend),
+                EmptyArray(backend=self._backend),
             )
 
     def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         return True
 
     def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
         elif len(others) == 1:
             return others[0]
         else:
             return others[0]._mergemany(others[1:])
 
     def _fill_none(self, value: Content) -> Content:
-        return EmptyArray(parameters=self._parameters, backend=self._backend)
+        return EmptyArray(backend=self._backend)
 
     def _local_index(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return ak.contents.NumpyArray(
                 self._backend.nplike.empty(0, dtype=np.int64),
                 parameters=None,
@@ -301,17 +294,15 @@
             negaxis, starts, shifts, parents, outlength, ascending, stable
         )
 
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
         return self
 
     def _combinations(self, n, replacement, recordlookup, parameters, axis, depth):
-        return ak.contents.EmptyArray(
-            parameters=self._parameters, backend=self._backend
-        )
+        return ak.contents.EmptyArray(backend=self._backend)
 
     def _reduce_next(
         self,
         reducer,
         negaxis,
         starts,
         shifts,
@@ -384,15 +375,15 @@
     ):
         if options["return_array"]:
 
             def continuation():
                 if options["keep_parameters"]:
                     return self
                 else:
-                    return EmptyArray(parameters=None, backend=self._backend)
+                    return EmptyArray(backend=self._backend)
 
         else:
 
             def continuation():
                 pass
 
         result = action(
@@ -418,11 +409,11 @@
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
             raise TypeError("cannot convert typetracer arrays to Python lists")
         return []
 
     def _to_backend(self, backend: Backend) -> Self:
-        return EmptyArray(parameters=self._parameters, backend=backend)
+        return EmptyArray(backend=backend)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return True
```

### Comparing `awkward-2.2.4/src/awkward/contents/indexedarray.py` & `awkward-2.3.0/src/awkward/contents/indexedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,15 @@
                 )
             )
             next = self._content._carry(nextcarry, False)
             return next.copy(
                 parameters=parameters_union(
                     next._parameters,
                     self._parameters,
-                    exclude=(("__array__", "categorical"),),
+                    exclude={("__array__", "categorical")},
                 )
             )
 
     def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
@@ -945,14 +945,19 @@
             outlength,
             mask,
             keepdims,
             behavior,
         )
 
     def _validity_error(self, path):
+        if self.parameter("__array__") == "categorical":
+            if not ak._do.is_unique(self._content):
+                return 'at {} ("{}"): __array__ = "categorical" requires contents to be unique'.format(
+                    path, type(self)
+                )
         error = self._backend["awkward_IndexedArray_validity", self.index.dtype.type](
             self.index.data, self.index.length, self._content.length, False
         )
         if error.str is not None:
             if error.filename is None:
                 filename = ""
             else:
```

### Comparing `awkward-2.2.4/src/awkward/contents/indexedoptionarray.py` & `awkward-2.3.0/src/awkward/contents/indexedoptionarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1458,14 +1458,20 @@
             next = self._content._carry(nextcarry, True)
             out = next._combinations(
                 n, replacement, recordlookup, parameters, axis, depth
             )
             return IndexedOptionArray.simplified(outindex, out, parameters=parameters)
 
     def _validity_error(self, path):
+        if self.parameter("__array__") == "categorical":
+            if not ak._do.is_unique(self._content):
+                return 'at {} ("{}"): __array__ = "categorical" requires contents to be unique'.format(
+                    path, type(self)
+                )
+
         assert self.index.nplike is self._backend.index_nplike
         error = self._backend["awkward_IndexedArray_validity", self.index.dtype.type](
             self.index.data, self.index.length, self._content.length, True
         )
         if error.str is not None:
             if error.filename is None:
                 filename = ""
```

### Comparing `awkward-2.2.4/src/awkward/contents/listarray.py` & `awkward-2.3.0/src/awkward/contents/listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/listoffsetarray.py` & `awkward-2.3.0/src/awkward/contents/listoffsetarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,20 @@
             )
         else:
             return ListOffsetArray(
                 self._offsets.to64(), self._content, parameters=self._parameters
             )
 
     def to_RegularArray(self):
-        start, stop = self._offsets[0], self._offsets[self._offsets.length - 1]
+        start, stop = (
+            self._offsets[0],
+            self._offsets[
+                self._backend.index_nplike.shape_item_as_index(self._offsets.length - 1)
+            ],
+        )
         content = self._content._getitem_range(start, stop)
         _size = Index64.empty(1, self._backend.index_nplike)
         assert (
             _size.nplike is self._backend.index_nplike
             and self._offsets.nplike is self._backend.index_nplike
         )
         self._backend.maybe_kernel_error(
@@ -2134,39 +2139,33 @@
 
         nextcontent = self._content._getitem_range(mini, maxi)
 
         if self.parameter("__array__") == "bytestring":
             convert_bytes = (
                 None if json_conversions is None else json_conversions["convert_bytes"]
             )
-            content = ak._util.tobytes(nextcontent.data)
+            data = nextcontent.data
             out = [None] * starts.length
             if convert_bytes is None:
                 for i in range(starts.length):
-                    out[i] = content[starts_data[i] : stops_data[i]]
+                    out[i] = ak._util.tobytes(data[starts_data[i] : stops_data[i]])
             else:
                 for i in range(starts.length):
-                    out[i] = convert_bytes(content[starts_data[i] : stops_data[i]])
+                    out[i] = convert_bytes(
+                        ak._util.tobytes(data[starts_data[i] : stops_data[i]])
+                    )
             return out
 
         elif self.parameter("__array__") == "string":
             data = nextcontent.data
-            if hasattr(data, "tobytes"):
-
-                def tostring(x):
-                    return x.tobytes().decode(errors="surrogateescape")
-
-            else:
-
-                def tostring(x):
-                    return x.tostring().decode(errors="surrogateescape")
-
             out = [None] * starts.length
             for i in range(starts.length):
-                out[i] = tostring(data[starts_data[i] : stops_data[i]])
+                out[i] = ak._util.tobytes(data[starts_data[i] : stops_data[i]]).decode(
+                    errors="surrogateescape"
+                )
             return out
 
         else:
             out = self._to_list_custom(behavior, json_conversions)
             if out is not None:
                 return out
```

### Comparing `awkward-2.2.4/src/awkward/contents/numpyarray.py` & `awkward-2.3.0/src/awkward/contents/numpyarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,17 +670,15 @@
         )
         out2 = NumpyArray(out, parameters=self._parameters, backend=self._backend)
 
         return out2, nextoffsets[: outlength[0]]
 
     def _numbers_to_type(self, name, including_unknown):
         if (
-            self.parameter("__array__") == "string"
-            or self.parameter("__array__") == "bytestring"
-            or self.parameter("__array__") == "char"
+            self.parameter("__array__") == "char"
             or self.parameter("__array__") == "byte"
         ):
             return self
         else:
             dtype = primitive_to_dtype(name)
             return NumpyArray(
                 self._backend.nplike.asarray(self._data, dtype=dtype),
@@ -1288,61 +1286,60 @@
                 return ak._util.tobytes(self._data)
             else:
                 return convert_bytes(ak._util.tobytes(self._data))
 
         elif self.parameter("__array__") == "char":
             return ak._util.tobytes(self._data).decode(errors="surrogateescape")
 
-        else:
-            out = self._to_list_custom(behavior, json_conversions)
-            if out is not None:
-                return out
-
-            if json_conversions is not None:
-                complex_real_string = json_conversions["complex_real_string"]
-                complex_imag_string = json_conversions["complex_imag_string"]
-                if complex_real_string is not None:
-                    if issubclass(self.dtype.type, np.complexfloating):
-                        return ak.contents.RecordArray(
-                            [
-                                ak.contents.NumpyArray(
-                                    self._data.real, backend=self._backend
-                                ),
-                                ak.contents.NumpyArray(
-                                    self._data.imag, backend=self._backend
-                                ),
-                            ],
-                            [complex_real_string, complex_imag_string],
-                            self.length,
-                            parameters=self._parameters,
-                            backend=self._backend,
-                        )._to_list(behavior, json_conversions)
-
-            out = self._data.tolist()
-
-            if json_conversions is not None:
-                nan_string = json_conversions["nan_string"]
-                if nan_string is not None:
-                    for i in self._backend.nplike.nonzero(
-                        self._backend.nplike.isnan(self._data)
-                    )[0]:
-                        out[i] = nan_string
-
-                posinf_string = json_conversions["posinf_string"]
-                if posinf_string is not None:
-                    for i in self._backend.nplike.nonzero(self._data == np.inf)[0]:
-                        out[i] = posinf_string
-
-                neginf_string = json_conversions["neginf_string"]
-                if neginf_string is not None:
-                    for i in self._backend.nplike.nonzero(self._data == -np.inf)[0]:
-                        out[i] = neginf_string
-
+        out = self._to_list_custom(behavior, json_conversions)
+        if out is not None:
             return out
 
+        if json_conversions is not None:
+            complex_real_string = json_conversions["complex_real_string"]
+            complex_imag_string = json_conversions["complex_imag_string"]
+            if complex_real_string is not None:
+                if issubclass(self.dtype.type, np.complexfloating):
+                    return ak.contents.RecordArray(
+                        [
+                            ak.contents.NumpyArray(
+                                self._data.real, backend=self._backend
+                            ),
+                            ak.contents.NumpyArray(
+                                self._data.imag, backend=self._backend
+                            ),
+                        ],
+                        [complex_real_string, complex_imag_string],
+                        self.length,
+                        parameters=self._parameters,
+                        backend=self._backend,
+                    )._to_list(behavior, json_conversions)
+
+        out = self._data.tolist()
+
+        if json_conversions is not None:
+            nan_string = json_conversions["nan_string"]
+            if nan_string is not None:
+                for i in self._backend.nplike.nonzero(
+                    self._backend.nplike.isnan(self._data)
+                )[0]:
+                    out[i] = nan_string
+
+            posinf_string = json_conversions["posinf_string"]
+            if posinf_string is not None:
+                for i in self._backend.nplike.nonzero(self._data == np.inf)[0]:
+                    out[i] = posinf_string
+
+            neginf_string = json_conversions["neginf_string"]
+            if neginf_string is not None:
+                for i in self._backend.nplike.nonzero(self._data == -np.inf)[0]:
+                    out[i] = neginf_string
+
+        return out
+
     def _to_backend(self, backend: Backend) -> Self:
         return NumpyArray(
             self._raw(backend.nplike),
             parameters=self._parameters,
             backend=backend,
         )
```

### Comparing `awkward-2.2.4/src/awkward/contents/recordarray.py` & `awkward-2.3.0/src/awkward/contents/recordarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/regulararray.py` & `awkward-2.3.0/src/awkward/contents/regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/contents/unionarray.py` & `awkward-2.3.0/src/awkward/contents/unionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import ctypes
 from collections.abc import Iterable, MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError, deprecate
 from awkward._layout import maybe_posaxis
-from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
@@ -1514,46 +1513,18 @@
                 ak._connect.pyarrow.to_length(nptags, length),
                 ak._connect.pyarrow.to_length(npindex, length),
             ],
             children=values,
         )
 
     def _to_backend_array(self, allow_missing, backend):
-        ak._errors.deprecate(
-            "Conversion of irreducible unions to backend arrays is deprecated.", "2.2.0"
+        raise TypeError(
+            "Conversion of irreducible unions to backend arrays is not supported."
         )
 
-        contents = [
-            self.project(i)._to_backend_array(allow_missing, backend)
-            for i in range(len(self.contents))
-        ]
-
-        if any(isinstance(x, backend.nplike.ma.MaskedArray) for x in contents):
-            try:
-                out = backend.nplike.ma.concatenate(contents)
-            except Exception as err:
-                raise ValueError(
-                    f"cannot convert {self} into numpy.ma.MaskedArray"
-                ) from err
-        else:
-            try:
-                out = backend.nplike.concat(contents)
-            except Exception as err:
-                raise ValueError(f"cannot convert {self} into np.ndarray") from err
-
-        tags = backend.index_nplike.asarray(self.tags)
-        for tag, content in enumerate(contents):
-            mask = tags == tag
-            if Jax.is_own_array(out):
-                out = out.at[mask].set(content)
-            else:
-                out[mask] = content
-
-        return out
-
     def _remove_structure(self, backend, options):
         out = []
         for i in range(len(self._contents)):
             index = self._index[self._tags.data == i]
             out.extend(
                 self._contents[i]
                 ._carry(index, False)
```

### Comparing `awkward-2.2.4/src/awkward/contents/unmaskedarray.py` & `awkward-2.3.0/src/awkward/contents/unmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/forms/__init__.py` & `awkward-2.3.0/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/forms/bitmaskedform.py` & `awkward-2.3.0/src/awkward/forms/bytemaskedform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import Self, final
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class BitMaskedForm(Form):
+class ByteMaskedForm(Form):
     is_option = True
 
     def __init__(
         self,
         mask,
         content,
         valid_when,
-        lsb_order,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(mask, str):
             raise TypeError(
                 "{} 'mask' must be of type str, not {}".format(
@@ -34,141 +33,121 @@
             )
         if not isinstance(valid_when, bool):
             raise TypeError(
                 "{} 'valid_when' must be bool, not {}".format(
                     type(self).__name__, repr(valid_when)
                 )
             )
-        if not isinstance(lsb_order, bool):
-            raise TypeError(
-                "{} 'lsb_order' must be bool, not {}".format(
-                    type(self).__name__, repr(lsb_order)
-                )
-            )
 
         self._mask = mask
         self._content = content
         self._valid_when = valid_when
-        self._lsb_order = lsb_order
         self._init(parameters=parameters, form_key=form_key)
 
     @property
     def mask(self):
         return self._mask
 
     @property
     def content(self):
         return self._content
 
     @property
     def valid_when(self):
         return self._valid_when
 
-    @property
-    def lsb_order(self):
-        return self._lsb_order
-
     def copy(
         self,
         mask=UNSET,
         content=UNSET,
         valid_when=UNSET,
-        lsb_order=UNSET,
         *,
         parameters=UNSET,
         form_key=UNSET,
     ):
-        return BitMaskedForm(
+        return ByteMaskedForm(
             self._mask if mask is UNSET else mask,
             self._content if content is UNSET else content,
             self._valid_when if valid_when is UNSET else valid_when,
-            self._lsb_order if lsb_order is UNSET else lsb_order,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         mask,
         content,
         valid_when,
-        lsb_order,
         *,
         parameters=None,
         form_key=None,
     ):
         if content.is_union:
             return content._union_of_optionarrays("i64", parameters)
         elif content.is_indexed or content.is_option:
             return ak.forms.IndexedOptionForm.simplified(
                 "i64",
                 content,
                 parameters=parameters,
             )
         else:
             return cls(
-                mask,
-                content,
-                valid_when,
-                lsb_order,
-                parameters=parameters,
-                form_key=form_key,
+                mask, content, valid_when, parameters=parameters, form_key=form_key
             )
 
     @property
     def is_identity_like(self):
         return False
 
     def __repr__(self):
         args = [
             repr(self._mask),
             repr(self._content),
             repr(self._valid_when),
-            repr(self._lsb_order),
             *self._repr_args(),
         ]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "BitMaskedArray",
+                "class": "ByteMaskedArray",
                 "mask": self._mask,
                 "valid_when": self._valid_when,
-                "lsb_order": self._lsb_order,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
         return ak.types.OptionType(
             self._content.type, parameters=self._parameters
         ).simplify_option_union()
 
     def __eq__(self, other):
-        if isinstance(other, BitMaskedForm):
+        if isinstance(other, ByteMaskedForm):
             return (
                 self._form_key == other._form_key
                 and self._mask == other._mask
                 and self._valid_when == other._valid_when
-                and self._lsb_order == other._lsb_order
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
@@ -198,28 +177,26 @@
         self._content._columns(path, output, list_indicator)
 
     def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
         next_content = self._content._prune_columns(is_inside_record_or_union)
         if next_content is None:
             return None
         else:
-            return BitMaskedForm(
+            return ByteMaskedForm(
                 self._mask,
                 next_content,
                 self._valid_when,
-                self._lsb_order,
                 parameters=self._parameters,
                 form_key=self._form_key,
             )
 
     def _select_columns(self, match_specifier):
-        return BitMaskedForm(
+        return ByteMaskedForm(
             self._mask,
             self._content._select_columns(match_specifier),
             self._valid_when,
-            self._lsb_order,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         return self._content._column_types()
```

### Comparing `awkward-2.2.4/src/awkward/forms/bytemaskedform.py` & `awkward-2.3.0/src/awkward/forms/indexedoptionform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,161 +1,152 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._parameters import type_parameters_equal
-from awkward._typing import Self, final
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class ByteMaskedForm(Form):
+class IndexedOptionForm(Form):
     is_option = True
+    is_indexed = True
 
     def __init__(
         self,
-        mask,
+        index,
         content,
-        valid_when,
         *,
         parameters=None,
         form_key=None,
     ):
-        if not isinstance(mask, str):
+        if not isinstance(index, str):
             raise TypeError(
-                "{} 'mask' must be of type str, not {}".format(
-                    type(self).__name__, repr(mask)
+                "{} 'index' must be of type str, not {}".format(
+                    type(self).__name__, repr(index)
                 )
             )
         if not isinstance(content, Form):
             raise TypeError(
                 "{} all 'contents' must be Form subclasses, not {}".format(
                     type(self).__name__, repr(content)
                 )
             )
-        if not isinstance(valid_when, bool):
-            raise TypeError(
-                "{} 'valid_when' must be bool, not {}".format(
-                    type(self).__name__, repr(valid_when)
-                )
-            )
 
-        self._mask = mask
+        self._index = index
         self._content = content
-        self._valid_when = valid_when
         self._init(parameters=parameters, form_key=form_key)
 
     @property
-    def mask(self):
-        return self._mask
+    def index(self):
+        return self._index
 
     @property
     def content(self):
         return self._content
 
-    @property
-    def valid_when(self):
-        return self._valid_when
-
     def copy(
         self,
-        mask=UNSET,
+        index=UNSET,
         content=UNSET,
-        valid_when=UNSET,
         *,
         parameters=UNSET,
         form_key=UNSET,
     ):
-        return ByteMaskedForm(
-            self._mask if mask is UNSET else mask,
+        return IndexedOptionForm(
+            self._index if index is UNSET else index,
             self._content if content is UNSET else content,
-            self._valid_when if valid_when is UNSET else valid_when,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
-        mask,
+        index,
         content,
-        valid_when,
         *,
         parameters=None,
         form_key=None,
     ):
-        if content.is_union:
-            return content._union_of_optionarrays("i64", parameters)
+        is_cat = parameters is not None and parameters.get("__array__") == "categorical"
+
+        if content.is_union and not is_cat:
+            return content._union_of_optionarrays(index, parameters)
+
         elif content.is_indexed or content.is_option:
             return ak.forms.IndexedOptionForm.simplified(
                 "i64",
-                content,
-                parameters=parameters,
-            )
-        else:
-            return cls(
-                mask, content, valid_when, parameters=parameters, form_key=form_key
+                content.content,
+                parameters=parameters_union(content._parameters, parameters),
             )
 
-    @property
-    def is_identity_like(self):
-        return False
+        else:
+            return cls(index, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
-        args = [
-            repr(self._mask),
-            repr(self._content),
-            repr(self._valid_when),
-            *self._repr_args(),
-        ]
+        args = [repr(self._index), repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "ByteMaskedArray",
-                "mask": self._mask,
-                "valid_when": self._valid_when,
+                "class": "IndexedOptionArray",
+                "index": self._index,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
+        if self.parameter("__array__") == "categorical":
+            parameters = dict(self._parameters)
+            del parameters["__array__"]
+            parameters["__categorical__"] = True
+        else:
+            parameters = self._parameters
+
         return ak.types.OptionType(
-            self._content.type, parameters=self._parameters
+            self._content.type,
+            parameters=parameters,
         ).simplify_option_union()
 
     def __eq__(self, other):
-        if isinstance(other, ByteMaskedForm):
+        if isinstance(other, IndexedOptionForm):
             return (
                 self._form_key == other._form_key
-                and self._mask == other._mask
-                and self._valid_when == other._valid_when
+                and self._index == other._index
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
         return self._content.purelist_depth
 
     @property
+    def is_identity_like(self):
+        return self._content.is_identity_like
+
+    @property
     def minmax_depth(self):
         return self._content.minmax_depth
 
     @property
     def branch_depth(self):
         return self._content.branch_depth
 
@@ -175,26 +166,24 @@
         self._content._columns(path, output, list_indicator)
 
     def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
         next_content = self._content._prune_columns(is_inside_record_or_union)
         if next_content is None:
             return None
         else:
-            return ByteMaskedForm(
-                self._mask,
+            return IndexedOptionForm(
+                self._index,
                 next_content,
-                self._valid_when,
                 parameters=self._parameters,
                 form_key=self._form_key,
             )
 
     def _select_columns(self, match_specifier):
-        return ByteMaskedForm(
-            self._mask,
+        return IndexedOptionForm(
+            self._index,
             self._content._select_columns(match_specifier),
-            self._valid_when,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         return self._content._column_types()
```

### Comparing `awkward-2.2.4/src/awkward/forms/emptyform.py` & `awkward-2.3.0/src/awkward/forms/emptyform.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,74 +2,69 @@
 from __future__ import annotations
 
 from inspect import signature
 
 import awkward as ak
 from awkward._errors import deprecate
 from awkward._nplikes.shape import ShapeItem
-from awkward._typing import Iterator, Self, final
+from awkward._typing import Iterator, JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form, JSONMapping
 
 
 @final
 class EmptyForm(Form):
     is_numpy = True
     is_unknown = True
 
     def __init__(self, *, parameters: JSONMapping | None = None, form_key=None):
         if not (parameters is None or len(parameters) == 0):
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
-            )
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         self._init(parameters=parameters, form_key=form_key)
 
     def copy(
         self, *, parameters: JSONMapping | None = UNSET, form_key=UNSET
     ) -> EmptyForm:
         if not (parameters is UNSET or parameters is None or len(parameters) == 0):
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
-            )
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         return EmptyForm(
-            parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(cls, *, parameters=None, form_key=None) -> Form:
         if not (parameters is None or len(parameters) == 0):
-            deprecate(f"{cls.__name__} cannot contain parameters", version="2.2.0")
+            raise TypeError(f"{cls.__name__} cannot contain parameters")
         return cls(parameters=parameters, form_key=form_key)
 
     def __repr__(self):
         args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra({"class": "EmptyArray"}, verbose)
 
     @property
     def type(self):
-        return ak.types.UnknownType(parameters=self._parameters)
+        return ak.types.UnknownType()
 
     def __eq__(self, other) -> bool:
         return isinstance(other, EmptyForm) and self._form_key == other._form_key
 
     def to_NumpyForm(self, *args, **kwargs):
         def legacy_impl(dtype):
             deprecate(
                 f"the `dtype` parameter in {type(self).__name__}.to_NumpyForm is deprecated, "
                 f"in favour of a new `primitive` argument. Pass `primitive` by keyword to opt-in to the new behavior.",
                 version="2.4.0",
             )
-            return ak.forms.numpyform.from_dtype(dtype, parameters=self._parameters)
+            return ak.forms.numpyform.from_dtype(dtype)
 
         def new_impl(*, primitive):
-            return ak.forms.numpyform.NumpyForm(primitive, parameters=self._parameters)
+            return ak.forms.numpyform.NumpyForm(primitive)
 
         dispatch_table = [
             new_impl,
             legacy_impl,
         ]
         for func in dispatch_table:
             sig = signature(func)
@@ -80,19 +75,16 @@
             else:
                 return func(*bound_arguments.args, **bound_arguments.kwargs)
         raise AssertionError(
             f"{type(self).__name__}.to_NumpyForm accepts either the new `primitive` argument as a keyword-only "
             f"argument, or the legacy `dtype` argument as positional or keyword"
         )
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return None
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        return None
 
     @property
     def purelist_isregular(self) -> bool:
         return True
 
     @property
     def purelist_depth(self) -> int:
```

### Comparing `awkward-2.2.4/src/awkward/forms/form.py` & `awkward-2.3.0/src/awkward/forms/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         ("__array__", "byte"),
         ("__array__", "sorted_map"),
         ("__array__", "categorical"),
     }
 )
 
 
-def from_dict(input: dict) -> Form:
+def from_dict(input: Mapping) -> Form:
     assert input is not None
     if isinstance(input, str):
         return ak.forms.NumpyForm(primitive=input)
 
-    assert isinstance(input, dict)
+    assert isinstance(input, Mapping)
     parameters = input.get("parameters", None)
     form_key = input.get("form_key", None)
 
     if input["class"] == "NumpyArray":
         primitive = input["primitive"]
         inner_shape = input.get("inner_shape", [])
         return ak.forms.NumpyForm(
@@ -86,15 +86,15 @@
         # New serialisation
         if "fields" in input:
             if isinstance(input["contents"], Mapping):
                 raise TypeError("new-style RecordForm contents must not be mappings")
             contents = [from_dict(content) for content in input["contents"]]
             fields = input["fields"]
         # Old style record
-        elif isinstance(input["contents"], dict):
+        elif isinstance(input["contents"], Mapping):
             contents = []
             fields = []
             for key, content in input["contents"].items():
                 contents.append(from_dict(content))
                 fields.append(key)
         # Old style tuple
         else:
@@ -373,14 +373,17 @@
     def parameter(self, key: str) -> JSONSerializable:
         if self._parameters is None:
             return None
         else:
             return self._parameters.get(key)
 
     def purelist_parameter(self, key: str) -> JSONSerializable:
+        return self.purelist_parameters(key)
+
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
         raise NotImplementedError
 
     @property
     def purelist_isregular(self):
         raise NotImplementedError
 
     @property
```

### Comparing `awkward-2.2.4/src/awkward/forms/indexedform.py` & `awkward-2.3.0/src/awkward/forms/indexedform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import awkward as ak
 from awkward._parameters import parameters_union, type_parameters_equal
-from awkward._typing import Self, final
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class IndexedForm(Form):
     is_indexed = True
@@ -137,19 +137,21 @@
                 and self._index == other._index
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
```

### Comparing `awkward-2.2.4/src/awkward/forms/indexedoptionform.py` & `awkward-2.3.0/src/awkward/forms/regularform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,170 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._parameters import parameters_union, type_parameters_equal
-from awkward._typing import Self, final
+from awkward._nplikes.shape import unknown_length
+from awkward._parameters import type_parameters_equal
+from awkward._regularize import is_integer
+from awkward._typing import JSONSerializable, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class IndexedOptionForm(Form):
-    is_option = True
-    is_indexed = True
-
-    def __init__(
-        self,
-        index,
-        content,
-        *,
-        parameters=None,
-        form_key=None,
-    ):
-        if not isinstance(index, str):
-            raise TypeError(
-                "{} 'index' must be of type str, not {}".format(
-                    type(self).__name__, repr(index)
-                )
-            )
+class RegularForm(Form):
+    is_list = True
+    is_regular = True
+
+    def __init__(self, content, size, *, parameters=None, form_key=None):
         if not isinstance(content, Form):
             raise TypeError(
                 "{} all 'contents' must be Form subclasses, not {}".format(
                     type(self).__name__, repr(content)
                 )
             )
+        if not (size is unknown_length or (is_integer(size) and size >= 0)):
+            raise TypeError(
+                "{} 'size' must be a non-negative int or None, not {}".format(
+                    type(self).__name__, repr(size)
+                )
+            )
 
-        self._index = index
         self._content = content
+        self._size = size
         self._init(parameters=parameters, form_key=form_key)
 
     @property
-    def index(self):
-        return self._index
-
-    @property
     def content(self):
         return self._content
 
-    def copy(
-        self,
-        index=UNSET,
-        content=UNSET,
-        *,
-        parameters=UNSET,
-        form_key=UNSET,
-    ):
-        return IndexedOptionForm(
-            self._index if index is UNSET else index,
+    @property
+    def size(self):
+        return self._size
+
+    def copy(self, content=UNSET, size=UNSET, *, parameters=UNSET, form_key=UNSET):
+        return RegularForm(
             self._content if content is UNSET else content,
+            self._size if size is UNSET else size,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
-    def simplified(
-        cls,
-        index,
-        content,
-        *,
-        parameters=None,
-        form_key=None,
-    ):
-        is_cat = parameters is not None and parameters.get("__array__") == "categorical"
-
-        if content.is_union and not is_cat:
-            return content._union_of_optionarrays(index, parameters)
-
-        elif content.is_indexed or content.is_option:
-            return ak.forms.IndexedOptionForm.simplified(
-                "i64",
-                content.content,
-                parameters=parameters_union(content._parameters, parameters),
-            )
-
-        else:
-            return cls(index, content, parameters=parameters, form_key=form_key)
+    def simplified(cls, content, size, *, parameters=None, form_key=None):
+        return cls(content, size, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
-        args = [repr(self._index), repr(self._content), *self._repr_args()]
+        args = [repr(self._content), repr(self._size), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "IndexedOptionArray",
-                "index": self._index,
+                "class": "RegularArray",
+                "size": None if self._size is unknown_length else self._size,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
-        if self.parameter("__array__") == "categorical":
-            parameters = dict(self._parameters)
-            del parameters["__array__"]
-            parameters["__categorical__"] = True
-        else:
-            parameters = self._parameters
-
-        return ak.types.OptionType(
+        return ak.types.RegularType(
             self._content.type,
-            parameters=parameters,
-        ).simplify_option_union()
+            self._size,
+            parameters=self._parameters,
+        )
 
     def __eq__(self, other):
-        if isinstance(other, IndexedOptionForm):
+        if isinstance(other, RegularForm):
             return (
                 self._form_key == other._form_key
-                and self._index == other._index
+                and self._size == other._size
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
-        return self._content.purelist_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return 1
+        else:
+            return self._content.purelist_depth + 1
 
     @property
     def is_identity_like(self):
-        return self._content.is_identity_like
+        return False
 
     @property
     def minmax_depth(self):
-        return self._content.minmax_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return (1, 1)
+        else:
+            mindepth, maxdepth = self._content.minmax_depth
+            return (mindepth + 1, maxdepth + 1)
 
     @property
     def branch_depth(self):
-        return self._content.branch_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return (False, 1)
+        else:
+            branch, depth = self._content.branch_depth
+            return (branch, depth + 1)
 
     @property
     def fields(self):
         return self._content.fields
 
     @property
     def is_tuple(self):
         return self._content.is_tuple
 
     @property
     def dimension_optiontype(self):
-        return True
+        return False
 
     def _columns(self, path, output, list_indicator):
+        if (
+            self.parameter("__array__") not in ("string", "bytestring")
+            and list_indicator is not None
+        ):
+            path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+    def _prune_columns(self, is_inside_record_or_union: bool):
         next_content = self._content._prune_columns(is_inside_record_or_union)
         if next_content is None:
             return None
         else:
-            return IndexedOptionForm(
-                self._index,
+            return RegularForm(
                 next_content,
+                self._size,
                 parameters=self._parameters,
                 form_key=self._form_key,
             )
 
     def _select_columns(self, match_specifier):
-        return IndexedOptionForm(
-            self._index,
+        return RegularForm(
             self._content._select_columns(match_specifier),
+            self._size,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
-        return self._content._column_types()
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return ("string",)
+        else:
+            return self._content._column_types()
```

### Comparing `awkward-2.2.4/src/awkward/forms/listform.py` & `awkward-2.3.0/src/awkward/forms/listform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import JSONSerializable, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ListForm(Form):
     is_list = True
@@ -119,19 +119,21 @@
                 and self._stops == other._stops
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return False
 
     @property
     def purelist_depth(self):
```

### Comparing `awkward-2.2.4/src/awkward/forms/listoffsetform.py` & `awkward-2.3.0/src/awkward/forms/listoffsetform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import JSONMapping, final
+from awkward._typing import JSONMapping, JSONSerializable, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ListOffsetForm(Form):
     is_list = True
@@ -86,19 +86,21 @@
                 and self._offsets == other._offsets
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return False
 
     @property
     def purelist_depth(self):
```

### Comparing `awkward-2.2.4/src/awkward/forms/numpyform.py` & `awkward-2.3.0/src/awkward/forms/numpyform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import type_parameters_equal
-from awkward._typing import Self, final
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 np = NumpyMetadata.instance()
 
 
 def from_dtype(dtype, parameters=None, *, time_units_as_parameter: bool = UNSET):
@@ -166,19 +166,19 @@
     def to_RegularForm(self):
         out = NumpyForm(self._primitive, (), parameters=None, form_key=None)
         for x in self._inner_shape[::-1]:
             out = ak.forms.RegularForm(out, x, parameters=None, form_key=None)
         out._parameters = self._parameters
         return out
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return None
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
 
     @property
     def purelist_isregular(self):
         return True
 
     @property
     def purelist_depth(self):
```

### Comparing `awkward-2.2.4/src/awkward/forms/recordform.py` & `awkward-2.3.0/src/awkward/forms/recordform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
-from awkward._typing import final
+from awkward._typing import JSONSerializable, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class RecordForm(Form):
     is_record = True
@@ -37,15 +37,15 @@
         if fields is not None and not isinstance(fields, Iterable):
             raise TypeError(
                 "{} 'fields' must be iterable, not {}".format(
                     type(self).__name__, repr(contents)
                 )
             )
 
-        self._fields = fields
+        self._fields = None if fields is None else list(fields)
         self._contents = list(contents)
         self._init(parameters=parameters, form_key=form_key)
 
     @property
     def contents(self):
         return self._contents
 
@@ -186,16 +186,19 @@
                         zip(other._fields, other._contents)
                     )
             else:
                 return False
         else:
             return False
 
-    def purelist_parameter(self, key):
-        return self.parameter(key)
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
 
     @property
     def purelist_isregular(self):
         return True
 
     @property
     def purelist_depth(self):
```

### Comparing `awkward-2.2.4/src/awkward/forms/regularform.py` & `awkward-2.3.0/src/awkward/forms/unmaskedform.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,159 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._nplikes.shape import unknown_length
-from awkward._parameters import type_parameters_equal
-from awkward._regularize import is_integer
-from awkward._typing import final
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class RegularForm(Form):
-    is_list = True
-    is_regular = True
+class UnmaskedForm(Form):
+    is_option = True
 
-    def __init__(self, content, size, *, parameters=None, form_key=None):
+    def __init__(
+        self,
+        content,
+        *,
+        parameters=None,
+        form_key=None,
+    ):
         if not isinstance(content, Form):
             raise TypeError(
                 "{} all 'contents' must be Form subclasses, not {}".format(
                     type(self).__name__, repr(content)
                 )
             )
-        if not (size is unknown_length or (is_integer(size) and size >= 0)):
-            raise TypeError(
-                "{} 'size' must be a non-negative int or None, not {}".format(
-                    type(self).__name__, repr(size)
-                )
-            )
 
         self._content = content
-        self._size = size
         self._init(parameters=parameters, form_key=form_key)
 
     @property
     def content(self):
         return self._content
 
-    @property
-    def size(self):
-        return self._size
-
-    def copy(self, content=UNSET, size=UNSET, *, parameters=UNSET, form_key=UNSET):
-        return RegularForm(
+    def copy(
+        self,
+        content=UNSET,
+        *,
+        parameters=UNSET,
+        form_key=UNSET,
+    ):
+        return UnmaskedForm(
             self._content if content is UNSET else content,
-            self._size if size is UNSET else size,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
-    def simplified(cls, content, size, *, parameters=None, form_key=None):
-        return cls(content, size, parameters=parameters, form_key=form_key)
+    def simplified(
+        cls,
+        content,
+        *,
+        parameters=None,
+        form_key=None,
+    ):
+        if content.is_union:
+            return content.copy(
+                contents=[cls.simplified(x) for x in content.contents],
+                parameters=parameters_union(content._parameters, parameters),
+            )
+        elif content.is_indexed or content.is_option:
+            return content.copy(
+                parameters=parameters_union(content._parameters, parameters)
+            )
+        else:
+            return cls(content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
-        args = [repr(self._content), repr(self._size), *self._repr_args()]
+        args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "RegularArray",
-                "size": None if self._size is unknown_length else self._size,
+                "class": "UnmaskedArray",
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
-        return ak.types.RegularType(
+        return ak.types.OptionType(
             self._content.type,
-            self._size,
             parameters=self._parameters,
-        )
+        ).simplify_option_union()
 
     def __eq__(self, other):
-        if isinstance(other, RegularForm):
+        if isinstance(other, UnmaskedForm):
             return (
                 self._form_key == other._form_key
-                and self._size == other._size
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
-            return self._content.purelist_parameter(key)
-        else:
-            return self._parameters[key]
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        return self._content.purelist_parameters(*keys)
 
     @property
     def purelist_isregular(self):
         return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return 1
-        else:
-            return self._content.purelist_depth + 1
+        return self._content.purelist_depth
 
     @property
     def is_identity_like(self):
-        return False
+        return self._content.is_identity_like
 
     @property
     def minmax_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return (1, 1)
-        else:
-            mindepth, maxdepth = self._content.minmax_depth
-            return (mindepth + 1, maxdepth + 1)
+        return self._content.minmax_depth
 
     @property
     def branch_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return (False, 1)
-        else:
-            branch, depth = self._content.branch_depth
-            return (branch, depth + 1)
+        return self._content.branch_depth
 
     @property
     def fields(self):
         return self._content.fields
 
     @property
     def is_tuple(self):
         return self._content.is_tuple
 
     @property
     def dimension_optiontype(self):
-        return False
+        return True
 
     def _columns(self, path, output, list_indicator):
-        if (
-            self.parameter("__array__") not in ("string", "bytestring")
-            and list_indicator is not None
-        ):
-            path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _prune_columns(self, is_inside_record_or_union: bool):
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
         next_content = self._content._prune_columns(is_inside_record_or_union)
         if next_content is None:
             return None
         else:
-            return RegularForm(
+            return UnmaskedForm(
                 next_content,
-                self._size,
                 parameters=self._parameters,
                 form_key=self._form_key,
             )
 
     def _select_columns(self, match_specifier):
-        return RegularForm(
+        return UnmaskedForm(
             self._content._select_columns(match_specifier),
-            self._size,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return ("string",)
-        else:
-            return self._content._column_types()
+        return self._content._column_types()
```

### Comparing `awkward-2.2.4/src/awkward/forms/unionform.py` & `awkward-2.3.0/src/awkward/forms/unionform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections import Counter
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import Self, final
+from awkward._typing import JSONSerializable, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class UnionForm(Form):
     is_union = True
@@ -148,24 +148,27 @@
             and len(self._contents) == len(other._contents)
             and type_parameters_equal(self._parameters, other._parameters)
         ):
             return self._contents == other._contents
 
         return False
 
-    def purelist_parameter(self, key):
-        if self._parameters is None or key not in self._parameters:
+    def purelist_parameters(self, *keys: str) -> JSONSerializable:
+        if self._parameters is not None:
+            for key in keys:
+                if key in self._parameters:
+                    return self._parameters[key]
+
+        for key in keys:
             out = self._contents[0].purelist_parameter(key)
             for content in self._contents[1:]:
                 tmp = content.purelist_parameter(key)
                 if out != tmp:
                     return None
             return out
-        else:
-            return self._parameters[key]
 
     @property
     def purelist_isregular(self):
         for content in self._contents:
             if not content.purelist_isregular:
                 return False
         return True
```

### Comparing `awkward-2.2.4/src/awkward/operations/__init__.py` & `awkward-2.3.0/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_all.py` & `awkward-2.3.0/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_almost_equal.py` & `awkward-2.3.0/src/awkward/operations/ak_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_any.py` & `awkward-2.3.0/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_argcartesian.py` & `awkward-2.3.0/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_argcombinations.py` & `awkward-2.3.0/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_argmax.py` & `awkward-2.3.0/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_argmin.py` & `awkward-2.3.0/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_argsort.py` & `awkward-2.3.0/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_backend.py` & `awkward-2.3.0/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.3.0/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.3.0/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_cartesian.py` & `awkward-2.3.0/src/awkward/operations/ak_cartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_categories.py` & `awkward-2.3.0/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_combinations.py` & `awkward-2.3.0/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_concatenate.py` & `awkward-2.3.0/src/awkward/operations/ak_concatenate.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from awkward.contents import Content
 from awkward.operations.ak_fill_none import fill_none
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@ak._connect.numpy.implements("concatenate")
 @high_level_function
 def concatenate(arrays, axis=0, *, mergebool=True, highlevel=True, behavior=None):
     """
     Args:
         arrays: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
```

### Comparing `awkward-2.2.4/src/awkward/operations/ak_copy.py` & `awkward-2.3.0/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_corr.py` & `awkward-2.3.0/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_count.py` & `awkward-2.3.0/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.3.0/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_covar.py` & `awkward-2.3.0/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_drop_none.py` & `awkward-2.3.0/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_enforce_type.py` & `awkward-2.3.0/src/awkward/operations/ak_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_fields.py` & `awkward-2.3.0/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_fill_none.py` & `awkward-2.3.0/src/awkward/operations/ak_fill_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_firsts.py` & `awkward-2.3.0/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_flatten.py` & `awkward-2.3.0/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_arrow.py` & `awkward-2.3.0/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.3.0/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.3.0/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_buffers.py` & `awkward-2.3.0/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_categorical.py` & `awkward-2.3.0/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_cupy.py` & `awkward-2.3.0/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_iter.py` & `awkward-2.3.0/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_jax.py` & `awkward-2.3.0/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_json.py` & `awkward-2.3.0/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_numpy.py` & `awkward-2.3.0/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_parquet.py` & `awkward-2.3.0/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.3.0/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_from_regular.py` & `awkward-2.3.0/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_full_like.py` & `awkward-2.3.0/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_is_categorical.py` & `awkward-2.3.0/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_is_none.py` & `awkward-2.3.0/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_is_tuple.py` & `awkward-2.3.0/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_is_valid.py` & `awkward-2.3.0/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_isclose.py` & `awkward-2.3.0/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_linear_fit.py` & `awkward-2.3.0/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_local_index.py` & `awkward-2.3.0/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_mask.py` & `awkward-2.3.0/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_max.py` & `awkward-2.3.0/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_mean.py` & `awkward-2.3.0/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.3.0/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.3.0/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.3.0/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_min.py` & `awkward-2.3.0/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_moment.py` & `awkward-2.3.0/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.3.0/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.3.0/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_num.py` & `awkward-2.3.0/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_ones_like.py` & `awkward-2.3.0/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_pad_none.py` & `awkward-2.3.0/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_parameters.py` & `awkward-2.3.0/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_prod.py` & `awkward-2.3.0/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_ptp.py` & `awkward-2.3.0/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_ravel.py` & `awkward-2.3.0/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_run_lengths.py` & `awkward-2.3.0/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_singletons.py` & `awkward-2.3.0/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_softmax.py` & `awkward-2.3.0/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_sort.py` & `awkward-2.3.0/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_std.py` & `awkward-2.3.0/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_strings_astype.py` & `awkward-2.3.0/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_sum.py` & `awkward-2.3.0/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_arrow.py` & `awkward-2.3.0/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.3.0/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_backend.py` & `awkward-2.3.0/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_buffers.py` & `awkward-2.3.0/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_categorical.py` & `awkward-2.3.0/src/awkward/operations/ak_to_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_categorical",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._categorical import as_hashable
 from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
@@ -103,15 +104,15 @@
                 content = layout.content
                 cls = ak.contents.IndexedOptionArray
             else:
                 content = layout
                 cls = ak.contents.IndexedArray
 
             content_list = ak.operations.to_list(content)
-            hashable = [ak.behaviors.categorical._as_hashable(x) for x in content_list]
+            hashable = [as_hashable(x) for x in content_list]
 
             lookup = {}
             is_first = numpy.empty(len(hashable), dtype=np.bool_)
             mapping = numpy.empty(len(hashable), dtype=np.int64)
             for i, x in enumerate(hashable):
                 if x in lookup:
                     is_first[i] = False
```

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_cupy.py` & `awkward-2.3.0/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.3.0/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_jax.py` & `awkward-2.3.0/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_json.py` & `awkward-2.3.0/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_layout.py` & `awkward-2.3.0/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_list.py` & `awkward-2.3.0/src/awkward/operations/ak_to_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_list",)
-from collections.abc import Iterable, Mapping
+from collections.abc import Mapping
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
 from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._regularize import is_non_string_like_iterable
 
 np = NumpyMetadata.instance()
 
 
 @high_level_function
 def to_list(array):
     """
@@ -73,12 +74,12 @@
 
     elif hasattr(array, "to_list"):
         return array.to_list()
 
     elif isinstance(array, Mapping):
         return {k: _impl(v) for k, v in array.items()}
 
-    elif isinstance(array, Iterable):
+    elif is_non_string_like_iterable(array):
         return [_impl(x) for x in array]
 
     else:
         return array
```

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_numpy.py` & `awkward-2.3.0/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_packed.py` & `awkward-2.3.0/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_parquet.py` & `awkward-2.3.0/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.3.0/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_to_regular.py` & `awkward-2.3.0/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_transform.py` & `awkward-2.3.0/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_type.py` & `awkward-2.3.0/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_unflatten.py` & `awkward-2.3.0/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_unzip.py` & `awkward-2.3.0/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_validity_error.py` & `awkward-2.3.0/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_values_astype.py` & `awkward-2.3.0/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_var.py` & `awkward-2.3.0/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_where.py` & `awkward-2.3.0/src/awkward/operations/ak_where.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@ak._connect.numpy.implements("where")
 @high_level_function
 def where(condition, *args, mergebool=True, highlevel=True, behavior=None):
     """
     Args:
         condition: Array-like data (anything #ak.to_layout recognizes) of booleans.
         x: Optional array-like data (anything #ak.to_layout recognizes) with the same
             length as `condition`.
```

### Comparing `awkward-2.2.4/src/awkward/operations/ak_with_field.py` & `awkward-2.3.0/src/awkward/operations/ak_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_with_name.py` & `awkward-2.3.0/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_with_parameter.py` & `awkward-2.3.0/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_without_field.py` & `awkward-2.3.0/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_without_parameters.py` & `awkward-2.3.0/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_zeros_like.py` & `awkward-2.3.0/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/operations/ak_zip.py` & `awkward-2.3.0/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/__init__.py` & `awkward-2.3.0/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.3.0/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/arraytype.py` & `awkward-2.3.0/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/listtype.py` & `awkward-2.3.0/src/awkward/types/listtype.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,19 +41,35 @@
         self._parameters = parameters
         self._typestr = typestr
 
     @property
     def content(self):
         return self._content
 
+    def _get_typestr(self, behavior) -> str | None:
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            return typestr
+
+        if self._parameters is None:
+            return None
+
+        name = self._parameters.get("__array__")
+        if name == "string":
+            return "string"
+        elif name == "bytestring":
+            return "bytes"
+        else:
+            return None
+
     def _str(self, indent, compact, behavior):
         if self._typestr is not None:
             deprecate("typestr argument is deprecated", "2.4.0")
 
-        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        typestr = self._get_typestr(behavior)
         if typestr is not None:
             out = [typestr]
         else:
             params = self._str_parameters()
             if params is None:
                 out = ["var * ", *self._content._str(indent, compact, behavior)]
             else:
```

### Comparing `awkward-2.2.4/src/awkward/types/numpytype.py` & `awkward-2.3.0/src/awkward/types/numpytype.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,19 +122,33 @@
 
     @property
     def primitive(self):
         return self._primitive
 
     _str_parameters_exclude = ("__categorical__", "__unit__")
 
+    def _get_typestr(self, behavior) -> str | None:
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            return typestr
+
+        if self._parameters is None:
+            return None
+
+        name = self._parameters.get("__array__")
+        if name in {"byte", "char"}:
+            return name
+
+        return None
+
     def _str(self, indent, compact, behavior):
         if self._typestr is not None:
             deprecate("typestr argument is deprecated", "2.4.0")
 
-        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        typestr = self._get_typestr(behavior)
         if typestr is not None:
             out = [typestr]
 
         else:
             if self.parameter("__unit__") is not None:
                 numpy_unit = str(np.dtype("M8[" + self._parameters["__unit__"] + "]"))
                 bracket_index = numpy_unit.index("[")
```

### Comparing `awkward-2.2.4/src/awkward/types/optiontype.py` & `awkward-2.3.0/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/recordtype.py` & `awkward-2.3.0/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/regulartype.py` & `awkward-2.3.0/src/awkward/types/regulartype.py`

 * *Files 19% similar despite different names*

```diff
@@ -62,19 +62,35 @@
     def content(self):
         return self._content
 
     @property
     def size(self):
         return self._size
 
+    def _get_typestr(self, behavior) -> str | None:
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            return typestr
+
+        if self._parameters is None:
+            return None
+
+        name = self._parameters.get("__array__")
+        if name == "string":
+            return "string"
+        elif name == "bytestring":
+            return "bytes"
+        else:
+            return None
+
     def _str(self, indent, compact, behavior):
         if self._typestr is not None:
             deprecate("typestr argument is deprecated", "2.4.0")
 
-        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        typestr = self._get_typestr(behavior)
         if typestr is not None:
             out = [f"{typestr}[{self._size}]"]
 
         else:
             params = self._str_parameters()
 
             if params is None:
```

### Comparing `awkward-2.2.4/src/awkward/types/scalartype.py` & `awkward-2.3.0/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/type.py` & `awkward-2.3.0/src/awkward/types/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,39 +41,42 @@
 
     def show(self, stream=sys.stdout):
         # TODO: deprecate lowlevel show
         stream.write("".join([*self._str("", False, None), "\n"]))
 
     _str_parameters_exclude = ("__categorical__",)
 
-    def _str_categorical_begin(self):
+    def _str_categorical_begin(self) -> str:
         if self.parameter("__categorical__") is not None:
             return "categorical[type="
         else:
             return ""
 
-    def _str_categorical_end(self):
+    def _str_categorical_end(self) -> str:
         if self.parameter("__categorical__") is not None:
             return "]"
         else:
             return ""
 
-    def _str_parameters(self):
+    def _str_parameters(self) -> str:
         out = []
         if self._parameters is not None:
             for k, v in self._parameters.items():
-                if k not in self._str_parameters_exclude:
-                    out.append(json.dumps(k) + ": " + json.dumps(v))
+                if v is None:
+                    continue
+                if k in self._str_parameters_exclude:
+                    continue
+                out.append(json.dumps(k) + ": " + json.dumps(v))
 
         if len(out) == 0:
             return None
         else:
             return "parameters={" + ", ".join(out) + "}"
 
-    def _repr_args(self):
+    def _repr_args(self) -> list[str]:
         out = []
 
         if self._parameters is not None and len(self._parameters) > 0:
             out.append("parameters=" + repr(self._parameters))
 
         if self._typestr is not None:
             out.append("typestr=" + repr(self._typestr))
```

### Comparing `awkward-2.2.4/src/awkward/types/uniontype.py` & `awkward-2.3.0/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/src/awkward/types/unknowntype.py` & `awkward-2.3.0/src/awkward/types/unknowntype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-from awkward._behavior import find_array_typestr
 from awkward._errors import deprecate
-from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.types.type import Type
 
 
 @final
 class UnknownType(Type):
     def copy(self, *, parameters=UNSET, typestr=UNSET) -> Self:
+        if not (parameters is UNSET or parameters is None or len(parameters) == 0):
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         return UnknownType(
-            parameters=self._parameters if parameters is UNSET else parameters,
             typestr=self._typestr if typestr is UNSET else typestr,
         )
 
     def __init__(self, *, parameters=None, typestr=None):
-        if parameters is not None:
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
-            )
-        if parameters is not None and not isinstance(parameters, dict):
-            raise TypeError(
-                "{} 'parameters' must be of type dict or None, not {}".format(
-                    type(self).__name__, repr(parameters)
-                )
-            )
+        if not (parameters is None or len(parameters) == 0):
+            raise TypeError(f"{type(self).__name__} cannot contain parameters")
         if typestr is not None and not isinstance(typestr, str):
             raise TypeError(
                 "{} 'typestr' must be of type string or None, not {}".format(
                     type(self).__name__, repr(typestr)
                 )
             )
-        self._parameters = parameters
+        self._parameters = None
         self._typestr = typestr
 
     def _str(self, indent, compact, behavior):
         if self._typestr is not None:
             deprecate("typestr argument is deprecated", "2.4.0")
 
-        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        typestr = self._typestr
         if typestr is not None:
             out = [typestr]
 
         else:
             params = self._str_parameters()
             if params is None:
                 out = ["unknown"]
@@ -55,13 +46,8 @@
         return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
-        compare_parameters = (
-            parameters_are_equal if all_parameters else type_parameters_equal
-        )
-        return isinstance(other, type(self)) and compare_parameters(
-            self._parameters, other._parameters
-        )
+        return isinstance(other, type(self))
```

### Comparing `awkward-2.2.4/tests/test_0002_minimal_listarray.py` & `awkward-2.3.0/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0008_slices_and_getitem.py` & `awkward-2.3.0/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0011_listarray.py` & `awkward-2.3.0/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0013_error_handling_struct.py` & `awkward-2.3.0/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0014_finish_up_getitem.py` & `awkward-2.3.0/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0018_fromiter_fillable.py` & `awkward-2.3.0/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0019_use_json_library.py` & `awkward-2.3.0/tests/test_0019_use_json_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,45 @@
 def test_bytearray():
     array = ak.contents.NumpyArray(
         np.frombuffer(b"hellothere", "u1"), parameters={"__array__": "byte"}
     )
     assert ak.operations.to_json(array, convert_bytes=bytes.decode) == '"hellothere"'
 
 
+def test_chararray():
+    array = ak.contents.NumpyArray(
+        np.frombuffer(b"hellothere", "u1"), parameters={"__array__": "char"}
+    )
+    assert ak.operations.to_json(array) == '"hellothere"'
+
+
+def test_string_array():
+    array = ak.contents.ListOffsetArray(
+        ak.index.Index64([0, 5, 10]),
+        ak.contents.NumpyArray(
+            np.frombuffer(b"hellothere", "u1"), parameters={"__array__": "char"}
+        ),
+        parameters={"__array__": "string"},
+    )
+    assert ak.operations.to_json(array) == '["hello","there"]'
+
+
+def test_bytestring_array():
+    array = ak.contents.ListOffsetArray(
+        ak.index.Index64([0, 5, 10]),
+        ak.contents.NumpyArray(
+            np.frombuffer(b"hellothere", "u1"), parameters={"__array__": "byte"}
+        ),
+        parameters={"__array__": "bytestring"},
+    )
+    assert (
+        ak.operations.to_json(array, convert_bytes=bytes.decode) == '["hello","there"]'
+    )
+
+
 def test_complex():
     content = ak.contents.NumpyArray(
         np.array([(1.1 + 0.1j), 2.2, 3.3, 4.4, 5.5, 6.6, 7.7, 8.8, 9.9])
     )
     assert (
         ak.operations.to_json(content, complex_record_fields=("r", "i"))
         == """[{"r":1.1,"i":0.1},{"r":2.2,"i":0.0},{"r":3.3,"i":0.0},{"r":4.4,"i":0.0},{"r":5.5,"i":0.0},{"r":6.6,"i":0.0},{"r":7.7,"i":0.0},{"r":8.8,"i":0.0},{"r":9.9,"i":0.0}]"""
```

### Comparing `awkward-2.2.4/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.3.0/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0021_emptyarray.py` & `awkward-2.3.0/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0023_regular_array.py` & `awkward-2.3.0/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0024_use_regular_array.py` & `awkward-2.3.0/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0025_record_array.py` & `awkward-2.3.0/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0028_add_dressed_types.py` & `awkward-2.3.0/tests/test_0028_add_dressed_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,21 +45,33 @@
     assert str(c) == "[{one: 3.14, two: [1.1, 2.2]}, {one: 99.9, two: [-3.14]}]"
 
 
 class Dummy(ak.highlevel.Array):
     pass
 
 
-def test_string1():
+def test_byte():
     a = ak.highlevel.Array(
-        np.array([ord(x) for x in "hey there"], dtype=np.uint8), check_valid=True
+        np.array([ord(x) for x in "hey there"], dtype=np.uint8),
+        check_valid=True,
     )
-    a.__class__ = ak.behaviors.string.ByteBehavior
-    assert str(a) == str(b"hey there")
-    assert str(a) == str(b"hey there")
+    a = ak.with_parameter(a, "__array__", "byte")
+    assert bytes(a) == b"hey there"
+    assert str(a) == str([ord(c) for c in "hey there"])
+    assert ak.to_list(a) == b"hey there"
+
+
+def test_char():
+    a = ak.highlevel.Array(
+        np.array([ord(x) for x in "hey there"], dtype=np.uint8),
+        check_valid=True,
+    )
+    a = ak.with_parameter(a, "__array__", "char")
+    assert str(a) == str([ord(c) for c in "hey there"])
+    assert ak.to_list(a) == "hey there"
 
 
 def test_string2():
     content = ak.contents.NumpyArray(
         np.array([ord(x) for x in "heythere"], dtype=np.uint8)
     )
     listoffsetarray = ak.contents.ListOffsetArray(
```

### Comparing `awkward-2.2.4/tests/test_0032_replace_dressedtype.py` & `awkward-2.3.0/tests/test_0032_replace_dressedtype.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,92 +8,83 @@
 to_list = ak.operations.to_list
 
 
 def test_types_with_parameters():
     t = ak.types.UnknownType()
     assert t.parameters == {}
 
-    with pytest.warns(DeprecationWarning):
-        t = ak.types.UnknownType(parameters={"__array__": ["val", "ue"]})
-        assert t.parameters == {"__array__": ["val", "ue"]}
-
-    t = ak.types.NumpyType("int32", parameters={"__array__": ["val", "ue"]})
-    assert t.parameters == {"__array__": ["val", "ue"]}
-    t = ak.types.NumpyType("float64", parameters={"__array__": ["val", "ue"]})
-    assert t.parameters == {"__array__": ["val", "ue"]}
+    with pytest.raises(TypeError):
+        ak.types.UnknownType(parameters={"latitude": ["val", "ue"]})
+    t = ak.types.UnknownType()
+    assert t.parameters == {}
+
+    t = ak.types.NumpyType("int32", parameters={"latitude": ["val", "ue"]})
+    assert t.parameters == {"latitude": ["val", "ue"]}
+    t = ak.types.NumpyType("float64", parameters={"latitude": ["val", "ue"]})
+    assert t.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.ArrayType(
-        ak.types.NumpyType("int32", parameters={"__array__": ["val", "ue"]}), 100
+        ak.types.NumpyType("int32", parameters={"latitude": ["val", "ue"]}), 100
     )
-    assert t.content.parameters == {"__array__": ["val", "ue"]}
+    assert t.content.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.ListType(
-        ak.types.NumpyType("int32"), parameters={"__array__": ["val", "ue"]}
+        ak.types.NumpyType("int32"), parameters={"latitude": ["val", "ue"]}
     )
-    assert t.parameters == {"__array__": ["val", "ue"]}
+    assert t.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.RegularType(
-        ak.types.NumpyType("int32"), 5, parameters={"__array__": ["val", "ue"]}
+        ak.types.NumpyType("int32"), 5, parameters={"latitude": ["val", "ue"]}
     )
-    assert t.parameters == {"__array__": ["val", "ue"]}
+    assert t.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.OptionType(
-        ak.types.NumpyType("int32"), parameters={"__array__": ["val", "ue"]}
+        ak.types.NumpyType("int32"), parameters={"latitude": ["val", "ue"]}
     )
-    assert t.parameters == {"__array__": ["val", "ue"]}
+    assert t.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.UnionType(
         (ak.types.NumpyType("int32"), ak.types.NumpyType("float64")),
-        parameters={"__array__": ["val", "ue"]},
+        parameters={"latitude": ["val", "ue"]},
     )
-    assert t.parameters == {"__array__": ["val", "ue"]}
+    assert t.parameters == {"latitude": ["val", "ue"]}
     t = ak.types.RecordType(
         [
             ak.types.NumpyType("int32"),
             ak.types.NumpyType("float64"),
         ],
         fields=["one", "two"],
-        parameters={"__array__": ["val", "ue"]},
+        parameters={"latitude": ["val", "ue"]},
     )
-    assert t.parameters == {"__array__": ["val", "ue"]}
-
-    with pytest.warns(DeprecationWarning):
-        t = ak.types.UnknownType(
-            parameters={"key1": ["val", "ue"], "__record__": "one \u2192 two"}
-        )
-        assert t.parameters == {"__record__": "one \u2192 two", "key1": ["val", "ue"]}
-
-        assert t == ak.types.UnknownType(
-            parameters={"__record__": "one \u2192 two", "key1": ["val", "ue"]}
-        )
-        assert t != ak.types.UnknownType(parameters={"__array__": ["val", "ue"]})
+    assert t.parameters == {"latitude": ["val", "ue"]}
 
 
 def test_dress():
     class Dummy(ak.highlevel.Array):
         def __str__(self):
             return f"<Dummy {super().__str__()}>"
 
     ns = {"Dummy": Dummy}
 
-    x = ak.contents.NumpyArray(np.array([1.1, 2.2, 3.3, 4.4, 5.5]))
-    x.parameters["__array__"] = "Dummy"
+    x = ak.contents.RegularArray(
+        ak.contents.NumpyArray(np.array([1.1, 2.2, 3.3, 4.4, 5.5, 6, 6])),
+        size=3,
+        parameters={"__list__": "Dummy"},
+    )
     a = ak.highlevel.Array(x, behavior=ns, check_valid=True)
-    assert str(a) == "<Dummy [1.1, 2.2, 3.3, 4.4, 5.5]>"
+    assert str(a) == "<Dummy [[1.1, 2.2, 3.3], [4.4, 5.5, 6]]>"
 
     x2 = ak.contents.ListOffsetArray(
-        ak.index.Index64(np.array([0, 3, 3, 5], dtype=np.int64)),
-        ak.contents.NumpyArray(
-            np.array([1.1, 2.2, 3.3, 4.4, 5.5]), parameters={"__array__": "Dummy"}
-        ),
+        ak.index.Index64(np.array([0, 2, 2, 2], dtype=np.int64)),
+        x,
     )
     a2 = ak.highlevel.Array(x2, behavior=ns, check_valid=True)
     # columns limit changed from 40 to 80 in v2
     assert (
         repr(a2)
-        == "<Array [<Dummy [1.1, 2.2, 3.3]>, <Dummy []>, <Dummy [4.4, 5.5]>] type='3 * ...'>"
+        == "<Array [<Dummy [[1.1, 2.2, 3.3], [4.4, 5.5, 6]]>, <Dummy []>, <Dummy []>] type='...'>"
     )
-    assert str(a2[0]) == "<Dummy [1.1, 2.2, 3.3]>"
+    assert str(a2[0]) == "<Dummy [[1.1, 2.2, 3.3], [4.4, 5.5, 6]]>"
     assert str(a2[1]) == "<Dummy []>"
-    assert str(a2[2]) == "<Dummy [4.4, 5.5]>"
+    assert str(a2[2]) == "<Dummy []>"
 
 
 def test_record_name():
     builder = ak.highlevel.ArrayBuilder()
 
     builder.begin_record("Dummy")
     builder.field("one")
```

### Comparing `awkward-2.2.4/tests/test_0046_start_indexedarray.py` & `awkward-2.3.0/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.3.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0057_introducing_forms.py` & `awkward-2.3.0/tests/test_0057_introducing_forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,30 +92,32 @@
         "content": "float64",
         "valid_when": True,
         "lsb_order": False,
         "parameters": {"hey": ["you"]},
         "form_key": "yowzers",
     }
 
-    with pytest.warns(DeprecationWarning):
-        form = ak.forms.EmptyForm(
+    with pytest.raises(TypeError):
+        ak.forms.EmptyForm(
             parameters={"hey": ["you"]},
             form_key="yowzers",
         )
-        assert form == form
-        assert pickle.loads(pickle.dumps(form, -1)) == form
-        assert ak.forms.from_json(form.to_json()) == form
+    form = ak.forms.EmptyForm(
+        form_key="yowzers",
+    )
+    assert form == form
+    assert pickle.loads(pickle.dumps(form, -1)) == form
+    assert ak.forms.from_json(form.to_json()) == form
     assert json.loads(form.to_json()) == {
         "class": "EmptyArray",
-        "parameters": {"hey": ["you"]},
+        "parameters": {},
         "form_key": "yowzers",
     }
     assert json.loads(str(form)) == {
         "class": "EmptyArray",
-        "parameters": {"hey": ["you"]},
         "form_key": "yowzers",
     }
 
     form = ak.forms.IndexedForm(
         "i64",
         ak.forms.NumpyForm("float64"),
         parameters={"hey": ["you"]},
```

### Comparing `awkward-2.2.4/tests/test_0070_argmin_and_argmax.py` & `awkward-2.3.0/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0072_fillna_operation.py` & `awkward-2.3.0/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0074_argsort_and_sort.py` & `awkward-2.3.0/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0077_zip_operation.py` & `awkward-2.3.0/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0078_argcross_and_cross.py` & `awkward-2.3.0/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0079_argchoose_and_choose.py` & `awkward-2.3.0/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.3.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0084_start_unionarray.py` & `awkward-2.3.0/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0086_nep13_ufunc.py` & `awkward-2.3.0/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0089_numpy_functions.py` & `awkward-2.3.0/tests/test_0089_numpy_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,25 +188,16 @@
     )
     content1 = ak.from_iter(["1", "2", "3"], highlevel=False)
     tags = ak.index.Index8(np.array([0, 1, 1, 0, 0, 0, 1, 0], dtype=np.int8))
     index = ak.index.Index64(np.array([0, 0, 1, 1, 2, 3, 2, 4], dtype=np.int64))
     array = ak.highlevel.Array(
         ak.contents.UnionArray(tags, index, [content0, content1]), check_valid=True
     )
-    with pytest.warns(DeprecationWarning):
-        assert ak.operations.to_numpy(array).tolist() == [
-            "1.1",
-            "1",
-            "2",
-            "2.2",
-            "3.3",
-            "4.4",
-            "3",
-            "5.5",
-        ]
+    with pytest.raises(TypeError):
+        assert ak.operations.to_numpy(array)
 
     assert ak.operations.to_numpy(
         ak.highlevel.Array([1.1, 2.2, None, None, 3.3], check_valid=True)
     ).tolist() == [1.1, 2.2, None, None, 3.3]
     assert ak.operations.to_numpy(
         ak.highlevel.Array([[1.1, 2.2], [None, None], [3.3, 4.4]], check_valid=True)
     ).tolist() == [[1.1, 2.2], [None, None], [3.3, 4.4]]
@@ -277,25 +268,16 @@
     )
     content1 = ak.from_iter(["1", "2", "3"], highlevel=False)
     tags = ak.index.Index8(np.array([0, 1, 1, 0, 0, 0, 1, 0], dtype=np.int8))
     index = ak.index.Index64(np.array([0, 0, 1, 1, 2, 3, 2, 4], dtype=np.int64))
     array = ak.highlevel.Array(
         ak.contents.UnionArray(tags, index, [content0, content1]), check_valid=True
     )
-    with pytest.warns(DeprecationWarning):
-        assert np.asarray(array).tolist() == [
-            "1.1",
-            "1",
-            "2",
-            "2.2",
-            "3.3",
-            "4.4",
-            "3",
-            "5.5",
-        ]
+    with pytest.raises(TypeError):
+        np.asarray(array)
 
     assert ak.operations.to_numpy(
         ak.highlevel.Array([1.1, 2.2, None, None, 3.3], check_valid=True)
     ).tolist() == [1.1, 2.2, None, None, 3.3]
     assert ak.operations.to_numpy(
         ak.highlevel.Array([[1.1, 2.2], [None, None], [3.3, 4.4]], check_valid=True)
     ).tolist() == [[1.1, 2.2], [None, None], [3.3, 4.4]]
```

### Comparing `awkward-2.2.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.3.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0107_assign_fields_to_records.py` & `awkward-2.3.0/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.3.0/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0115_generic_reducer_operation.py` & `awkward-2.3.0/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0118_numba_cpointers.py` & `awkward-2.3.0/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.3.0/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0124_strings_in_numba.py` & `awkward-2.3.0/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0127_tomask_operation.py` & `awkward-2.3.0/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.3.0/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0138_emptyarray_type.py` & `awkward-2.3.0/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0150_flatten.py` & `awkward-2.3.0/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0163_negative_axis_wrap.py` & `awkward-2.3.0/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.3.0/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0173_astype_operation.py` & `awkward-2.3.0/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0184_concatenate_operation.py` & `awkward-2.3.0/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.3.0/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.3.0/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0222_count_with_axis0.py` & `awkward-2.3.0/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0224_arrow_to_awkward.py` & `awkward-2.3.0/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0264_reduce_last_empty.py` & `awkward-2.3.0/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0273_path_for_with_field.py` & `awkward-2.3.0/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.3.0/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.3.0/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0315_integerindex.py` & `awkward-2.3.0/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0331_pandas_indexedarray.py` & `awkward-2.3.0/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.3.0/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.3.0/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0348_form_keys.py` & `awkward-2.3.0/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0355_mixins.py` & `awkward-2.3.0/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0395_complex_type_arrays.py` & `awkward-2.3.0/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.3.0/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.3.0/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.3.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0404_array_validity_check.py` & `awkward-2.3.0/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.3.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.3.0/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.3.0/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.3.0/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.3.0/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0496_provide_local_index.py` & `awkward-2.3.0/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.3.0/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.3.0/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.3.0/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.3.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 #    * if arrays have different `__array__` or `__record__` parameters, they are not equal;
 #    * if they otherwise have different parameters, the types can be equal, but merging
 #      (concatenation, option-simplify, or union-simplify) removes parameters other than
 #      `__array__` and `__record__`.
 
 
 def test_0459_types():
-    plain_plain = ak.highlevel.Array([0.0, 1.1, 2.2, 3.3, 4.4])
-    array_plain = ak.operations.with_parameter(plain_plain, "__array__", "zoinks")
+    plain_plain = ak.highlevel.Array([[0.0, 1.1, 2.2, 3.3, 4.4]])
+    array_plain = ak.operations.with_parameter(plain_plain, "__list__", "zoinks")
     plain_isdoc = ak.operations.with_parameter(
         plain_plain, "__doc__", "This is a zoink."
     )
     array_isdoc = ak.operations.with_parameter(
         array_plain, "__doc__", "This is a zoink."
     )
 
     assert ak.operations.parameters(plain_plain) == {}
-    assert ak.operations.parameters(array_plain) == {"__array__": "zoinks"}
+    assert ak.operations.parameters(array_plain) == {"__list__": "zoinks"}
     assert ak.operations.parameters(plain_isdoc) == {"__doc__": "This is a zoink."}
     assert ak.operations.parameters(array_isdoc) == {
-        "__array__": "zoinks",
+        "__list__": "zoinks",
         "__doc__": "This is a zoink.",
     }
 
     assert ak.operations.type(plain_plain) == ak.operations.type(plain_plain)
     assert ak.operations.type(array_plain) == ak.operations.type(array_plain)
     assert ak.operations.type(plain_isdoc) == ak.operations.type(plain_isdoc)
     assert ak.operations.type(array_isdoc) == ak.operations.type(array_isdoc)
@@ -45,75 +45,75 @@
 
     assert ak.operations.type(array_plain) == ak.operations.type(array_isdoc)
     assert ak.operations.type(array_isdoc) == ak.operations.type(array_plain)
 
     assert ak.operations.type(plain_isdoc) != ak.operations.type(array_isdoc)
     assert ak.operations.type(array_isdoc) != ak.operations.type(plain_isdoc)
 
-    assert array_plain.layout.parameters == {"__array__": "zoinks"}
+    assert array_plain.layout.parameters == {"__list__": "zoinks"}
     assert ak.operations.without_parameters(array_plain).layout.parameters == {}
     assert plain_isdoc.layout.parameters == {"__doc__": "This is a zoink."}
     assert ak.operations.without_parameters(plain_isdoc).layout.parameters == {}
     assert array_isdoc.layout.parameters == {
-        "__array__": "zoinks",
+        "__list__": "zoinks",
         "__doc__": "This is a zoink.",
     }
     assert ak.operations.without_parameters(array_isdoc).layout.parameters == {}
 
 
 def test_0459():
-    plain_plain = ak.highlevel.Array([0.0, 1.1, 2.2, 3.3, 4.4])
-    array_plain = ak.operations.with_parameter(plain_plain, "__array__", "zoinks")
+    plain_plain = ak.highlevel.Array([[0.0, 1.1, 2.2, 3.3, 4.4]])
+    array_plain = ak.operations.with_parameter(plain_plain, "__list__", "zoinks")
     plain_isdoc = ak.operations.with_parameter(
         plain_plain, "__doc__", "This is a zoink."
     )
     array_isdoc = ak.operations.with_parameter(
         array_plain, "__doc__", "This is a zoink."
     )
 
     assert ak.operations.parameters(plain_plain) == {}
-    assert ak.operations.parameters(array_plain) == {"__array__": "zoinks"}
+    assert ak.operations.parameters(array_plain) == {"__list__": "zoinks"}
     assert ak.operations.parameters(plain_isdoc) == {"__doc__": "This is a zoink."}
     assert ak.operations.parameters(array_isdoc) == {
-        "__array__": "zoinks",
+        "__list__": "zoinks",
         "__doc__": "This is a zoink.",
     }
 
     assert (
         ak.operations.parameters(ak.operations.concatenate([plain_plain, plain_plain]))
         == {}
     )
     assert ak.operations.parameters(
         ak.operations.concatenate([array_plain, array_plain])
-    ) == {"__array__": "zoinks"}
+    ) == {"__list__": "zoinks"}
     assert ak.operations.parameters(
         ak.operations.concatenate([plain_isdoc, plain_isdoc])
     ) == {"__doc__": "This is a zoink."}
     assert ak.operations.parameters(
         ak.operations.concatenate([array_isdoc, array_isdoc])
     ) == {
-        "__array__": "zoinks",
+        "__list__": "zoinks",
         "__doc__": "This is a zoink.",
     }
 
     assert isinstance(
         ak.operations.concatenate([plain_plain, plain_plain]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([array_plain, array_plain]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([plain_isdoc, plain_isdoc]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([array_isdoc, array_isdoc]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
 
     assert (
         ak.operations.parameters(ak.operations.concatenate([plain_plain, array_plain]))
         == {}
     )
     assert (
@@ -148,38 +148,38 @@
 
     assert (
         ak.operations.parameters(ak.operations.concatenate([plain_plain, plain_isdoc]))
         == {}
     )
     assert ak.operations.parameters(
         ak.operations.concatenate([array_plain, array_isdoc])
-    ) == {"__array__": "zoinks"}
+    ) == {"__list__": "zoinks"}
     assert (
         ak.operations.parameters(ak.operations.concatenate([plain_isdoc, plain_plain]))
         == {}
     )
     assert ak.operations.parameters(
         ak.operations.concatenate([array_isdoc, array_plain])
-    ) == {"__array__": "zoinks"}
+    ) == {"__list__": "zoinks"}
 
     assert isinstance(
         ak.operations.concatenate([plain_plain, plain_isdoc]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([array_plain, array_isdoc]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([plain_isdoc, plain_plain]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
     assert isinstance(
         ak.operations.concatenate([array_isdoc, array_plain]).layout,
-        ak.contents.NumpyArray,
+        ak.contents.ListOffsetArray,
     )
 
 
 def test_0522():
     content1 = ak.highlevel.Array([0.0, 1.1, 2.2, 3.3, 4.4]).layout
     content2 = ak.highlevel.Array([[0], [100], [200], [300], [400]]).layout
     tags = ak.index.Index8(np.array([0, 0, 0, 1, 1, 0, 0, 1, 1, 1], np.int8))
```

### Comparing `awkward-2.2.4/tests/test_0549_numba_array_asarray.py` & `awkward-2.3.0/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0557_min_max_initial_argument.py` & `awkward-2.3.0/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.3.0/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0572_numba_array_ndim.py` & `awkward-2.3.0/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.3.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0583_implement_unflatten_function.py` & `awkward-2.3.0/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.3.0/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.3.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.3.0/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0674_categorical_validation.py` & `awkward-2.3.0/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.3.0/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.3.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.3.0/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0733_run_lengths.py` & `awkward-2.3.0/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.3.0/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.3.0/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0773_typeparser.py` & `awkward-2.3.0/tests/test_0773_typeparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,16 @@
     parsedtype = ak.types.from_datashape(text, highlevel=False)
     assert isinstance(parsedtype, ak.types.UnknownType)
     assert (str(parsedtype)) == text
 
 
 def test_unknown_2():
     text = 'unknown[parameters={"wonky": ["parameter", 3.14]}]'
-    with pytest.warns(DeprecationWarning):
-        parsedtype = ak.types.from_datashape(text, highlevel=False)
-    assert isinstance(parsedtype, ak.types.UnknownType)
-    assert str(parsedtype) == text
+    with pytest.raises(TypeError):
+        ak.types.from_datashape(text, highlevel=False)
 
 
 def test_record_tuple_1():
     text = "(int64)"
     parsedtype = ak.types.from_datashape(text, highlevel=False)
     assert isinstance(parsedtype, ak.types.RecordType)
     assert str(parsedtype) == text
@@ -144,18 +142,16 @@
     parsedtype = ak.types.from_datashape(text, highlevel=False)
     assert isinstance(parsedtype, ak.types.OptionType)
     assert str(parsedtype) == text
 
 
 def test_option_unknown_2():
     text = '?unknown[parameters={"foo": "bar"}]'
-    with pytest.warns(DeprecationWarning):
-        parsedtype = ak.types.from_datashape(text, highlevel=False)
-    assert isinstance(parsedtype, ak.types.OptionType)
-    assert str(parsedtype) == text
+    with pytest.raises(TypeError):
+        ak.types.from_datashape(text, highlevel=False)
 
 
 def test_option_unknown_1_parm():
     text = 'option[unknown, parameters={"foo": "bar"}]'
     parsedtype = ak.types.from_datashape(text, highlevel=False)
     assert isinstance(parsedtype, ak.types.OptionType)
     assert str(parsedtype) == text
@@ -485,29 +481,26 @@
 
 def test_unknowntype():
     t = UnknownType()
     assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
 
 
 def test_unknowntype_parameter():
-    with pytest.warns(DeprecationWarning):
-        t = UnknownType(parameters={"__array__": "Something"})
-        assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
+    with pytest.raises(TypeError):
+        UnknownType(parameters={"__array__": "Something"})
 
 
 def test_unknowntype_categorical():
-    with pytest.warns(DeprecationWarning):
-        t = UnknownType(parameters={"__categorical__": True})
-        assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
+    with pytest.raises(TypeError):
+        UnknownType(parameters={"__categorical__": True})
 
 
 def test_unknowntype_categorical_parameter():
-    with pytest.warns(DeprecationWarning):
-        t = UnknownType(parameters={"__array__": "Something", "__categorical__": True})
-        assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
+    with pytest.raises(TypeError):
+        UnknownType(parameters={"__array__": "Something", "__categorical__": True})
 
 
 def test_regulartype_numpytype():
     t = RegularType(NumpyType("int32"), 5)
     assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
```

### Comparing `awkward-2.2.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.3.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.3.0/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0803_argsort_fix_type.py` & `awkward-2.3.0/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.3.0/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.3.0/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.3.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0828_arrow_datatype_null.py` & `awkward-2.3.0/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0835_datetime_type.py` & `awkward-2.3.0/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0835_datetime_type_pandas.py` & `awkward-2.3.0/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.3.0/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0850_argsort_mask_array.py` & `awkward-2.3.0/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.3.0/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0875_arrow_null_type.py` & `awkward-2.3.0/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0879_non_primitive_with_field.py` & `awkward-2.3.0/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.3.0/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0889_ptp.py` & `awkward-2.3.0/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0896_content_classes_refactoring.py` & `awkward-2.3.0/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.3.0/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.3.0/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.3.0/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.3.0/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0912_packed.py` & `awkward-2.3.0/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0914_types_and_forms.py` & `awkward-2.3.0/tests/test_0914_types_and_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,69 +1,43 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
+from typing import Optional
+
 import numpy as np
 import pytest
 
 import awkward as ak
 
 
-def assert_overrides_typestr(type_, typestr: str = "override", expected: str = None):
+def assert_overrides_typestr(
+    type_, typestr: str = "override", expected: Optional[str] = None
+):
     # Assume typestr is expected result
     if expected is None:
         expected = typestr
     # Set appropriate array or record parameter
     if isinstance(type_, ak.types.RecordType):
         parameters = {**type_.parameters, "__record__": "custom"}
     else:
-        parameters = {**type_.parameters, "__array__": "custom"}
+        assert isinstance(type_, (ak.types.ListType, ak.types.RegularType))
+        parameters = {**type_.parameters, "__list__": "custom"}
     behavior = {("__typestr__", "custom"): typestr}
     # Build highlevel type with custom behavior
     with_parameter = type_.copy(parameters=parameters)
     as_str = "".join(with_parameter._str("", False, behavior))
     assert as_str == expected
 
 
 def test_UnknownType():
     assert str(ak.types.unknowntype.UnknownType()) == "unknown"
-    with pytest.warns(DeprecationWarning):
-        assert (
-            str(ak.types.unknowntype.UnknownType(parameters={"x": 123}))
-            == 'unknown[parameters={"x": 123}]'
-        )
-    with pytest.warns(DeprecationWarning):
-        assert_overrides_typestr(ak.types.unknowntype.UnknownType())
-
-        assert_overrides_typestr(
-            ak.types.unknowntype.UnknownType(parameters={"x": 123})
-        )
-        assert (
-            str(ak.types.unknowntype.UnknownType(parameters={"__categorical__": True}))
-            == "categorical[type=unknown]"
-        )
-        assert (
-            str(
-                ak.types.unknowntype.UnknownType(
-                    parameters={"__categorical__": True, "x": 123}
-                )
-            )
-            == 'categorical[type=unknown[parameters={"x": 123}]]'
-        )
-        assert_overrides_typestr(
-            ak.types.unknowntype.UnknownType(
-                parameters={"__categorical__": True, "x": 123}
-            ),
-            expected="categorical[type=override]",
-        )
-
+    with pytest.raises(TypeError):
+        ak.types.unknowntype.UnknownType(parameters={"x": 123})
+    with pytest.raises(TypeError):
+        ak.types.unknowntype.UnknownType(parameters={"__categorical__": True})
     assert repr(ak.types.unknowntype.UnknownType()) == "UnknownType()"
-    with pytest.warns(DeprecationWarning):
-        assert (
-            repr(ak.types.unknowntype.UnknownType(parameters={"__categorical__": True}))
-            == "UnknownType(parameters={'__categorical__': True})"
-        )
 
 
 @pytest.mark.skipif(
     ak._util.win,
     reason="NumPy does not have float16, float128, and complex256 -- on Windows",
 )
 def test_NumpyType():
@@ -86,36 +60,27 @@
     assert str(ak.types.numpytype.NumpyType("complex128")) == "complex128"
     if hasattr(np, "complex256"):
         assert str(ak.types.numpytype.NumpyType("complex256")) == "complex256"
     assert (
         str(ak.types.numpytype.NumpyType("bool", parameters={"x": 123}))
         == 'bool[parameters={"x": 123}]'
     )
-    assert_overrides_typestr(ak.types.numpytype.NumpyType("bool"))
-
-    assert_overrides_typestr(
-        ak.types.numpytype.NumpyType("bool", parameters={"x": 123})
-    )
     assert (
         str(ak.types.numpytype.NumpyType("bool", parameters={"__categorical__": True}))
         == "categorical[type=bool]"
     )
     assert (
         str(
             ak.types.numpytype.NumpyType(
                 "bool", parameters={"__categorical__": True, "x": 123}
             )
         )
         == 'categorical[type=bool[parameters={"x": 123}]]'
     )
 
-    assert_overrides_typestr(
-        ak.types.numpytype.NumpyType("bool", parameters={"__categorical__": True}),
-        expected="categorical[type=override]",
-    )
     assert str(ak.types.numpytype.NumpyType("datetime64")) == "datetime64"
     assert (
         str(ak.types.numpytype.NumpyType("datetime64", parameters={"__unit__": "Y"}))
         == 'datetime64[unit="Y"]'
     )
     assert (
         str(ak.types.numpytype.NumpyType("datetime64", parameters={"__unit__": "M"}))
@@ -1013,48 +978,14 @@
                     ak.types.unknowntype.UnknownType(), 10
                 ),
                 parameters={"x": 123},
             )
         )
         == 'option[10 * unknown, parameters={"x": 123}]'
     )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.unknowntype.UnknownType(), parameters=None
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-            parameters=None,
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10)
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.unknowntype.UnknownType(),
-            parameters={"x": 123},
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-            parameters={"x": 123},
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
-            parameters={"x": 123},
-        )
-    )
     assert (
         str(
             ak.types.optiontype.OptionType(
                 ak.types.unknowntype.UnknownType(), parameters={"__categorical__": True}
             )
         )
         == "?categorical[type=unknown]"
@@ -1104,56 +1035,14 @@
                     ak.types.unknowntype.UnknownType(), 10
                 ),
                 parameters={"x": 123, "__categorical__": True},
             )
         )
         == 'option[categorical[type=10 * unknown], parameters={"x": 123}]'
     )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.unknowntype.UnknownType(),
-            parameters={"__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-            parameters={"__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
-            parameters={"__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.unknowntype.UnknownType(),
-            parameters={"x": 123, "__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-            parameters={"x": 123, "__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.optiontype.OptionType(
-            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
-            parameters={"x": 123, "__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
 
     assert (
         repr(ak.types.optiontype.OptionType(content=ak.types.unknowntype.UnknownType()))
         == "OptionType(UnknownType())"
     )
     assert (
         repr(
@@ -1196,32 +1085,14 @@
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 parameters={"x": 123},
             )
         )
         == 'union[unknown, bool, parameters={"x": 123}]'
     )
-    assert_overrides_typestr(
-        ak.types.uniontype.UnionType(
-            [
-                ak.types.unknowntype.UnknownType(),
-                ak.types.numpytype.NumpyType("bool"),
-            ],
-            parameters=None,
-        )
-    )
-    assert_overrides_typestr(
-        ak.types.uniontype.UnionType(
-            [
-                ak.types.unknowntype.UnknownType(),
-                ak.types.numpytype.NumpyType("bool"),
-            ],
-            parameters={"x": 123},
-        )
-    )
     assert (
         str(
             ak.types.uniontype.UnionType(
                 [
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
                 ],
@@ -1238,34 +1109,14 @@
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 parameters={"x": 123, "__categorical__": True},
             )
         )
         == 'categorical[type=union[unknown, bool, parameters={"x": 123}]]'
     )
-    assert_overrides_typestr(
-        ak.types.uniontype.UnionType(
-            [
-                ak.types.unknowntype.UnknownType(),
-                ak.types.numpytype.NumpyType("bool"),
-            ],
-            parameters={"__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
-    assert_overrides_typestr(
-        ak.types.uniontype.UnionType(
-            [
-                ak.types.unknowntype.UnknownType(),
-                ak.types.numpytype.NumpyType("bool"),
-            ],
-            parameters={"x": 123, "__categorical__": True},
-        ),
-        expected="categorical[type=override]",
-    )
 
     assert (
         repr(
             ak.types.uniontype.UnionType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -1315,94 +1166,58 @@
         == "ArrayType(UnknownType(), 10, None)"
     )
 
     assert (
         str(
             ak.types.arraytype.ArrayType(
                 content=ak.types.numpytype.NumpyType(
-                    "int64", parameters={"__array__": "custom"}
+                    "int64", parameters={"catastrophe": "apocalypse"}
                 ),
                 length=10,
-                behavior={("__typestr__", "custom"): "override"},
             )
         )
-        == "10 * override"
-    )
-
-    assert (
-        str(
-            ak.types.arraytype.ArrayType(
-                content=ak.types.numpytype.NumpyType(
-                    "int64", parameters={"__array__": "custom"}
-                ),
-                length=10,
-            )
-        )
-        == '10 * int64[parameters={"__array__": "custom"}]'
+        == '10 * int64[parameters={"catastrophe": "apocalypse"}]'
     )
 
 
 def test_EmptyForm():
     assert (
         str(ak.forms.emptyform.EmptyForm())
         == """{
     "class": "EmptyArray"
 }"""
     )
-    with pytest.warns(DeprecationWarning):
-        assert (
-            str(ak.forms.emptyform.EmptyForm(parameters={"x": 123}, form_key="hello"))
-            == """{
+    assert (
+        str(ak.forms.emptyform.EmptyForm(form_key="hello"))
+        == """{
     "class": "EmptyArray",
-    "parameters": {
-        "x": 123
-    },
     "form_key": "hello"
 }"""
-        )
+    )
     assert repr(ak.forms.emptyform.EmptyForm()) == "EmptyForm()"
-    with pytest.warns(DeprecationWarning):
-        assert (
-            repr(ak.forms.emptyform.EmptyForm(parameters={"x": 123}, form_key="hello"))
-            == "EmptyForm(parameters={'x': 123}, form_key='hello')"
-        )
+    with pytest.raises(TypeError):
+        ak.forms.emptyform.EmptyForm(parameters={"x": 123}, form_key="hello")
 
     assert ak.forms.emptyform.EmptyForm().to_dict(verbose=False) == {
         "class": "EmptyArray"
     }
     assert ak.forms.emptyform.EmptyForm().to_dict() == {
         "class": "EmptyArray",
         "parameters": {},
         "form_key": None,
     }
-    with pytest.warns(DeprecationWarning):
-        assert ak.forms.emptyform.EmptyForm(
-            parameters={"x": 123}, form_key="hello"
-        ).to_dict(verbose=False) == {
-            "class": "EmptyArray",
-            "parameters": {"x": 123},
-            "form_key": "hello",
-        }
+    assert ak.forms.emptyform.EmptyForm(form_key="hello").to_dict(verbose=False) == {
+        "class": "EmptyArray",
+        "form_key": "hello",
+    }
     assert ak.forms.from_dict({"class": "EmptyArray"}).to_dict() == {
         "class": "EmptyArray",
         "parameters": {},
         "form_key": None,
     }
-    with pytest.warns(DeprecationWarning):
-        assert ak.forms.from_dict(
-            {
-                "class": "EmptyArray",
-                "parameters": {"x": 123},
-                "form_key": "hello",
-            }
-        ).to_dict() == {
-            "class": "EmptyArray",
-            "parameters": {"x": 123},
-            "form_key": "hello",
-        }
 
 
 @pytest.mark.skipif(
     ak._util.win,
     reason="NumPy does not have float16, float128, and complex256 -- on Windows",
 )
 def test_NumpyForm():
```

### Comparing `awkward-2.2.4/tests/test_0916_datetime_values_astype.py` & `awkward-2.3.0/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.3.0/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.3.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.3.0/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.3.0/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0959__getitem_array_implementation.py` & `awkward-2.3.0/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.3.0/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.3.0/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.3.0/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0984_ravel.py` & `awkward-2.3.0/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.3.0/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.3.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.3.0/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1030_mixin_class_name.py` & `awkward-2.3.0/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1031_start_getitem_next.py` & `awkward-2.3.0/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.3.0/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1049_concatenate_single_array.py` & `awkward-2.3.0/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.3.0/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1059_localindex.py` & `awkward-2.3.0/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.3.0/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.3.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1072_sort.py` & `awkward-2.3.0/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1074_combinations.py` & `awkward-2.3.0/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1075_validityerror.py` & `awkward-2.3.0/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1110_type_tracer_1.py` & `awkward-2.3.0/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1116_project_maskedarrays.py` & `awkward-2.3.0/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.3.0/tests/test_1125_to_arrow_from_arrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,23 +237,22 @@
     paarray = akarray.to_arrow(extensionarray=extensionarray)
     arrow_round_trip(akarray, paarray, extensionarray)
     parquet_round_trip(akarray, paarray, extensionarray, tmp_path)
 
 
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_indexedoptionarray_emptyarray(tmp_path, extensionarray):
-    with pytest.warns(DeprecationWarning):
-        akarray = ak.contents.IndexedOptionArray(
-            ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
-            ak.contents.EmptyArray(parameters={"which": "inner"}),
-            parameters={"which": "outer"},
-        )
-        paarray = akarray.to_arrow(extensionarray=extensionarray)
-        arrow_round_trip(akarray, paarray, extensionarray)
-        parquet_round_trip(akarray, paarray, extensionarray, tmp_path)
+    akarray = ak.contents.IndexedOptionArray(
+        ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
+        ak.contents.EmptyArray(),
+        parameters={"which": "outer"},
+    )
+    paarray = akarray.to_arrow(extensionarray=extensionarray)
+    arrow_round_trip(akarray, paarray, extensionarray)
+    parquet_round_trip(akarray, paarray, extensionarray, tmp_path)
 
 
 @pytest.mark.parametrize("categorical_as_dictionary", [False, True])
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_dictionary_encoding(tmp_path, categorical_as_dictionary, extensionarray):
     akarray = ak.contents.IndexedArray(
         ak.index.Index64(np.array([3, 2, 2, 2, 0, 1, 3], dtype=np.uint64)),
```

### Comparing `awkward-2.2.4/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.3.0/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.3.0/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1135_rpad_operation.py` & `awkward-2.3.0/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.3.0/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1137_num.py` & `awkward-2.3.0/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1142_numbers_to_type.py` & `awkward-2.3.0/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1149_datetime_sort.py` & `awkward-2.3.0/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.3.0/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1162_ak_from_json_schema.py` & `awkward-2.3.0/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.3.0/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.3.0/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.3.0/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1193_is_none_nested_option.py` & `awkward-2.3.0/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1233_ak_with_name.py` & `awkward-2.3.0/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.3.0/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1259_simplify_optiontype.py` & `awkward-2.3.0/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.3.0/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1271_fix_4D_reducers.py` & `awkward-2.3.0/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1294_to_and_from_parquet.py` & `awkward-2.3.0/tests/test_1294_to_and_from_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,26 +286,24 @@
     )
     assert predicted_form == array_form
 
 
 @pytest.mark.parametrize("through", [through_arrow, through_parquet])
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_indexedoptionarray_emptyarray(tmp_path, through, extensionarray):
-    with pytest.warns(DeprecationWarning):
-        akarray = ak.contents.IndexedOptionArray(
-            ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
-            ak.contents.EmptyArray(parameters={"which": "inner"}),
-            parameters={"which": "outer"},
-        )
+    akarray = ak.contents.IndexedOptionArray(
+        ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
+        ak.contents.EmptyArray(),
+    )
 
-        schema_arrow, array_form = through(akarray, extensionarray, tmp_path)
-        predicted_form = ak._connect.pyarrow.form_handle_arrow(
-            schema_arrow, pass_empty_field=True
-        )
-        assert predicted_form == array_form
+    schema_arrow, array_form = through(akarray, extensionarray, tmp_path)
+    predicted_form = ak._connect.pyarrow.form_handle_arrow(
+        schema_arrow, pass_empty_field=True
+    )
+    assert predicted_form == array_form
 
 
 @pytest.mark.parametrize("categorical_as_dictionary", [False, True])
 @pytest.mark.parametrize("through", [through_arrow, through_parquet])
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_dictionary_encoding(
     tmp_path, categorical_as_dictionary, through, extensionarray
```

### Comparing `awkward-2.2.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.3.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.3.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1300b_same_for_numba.py` & `awkward-2.3.0/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1308_zip_after_option.py` & `awkward-2.3.0/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1318_array_function_types.py` & `awkward-2.3.0/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1320_mask_identity_defaults.py` & `awkward-2.3.0/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.3.0/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1345_avro_reader.py` & `awkward-2.3.0/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1351_is_tuple.py` & `awkward-2.3.0/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1374_to_rdataframe.py` & `awkward-2.3.0/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1377_ravel_string.py` & `awkward-2.3.0/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.3.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1399_from_jax.py` & `awkward-2.3.0/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1399_to_jax.py` & `awkward-2.3.0/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1405_slicing_untested_cases.py` & `awkward-2.3.0/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1415_behaviour_forwarding.py` & `awkward-2.3.0/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.3.0/tests/test_1440_start_v2_to_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,21 +208,20 @@
         parameters={"which": "outer"},
     )
     parquet_round_trip(ak.Array(akarray), extensionarray, tmp_path)
 
 
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_indexedoptionarray_emptyarray(tmp_path, extensionarray):
-    with pytest.warns(DeprecationWarning):
-        akarray = ak.contents.IndexedOptionArray(
-            ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
-            ak.contents.EmptyArray(parameters={"which": "inner"}),
-            parameters={"which": "outer"},
-        )
-        parquet_round_trip(ak.Array(akarray), extensionarray, tmp_path)
+    akarray = ak.contents.IndexedOptionArray(
+        ak.index.Index64(np.array([-1, -1, -1, -1, -1], dtype=np.int64)),
+        ak.contents.EmptyArray(),
+        parameters={"which": "outer"},
+    )
+    parquet_round_trip(ak.Array(akarray), extensionarray, tmp_path)
 
 
 @pytest.mark.skip(
     "Categorical arrays can't roundtrip through Parquet due to ARROW-14525"
 )
 @pytest.mark.parametrize("categorical_as_dictionary", [False, True])
 @pytest.mark.parametrize("extensionarray", [False, True])
```

### Comparing `awkward-2.2.4/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.3.0/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.3.0/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.3.0/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1473_from_rdataframe.py` & `awkward-2.3.0/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.3.0/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.3.0/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.3.0/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1504_typetracer_like.py` & `awkward-2.3.0/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.3.0/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1511_set_attribute.py` & `awkward-2.3.0/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.3.0/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.3.0/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.3.0/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.3.0/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.3.0/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.3.0/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.3.0/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1607_no_reducers_on_records.py` & `awkward-2.3.0/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1613_generator_tolayout_records.py` & `awkward-2.3.0/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.3.0/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1620_layout_builders.py` & `awkward-2.3.0/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.3.0/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.3.0/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.3.0/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1671_categorical_type.py` & `awkward-2.3.0/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1672_broadcast_parameters.py` & `awkward-2.3.0/tests/test_1672_broadcast_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         broadcast_parameters_rule="intersect",
     )
 
     assert this_next.parameters == that_next.parameters
     assert that_next.parameters == {"key": "value", "pets": [{"name": "fido"}]}
 
 
-def test_transform_float_int_2d_one_to_one_error():
+def test_transform_float_int_2d_one_to_one_none():
     this = ak.contents.ListOffsetArray(
         ak.index.Index64(np.array([0, 3, 4], dtype="int64")),
         ak.contents.NumpyArray(np.array([1.0, 2.0, 3.0, 4.0], dtype="float64")),
         parameters={"name": "this"},
     )
     that = ak.contents.ListOffsetArray(
         ak.index.Index64(np.array([0, 3, 4], dtype="int64")),
@@ -294,18 +294,18 @@
     )
 
     def apply(arrays, **kwargs):
         layout = ak.operations.ak_to_layout.to_layout(arrays[0])
         if isinstance(layout, ak.contents.NumpyArray):
             return layout
 
-    with pytest.raises(ValueError):
-        ak.operations.ak_transform.transform(
-            apply, this, that, highlevel=False, broadcast_parameters_rule="one_to_one"
-        )
+    result = ak.operations.ak_transform.transform(
+        apply, this, that, highlevel=False, broadcast_parameters_rule="one_to_one"
+    )
+    assert result._parameters is None
 
 
 def test_transform_string_self_one_to_one():
     this = ak.Array(["one", "two", "one", "nine"])
     that = this
 
     def apply(arrays, **kwargs):
```

### Comparing `awkward-2.2.4/tests/test_1677_array_builder_in_numba.py` & `awkward-2.3.0/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.3.0/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.3.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1688_pack_categorical.py` & `awkward-2.3.0/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1703_fill_none_typetracer.py` & `awkward-2.3.0/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.3.0/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.3.0/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 class MyBehavior(ak.Array):
     ...
 
 
 def test():
     behavior = {"MyBehavior": MyBehavior}
-    array = ak.with_parameter([1, 2, 3], "__array__", "MyBehavior", behavior=behavior)
+    array = ak.with_parameter([[1, 2, 3]], "__list__", "MyBehavior", behavior=behavior)
     assert isinstance(array, MyBehavior)
 
     shallow_copy = ak.Array(array)
     assert isinstance(shallow_copy, MyBehavior)
```

### Comparing `awkward-2.2.4/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.3.0/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.3.0/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1762_jax_behavior_support.py` & `awkward-2.3.0/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1764_jax_jacobian.py` & `awkward-2.3.0/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.3.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1766_record_form_fields.py` & `awkward-2.3.0/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.3.0/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.3.0/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1790_reduce_regulararray.py` & `awkward-2.3.0/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.3.0/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.3.0/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.3.0/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.3.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.3.0/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.3.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.3.0/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1904_drop_none.py` & `awkward-2.3.0/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.3.0/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.3.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.3.0/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1936_with_field_broadcasting.py` & `awkward-2.3.0/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1940_ak_backend.py` & `awkward-2.3.0/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1943_regular_indexing.py` & `awkward-2.3.0/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.3.0/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_1961_ak_without_field.py` & `awkward-2.3.0/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2020_reduce_axis_none.py` & `awkward-2.3.0/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.3.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2023_from_rdataframe.py` & `awkward-2.3.0/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.3.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.3.0/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2055_array_builder_check.py` & `awkward-2.3.0/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2058_merge_numpy_array.py` & `awkward-2.3.0/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2064_fill_none_record.py` & `awkward-2.3.0/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.3.0/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2070_to_layout_string.py` & `awkward-2.3.0/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.3.0/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2078_array_function_wrap.py` & `awkward-2.3.0/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2082_broadcast_zero_size.py` & `awkward-2.3.0/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2085_empty_if_typetracer.py` & `awkward-2.3.0/tests/test_2085_empty_if_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2096_ak_scalar_type.py` & `awkward-2.3.0/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2101_pickle_behavior_class.py` & `awkward-2.3.0/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2104_numpy_merge_option.py` & `awkward-2.3.0/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2106_pickle_class.py` & `awkward-2.3.0/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2108_fill_none_indexed.py` & `awkward-2.3.0/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2115_fix_up_typetracers.py` & `awkward-2.3.0/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2125_type_of_scalar.py` & `awkward-2.3.0/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.3.0/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2179_parameter_merging_rules.py` & `awkward-2.3.0/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2185_merge_union_of_records.py` & `awkward-2.3.0/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.3.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2192_union_absorb_indexed.py` & `awkward-2.3.0/tests/test_2192_union_absorb_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2198_almost_equal.py` & `awkward-2.3.0/tests/test_2198_almost_equal.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,20 @@
 
 def test_behavior():
     class CustomList(ak.Array):
         ...
 
     behavior = {"custom_list": CustomList}
 
-    array = ak.with_parameter([1, 2, 3], "__array__", "custom_list", behavior=behavior)
-    other_array = ak.with_parameter([1, 2, 3], "__array__", "custom_list")
+    array = ak.with_parameter([[1, 2, 3]], "__list__", "custom_list", behavior=behavior)
+    other_array = ak.with_parameter([[1, 2, 3]], "__list__", "custom_list")
     assert not ak.almost_equal(array, other_array)
     assert ak.almost_equal(array, other_array, check_parameters=False)
 
-    another_array = ak.Array([1, 2, 3], behavior=behavior)
+    another_array = ak.Array([[1, 2, 3]], behavior=behavior)
     assert not ak.almost_equal(array, another_array)
     assert not ak.almost_equal(other_array, another_array)
 
 
 def test_empty_outer_ragged():
     array = ak.Array([[1]])[0:0]
     assert not ak.almost_equal(array, [])
```

### Comparing `awkward-2.2.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.3.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2214_offset_bool_index.py` & `awkward-2.3.0/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.3.0/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2229_getitem_range_slice.py` & `awkward-2.3.0/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.3.0/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.3.0/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.3.0/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2246_slice_not_packed.py` & `awkward-2.3.0/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2250_full_like_bool.py` & `awkward-2.3.0/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.3.0/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2263_to_packed_list.py` & `awkward-2.3.0/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2267_broadcast_fields.py` & `awkward-2.3.0/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2293_unflatten_typetracer.py` & `awkward-2.3.0/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2296_duplicate_field.py` & `awkward-2.3.0/tests/test_2296_duplicate_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2297_common_backend.py` & `awkward-2.3.0/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.3.0/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2306_cppyy_git.py` & `awkward-2.3.0/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2319_from_buffers_array.py` & `awkward-2.3.0/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2327_array_interface.py` & `awkward-2.3.0/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.3.0/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.3.0/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2354_ufunc_same_backend.py` & `awkward-2.3.0/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2355_to_backend_record.py` & `awkward-2.3.0/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.3.0/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2364_empty_list_of_string.py` & `awkward-2.3.0/tests/test_2364_empty_list_of_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2365_enforce_type.py` & `awkward-2.3.0/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2368_type_is_equal.py` & `awkward-2.3.0/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2373_unzip_touching.py` & `awkward-2.3.0/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2374_cartesian_touching.py` & `awkward-2.3.0/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2385_with_field_empty_record.py` & `awkward-2.3.0/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2395_copy_asarray_touch.py` & `awkward-2.3.0/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.3.0/tests/test_2411_cartesian_axis_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2417_bytemasked_singletons.py` & `awkward-2.3.0/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2424_almost_equal_union_record.py` & `awkward-2.3.0/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2425_forms_from_type.py` & `awkward-2.3.0/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2426_is_equal_to.py` & `awkward-2.3.0/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2471_flatten_string.py` & `awkward-2.3.0/tests/test_2471_flatten_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2484_reduce_starts_empty.py` & `awkward-2.3.0/tests/test_2484_reduce_starts_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2487_broadcast_list_offsets.py` & `awkward-2.3.0/tests/test_2487_broadcast_list_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2490_reduce_regulararray_positional.py` & `awkward-2.3.0/tests/test_2490_reduce_regulararray_positional.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2495_concatenate_typetracer.py` & `awkward-2.3.0/tests/test_2495_concatenate_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2501_positional_record_reducer.py` & `awkward-2.3.0/tests/test_2501_positional_record_reducer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2503_deprecate_to_numpyform.py` & `awkward-2.3.0/tests/test_2503_deprecate_to_numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2512_record_array_carry.py` & `awkward-2.3.0/tests/test_2512_record_array_carry.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2518_datetime_units_as_parameter.py` & `awkward-2.3.0/tests/test_2518_datetime_units_as_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/test_2536_select_columns.py` & `awkward-2.3.0/tests/test_2536_select_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/list-depths-records-list.parquet` & `awkward-2.3.0/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/list-depths-records.parquet` & `awkward-2.3.0/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/list-depths-strings.parquet` & `awkward-2.3.0/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/list-depths.parquet` & `awkward-2.3.0/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nonnullable-depths.parquet` & `awkward-2.3.0/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-depths.parquet` & `awkward-2.3.0/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-levels.parquet` & `awkward-2.3.0/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.3.0/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.3.0/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.3.0/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-list-depths.parquet` & `awkward-2.3.0/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/nullable-record-primitives.parquet` & `awkward-2.3.0/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/record-primitives.parquet` & `awkward-2.3.0/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/test-nan-inf.json` & `awkward-2.3.0/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/test-two-arrays.json` & `awkward-2.3.0/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests/samples/test.json` & `awkward-2.3.0/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1276_cuda_num.py` & `awkward-2.3.0/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.3.0/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.3.0/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1276_from_cupy.py` & `awkward-2.3.0/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.3.0/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1381_check_errors.py` & `awkward-2.3.0/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.3.0/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/.gitignore` & `awkward-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/LICENSE` & `awkward-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.2.4/pyproject.toml` & `awkward-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.2.4"
+version = "2.3.0"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
@@ -36,17 +36,17 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==17",
+    "awkward_cpp==20",
     "importlib_resources;python_version < \"3.9\"",
-    "numpy>=1.17.0",
+    "numpy>=1.18.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
 ]
 
@@ -288,30 +288,33 @@
     "PLR",     # Design related pylint codes
     "PT011",   # Exception too broad
     "NPY002",  # Replace legacy `np.random` call with `np.random.Generator`
     "PLW2901", # Outer for loop variable  overwritten by inner assignment target
     "PLW0603", # Using the global statement to update is discouraged
     "PLC1901", # x == "" can be simplified to not x (empty string is falsey)
 ]
-target-version = "py37"
 typing-modules = ["awkward._typing"]
 src = ["src"]
 unfixable = [
     "T20",  # Removes print statements
     "F841", # Removes unused variables
 ]
 external = []
 mccabe.max-complexity = 100
 
 [tool.ruff.per-file-ignores]
 "dev/*" = ["T20", "TID251"]
+"src/awkward/numba/*" = ["TID251"]
 "src/awkward/_connect/*" = ["TID251"]
 "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"]
 "src/awkward/operations/__init__.py" = ["F403"]
 "src/awkward/_nplikes/*" = ["TID251"]
 "src/awkward/_operators.py" = ["TID251"]
 "tests*/*" = ["T20", "TID251"]
 
 [tool.ruff.flake8-tidy-imports.banned-api]
 "numpy".msg = "Use `numpy = ak._nplikes.Numpy.instance()` instead"
 "jax".msg = "Use `jax = ak._nplikes.Jax.instance()` instead"
 "cupy".msg = "Use `cupy = ak._nplikes.Cupy.instance()` instead"
+
+[tool.nbqa.addopts]
+pyupgrade = ["--py38-plus"]
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.4"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.3.0"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
-{ text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
+{ text = "BSD-3-Clause" } requires-python = ">=3.8" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
 Linux", "Operating System :: Unix", "Programming Language :: Python",
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==17",
-"importlib_resources;python_version < \"3.9\"", "numpy>=1.17.0", "packaging",
+Utilities", ] dependencies = [ "awkward_cpp==20",
+"importlib_resources;python_version < \"3.9\"", "numpy>=1.18.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
 awkward-1.0" "Releases" = "https://github.com/scikit-hep/awkward-1.0/releases"
@@ -84,18 +84,19 @@
 pyupgrade "YTT", # flake8-2020 "EXE", # flake8-executable "NPY", # NumPy
 specific rules "TID251", # flake8-tidy-imports ] extend-ignore = [ "E501", #
 Line too long "UP030", # {0} -> {} "PLR", # Design related pylint codes
 "PT011", # Exception too broad "NPY002", # Replace legacy `np.random` call with
 `np.random.Generator` "PLW2901", # Outer for loop variable overwritten by inner
 assignment target "PLW0603", # Using the global statement to update is
 discouraged "PLC1901", # x == "" can be simplified to not x (empty string is
-falsey) ] target-version = "py37" typing-modules = ["awkward._typing"] src =
-["src"] unfixable = [ "T20", # Removes print statements "F841", # Removes
-unused variables ] external = [] mccabe.max-complexity = 100 [tool.ruff.per-
-file-ignores] "dev/*" = ["T20", "TID251"] "src/awkward/_connect/*" = ["TID251"]
-"src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"] "src/awkward/
-operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" = ["TID251"] "src/
-awkward/_operators.py" = ["TID251"] "tests*/*" = ["T20", "TID251"]
-[tool.ruff.flake8-tidy-imports.banned-api] "numpy".msg = "Use `numpy =
-ak._nplikes.Numpy.instance()` instead" "jax".msg = "Use `jax =
+falsey) ] typing-modules = ["awkward._typing"] src = ["src"] unfixable =
+[ "T20", # Removes print statements "F841", # Removes unused variables ]
+external = [] mccabe.max-complexity = 100 [tool.ruff.per-file-ignores] "dev/*"
+= ["T20", "TID251"] "src/awkward/numba/*" = ["TID251"] "src/awkward/_connect/*"
+= ["TID251"] "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"] "src/
+awkward/operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" =
+["TID251"] "src/awkward/_operators.py" = ["TID251"] "tests*/*" = ["T20",
+"TID251"] [tool.ruff.flake8-tidy-imports.banned-api] "numpy".msg = "Use `numpy
+= ak._nplikes.Numpy.instance()` instead" "jax".msg = "Use `jax =
 ak._nplikes.Jax.instance()` instead" "cupy".msg = "Use `cupy =
-ak._nplikes.Cupy.instance()` instead"
+ak._nplikes.Cupy.instance()` instead" [tool.nbqa.addopts] pyupgrade = ["--py38-
+plus"]
```

### Comparing `awkward-2.2.4/PKG-INFO` & `awkward-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.2.4
+Version: 2.3.0
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -31,18 +31,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==17
+Requires-Python: >=3.8
+Requires-Dist: awkward-cpp==20
 Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: numpy>=1.17.0
+Requires-Dist: numpy>=1.18.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
     <img src="https://github.com/scikit-hep/awkward-1.0/raw/main/docs-img/logo/logo-300px.png">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.2.4 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.3.0 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -17,17 +17,17 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
-Software Development Classifier: Topic :: Utilities Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==17 Requires-Dist: importlib-resources;
-python_version < '3.9' Requires-Dist: numpy>=1.17.0 Requires-Dist: packaging
+Software Development Classifier: Topic :: Utilities Requires-Python: >=3.8
+Requires-Dist: awkward-cpp==20 Requires-Dist: importlib-resources;
+python_version < '3.9' Requires-Dist: numpy>=1.18.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
 3.7%E2%80%923.11-blue)](https://www.python.org) [![BSD-3 Clause License](https:
```

