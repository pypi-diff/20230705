# Comparing `tmp/python-parakeet-0.4.4.tar.gz` & `tmp/python-parakeet-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-parakeet-0.4.4.tar", last modified: Fri Jun 16 11:31:50 2023, max compression
+gzip compressed data, was "python-parakeet-0.4.5.tar", last modified: Wed Jul  5 14:50:51 2023, max compression
```

## Comparing `python-parakeet-0.4.4.tar` & `python-parakeet-0.4.5.tar`

### file list

```diff
@@ -1,427 +1,427 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.069758 python-parakeet-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/quay-io-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/snapcraft.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/conda/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/source/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/ext/pydantic_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   153379 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet.png
--rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet_small.png
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/publications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/39.feature
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/44.doc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/50.feature
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/51.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/pybind11/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/labeler_merged.yml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)    74047 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    58510 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.069758 python-parakeet-0.4.4/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    57522 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    42083 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    69754 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   105769 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    67597 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/snap/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/parakeet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_average_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/beam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_all_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_refine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/config/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/metadata/_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/pdb/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_mill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_sputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_cbed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_exit_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/data/files/
--rw-r--r--   0 runner    (1001) docker     (123)  6040922 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/3jb9.cif
--rw-r--r--   0 runner    (1001) docker     (123)  3095859 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/4v1w.cif
--rw-r--r--   0 runner    (1001) docker     (123) 18908004 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/4v5d.cif
--rw-r--r--   0 runner    (1001) docker     (123)  7821805 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/6qt9.cif
--rw-r--r--   0 runner    (1001) docker     (123)  2781544 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/6z6u.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/water.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/dqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/error.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/freeze/
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/freeze_ext.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/sphere_packer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/inelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/landau.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/microscope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/sample/
--rw-r--r--   0 runner    (1001) docker     (123)    57480 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_mill.py
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_sputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/distribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    25109 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/parakeet/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_cbed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_exit_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/phase_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/parakeet/util/
--rw-r--r--   0 runner    (1001) docker     (123)    37870 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/util/calibrate_ice_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/python_parakeet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-16 11:31:50.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_beam.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_inelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_landau.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sample_distribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sphere_packer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.049102 python-parakeet-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.049102 python-parakeet-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/quay-io-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/snapcraft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.049102 python-parakeet-0.4.5/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/conda/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/docs/source/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/ext/pydantic_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   153379 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/images/parakeet.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/images/parakeet_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/images/parakeet_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/newsfragments/39.feature
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/newsfragments/44.doc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/newsfragments/50.feature
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/newsfragments/51.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 14:50:29.000000 python-parakeet-0.4.5/pybind11/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.053102 python-parakeet-0.4.5/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    74047 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.057101 python-parakeet-0.4.5/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    58510 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.049102 python-parakeet-0.4.5/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.065101 python-parakeet-0.4.5/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57522 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.065101 python-parakeet-0.4.5/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42083 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69754 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105769 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67597 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.065101 python-parakeet-0.4.5/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pybind11/setup_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.069101 python-parakeet-0.4.5/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.073101 python-parakeet-0.4.5/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-05 14:50:30.000000 python-parakeet-0.4.5/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.073101 python-parakeet-0.4.5/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.049102 python-parakeet-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.073101 python-parakeet-0.4.5/src/parakeet/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/parakeet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.073101 python-parakeet-0.4.5/src/parakeet/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/_average_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/analyse/_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/beam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.073101 python-parakeet-0.4.5/src/parakeet/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_average_all_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_average_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/analyse/_refine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/config/_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/config/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/config/_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/metadata/_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/pdb/_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/pdb/_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/_add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/_mill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/sample/_sputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/command_line/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_cbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_exit_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/command_line/simulate/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.077101 python-parakeet-0.4.5/src/parakeet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.113101 python-parakeet-0.4.5/src/parakeet/data/files/
+-rw-r--r--   0 runner    (1001) docker     (123)  6040922 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/3jb9.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  3095859 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/4v1w.cif
+-rw-r--r--   0 runner    (1001) docker     (123) 18908004 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/4v5d.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  7821805 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/6qt9.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  2781544 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/6z6u.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/data/files/water.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/dqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/error.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.113101 python-parakeet-0.4.5/src/parakeet/freeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/freeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/freeze/freeze_ext.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/freeze/sphere_packer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/inelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/landau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/microscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/src/parakeet/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)    57478 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/_add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/_mill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/_sputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/sample/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26455 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/src/parakeet/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_cbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_exit_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/phase_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/simulate/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/src/parakeet/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    37870 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/src/parakeet/util/calibrate_ice_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/src/python_parakeet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-05 14:50:51.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 14:50:50.000000 python-parakeet-0.4.5/src/python_parakeet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:50:51.117101 python-parakeet-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_inelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_landau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_sample_distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-05 14:50:28.000000 python-parakeet-0.4.5/tests/test_sphere_packer.py
```

### Comparing `python-parakeet-0.4.4/.github/workflows/conda.yml` & `python-parakeet-0.4.5/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/docker-publish.yml` & `python-parakeet-0.4.5/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/python-package.yml` & `python-parakeet-0.4.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/python-publish.yml` & `python-parakeet-0.4.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/quay-io-publish.yml` & `python-parakeet-0.4.5/.github/workflows/quay-io-publish.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/snapcraft.yml` & `python-parakeet-0.4.5/.github/workflows/snapcraft.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.github/workflows/sphinx.yml` & `python-parakeet-0.4.5/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.gitignore` & `python-parakeet-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/.pre-commit-config.yaml` & `python-parakeet-0.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/CMakeLists.txt` & `python-parakeet-0.4.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/LICENSE` & `python-parakeet-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/PKG-INFO` & `python-parakeet-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-parakeet
-Version: 0.4.4
+Version: 0.4.5
 Summary: A phantom generator
 Home-page: https://github.com/rosalindfranklininstitute/parakeet
 Author: James Parkhurst
 Author-email: james.parkhurst@diamond.ac.uk
 License: GPL v3
 Project-URL: Source, https://github.com/rosalindfranklininstitute/parakeet
 Project-URL: Tracker, https://github.com/rosalindfranklininstitute/parakeet/issues
