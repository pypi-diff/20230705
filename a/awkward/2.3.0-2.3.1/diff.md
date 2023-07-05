# Comparing `tmp/awkward-2.3.0.tar.gz` & `tmp/awkward-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jul  4 08:50:40 2023, max compression
+gzip compressed data, last modified: Wed Jul  5 18:40:12 2023, max compression
```

## Comparing `awkward-2.3.0.tar` & `awkward-2.3.1.tar`

### file list

```diff
@@ -1,874 +1,875 @@
--rw-r--r--   0        0        0     1893 2023-07-04 08:50:40.000000 awkward-2.3.0/CITATION.cff
--rw-r--r--   0        0        0    13855 2023-07-04 08:50:40.000000 awkward-2.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-07-04 08:50:40.000000 awkward-2.3.0/README.md
--rw-r--r--   0        0        0      241 2023-07-04 08:50:40.000000 awkward-2.3.0/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/conf.py
--rw-r--r--   0        0        0      346 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/index.md
--rw-r--r--   0        0        0    11642 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/redirects.json
--rw-r--r--   0        0        0       32 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/requirements-wasm.txt
--rw-r--r--   0        0        0      566 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/requirements.txt
--rw-r--r--   0        0        0      460 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24368 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/ak.behavior.md
--rw-r--r--   0        0        0     1426 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/index.md
--rw-r--r--   0        0        0     7349 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18472 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36902 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11694 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-07-04 08:50:40.000000 awkward-2.3.0/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1232 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/__init__.py
--rw-r--r--   0        0        0     4728 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_behavior.py
--rw-r--r--   0        0        0    37966 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0     1259 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_categorical.py
--rw-r--r--   0        0        0     2221 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_dispatch.py
--rw-r--r--   0        0        0    13571 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_do.py
--rw-r--r--   0        0        0    14543 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_errors.py
--rw-r--r--   0        0        0     5727 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5860 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_lookup.py
--rw-r--r--   0        0        0     8456 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_operators.py
--rw-r--r--   0        0        0     4861 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    28974 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_reducers.py
--rw-r--r--   0        0        0     1492 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1162 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_typing.py
--rw-r--r--   0        0        0     2263 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forth.py
--rw-r--r--   0        0        0   101292 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8044 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/jax.py
--rw-r--r--   0        0        0     8346 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/record.py
--rw-r--r--   0        0        0     1679 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     2082 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3763 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1453 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1425 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32612 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53532 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4491 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    16494 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    38024 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      806 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0      789 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    71373 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0    11085 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35828 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31510 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9698 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    52212 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0    43059 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/numba/layoutbuilder.py
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1118 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    16149 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     5365 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2276 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     1833 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    14154 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     3579 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/placeholder.py
--rw-r--r--   0        0        0     2379 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    48309 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0      542 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     1642 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    28289 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    41835 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    45406 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13361 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    41911 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    64744 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    62401 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    84928 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    48395 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    46696 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    56591 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    60368 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    19483 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      962 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6499 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5754 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     4104 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    21520 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/form.py
--rw-r--r--   0        0        0     6106 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5502 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5990 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     5213 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6412 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     9175 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5425 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     8237 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4564 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     9508 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/numba/__init__.py
--rw-r--r--   0        0        0    23907 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/numba/layoutbuilder.py
--rw-r--r--   0        0        0     4828 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3332 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     8301 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     3335 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5019 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3513 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5561 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5518 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     2998 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      943 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9540 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6499 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15528 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1418 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     7815 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12773 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2737 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5151 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4560 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3359 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     4503 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4544 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50327 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5203 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3433 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7767 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     2975 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      748 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2417 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14159 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1809 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1446 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     3872 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1522 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    29428 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2036 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11457 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     2960 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8680 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      890 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2478 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      728 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      929 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2396 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8760 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3219 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4627 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     5926 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     7760 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3552 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12363 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3078 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     5948 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4237 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2009 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     4922 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3878 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1800 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4211 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1807 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5037 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4118 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2256 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9532 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3025 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     2741 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2513 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     6788 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3020 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10397 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4573 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6361 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2267 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6144 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6041 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13339 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11167 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4357 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2693 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2115 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3331 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    17406 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2797 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3344 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23334 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4428 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9335 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2465 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2511 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     8016 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5544 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6008 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2563 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1709 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3713 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1477 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     1982 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8602 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     2168 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     3434 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6523 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4886 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8774 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     4355 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1341 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0    10177 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/type.py
--rw-r--r--   0        0        0     4593 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     1908 2023-07-04 08:50:40.000000 awkward-2.3.0/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     9772 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3786 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     5796 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12215 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12177 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9151 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2335 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    25853 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0912_packed.py
--rw-r--r--   0        0        0   109110 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28350 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26468 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33092 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18752 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     4372 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11759 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      513 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4607 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2845 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     1716 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2085_empty_if_typetracer.py
--rw-r--r--   0        0        0     2765 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     6369 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2192_union_absorb_indexed.py
--rw-r--r--   0        0        0     6063 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4104 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      315 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0      720 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2296_duplicate_field.py
--rw-r--r--   0        0        0     2262 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      648 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2929 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15615 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0      934 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2364_empty_list_of_string.py
--rw-r--r--   0        0        0    37200 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2921 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5250 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5848 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      956 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      212 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0    34463 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2408_layoutbuilder_in_numba.py
--rw-r--r--   0        0        0      854 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      800 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      704 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      351 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1563 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1211 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      545 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      495 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      857 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2471_flatten_string.py
--rw-r--r--   0        0        0     1032 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2484_reduce_starts_empty.py
--rw-r--r--   0        0        0      659 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2487_broadcast_list_offsets.py
--rw-r--r--   0        0        0     1319 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2490_reduce_regulararray_positional.py
--rw-r--r--   0        0        0     1816 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2495_concatenate_typetracer.py
--rw-r--r--   0        0        0     3800 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2501_positional_record_reducer.py
--rw-r--r--   0        0        0      603 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2503_deprecate_to_numpyform.py
--rw-r--r--   0        0        0     4942 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2512_record_array_carry.py
--rw-r--r--   0        0        0     1014 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2518_datetime_units_as_parameter.py
--rw-r--r--   0        0        0     5946 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2536_select_columns.py
--rw-r--r--   0        0        0      735 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2548_record_form_fields.py
--rw-r--r--   0        0        0     3629 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2549_list_nominal_type.py
--rw-r--r--   0        0        0      670 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2550_validity_error_recursive.py
--rw-r--r--   0        0        0      443 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2560_minimal_listarray.py
--rw-r--r--   0        0        0     1451 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/test_2564_string_broadcast_regular.py
--rw-r--r--   0        0        0      128 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-07-04 08:50:40.000000 awkward-2.3.0/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9757 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1629 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-07-04 08:50:40.000000 awkward-2.3.0/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-07-04 08:50:40.000000 awkward-2.3.0/.gitignore
--rw-r--r--   0        0        0     1520 2023-07-04 08:50:40.000000 awkward-2.3.0/LICENSE
--rw-r--r--   0        0        0     8580 2023-07-04 08:50:40.000000 awkward-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-07-04 08:50:40.000000 awkward-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-07-05 18:40:12.000000 awkward-2.3.1/CITATION.cff
+-rw-r--r--   0        0        0    13855 2023-07-05 18:40:12.000000 awkward-2.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-07-05 18:40:12.000000 awkward-2.3.1/README.md
+-rw-r--r--   0        0        0      241 2023-07-05 18:40:12.000000 awkward-2.3.1/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/redirects.json
+-rw-r--r--   0        0        0       32 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/requirements-wasm.txt
+-rw-r--r--   0        0        0      566 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/requirements.txt
+-rw-r--r--   0        0        0      460 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24368 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/reference/index.md
+-rw-r--r--   0        0        0     7349 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18472 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36902 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11694 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-07-05 18:40:12.000000 awkward-2.3.1/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1232 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/__init__.py
+-rw-r--r--   0        0        0     4728 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    37966 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0     1259 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_categorical.py
+-rw-r--r--   0        0        0     2221 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_dispatch.py
+-rw-r--r--   0        0        0    13571 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_do.py
+-rw-r--r--   0        0        0    14543 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5727 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     8456 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_operators.py
+-rw-r--r--   0        0        0     4861 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    28974 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     1492 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1162 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2263 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forth.py
+-rw-r--r--   0        0        0   101292 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8044 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/jax.py
+-rw-r--r--   0        0        0     8346 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/record.py
+-rw-r--r--   0        0        0     1679 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     2082 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1453 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1425 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32612 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53532 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4491 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    16494 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    38024 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      806 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0      789 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    71373 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0    11085 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35828 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31510 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9698 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    52212 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0    43059 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/numba/layoutbuilder.py
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1118 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    16149 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     5365 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2276 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     1833 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14154 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     3579 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/placeholder.py
+-rw-r--r--   0        0        0     2379 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    48309 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0      542 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     1642 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    28289 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    41835 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45406 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13361 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    41911 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    64744 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    62401 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    85072 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    48395 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    46696 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    56591 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    60368 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    19483 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      962 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6499 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5754 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     4104 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    21520 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     6106 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5502 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5990 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     5213 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6412 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     9175 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5425 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     8237 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4564 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     9508 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/numba/__init__.py
+-rw-r--r--   0        0        0    23907 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/numba/layoutbuilder.py
+-rw-r--r--   0        0        0     4828 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3332 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8301 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     3335 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5019 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3513 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5561 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5518 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     2998 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      943 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9540 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6499 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15528 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1418 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     7815 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12773 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2737 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5151 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4560 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3359 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     4503 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4544 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50327 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5203 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3433 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7767 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     2975 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      748 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2417 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14159 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1809 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1446 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     3872 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1522 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    29428 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2036 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11457 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3025 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     2960 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8680 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      890 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2478 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      728 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      929 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2396 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8760 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3219 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4627 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     5926 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     7760 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3552 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12363 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3078 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     5948 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4237 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2009 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     4922 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3878 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1800 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4211 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1807 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5037 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4118 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2256 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9532 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3025 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     2741 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2513 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     6788 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3020 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10397 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4573 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6361 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2267 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6144 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6041 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13339 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11167 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4357 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2693 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2115 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3331 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    17406 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2797 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3344 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23334 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4428 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9335 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2465 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2511 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     8016 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5544 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6008 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2563 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1709 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3713 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1477 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     1982 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8602 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2168 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     3434 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6523 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4886 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8774 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     4355 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1341 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10177 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4593 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1908 2023-07-05 18:40:12.000000 awkward-2.3.1/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     9772 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3786 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     5796 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12215 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12177 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9151 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2335 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    25853 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   109110 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28350 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26468 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33092 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18752 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4372 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      757 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11759 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      513 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4607 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2845 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1716 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2765 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     6369 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2192_union_absorb_indexed.py
+-rw-r--r--   0        0        0     6063 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4104 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      315 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      720 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2262 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      934 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37200 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2921 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5250 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5848 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      956 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0    34463 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2408_layoutbuilder_in_numba.py
+-rw-r--r--   0        0        0      854 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1211 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      545 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      495 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      857 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2471_flatten_string.py
+-rw-r--r--   0        0        0     1032 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2484_reduce_starts_empty.py
+-rw-r--r--   0        0        0      659 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2487_broadcast_list_offsets.py
+-rw-r--r--   0        0        0     1319 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2490_reduce_regulararray_positional.py
+-rw-r--r--   0        0        0     1816 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2495_concatenate_typetracer.py
+-rw-r--r--   0        0        0     3800 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2501_positional_record_reducer.py
+-rw-r--r--   0        0        0      603 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2503_deprecate_to_numpyform.py
+-rw-r--r--   0        0        0     4942 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2512_record_array_carry.py
+-rw-r--r--   0        0        0     1014 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2518_datetime_units_as_parameter.py
+-rw-r--r--   0        0        0     5946 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2536_select_columns.py
+-rw-r--r--   0        0        0      735 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2548_record_form_fields.py
+-rw-r--r--   0        0        0     3629 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2549_list_nominal_type.py
+-rw-r--r--   0        0        0      670 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2550_validity_error_recursive.py
+-rw-r--r--   0        0        0      443 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2560_minimal_listarray.py
+-rw-r--r--   0        0        0     1451 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2564_string_broadcast_regular.py
+-rw-r--r--   0        0        0      890 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/test_2571_awkward_ListOffsetArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      128 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-07-05 18:40:12.000000 awkward-2.3.1/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9757 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1629 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-07-05 18:40:12.000000 awkward-2.3.1/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-07-05 18:40:12.000000 awkward-2.3.1/.gitignore
+-rw-r--r--   0        0        0     1520 2023-07-05 18:40:12.000000 awkward-2.3.1/LICENSE
+-rw-r--r--   0        0        0     8580 2023-07-05 18:40:12.000000 awkward-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-07-05 18:40:12.000000 awkward-2.3.1/PKG-INFO
```

### Comparing `awkward-2.3.0/CITATION.cff` & `awkward-2.3.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/CONTRIBUTING.md` & `awkward-2.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/README.md` & `awkward-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/_toc.yml` & `awkward-2.3.1/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/conf.py` & `awkward-2.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/index.md` & `awkward-2.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/prepare_docstrings.py` & `awkward-2.3.1/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/redirects-user-guide.json` & `awkward-2.3.1/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/redirects.json` & `awkward-2.3.1/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/requirements.txt` & `awkward-2.3.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/_static/css/awkward.css` & `awkward-2.3.1/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/getting-started/community-tutorials.md` & `awkward-2.3.1/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/getting-started/index.md` & `awkward-2.3.1/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/getting-started/papers-and-talks.md` & `awkward-2.3.1/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.3.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/image/example-hierarchy.svg` & `awkward-2.3.1/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/reference/ak.behavior.md` & `awkward-2.3.1/docs/reference/ak.behavior.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.3.1/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/reference/awkwardforth.rst` & `awkward-2.3.1/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/reference/toctree.txt` & `awkward-2.3.1/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.3.1/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.3.1/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.3.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-json.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-python.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.3.1/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.3.1/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-constructors.md` & `awkward-2.3.1/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-lists.md` & `awkward-2.3.1/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-missing.md` & `awkward-2.3.1/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-records.md` & `awkward-2.3.1/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-strings.md` & `awkward-2.3.1/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.3.1/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.3.1/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.3.1/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.3.1/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.3.1/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-examine-type.md` & `awkward-2.3.1/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.3.1/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-filter-masked.md` & `awkward-2.3.1/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-filter-num.md` & `awkward-2.3.1/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.3.1/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.3.1/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.3.1/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-gpu.md` & `awkward-2.3.1/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-numpy.md` & `awkward-2.3.1/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-reducing.md` & `awkward-2.3.1/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-math-statistics.md` & `awkward-2.3.1/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.3.1/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.3.1/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.3.1/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.3.1/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.3.1/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.3.1/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.3.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.3.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.3.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.3.1/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-data-analysts.png` & `awkward-2.3.1/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-data-analysts.svg` & `awkward-2.3.1/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-developers.png` & `awkward-2.3.1/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-developers.svg` & `awkward-2.3.1/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-doxygen.png` & `awkward-2.3.1/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-sphinx.png` & `awkward-2.3.1/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-tutorials-alternate.png` & `awkward-2.3.1/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/panel-tutorials.png` & `awkward-2.3.1/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.3.1/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.3.1/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-timeline.png` & `awkward-2.3.1/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.3.1/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.3.1/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.3.1/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.3.1/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.3.1/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.3.1/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.3.1/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.3.1/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.3.1/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.3.1/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-array.svg` & `awkward-2.3.1/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-hierarchy.png` & `awkward-2.3.1/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.3.1/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.3.1/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.3.1/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-reduction.png` & `awkward-2.3.1/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/example-reduction.svg` & `awkward-2.3.1/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/git-strategy.pdf` & `awkward-2.3.1/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/git-strategy.png` & `awkward-2.3.1/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/git-strategy.svg` & `awkward-2.3.1/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.3.1/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.3.1/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/how-it-works.svg` & `awkward-2.3.1/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/sorting-axis.svg` & `awkward-2.3.1/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/all.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/any.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/count.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/max.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/min.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/product.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/diagrams/reducers/sum.svg` & `awkward-2.3.1/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/logo/favicon.ico` & `awkward-2.3.1/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/logo/logo-300px-white.png` & `awkward-2.3.1/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/logo/logo-300px.png` & `awkward-2.3.1/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/logo/logo-600px.png` & `awkward-2.3.1/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/logo/logo.svg` & `awkward-2.3.1/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/photos/desire-path.jpg` & `awkward-2.3.1/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.3.1/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/plots/awkward-0-popularity.png` & `awkward-2.3.1/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.3.1/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.3.1/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.3.1/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/__init__.py` & `awkward-2.3.1/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_behavior.py` & `awkward-2.3.1/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_broadcasting.py` & `awkward-2.3.1/src/awkward/_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_categorical.py` & `awkward-2.3.1/src/awkward/_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_dispatch.py` & `awkward-2.3.1/src/awkward/_dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_do.py` & `awkward-2.3.1/src/awkward/_do.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_errors.py` & `awkward-2.3.1/src/awkward/_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_kernels.py` & `awkward-2.3.1/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_layout.py` & `awkward-2.3.1/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_lookup.py` & `awkward-2.3.1/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_operators.py` & `awkward-2.3.1/src/awkward/_operators.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_parameters.py` & `awkward-2.3.1/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_prettyprint.py` & `awkward-2.3.1/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_reducers.py` & `awkward-2.3.1/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_regularize.py` & `awkward-2.3.1/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_slicing.py` & `awkward-2.3.1/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_typetracer.py` & `awkward-2.3.1/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_typing.py` & `awkward-2.3.1/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_util.py` & `awkward-2.3.1/src/awkward/_util.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_v2.py` & `awkward-2.3.1/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/cppyy.py` & `awkward-2.3.1/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/highlevel.py` & `awkward-2.3.1/src/awkward/highlevel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/index.py` & `awkward-2.3.1/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/jax.py` & `awkward-2.3.1/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/record.py` & `awkward-2.3.1/src/awkward/record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/typetracer.py` & `awkward-2.3.1/src/awkward/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/backend.py` & `awkward-2.3.1/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/cupy.py` & `awkward-2.3.1/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/dispatch.py` & `awkward-2.3.1/src/awkward/_backends/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/jax.py` & `awkward-2.3.1/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/numpy.py` & `awkward-2.3.1/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_backends/typetracer.py` & `awkward-2.3.1/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/avro.py` & `awkward-2.3.1/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cling.py` & `awkward-2.3.1/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/hist.py` & `awkward-2.3.1/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numexpr.py` & `awkward-2.3.1/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numpy.py` & `awkward-2.3.1/src/awkward/_connect/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/pyarrow.py` & `awkward-2.3.1/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/__init__.py` & `awkward-2.3.1/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.3.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.3.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.3.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.3.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.3.1/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/jax/reducers.py` & `awkward-2.3.1/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/jax/trees.py` & `awkward-2.3.1/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/arrayview.py` & `awkward-2.3.1/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.3.1/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/builder.py` & `awkward-2.3.1/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.3.1/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/layout.py` & `awkward-2.3.1/src/awkward/_connect/numba/layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/numba/layoutbuilder.py` & `awkward-2.3.1/src/awkward/_connect/numba/layoutbuilder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.3.1/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.3.1/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.3.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/__init__.py` & `awkward-2.3.1/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/array_module.py` & `awkward-2.3.1/src/awkward/_nplikes/array_module.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/cupy.py` & `awkward-2.3.1/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/dispatch.py` & `awkward-2.3.1/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/jax.py` & `awkward-2.3.1/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/numpy.py` & `awkward-2.3.1/src/awkward/_nplikes/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/numpylike.py` & `awkward-2.3.1/src/awkward/_nplikes/numpylike.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/placeholder.py` & `awkward-2.3.1/src/awkward/_nplikes/placeholder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/shape.py` & `awkward-2.3.1/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/typetracer.py` & `awkward-2.3.1/src/awkward/_nplikes/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/_nplikes/ufuncs.py` & `awkward-2.3.1/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/behaviors/categorical.py` & `awkward-2.3.1/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/behaviors/mixins.py` & `awkward-2.3.1/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/behaviors/string.py` & `awkward-2.3.1/src/awkward/behaviors/string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/__init__.py` & `awkward-2.3.1/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/bitmaskedarray.py` & `awkward-2.3.1/src/awkward/contents/bitmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/bytemaskedarray.py` & `awkward-2.3.1/src/awkward/contents/bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/content.py` & `awkward-2.3.1/src/awkward/contents/content.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/emptyarray.py` & `awkward-2.3.1/src/awkward/contents/emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/indexedarray.py` & `awkward-2.3.1/src/awkward/contents/indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/indexedoptionarray.py` & `awkward-2.3.1/src/awkward/contents/indexedoptionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/listarray.py` & `awkward-2.3.1/src/awkward/contents/listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/listoffsetarray.py` & `awkward-2.3.1/src/awkward/contents/listoffsetarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,17 +882,18 @@
 
         if negaxis is None:
             return self._content._is_unique(negaxis, starts, parents, outlength)
 
         if not branch and (negaxis == depth):
             return self._content._is_unique(negaxis - 1, starts, parents, outlength)
         else:
-            nextparents = Index64.empty(
-                self._offsets[-1] - self._offsets[0], self._backend.index_nplike
+            nextlen = self._backend.index_nplike.index_as_shape_item(
+                self._offsets[-1] - self._offsets[0]
             )
+            nextparents = Index64.empty(nextlen, self._backend.index_nplike)
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
             self._backend.maybe_kernel_error(
                 self._backend[
@@ -977,17 +978,18 @@
             return ak.contents.ListOffsetArray(
                 outcontent._compact_offsets64(True),
                 outcontent._content._carry(outcarry, False),
                 parameters=self._parameters,
             )
 
         else:
-            nextparents = Index64.empty(
-                self._offsets[-1] - self._offsets[0], self._backend.index_nplike
+            nextlen = self._backend.index_nplike.index_as_shape_item(
+                self._offsets[-1] - self._offsets[0]
             )
+            nextparents = Index64.empty(nextlen, self._backend.index_nplike)
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
             self._backend.maybe_kernel_error(
                 self._backend[
@@ -1161,20 +1163,18 @@
 
             out_offsets = self._compact_offsets64(True)
             out = outcontent._carry(outcarry, False)
             return ak.contents.ListOffsetArray(
                 out_offsets, out, parameters=self._parameters
             )
         else:
-            nextparents = Index64.empty(
-                self._backend.index_nplike.index_as_shape_item(
-                    self._offsets[-1] - self._offsets[0]
-                ),
-                self._backend.index_nplike,
+            nextlen = self._backend.index_nplike.index_as_shape_item(
+                self._offsets[-1] - self._offsets[0]
             )
+            nextparents = Index64.empty(nextlen, self._backend.index_nplike)
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
             self._backend.maybe_kernel_error(
                 self._backend[
@@ -1295,18 +1295,18 @@
 
             return ak.contents.ListOffsetArray(
                 self._compact_offsets64(True),
                 outcontent._carry(outcarry, False),
                 parameters=self._parameters,
             )
         else:
-            nextparents = Index64.empty(
-                index_nplike.index_as_shape_item(self._offsets[-1] - self._offsets[0]),
-                index_nplike,
+            nextlen = index_nplike.index_as_shape_item(
+                self._offsets[-1] - self._offsets[0]
             )
+            nextparents = Index64.empty(nextlen, index_nplike)
             lenstarts = self._offsets.length - 1
 
             assert (
                 nextparents.nplike is index_nplike
                 and self._offsets.nplike is index_nplike
             )
             self._backend.maybe_kernel_error(
```

### Comparing `awkward-2.3.0/src/awkward/contents/numpyarray.py` & `awkward-2.3.1/src/awkward/contents/numpyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/recordarray.py` & `awkward-2.3.1/src/awkward/contents/recordarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/regulararray.py` & `awkward-2.3.1/src/awkward/contents/regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/unionarray.py` & `awkward-2.3.1/src/awkward/contents/unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/contents/unmaskedarray.py` & `awkward-2.3.1/src/awkward/contents/unmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/__init__.py` & `awkward-2.3.1/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/bitmaskedform.py` & `awkward-2.3.1/src/awkward/forms/bitmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/bytemaskedform.py` & `awkward-2.3.1/src/awkward/forms/bytemaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/emptyform.py` & `awkward-2.3.1/src/awkward/forms/emptyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/form.py` & `awkward-2.3.1/src/awkward/forms/form.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/indexedform.py` & `awkward-2.3.1/src/awkward/forms/indexedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/indexedoptionform.py` & `awkward-2.3.1/src/awkward/forms/indexedoptionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/listform.py` & `awkward-2.3.1/src/awkward/forms/listform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/listoffsetform.py` & `awkward-2.3.1/src/awkward/forms/listoffsetform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/numpyform.py` & `awkward-2.3.1/src/awkward/forms/numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/recordform.py` & `awkward-2.3.1/src/awkward/forms/recordform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/regularform.py` & `awkward-2.3.1/src/awkward/forms/regularform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/unionform.py` & `awkward-2.3.1/src/awkward/forms/unionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/forms/unmaskedform.py` & `awkward-2.3.1/src/awkward/forms/unmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/numba/__init__.py` & `awkward-2.3.1/src/awkward/numba/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/numba/layoutbuilder.py` & `awkward-2.3.1/src/awkward/numba/layoutbuilder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/__init__.py` & `awkward-2.3.1/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_all.py` & `awkward-2.3.1/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_almost_equal.py` & `awkward-2.3.1/src/awkward/operations/ak_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_any.py` & `awkward-2.3.1/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_argcartesian.py` & `awkward-2.3.1/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_argcombinations.py` & `awkward-2.3.1/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_argmax.py` & `awkward-2.3.1/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_argmin.py` & `awkward-2.3.1/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_argsort.py` & `awkward-2.3.1/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_backend.py` & `awkward-2.3.1/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.3.1/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.3.1/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_cartesian.py` & `awkward-2.3.1/src/awkward/operations/ak_cartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_categories.py` & `awkward-2.3.1/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_combinations.py` & `awkward-2.3.1/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_concatenate.py` & `awkward-2.3.1/src/awkward/operations/ak_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_copy.py` & `awkward-2.3.1/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_corr.py` & `awkward-2.3.1/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_count.py` & `awkward-2.3.1/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.3.1/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_covar.py` & `awkward-2.3.1/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_drop_none.py` & `awkward-2.3.1/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_enforce_type.py` & `awkward-2.3.1/src/awkward/operations/ak_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_fields.py` & `awkward-2.3.1/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_fill_none.py` & `awkward-2.3.1/src/awkward/operations/ak_fill_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_firsts.py` & `awkward-2.3.1/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_flatten.py` & `awkward-2.3.1/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_arrow.py` & `awkward-2.3.1/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.3.1/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.3.1/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_buffers.py` & `awkward-2.3.1/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_categorical.py` & `awkward-2.3.1/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_cupy.py` & `awkward-2.3.1/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_iter.py` & `awkward-2.3.1/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_jax.py` & `awkward-2.3.1/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_json.py` & `awkward-2.3.1/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_numpy.py` & `awkward-2.3.1/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_parquet.py` & `awkward-2.3.1/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.3.1/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_from_regular.py` & `awkward-2.3.1/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_full_like.py` & `awkward-2.3.1/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_is_categorical.py` & `awkward-2.3.1/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_is_none.py` & `awkward-2.3.1/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_is_tuple.py` & `awkward-2.3.1/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_is_valid.py` & `awkward-2.3.1/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_isclose.py` & `awkward-2.3.1/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_linear_fit.py` & `awkward-2.3.1/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_local_index.py` & `awkward-2.3.1/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_mask.py` & `awkward-2.3.1/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_max.py` & `awkward-2.3.1/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_mean.py` & `awkward-2.3.1/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.3.1/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.3.1/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.3.1/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_min.py` & `awkward-2.3.1/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_moment.py` & `awkward-2.3.1/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.3.1/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.3.1/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_num.py` & `awkward-2.3.1/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_ones_like.py` & `awkward-2.3.1/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_pad_none.py` & `awkward-2.3.1/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_parameters.py` & `awkward-2.3.1/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_prod.py` & `awkward-2.3.1/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_ptp.py` & `awkward-2.3.1/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_ravel.py` & `awkward-2.3.1/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_run_lengths.py` & `awkward-2.3.1/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_singletons.py` & `awkward-2.3.1/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_softmax.py` & `awkward-2.3.1/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_sort.py` & `awkward-2.3.1/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_std.py` & `awkward-2.3.1/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_strings_astype.py` & `awkward-2.3.1/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_sum.py` & `awkward-2.3.1/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_arrow.py` & `awkward-2.3.1/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.3.1/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_backend.py` & `awkward-2.3.1/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_buffers.py` & `awkward-2.3.1/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_categorical.py` & `awkward-2.3.1/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_cupy.py` & `awkward-2.3.1/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.3.1/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_jax.py` & `awkward-2.3.1/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_json.py` & `awkward-2.3.1/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_layout.py` & `awkward-2.3.1/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_list.py` & `awkward-2.3.1/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_numpy.py` & `awkward-2.3.1/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_packed.py` & `awkward-2.3.1/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_parquet.py` & `awkward-2.3.1/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.3.1/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_to_regular.py` & `awkward-2.3.1/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_transform.py` & `awkward-2.3.1/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_type.py` & `awkward-2.3.1/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_unflatten.py` & `awkward-2.3.1/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_unzip.py` & `awkward-2.3.1/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_validity_error.py` & `awkward-2.3.1/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_values_astype.py` & `awkward-2.3.1/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_var.py` & `awkward-2.3.1/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_where.py` & `awkward-2.3.1/src/awkward/operations/ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_with_field.py` & `awkward-2.3.1/src/awkward/operations/ak_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_with_name.py` & `awkward-2.3.1/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_with_parameter.py` & `awkward-2.3.1/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_without_field.py` & `awkward-2.3.1/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_without_parameters.py` & `awkward-2.3.1/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_zeros_like.py` & `awkward-2.3.1/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/operations/ak_zip.py` & `awkward-2.3.1/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/__init__.py` & `awkward-2.3.1/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.3.1/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/arraytype.py` & `awkward-2.3.1/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/listtype.py` & `awkward-2.3.1/src/awkward/types/listtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/numpytype.py` & `awkward-2.3.1/src/awkward/types/numpytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/optiontype.py` & `awkward-2.3.1/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/recordtype.py` & `awkward-2.3.1/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/regulartype.py` & `awkward-2.3.1/src/awkward/types/regulartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/scalartype.py` & `awkward-2.3.1/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/type.py` & `awkward-2.3.1/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/uniontype.py` & `awkward-2.3.1/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/src/awkward/types/unknowntype.py` & `awkward-2.3.1/src/awkward/types/unknowntype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0002_minimal_listarray.py` & `awkward-2.3.1/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0008_slices_and_getitem.py` & `awkward-2.3.1/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0011_listarray.py` & `awkward-2.3.1/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0013_error_handling_struct.py` & `awkward-2.3.1/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0014_finish_up_getitem.py` & `awkward-2.3.1/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0018_fromiter_fillable.py` & `awkward-2.3.1/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0019_use_json_library.py` & `awkward-2.3.1/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.3.1/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0021_emptyarray.py` & `awkward-2.3.1/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0023_regular_array.py` & `awkward-2.3.1/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0024_use_regular_array.py` & `awkward-2.3.1/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0025_record_array.py` & `awkward-2.3.1/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0028_add_dressed_types.py` & `awkward-2.3.1/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0032_replace_dressedtype.py` & `awkward-2.3.1/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0046_start_indexedarray.py` & `awkward-2.3.1/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.3.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0057_introducing_forms.py` & `awkward-2.3.1/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0070_argmin_and_argmax.py` & `awkward-2.3.1/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0072_fillna_operation.py` & `awkward-2.3.1/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0074_argsort_and_sort.py` & `awkward-2.3.1/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0077_zip_operation.py` & `awkward-2.3.1/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0078_argcross_and_cross.py` & `awkward-2.3.1/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0079_argchoose_and_choose.py` & `awkward-2.3.1/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.3.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0084_start_unionarray.py` & `awkward-2.3.1/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0086_nep13_ufunc.py` & `awkward-2.3.1/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0089_numpy_functions.py` & `awkward-2.3.1/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.3.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0107_assign_fields_to_records.py` & `awkward-2.3.1/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.3.1/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0115_generic_reducer_operation.py` & `awkward-2.3.1/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0118_numba_cpointers.py` & `awkward-2.3.1/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.3.1/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0124_strings_in_numba.py` & `awkward-2.3.1/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0127_tomask_operation.py` & `awkward-2.3.1/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.3.1/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0138_emptyarray_type.py` & `awkward-2.3.1/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0150_flatten.py` & `awkward-2.3.1/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0163_negative_axis_wrap.py` & `awkward-2.3.1/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.3.1/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0173_astype_operation.py` & `awkward-2.3.1/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0184_concatenate_operation.py` & `awkward-2.3.1/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.3.1/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.3.1/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0222_count_with_axis0.py` & `awkward-2.3.1/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0224_arrow_to_awkward.py` & `awkward-2.3.1/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0264_reduce_last_empty.py` & `awkward-2.3.1/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0273_path_for_with_field.py` & `awkward-2.3.1/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.3.1/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.3.1/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0315_integerindex.py` & `awkward-2.3.1/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0331_pandas_indexedarray.py` & `awkward-2.3.1/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.3.1/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.3.1/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0348_form_keys.py` & `awkward-2.3.1/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0355_mixins.py` & `awkward-2.3.1/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0395_complex_type_arrays.py` & `awkward-2.3.1/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.3.1/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.3.1/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.3.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0404_array_validity_check.py` & `awkward-2.3.1/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.3.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.3.1/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.3.1/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.3.1/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.3.1/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0496_provide_local_index.py` & `awkward-2.3.1/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.3.1/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.3.1/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.3.1/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.3.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0549_numba_array_asarray.py` & `awkward-2.3.1/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0557_min_max_initial_argument.py` & `awkward-2.3.1/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.3.1/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0572_numba_array_ndim.py` & `awkward-2.3.1/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.3.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0583_implement_unflatten_function.py` & `awkward-2.3.1/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.3.1/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.3.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.3.1/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0674_categorical_validation.py` & `awkward-2.3.1/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.3.1/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.3.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.3.1/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0733_run_lengths.py` & `awkward-2.3.1/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.3.1/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.3.1/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0773_typeparser.py` & `awkward-2.3.1/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.3.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.3.1/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0803_argsort_fix_type.py` & `awkward-2.3.1/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.3.1/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.3.1/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.3.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0828_arrow_datatype_null.py` & `awkward-2.3.1/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0835_datetime_type.py` & `awkward-2.3.1/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0835_datetime_type_pandas.py` & `awkward-2.3.1/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.3.1/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0850_argsort_mask_array.py` & `awkward-2.3.1/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.3.1/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0875_arrow_null_type.py` & `awkward-2.3.1/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0879_non_primitive_with_field.py` & `awkward-2.3.1/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.3.1/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0889_ptp.py` & `awkward-2.3.1/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0896_content_classes_refactoring.py` & `awkward-2.3.1/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.3.1/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.3.1/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.3.1/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.3.1/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0912_packed.py` & `awkward-2.3.1/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0914_types_and_forms.py` & `awkward-2.3.1/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0916_datetime_values_astype.py` & `awkward-2.3.1/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.3.1/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.3.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.3.1/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.3.1/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0959__getitem_array_implementation.py` & `awkward-2.3.1/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.3.1/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.3.1/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.3.1/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0984_ravel.py` & `awkward-2.3.1/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.3.1/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.3.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.3.1/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1030_mixin_class_name.py` & `awkward-2.3.1/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1031_start_getitem_next.py` & `awkward-2.3.1/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.3.1/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1049_concatenate_single_array.py` & `awkward-2.3.1/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.3.1/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1059_localindex.py` & `awkward-2.3.1/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.3.1/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.3.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1072_sort.py` & `awkward-2.3.1/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1074_combinations.py` & `awkward-2.3.1/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1075_validityerror.py` & `awkward-2.3.1/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1110_type_tracer_1.py` & `awkward-2.3.1/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1116_project_maskedarrays.py` & `awkward-2.3.1/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.3.1/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.3.1/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.3.1/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1135_rpad_operation.py` & `awkward-2.3.1/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.3.1/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1137_num.py` & `awkward-2.3.1/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1142_numbers_to_type.py` & `awkward-2.3.1/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1149_datetime_sort.py` & `awkward-2.3.1/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.3.1/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1162_ak_from_json_schema.py` & `awkward-2.3.1/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.3.1/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.3.1/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.3.1/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1193_is_none_nested_option.py` & `awkward-2.3.1/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1233_ak_with_name.py` & `awkward-2.3.1/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.3.1/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1259_simplify_optiontype.py` & `awkward-2.3.1/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.3.1/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1271_fix_4D_reducers.py` & `awkward-2.3.1/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1294_to_and_from_parquet.py` & `awkward-2.3.1/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.3.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.3.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1300b_same_for_numba.py` & `awkward-2.3.1/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1308_zip_after_option.py` & `awkward-2.3.1/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1318_array_function_types.py` & `awkward-2.3.1/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1320_mask_identity_defaults.py` & `awkward-2.3.1/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.3.1/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1345_avro_reader.py` & `awkward-2.3.1/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1351_is_tuple.py` & `awkward-2.3.1/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1374_to_rdataframe.py` & `awkward-2.3.1/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1377_ravel_string.py` & `awkward-2.3.1/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.3.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1399_from_jax.py` & `awkward-2.3.1/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1399_to_jax.py` & `awkward-2.3.1/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1405_slicing_untested_cases.py` & `awkward-2.3.1/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1415_behaviour_forwarding.py` & `awkward-2.3.1/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.3.1/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.3.1/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.3.1/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.3.1/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1473_from_rdataframe.py` & `awkward-2.3.1/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.3.1/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.3.1/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.3.1/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1504_typetracer_like.py` & `awkward-2.3.1/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.3.1/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1511_set_attribute.py` & `awkward-2.3.1/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.3.1/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.3.1/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.3.1/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.3.1/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.3.1/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.3.1/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.3.1/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1607_no_reducers_on_records.py` & `awkward-2.3.1/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1613_generator_tolayout_records.py` & `awkward-2.3.1/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.3.1/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1620_layout_builders.py` & `awkward-2.3.1/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.3.1/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.3.1/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.3.1/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1671_categorical_type.py` & `awkward-2.3.1/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1672_broadcast_parameters.py` & `awkward-2.3.1/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1677_array_builder_in_numba.py` & `awkward-2.3.1/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.3.1/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.3.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1688_pack_categorical.py` & `awkward-2.3.1/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1703_fill_none_typetracer.py` & `awkward-2.3.1/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.3.1/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.3.1/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.3.1/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.3.1/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1762_jax_behavior_support.py` & `awkward-2.3.1/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1764_jax_jacobian.py` & `awkward-2.3.1/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.3.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1766_record_form_fields.py` & `awkward-2.3.1/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.3.1/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.3.1/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1790_reduce_regulararray.py` & `awkward-2.3.1/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.3.1/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.3.1/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.3.1/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.3.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.3.1/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.3.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.3.1/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1904_drop_none.py` & `awkward-2.3.1/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.3.1/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.3.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.3.1/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1936_with_field_broadcasting.py` & `awkward-2.3.1/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1940_ak_backend.py` & `awkward-2.3.1/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1943_regular_indexing.py` & `awkward-2.3.1/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.3.1/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_1961_ak_without_field.py` & `awkward-2.3.1/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2020_reduce_axis_none.py` & `awkward-2.3.1/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.3.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2023_from_rdataframe.py` & `awkward-2.3.1/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.3.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.3.1/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2055_array_builder_check.py` & `awkward-2.3.1/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2058_merge_numpy_array.py` & `awkward-2.3.1/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2064_fill_none_record.py` & `awkward-2.3.1/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.3.1/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2070_to_layout_string.py` & `awkward-2.3.1/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.3.1/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2078_array_function_wrap.py` & `awkward-2.3.1/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2082_broadcast_zero_size.py` & `awkward-2.3.1/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2085_empty_if_typetracer.py` & `awkward-2.3.1/tests/test_2085_empty_if_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2096_ak_scalar_type.py` & `awkward-2.3.1/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2101_pickle_behavior_class.py` & `awkward-2.3.1/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2104_numpy_merge_option.py` & `awkward-2.3.1/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2106_pickle_class.py` & `awkward-2.3.1/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2108_fill_none_indexed.py` & `awkward-2.3.1/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2115_fix_up_typetracers.py` & `awkward-2.3.1/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2125_type_of_scalar.py` & `awkward-2.3.1/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.3.1/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2179_parameter_merging_rules.py` & `awkward-2.3.1/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2185_merge_union_of_records.py` & `awkward-2.3.1/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.3.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2192_union_absorb_indexed.py` & `awkward-2.3.1/tests/test_2192_union_absorb_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2198_almost_equal.py` & `awkward-2.3.1/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.3.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2214_offset_bool_index.py` & `awkward-2.3.1/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.3.1/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2229_getitem_range_slice.py` & `awkward-2.3.1/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.3.1/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.3.1/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.3.1/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2246_slice_not_packed.py` & `awkward-2.3.1/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2250_full_like_bool.py` & `awkward-2.3.1/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.3.1/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2263_to_packed_list.py` & `awkward-2.3.1/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2267_broadcast_fields.py` & `awkward-2.3.1/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2293_unflatten_typetracer.py` & `awkward-2.3.1/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2296_duplicate_field.py` & `awkward-2.3.1/tests/test_2296_duplicate_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2297_common_backend.py` & `awkward-2.3.1/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.3.1/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2306_cppyy_git.py` & `awkward-2.3.1/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2319_from_buffers_array.py` & `awkward-2.3.1/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2327_array_interface.py` & `awkward-2.3.1/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.3.1/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.3.1/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2354_ufunc_same_backend.py` & `awkward-2.3.1/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2355_to_backend_record.py` & `awkward-2.3.1/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.3.1/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2364_empty_list_of_string.py` & `awkward-2.3.1/tests/test_2364_empty_list_of_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2365_enforce_type.py` & `awkward-2.3.1/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2368_type_is_equal.py` & `awkward-2.3.1/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2373_unzip_touching.py` & `awkward-2.3.1/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2374_cartesian_touching.py` & `awkward-2.3.1/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2385_with_field_empty_record.py` & `awkward-2.3.1/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2395_copy_asarray_touch.py` & `awkward-2.3.1/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2408_layoutbuilder_in_numba.py` & `awkward-2.3.1/tests/test_2408_layoutbuilder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2410_string_broadcast.py` & `awkward-2.3.1/tests/test_2410_string_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.3.1/tests/test_2411_cartesian_axis_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2417_bytemasked_singletons.py` & `awkward-2.3.1/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2424_almost_equal_union_record.py` & `awkward-2.3.1/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2425_forms_from_type.py` & `awkward-2.3.1/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2426_is_equal_to.py` & `awkward-2.3.1/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2471_flatten_string.py` & `awkward-2.3.1/tests/test_2471_flatten_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2484_reduce_starts_empty.py` & `awkward-2.3.1/tests/test_2484_reduce_starts_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2487_broadcast_list_offsets.py` & `awkward-2.3.1/tests/test_2487_broadcast_list_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2490_reduce_regulararray_positional.py` & `awkward-2.3.1/tests/test_2490_reduce_regulararray_positional.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2495_concatenate_typetracer.py` & `awkward-2.3.1/tests/test_2495_concatenate_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2501_positional_record_reducer.py` & `awkward-2.3.1/tests/test_2501_positional_record_reducer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2503_deprecate_to_numpyform.py` & `awkward-2.3.1/tests/test_2503_deprecate_to_numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2512_record_array_carry.py` & `awkward-2.3.1/tests/test_2512_record_array_carry.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2518_datetime_units_as_parameter.py` & `awkward-2.3.1/tests/test_2518_datetime_units_as_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2536_select_columns.py` & `awkward-2.3.1/tests/test_2536_select_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2548_record_form_fields.py` & `awkward-2.3.1/tests/test_2548_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2549_list_nominal_type.py` & `awkward-2.3.1/tests/test_2549_list_nominal_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2550_validity_error_recursive.py` & `awkward-2.3.1/tests/test_2550_validity_error_recursive.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/test_2564_string_broadcast_regular.py` & `awkward-2.3.1/tests/test_2564_string_broadcast_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/list-depths-records-list.parquet` & `awkward-2.3.1/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/list-depths-records.parquet` & `awkward-2.3.1/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/list-depths-strings.parquet` & `awkward-2.3.1/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/list-depths.parquet` & `awkward-2.3.1/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nonnullable-depths.parquet` & `awkward-2.3.1/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-depths.parquet` & `awkward-2.3.1/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-levels.parquet` & `awkward-2.3.1/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.3.1/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.3.1/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.3.1/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-list-depths.parquet` & `awkward-2.3.1/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/nullable-record-primitives.parquet` & `awkward-2.3.1/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/record-primitives.parquet` & `awkward-2.3.1/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/test-nan-inf.json` & `awkward-2.3.1/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/test-two-arrays.json` & `awkward-2.3.1/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests/samples/test.json` & `awkward-2.3.1/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1276_cuda_num.py` & `awkward-2.3.1/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.3.1/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.3.1/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1276_from_cupy.py` & `awkward-2.3.1/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.3.1/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1381_check_errors.py` & `awkward-2.3.1/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.3.1/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/.gitignore` & `awkward-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/LICENSE` & `awkward-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.3.0/pyproject.toml` & `awkward-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.3.0"
+version = "2.3.1"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.8"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,15 +36,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==20",
+    "awkward_cpp==21",
     "importlib_resources;python_version < \"3.9\"",
     "numpy>=1.18.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.3.0"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.3.1"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.8" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -11,15 +11,15 @@
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==20",
+Utilities", ] dependencies = [ "awkward_cpp==21",
 "importlib_resources;python_version < \"3.9\"", "numpy>=1.18.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
```

### Comparing `awkward-2.3.0/PKG-INFO` & `awkward-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.3.0
+Version: 2.3.1
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,15 +32,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
-Requires-Dist: awkward-cpp==20
+Requires-Dist: awkward-cpp==21
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: numpy>=1.18.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.3.0 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.3.1 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,15 +18,15 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.8
-Requires-Dist: awkward-cpp==20 Requires-Dist: importlib-resources;
+Requires-Dist: awkward-cpp==21 Requires-Dist: importlib-resources;
 python_version < '3.9' Requires-Dist: numpy>=1.18.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
```