```

### Comparing `python-parakeet-0.4.4/README.md` & `python-parakeet-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/conda/meta.yaml` & `python-parakeet-0.4.5/conda/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     - maptools
     - mrcfile
     - numpy
     - pandas
     - pillow
     - pip
     - profet
-    - pydantic
+    - pydantic==1.10.10
     - python
     - python-multem
     - pyyaml
     - scipy
     - starfile
     - importlib_resources
   run:
@@ -71,15 +71,15 @@
     - h5py
     - maptools
     - mrcfile
     - numpy
     - pandas
     - pillow
     - profet
-    - pydantic
+    - pydantic==1.10.10
     - python
     - python-multem
     - pyyaml
     - scipy
     - starfile
     - importlib_resources
```

### Comparing `python-parakeet-0.4.4/docs/Makefile` & `python-parakeet-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/make.bat` & `python-parakeet-0.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/api.rst` & `python-parakeet-0.4.5/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/conf.py` & `python-parakeet-0.4.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/configuration.rst` & `python-parakeet-0.4.5/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/ext/pydantic_settings.py` & `python-parakeet-0.4.5/docs/source/ext/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/images/parakeet.png` & `python-parakeet-0.4.5/docs/source/images/parakeet.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/images/parakeet_logo.png` & `python-parakeet-0.4.5/docs/source/images/parakeet_logo.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/images/parakeet_small.png` & `python-parakeet-0.4.5/docs/source/images/parakeet_small.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/index.rst` & `python-parakeet-0.4.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/installation.rst` & `python-parakeet-0.4.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/tutorial.rst` & `python-parakeet-0.4.5/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/docs/source/usage.rst` & `python-parakeet-0.4.5/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.appveyor.yml` & `python-parakeet-0.4.5/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.clang-format` & `python-parakeet-0.4.5/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.cmake-format.yaml` & `python-parakeet-0.4.5/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/CONTRIBUTING.md` & `python-parakeet-0.4.5/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.md` & `python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/feature-request.md` & `python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/question.md` & `python-parakeet-0.4.5/pybind11/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/dependabot.yml` & `python-parakeet-0.4.5/pybind11/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/workflows/ci.yml` & `python-parakeet-0.4.5/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/workflows/configure.yml` & `python-parakeet-0.4.5/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/workflows/format.yml` & `python-parakeet-0.4.5/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.github/workflows/pip.yml` & `python-parakeet-0.4.5/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/.pre-commit-config.yaml` & `python-parakeet-0.4.5/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/LICENSE` & `python-parakeet-0.4.5/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/README.rst` & `python-parakeet-0.4.5/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/Doxyfile` & `python-parakeet-0.4.5/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/Makefile` & `python-parakeet-0.4.5/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/chrono.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/custom.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/eigen.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/functional.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/index.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/overview.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/stl.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/cast/strings.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/classes.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/embedding.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/exceptions.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/functions.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/misc.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/numpy.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/object.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/utilities.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/advanced/smart_ptrs.rst` & `python-parakeet-0.4.5/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/basics.rst` & `python-parakeet-0.4.5/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/benchmark.py` & `python-parakeet-0.4.5/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/benchmark.rst` & `python-parakeet-0.4.5/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/changelog.rst` & `python-parakeet-0.4.5/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/classes.rst` & `python-parakeet-0.4.5/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/compiling.rst` & `python-parakeet-0.4.5/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/conf.py` & `python-parakeet-0.4.5/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/faq.rst` & `python-parakeet-0.4.5/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/index.rst` & `python-parakeet-0.4.5/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/installing.rst` & `python-parakeet-0.4.5/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/limitations.rst` & `python-parakeet-0.4.5/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/pybind11-logo.png` & `python-parakeet-0.4.5/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.png` & `python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.svg` & `python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.png` & `python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.svg` & `python-parakeet-0.4.5/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/reference.rst` & `python-parakeet-0.4.5/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/release.rst` & `python-parakeet-0.4.5/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/docs/upgrade.rst` & `python-parakeet-0.4.5/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/attr.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/buffer_info.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/cast.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/chrono.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/complex.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/class.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/common.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/descr.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/init.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/internals.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/type_caster_base.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/detail/typeid.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/eigen.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/embed.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/eval.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/functional.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/gil.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/iostream.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/numpy.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/operators.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/options.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/pybind11.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/pytypes.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/stl.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/include/pybind11/stl_bind.h` & `python-parakeet-0.4.5/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/pybind11/__main__.py` & `python-parakeet-0.4.5/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/pybind11/commands.py` & `python-parakeet-0.4.5/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.py` & `python-parakeet-0.4.5/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.pyi` & `python-parakeet-0.4.5/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/setup.cfg` & `python-parakeet-0.4.5/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/setup.py` & `python-parakeet-0.4.5/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/conftest.py` & `python-parakeet-0.4.5/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/constructor_stats.h` & `python-parakeet-0.4.5/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/cross_module_gil_utils.cpp` & `python-parakeet-0.4.5/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/env.py` & `python-parakeet-0.4.5/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/extra_python_package/test_files.py` & `python-parakeet-0.4.5/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/extra_setuptools/test_setuphelper.py` & `python-parakeet-0.4.5/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/local_bindings.h` & `python-parakeet-0.4.5/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/object.h` & `python-parakeet-0.4.5/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/pybind11_cross_module_tests.cpp` & `python-parakeet-0.4.5/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/pybind11_tests.cpp` & `python-parakeet-0.4.5/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/pybind11_tests.h` & `python-parakeet-0.4.5/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/pytest.ini` & `python-parakeet-0.4.5/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/requirements.txt` & `python-parakeet-0.4.5/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_async.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_async.py` & `python-parakeet-0.4.5/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_buffers.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_buffers.py` & `python-parakeet-0.4.5/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.py` & `python-parakeet-0.4.5/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_call_policies.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_call_policies.py` & `python-parakeet-0.4.5/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_callbacks.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_callbacks.py` & `python-parakeet-0.4.5/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_chrono.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_chrono.py` & `python-parakeet-0.4.5/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_class.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_class.py` & `python-parakeet-0.4.5/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/embed.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.py` & `python-parakeet-0.4.5/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_copy_move.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_copy_move.py` & `python-parakeet-0.4.5/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.py` & `python-parakeet-0.4.5/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_docstring_options.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_docstring_options.py` & `python-parakeet-0.4.5/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_eigen.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_eigen.py` & `python-parakeet-0.4.5/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_embed/CMakeLists.txt` & `python-parakeet-0.4.5/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_embed/catch.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_embed/external_module.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_enum.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_enum.py` & `python-parakeet-0.4.5/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_eval.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_eval.py` & `python-parakeet-0.4.5/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_exceptions.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_exceptions.py` & `python-parakeet-0.4.5/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.py` & `python-parakeet-0.4.5/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.py` & `python-parakeet-0.4.5/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_iostream.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_iostream.py` & `python-parakeet-0.4.5/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.py` & `python-parakeet-0.4.5/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_local_bindings.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_local_bindings.py` & `python-parakeet-0.4.5/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.py` & `python-parakeet-0.4.5/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_modules.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_modules.py` & `python-parakeet-0.4.5/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.py` & `python-parakeet-0.4.5/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_array.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_array.py` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.py` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.py` & `python-parakeet-0.4.5/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_opaque_types.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_opaque_types.py` & `python-parakeet-0.4.5/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.py` & `python-parakeet-0.4.5/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_pickling.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_pickling.py` & `python-parakeet-0.4.5/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_pytypes.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_pytypes.py` & `python-parakeet-0.4.5/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.py` & `python-parakeet-0.4.5/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.py` & `python-parakeet-0.4.5/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_stl.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_stl.py` & `python-parakeet-0.4.5/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_stl_binders.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_stl_binders.py` & `python-parakeet-0.4.5/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.py` & `python-parakeet-0.4.5/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_union.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.cpp` & `python-parakeet-0.4.5/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.py` & `python-parakeet-0.4.5/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/valgrind-numpy-scipy.supp` & `python-parakeet-0.4.5/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tests/valgrind-python.supp` & `python-parakeet-0.4.5/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/FindCatch.cmake` & `python-parakeet-0.4.5/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/FindEigen3.cmake` & `python-parakeet-0.4.5/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/FindPythonLibsNew.cmake` & `python-parakeet-0.4.5/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/check-style.sh` & `python-parakeet-0.4.5/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/cmake_uninstall.cmake.in` & `python-parakeet-0.4.5/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/libsize.py` & `python-parakeet-0.4.5/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/make_changelog.py` & `python-parakeet-0.4.5/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/pybind11Common.cmake` & `python-parakeet-0.4.5/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/pybind11Config.cmake.in` & `python-parakeet-0.4.5/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/pybind11NewTools.cmake` & `python-parakeet-0.4.5/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/pybind11Tools.cmake` & `python-parakeet-0.4.5/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/setup_global.py.in` & `python-parakeet-0.4.5/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/pybind11/tools/setup_main.py.in` & `python-parakeet-0.4.5/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/setup.cfg` & `python-parakeet-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/setup.py` & `python-parakeet-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             "h5py",
             "maptools",
             "mrcfile",
             "numpy==1.23",  # Until scikit-image updates
             "pandas",
             "pillow",
             "profet",
-            "pydantic",
+            "pydantic==1.10.10",
             "python-multem",
             "pyyaml",
             "scipy",
             "starfile",
         ],
         tests_require=tests_require,
         test_suite="tests",
```

### Comparing `python-parakeet-0.4.4/snap/snapcraft.yaml` & `python-parakeet-0.4.5/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/_run.py` & `python-parakeet-0.4.5/src/parakeet/_run.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/analyse/_average_particles.py` & `python-parakeet-0.4.5/src/parakeet/analyse/_average_particles.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/analyse/_correct.py` & `python-parakeet-0.4.5/src/parakeet/analyse/_correct.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/analyse/_extract.py` & `python-parakeet-0.4.5/src/parakeet/analyse/_extract.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/analyse/_reconstruct.py` & `python-parakeet-0.4.5/src/parakeet/analyse/_reconstruct.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/analyse/_refine.py` & `python-parakeet-0.4.5/src/parakeet/analyse/_refine.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/beam.py` & `python-parakeet-0.4.5/src/parakeet/beam.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/__init__.py` & `python-parakeet-0.4.5/src/parakeet/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/_export.py` & `python-parakeet-0.4.5/src/parakeet/command_line/_export.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/_main.py` & `python-parakeet-0.4.5/src/parakeet/command_line/_main.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/_run.py` & `python-parakeet-0.4.5/src/parakeet/command_line/_run.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_all_particles.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_average_all_particles.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_particles.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_average_particles.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_correct.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_correct.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_extract.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_extract.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_reconstruct.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_reconstruct.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_refine.py` & `python-parakeet-0.4.5/src/parakeet/command_line/analyse/_refine.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/config/_edit.py` & `python-parakeet-0.4.5/src/parakeet/command_line/config/_edit.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/config/_new.py` & `python-parakeet-0.4.5/src/parakeet/command_line/config/_new.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/config/_show.py` & `python-parakeet-0.4.5/src/parakeet/command_line/config/_show.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/metadata/_export.py` & `python-parakeet-0.4.5/src/parakeet/command_line/metadata/_export.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/pdb/_get.py` & `python-parakeet-0.4.5/src/parakeet/command_line/pdb/_get.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/pdb/_read.py` & `python-parakeet-0.4.5/src/parakeet/command_line/pdb/_read.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/sample/_add_molecules.py` & `python-parakeet-0.4.5/src/parakeet/command_line/sample/_add_molecules.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/sample/_mill.py` & `python-parakeet-0.4.5/src/parakeet/command_line/sample/_mill.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/sample/_new.py` & `python-parakeet-0.4.5/src/parakeet/command_line/sample/_new.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/sample/_show.py` & `python-parakeet-0.4.5/src/parakeet/command_line/sample/_show.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/sample/_sputter.py` & `python-parakeet-0.4.5/src/parakeet/command_line/sample/_sputter.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_cbed.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_cbed.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_ctf.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_ctf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_exit_wave.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_exit_wave.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_image.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_image.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_optics.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_optics.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_potential.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_potential.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_simple.py` & `python-parakeet-0.4.5/src/parakeet/command_line/simulate/_simple.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/config.py` & `python-parakeet-0.4.5/src/parakeet/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -606,14 +606,22 @@
         None,
         description=(
             "The list of positions to use (A). This field is used when the mode"
             "is set to 'manual' or 'beam tilt'."
         ),
     )
 
+    defocus_offset: Optional[List[float]] = Field(
+        None,
+        description=(
+            "The list of defoci to use (A). This field is used when the mode"
+            "is set to 'manual' or 'single_particle'"
+        ),
+    )
+
     theta: Optional[Union[float, List[float]]] = Field(
         None,
         description=(
             "The list of theta angles to use (mrad) for the beam tilt."
             "This must either be the same length as phi or a scalar"
         ),
     )
@@ -647,14 +655,29 @@
 
     """
 
     peak = "peak"
     optimal = "optimal"
 
 
+class IceParameters(BaseModel):
+    """
+    A model to describe the ice parameters
+
+    """
+
+    m1: float = Field(0, description="The mean of gaussian 1")
+    m2: float = Field(1.0 / 2.88, description="The mean of gaussian 2")
+    s1: float = Field(0.731, description="The standard deviation of gaussian 1")
+    s2: float = Field(0.081, description="The standard deviation of gaussian 2")
+    a1: float = Field(0.199, description="The amplitude of gaussian 1")
+    a2: float = Field(0.801, description="The amplitude of gaussian 2")
+    density: float = Field(0.91, gt=0, description="The density of the ice (g/cm^3)")
+
+
 class Simulation(BaseModel):
     """
     A model to describe the simulation parameters
 
     """
 
     slice_thickness: float = Field(3.0, description="The multislice thickness (A)")
@@ -665,14 +688,18 @@
 
     division_thickness: int = Field(100, description="Deprecated")
 
     ice: bool = Field(
         False, description="Use the Gaussian Random Field ice model (True/False)"
     )
 
+    ice_parameters: IceParameters = Field(
+        IceParameters(), description="The parameters for the GRF ice model"
+    )
+
     radiation_damage_model: bool = Field(
         False, description="Use the radiation damage model (True/False)"
     )
 
     inelastic_model: InelasticModel = Field(
         None, description="The inelastic model parameters"
     )
```

### Comparing `python-parakeet-0.4.4/src/parakeet/data/__init__.py` & `python-parakeet-0.4.5/src/parakeet/data/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/3jb9.cif` & `python-parakeet-0.4.5/src/parakeet/data/files/3jb9.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/4v1w.cif` & `python-parakeet-0.4.5/src/parakeet/data/files/4v1w.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/4v5d.cif` & `python-parakeet-0.4.5/src/parakeet/data/files/4v5d.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/6qt9.cif` & `python-parakeet-0.4.5/src/parakeet/data/files/6qt9.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/6z6u.pdb` & `python-parakeet-0.4.5/src/parakeet/data/files/6z6u.pdb`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/data/files/water.cif` & `python-parakeet-0.4.5/src/parakeet/data/files/water.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/detector.py` & `python-parakeet-0.4.5/src/parakeet/detector.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/dqe.py` & `python-parakeet-0.4.5/src/parakeet/dqe.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/error.h` & `python-parakeet-0.4.5/src/parakeet/error.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/freeze/__init__.py` & `python-parakeet-0.4.5/src/parakeet/freeze/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/freeze/freeze_ext.cc` & `python-parakeet-0.4.5/src/parakeet/freeze/freeze_ext.cc`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/freeze/sphere_packer.h` & `python-parakeet-0.4.5/src/parakeet/freeze/sphere_packer.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/futures.py` & `python-parakeet-0.4.5/src/parakeet/futures.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/inelastic.py` & `python-parakeet-0.4.5/src/parakeet/inelastic.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/io.py` & `python-parakeet-0.4.5/src/parakeet/io.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/landau.py` & `python-parakeet-0.4.5/src/parakeet/landau.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/lens.py` & `python-parakeet-0.4.5/src/parakeet/lens.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/metadata.py` & `python-parakeet-0.4.5/src/parakeet/metadata.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/microscope.py` & `python-parakeet-0.4.5/src/parakeet/microscope.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/__init__.py` & `python-parakeet-0.4.5/src/parakeet/sample/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
     column_data = {
         "atomic_number": "uint8",
         "x": "float32",
         "y": "float32",
         "z": "float32",
         "sigma": "float32",
         "occupancy": "float32",
-        "charge": "uint8",
+        "charge": "int8",
     }
 
     def __init__(self, data=None, **kwargs):
         """
         Initialise the class
 
         Either the data attribute or the individual arrays must be set.
@@ -517,15 +517,15 @@
                 self.data["atomic_number"].astype("uint8"),
                 self.data["x"].astype("float32"),
                 self.data["y"].astype("float32"),
                 self.data["z"].astype("float32"),
                 self.data["sigma"].astype("float32"),
                 self.data["occupancy"].astype("float32"),
                 [int(0) for i in range(self.data.shape[0])],
-                self.data["charge"].astype("uint8"),
+                self.data["charge"].astype("int8"),
             )
         )
 
     def rows(self):
         """
         Iterate through atoms rows
```

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/_add_molecules.py` & `python-parakeet-0.4.5/src/parakeet/sample/_add_molecules.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/_mill.py` & `python-parakeet-0.4.5/src/parakeet/sample/_mill.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/_new.py` & `python-parakeet-0.4.5/src/parakeet/sample/_new.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/_sputter.py` & `python-parakeet-0.4.5/src/parakeet/sample/_sputter.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/sample/distribute.py` & `python-parakeet-0.4.5/src/parakeet/sample/distribute.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/scan.py` & `python-parakeet-0.4.5/src/parakeet/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         axis: np.ndarray = None,
         angle: np.ndarray = None,
         shift: np.ndarray = None,
         shift_delta: np.ndarray = None,
         beam_tilt_theta: np.ndarray = None,
         beam_tilt_phi: np.ndarray = None,
         electrons_per_angstrom: np.ndarray = None,
+        defocus_offset: np.ndarray = None,
         exposure_time: float = 1,
         is_uniform_angular_scan: bool = False,
     ):
         """
         Initialise the scan
 
         """
@@ -65,14 +66,17 @@
 
         if beam_tilt_phi is None:
             beam_tilt_phi = np.zeros(len(image_number))
 
         if electrons_per_angstrom is None:
             electrons_per_angstrom = np.ones(len(image_number))
 
+        if defocus_offset is None:
+            defocus_offset = np.zeros(len(image_number))
+
         self.data = pd.DataFrame(
             data={
                 "image_number": image_number,
                 "fraction_number": fraction_number,
                 "axis_x": axis[:, 0],
                 "axis_y": axis[:, 1],
                 "axis_z": axis[:, 2],
@@ -82,14 +86,15 @@
                 "shift_z": shift[:, 2],
                 "shift_delta_x": shift_delta[:, 0],
                 "shift_delta_y": shift_delta[:, 1],
                 "shift_delta_z": shift_delta[:, 2],
                 "beam_tilt_theta": beam_tilt_theta,
                 "beam_tilt_phi": beam_tilt_phi,
                 "electrons_per_angstrom": electrons_per_angstrom,
+                "defocus_offset": defocus_offset,
                 "exposure_time": np.ones(len(axis)) * exposure_time,
             }
         )
 
     @property
     def image_number(self) -> np.ndarray:
         """
@@ -183,14 +188,22 @@
         """
         Get the axes
 
         """
         return np.array(self.data[["axis_x", "axis_y", "axis_z"]])
 
     @property
+    def defocus_offset(self) -> np.ndarray:
+        """
+        Get the defocus offset
+
+        """
+        return self.data["defocus_offset"]
+
+    @property
     def euler_angles(self) -> np.ndarray:
         """
         Euler angle representation of the orientations.
 
         The Euler angles are intrinsic, right handed rotations around ZYZ.
         This matches the convention used by XMIPP/RELION.
 
@@ -287,14 +300,15 @@
 
     @classmethod
     def single_axis(
         Class,
         axis: Union[np.ndarray, tuple] = (0, 1, 0),
         angles: np.ndarray = None,
         positions: np.ndarray = None,
+        defocus_offset: np.ndarray = None,
         num_fractions: int = 1,
         electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
@@ -303,17 +317,21 @@
         """
 
         # Check input
         if angles is None:
             angles = np.array([])
         if positions is None:
             positions = np.array([])
+        if defocus_offset is None:
+            defocus_offset = np.zeros(len(angles))
         assert angles is not None
         assert positions is not None
+        assert defocus_offset is not None
         assert len(angles) == len(positions)
+        assert len(angles) == len(defocus_offset)
         num_images = len(angles)
 
         # Create the orientation and shift
         axis, angle = Class._rotvec_from_axis_and_angles(np.array(axis), angles)
         shift = Class._shift_from_axis_and_positions(np.array(axis), positions)
 
         # Set the image number and frame number
@@ -323,14 +341,15 @@
 
         # Duplicate for the number of movie frames per step
         image_number = np.repeat(image_number, num_fractions, axis=0)
         axis = np.repeat(axis, num_fractions, axis=0)
         angle = np.repeat(angle, num_fractions, axis=0)
         shift = np.repeat(shift, num_fractions, axis=0)
         dose = np.full(angle.shape, electrons_per_angstrom / num_fractions)
+        defocus_offset = np.repeat(defocus_offset, num_fractions, axis=0)
 
         # Create the shift delta
         shift_delta = None
         if drift is not None:
             shift_delta = Class._generate_drift(angles, **drift)
             shift_delta = np.repeat(shift_delta, num_fractions, axis=0)
 
@@ -340,22 +359,24 @@
             fraction_number=fraction_number,
             axis=np.array(axis),
             angle=angle,
             shift=shift,
             shift_delta=shift_delta,
             electrons_per_angstrom=dose,
             exposure_time=exposure_time,
+            defocus_offset=defocus_offset,
         )
 
     @classmethod
     def manual(
         Class,
         axis: tuple = (0, 1, 0),
         angles: np.ndarray = None,
         positions: np.ndarray = None,
+        defocus_offset: np.ndarray = None,
         num_fractions: int = 1,
         electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
@@ -366,25 +387,29 @@
         if angles is None and positions is None:
             angles = np.array([0])
             positions = np.array([0])
         elif angles is None and positions is not None:
             angles = np.zeros(len(positions))
         elif positions is None and angles is not None:
             positions = np.zeros(len(angles))
+        if defocus_offset is None:
+            defocus_offset = np.zeros(angles.shape[0])  # type: ignore
         assert angles is not None
         assert positions is not None
         assert len(angles) == len(positions)
+        assert len(angles) == len(defocus_offset)
         angles = np.array(angles)
         positions = np.array(positions)
 
         # Create the single axis scan
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            defocus_offset=defocus_offset,
             num_fractions=num_fractions,
             electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
@@ -561,21 +586,25 @@
     def single_particle(
         Class,
         num_images: int = 1,
         num_fractions: int = 1,
         exposure_time: float = 1,
         electrons_per_angstrom: float = 1,
         drift: dict = None,
+        defocus_offset: np.ndarray = None,
         **kwargs
     ) -> Scan:
         """
         Create a single particle scan. This is a special scan that is actually
         just the particle in different orientations
 
         """
+        if defocus_offset is None:
+            defocus_offset = np.zeros(num_images)
+        assert num_images == len(defocus_offset)
 
         # Get a random list of uniform orientations
         orientation = R.from_matrix(
             special_ortho_group.rvs(dim=3, size=num_images)
         ).as_rotvec()
 
         # Get the axis and angle
@@ -587,30 +616,32 @@
         fraction_number = np.repeat([fraction_number], len(angle), axis=0).flatten()
 
         # Duplicate for the number of movie frames per step
         image_number = np.repeat(image_number, num_fractions, axis=0)
         axis = np.repeat(axis, num_fractions, axis=0)
         angle = np.repeat(angle, num_fractions, axis=0)
         dose = np.full(angle.shape, electrons_per_angstrom / num_fractions)
+        defocus_offset = np.repeat(defocus_offset, num_fractions, axis=0)
 
         # Create the shift delta
         shift_delta = None
         if drift is not None:
             shift_delta = Class._generate_drift(np.zeros(num_images), **drift)
             shift_delta = np.repeat(shift_delta, num_fractions, axis=0)
 
         # Create the scan
         return Scan(
             image_number=image_number,
             fraction_number=fraction_number,
             axis=axis,
             angle=angle,
+            shift_delta=shift_delta,
             electrons_per_angstrom=dose,
             exposure_time=exposure_time,
-            shift_delta=shift_delta,
+            defocus_offset=defocus_offset,
             is_uniform_angular_scan=True,
         )
 
     @classmethod
     def beam_tilt(
         Class,
         axis: Union[np.ndarray, tuple] = (0, 1, 0),
@@ -780,14 +811,15 @@
     step_angle: float = 0,
     start_pos: float = 0,
     step_pos: float = 0,
     num_images: int = 1,
     num_fractions: int = 1,
     num_nhelix: int = 1,
     exposure_time: float = 1,
+    defocus_offset: np.ndarray = None,
     theta: np.ndarray = None,
     phi: np.ndarray = None,
     drift: dict = None,
     electrons_per_angstrom: float = 40,
 ) -> Scan:
     """
     Create an scan
@@ -804,14 +836,15 @@
         step_angle: The angle step (deg)
         start_pos: The starting position (A)
         step_pos: The step in position (A)
         num_images: The number of images
         num_fractions: The number of movie frames per image
         num_nhelix: The number of scans in an n-helix
         exposure_time: The exposure time (seconds)
+        defocus_offset: The defocus_offset (A)
         theta: The beam tilt theta angle
         phi: The beam tilt phi angle
         drift: The beam drift model
         electrons_per_angstrom: The number of electrons per angstrom (per image)
 
     Returns:
         The scan object
@@ -825,13 +858,14 @@
         "step_angle": step_angle,
         "start_pos": start_pos,
         "step_pos": step_pos,
         "num_images": num_images,
         "num_fractions": num_fractions,
         "num_nhelix": num_nhelix,
         "exposure_time": exposure_time,
+        "defocus_offset": defocus_offset,
         "theta": theta,
         "phi": phi,
         "drift": drift,
         "electrons_per_angstrom": electrons_per_angstrom,
     }
     return ScanFactory.make_scan(mode, **kwargs)
```

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_cbed.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_cbed.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_ctf.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_ctf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_exit_wave.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_exit_wave.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,23 @@
 import parakeet.futures
 import parakeet.inelastic
 import parakeet.io
 import parakeet.sample
 import parakeet.simulate
 from parakeet.simulate.simulation import Simulation
 from parakeet.microscope import Microscope
-from parakeet.scan import Scan
 from functools import singledispatch
 from math import pi
 from collections.abc import Iterable
 from scipy.spatial.transform import Rotation as R
 
 
 __all__ = ["exit_wave"]
 
 
-Device = parakeet.config.Device
-ClusterMethod = parakeet.config.ClusterMethod
-Sample = parakeet.sample.Sample
-
 # Get the logger
 logger = logging.getLogger(__name__)
 
 # Try to input MULTEM
 try:
     import multem
 except ImportError:
@@ -81,14 +76,25 @@
         Get the masker object for the ice specification
 
         """
 
         # Create the masker
         masker = multem.Masker(input_multislice.nx, input_multislice.ny, pixel_size)
 
+        # Set the ice parameters
+        ice_parameters = multem.IceParameters()
+        ice_parameters.m1 = self.simulation["ice_parameters"]["m1"]
+        ice_parameters.m2 = self.simulation["ice_parameters"]["m2"]
+        ice_parameters.s1 = self.simulation["ice_parameters"]["s1"]
+        ice_parameters.s2 = self.simulation["ice_parameters"]["s2"]
+        ice_parameters.a1 = self.simulation["ice_parameters"]["a1"]
+        ice_parameters.a2 = self.simulation["ice_parameters"]["a2"]
+        ice_parameters.density = self.simulation["ice_parameters"]["density"]
+        masker.set_ice_parameters(ice_parameters)
+
         # Get the sample centre
         shape = self.sample.shape
         centre = np.array(self.sample.centre)
         drift = np.array(drift)
         detector_origin = np.array([origin[0], origin[1], 0])
         centre = centre + offset - detector_origin - shift
 
@@ -343,17 +349,17 @@
 
         # Compute the image scaled with Poisson noise
         return (index, image, metadata)
 
 
 def simulation_factory(
     microscope: Microscope,
-    sample: Sample,
-    scan: Scan,
-    device: Device = Device.gpu,
+    sample: parakeet.sample.Sample,
+    scan: parakeet.scan.Scan,
+    device: parakeet.config.Device = parakeet.config.Device.gpu,
     simulation: dict = None,
     cluster: dict = None,
 ) -> Simulation:
     """
     Create the simulation
 
     Args:
@@ -391,16 +397,16 @@
 
 
 @singledispatch
 def exit_wave(
     config_file,
     sample_file: str,
     exit_wave_file: str,
-    device: Device = Device.gpu,
-    cluster_method: ClusterMethod = None,
+    device: parakeet.config.Device = parakeet.config.Device.gpu,
+    cluster_method: parakeet.config.ClusterMethod = None,
     cluster_max_workers: int = 1,
 ):
     """
     Simulate the exit wave from the sample
 
     Args:
         config_file: The config filename
```

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_image.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_image.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_optics.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_optics.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
             psi = np.fft.ifft2(np.fft.fft2(psi) * ctf)
             image = np.abs(psi) ** 2
 
             return image
 
         # Get the rotation angle
         angle = self.scan.angles[index]
+        defocus_offset = self.scan.defocus_offset[index]
 
         # Check the angle and position
         assert abs(angle - self.exit_wave.header[index]["tilt_alpha"]) < 1e7
 
         # The field of view
         nx = self.microscope.detector.nx
         ny = self.microscope.detector.ny
@@ -155,15 +156,15 @@
 
         # Set the input wave
         psi = self.exit_wave.data[index]
 
         microscope = copy.deepcopy(self.microscope)
 
         # Get the defocus
-        defocus = microscope.lens.c_10
+        defocus = microscope.lens.c_10 + defocus_offset
 
         # If we do CC correction then set spherical aberration and chromatic
         # aberration to zero
         shape = self.sample["shape"]
         energy_shift = 0
         if self.simulation["inelastic_model"] is None:
             # If no inelastic model just calculate image as normal
@@ -555,14 +556,18 @@
     # Create the exit wave data
     logger.info(f"Loading sample from {exit_wave_file}")
     exit_wave = parakeet.io.open(exit_wave_file)
 
     # Create the scan
     scan = exit_wave.header.scan
 
+    # Override the defocus_offset
+    scan_new = parakeet.scan.new(**config.scan.dict())
+    scan.data["defocus_offset"] = scan_new.defocus_offset
+
     # Create the simulation
     simulation = simulation_factory(
         microscope,
         exit_wave,
         scan,
         device=config.device,
         simulation=config.simulation.dict(),
```

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_potential.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_potential.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/_simple.py` & `python-parakeet-0.4.5/src/parakeet/simulate/_simple.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/phase_plate.py` & `python-parakeet-0.4.5/src/parakeet/simulate/phase_plate.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/simulate/simulation.py` & `python-parakeet-0.4.5/src/parakeet/simulate/simulation.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/parakeet/util/calibrate_ice_model.py` & `python-parakeet-0.4.5/src/parakeet/util/calibrate_ice_model.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/python_parakeet.egg-info/PKG-INFO` & `python-parakeet-0.4.5/src/python_parakeet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-parakeet
-Version: 0.4.4
+Version: 0.4.5
 Summary: A phantom generator
 Home-page: https://github.com/rosalindfranklininstitute/parakeet
 Author: James Parkhurst
 Author-email: james.parkhurst@diamond.ac.uk
 License: GPL v3
 Project-URL: Source, https://github.com/rosalindfranklininstitute/parakeet
 Project-URL: Tracker, https://github.com/rosalindfranklininstitute/parakeet/issues
```

### Comparing `python-parakeet-0.4.4/src/python_parakeet.egg-info/SOURCES.txt` & `python-parakeet-0.4.5/src/python_parakeet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/src/python_parakeet.egg-info/entry_points.txt` & `python-parakeet-0.4.5/src/python_parakeet.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_command_line.py` & `python-parakeet-0.4.5/tests/test_command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         },
         "scan": {
             "mode": "tilt_series",
             "num_images": 10,
             "start_angle": -90,
             "step_angle": 18,
         },
+        "simulation": {
+            "ice": True,
+        },
     }
 
     config = parakeet.config.load(config_dict)
     config_path = os.path.abspath(os.path.join(directory, "config.yaml"))
     yaml.safe_dump(config.dict(), open(config_path, "w"))
     return directory
```

### Comparing `python-parakeet-0.4.4/tests/test_config.py` & `python-parakeet-0.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_inelastic.py` & `python-parakeet-0.4.5/tests/test_inelastic.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_io.py` & `python-parakeet-0.4.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_landau.py` & `python-parakeet-0.4.5/tests/test_landau.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_sample.py` & `python-parakeet-0.4.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_sample_distribute.py` & `python-parakeet-0.4.5/tests/test_sample_distribute.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_scan.py` & `python-parakeet-0.4.5/tests/test_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     assert np.all(np.equal(scan.axes, np.array([[0, 1, 0]])))
     assert np.all(np.equal(scan.angles, np.array([0])))
     assert np.all(np.equal(scan.position, np.array([(0, 0, 0)])))
 
 
 def test_manual():
     scan = parakeet.scan.new(
-        mode="manual", axis=(0, 1, 0), angles=[1, 2, 3], positions=[4, 5, 6]
+        mode="manual",
+        axis=(0, 1, 0),
+        angles=[1, 2, 3],
+        positions=[4, 5, 6],
+        defocus_offset=[0, 500, 1000],
     )
     assert np.all(np.equal(scan.axes, np.array([[0, 1, 0]])))
     assert np.allclose(scan.angles, np.array([1, 2, 3]))
     assert np.allclose(scan.position, np.array([(0, i, 0) for i in [4, 5, 6]]))
 
 
 def test_still():
@@ -91,14 +95,15 @@
     assert np.allclose(scan.position, positions)
 
 
 def test_single_particle():
     scan = parakeet.scan.new(
         mode="single_particle",
         num_images=8,
+        defocus_offset=[0, 500, 1000, 1500, 2000, 2500, 3000, 3500],
     )
     assert len(scan) == 8
 
 
 def test_grid_scan():
     scan = parakeet.scan.new(
         mode="grid_scan",
```

### Comparing `python-parakeet-0.4.4/tests/test_slice.py` & `python-parakeet-0.4.5/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.4/tests/test_sphere_packer.py` & `python-parakeet-0.4.5/tests/test_sphere_packer.py`

 * *Files identical despite different names*

