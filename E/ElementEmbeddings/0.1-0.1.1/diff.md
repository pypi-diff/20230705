# Comparing `tmp/ElementEmbeddings-0.1.tar.gz` & `tmp/ElementEmbeddings-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElementEmbeddings-0.1.tar", last modified: Tue Jul  4 08:46:21 2023, max compression
+gzip compressed data, was "ElementEmbeddings-0.1.1.tar", last modified: Wed Jul  5 16:30:32 2023, max compression
```

## Comparing `ElementEmbeddings-0.1.tar` & `ElementEmbeddings-0.1.1.tar`

### file list

```diff
@@ -1,73 +1,46 @@
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.448228 ElementEmbeddings-0.1/
--rw-r--r--   0 antobi    (1000) antobi    (1000)      182 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.flake8
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.408228 ElementEmbeddings-0.1/.github/
--rw-r--r--   0 antobi    (1000) antobi    (1000)      597 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.github/dependabot.yml
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1667 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.github/pull_request_template.md
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.408228 ElementEmbeddings-0.1/.github/workflows/
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1059 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/.github/workflows/ci.yml
--rw-r--r--   0 antobi    (1000) antobi    (1000)     6310 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.github/workflows/combine-prs.yml
--rw-r--r--   0 antobi    (1000) antobi    (1000)     4231 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.gitignore
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1360 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/.pre-commit-config.yaml
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1079 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/LICENSE.md
--rw-r--r--   0 antobi    (1000) antobi    (1000)     4184 2023-07-04 08:46:21.448228 ElementEmbeddings-0.1/PKG-INFO
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/Publication/
--rw-r--r--   0 antobi    (1000) antobi    (1000)    16630 2023-06-30 14:47:55.000000 ElementEmbeddings-0.1/Publication/element_similarity.ipynb
--rw-r--r--   0 antobi    (1000) antobi    (1000)     3731 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/README.md
--rw-r--r--   0 antobi    (1000) antobi    (1000)     2224 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/contributing.md
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.398228 ElementEmbeddings-0.1/dev_docs/
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/dev_docs/design_docs/
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1781 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/dev_docs/design_docs/Restructuring.md
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/dev_docs/dev_notebooks/
--rw-r--r--   0 antobi    (1000) antobi    (1000)    23912 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/dev_docs/dev_notebooks/composition_statistics.ipynb
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/examples/
--rw-r--r--   0 antobi    (1000) antobi    (1000)      318 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/examples/README.md
--rw-r--r--   0 antobi    (1000) antobi    (1000)     6085 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/examples/composition.ipynb
--rw-r--r--   0 antobi    (1000) antobi    (1000)    13045 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/examples/usage.ipynb
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1023 2023-06-19 11:46:20.000000 ElementEmbeddings-0.1/mkdocs.yml
--rw-r--r--   0 antobi    (1000) antobi    (1000)      238 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/requirements-dev.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)      199 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/requirements.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)       38 2023-07-04 08:46:21.448228 ElementEmbeddings-0.1/setup.cfg
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1315 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/setup.py
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.408228 ElementEmbeddings-0.1/src/
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/
--rw-r--r--   0 antobi    (1000) antobi    (1000)     4184 2023-07-04 08:46:21.000000 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/PKG-INFO
--rw-r--r--   0 antobi    (1000) antobi    (1000)     2067 2023-07-04 08:46:21.000000 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/SOURCES.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)        1 2023-07-04 08:46:21.000000 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/dependency_links.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)       75 2023-07-04 08:46:21.000000 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/requires.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)       18 2023-07-04 08:46:21.000000 ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/top_level.txt
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.418228 ElementEmbeddings-0.1/src/elementembeddings/
--rw-r--r--   0 antobi    (1000) antobi    (1000)      267 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/__init__.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)    11723 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/composition.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)    33383 2023-06-30 14:47:55.000000 ElementEmbeddings-0.1/src/elementembeddings/core.py
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.438228 ElementEmbeddings-0.1/src/elementembeddings/data/
--rw-r--r--   0 antobi    (1000) antobi    (1000)     4239 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/README.md
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.438228 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/
--rw-r--r--   0 antobi    (1000) antobi    (1000)      453 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/README.md
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1870 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/element_group.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)     2109 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/element_symbols.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)      343 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/ordered_periodic.txt
--rw-r--r--   0 antobi    (1000) antobi    (1000)   199959 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)   259692 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/element_data/periodic-table-lookup.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)    10915 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/magpie.csv
--rw-r--r--   0 antobi    (1000) antobi    (1000)    44406 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/magpie_sc.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)   476891 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/mat2vec.csv
--rw-r--r--   0 antobi    (1000) antobi    (1000)   449163 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/matscholar-embedding.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)    32012 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/megnet16.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1191 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/mod_petti.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)    19636 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/oliynyk.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)    77531 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/oliynyk_sc.json
--rw-r--r--   0 antobi    (1000) antobi    (1000)   487394 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/random_200.csv
--rw-r--r--   0 antobi    (1000) antobi    (1000)   488226 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/random_200_new.csv
--rw-r--r--   0 antobi    (1000) antobi    (1000)   356292 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/data/skipatom_20201009_induced.csv
--rw-r--r--   0 antobi    (1000) antobi    (1000)     5846 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/plotter.py
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.448228 ElementEmbeddings-0.1/src/elementembeddings/tests/
--rw-r--r--   0 antobi    (1000) antobi    (1000)       51 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/__init__.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)     2712 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/test_composition.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)     7914 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/test_core.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)    10551 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/test_core.py.bak
--rw-r--r--   0 antobi    (1000) antobi    (1000)     1133 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/test_plotter.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)      897 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/tests/test_utils.py
-drwxr-xr-x   0 antobi    (1000) antobi    (1000)        0 2023-07-04 08:46:21.448228 ElementEmbeddings-0.1/src/elementembeddings/utils/
--rw-r--r--   0 antobi    (1000) antobi    (1000)       47 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/utils/__init__.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)      344 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/utils/io.py
--rw-r--r--   0 antobi    (1000) antobi    (1000)      673 2023-06-20 13:52:33.000000 ElementEmbeddings-0.1/src/elementembeddings/utils/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.387287 ElementEmbeddings-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.391287 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.391287 ElementEmbeddings-0.1.1/src/elementembeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33383 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/ordered_periodic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   199959 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)   259692 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   476891 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/mat2vec.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/matscholar-embedding.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/megnet16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/mod_petti.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk.json
+-rw-r--r--   0 runner    (1001) docker     (123)    77531 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   487394 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488226 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200_new.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   356292 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/skipatom_20201009_induced.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/math.py
```

### Comparing `ElementEmbeddings-0.1/LICENSE.md` & `ElementEmbeddings-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/PKG-INFO` & `ElementEmbeddings-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: ElementEmbeddings
-Version: 0.1
+Version: 0.1.1
 Summary: Element Embeddings
 Author: Anthony O. Onwuli
 Author-email: anthony.onwuli16@imperial.ac.uk
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ElementEmbeddings
 ====
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/ElementEmbeddings)](https://github.com/WMD-group/ElementEmbeddings/issues)
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
+[![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
+[![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
+![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
+
 
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
@@ -42,28 +52,31 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
-
+The latest stable release can be installed via pip using:
+```bash
+pip install ElementEmbeddings
+```
 The latest version can be installed using:
 
 ```bash
 pip install git+git://github.com/WMD-group/ElementEmbeddings.git
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
 cd ElementEmbeddings
-pip install --user -e .
+pip install  -e .
 ```
 
 With -e pip will create links to the source folder so that changes to the code will be immediately reflected on the PATH.
 
 Usage
 --------
```

### Comparing `ElementEmbeddings-0.1/README.md` & `ElementEmbeddings-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/ElementEmbeddings)](https://github.com/WMD-group/ElementEmbeddings/issues)
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
+[![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
+[![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
+![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
+
 
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
@@ -28,28 +33,31 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
-
+The latest stable release can be installed via pip using:
+```bash
+pip install ElementEmbeddings
+```
 The latest version can be installed using:
 
 ```bash
 pip install git+git://github.com/WMD-group/ElementEmbeddings.git
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
 cd ElementEmbeddings
-pip install --user -e .
+pip install  -e .
 ```
 
 With -e pip will create links to the source folder so that changes to the code will be immediately reflected on the PATH.
 
 Usage
 --------
```

### Comparing `ElementEmbeddings-0.1/setup.py` & `ElementEmbeddings-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup script for AtomicEmbeddings."""
 import os
 
 from setuptools import find_namespace_packages, setup
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
-VERSION = "0.1"
+VERSION = "0.1.1"
 DESCRIPTION = "Element Embeddings"
 with open(os.path.join(module_dir, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 # Setting up
 setup(
@@ -24,24 +24,29 @@
     package_dir={"": "src"},
     package_data={
         "elementembeddings.data": ["*.json", "*.csv"],
         "elementembeddings.data.element_data": ["*.json", "*.txt"],
     },
     test_suite="elementembeddings.tests.test",
     install_requires=[
-        "numpy",
-        "scipy",
-        "pymatgen",
-        "seaborn",
-        "matplotlib",
-        "scikit-learn",
-        "umap-learn",
-        "adjustText",
+        "numpy==1.23.3",
+        "scipy==1.10.1",
+        "pymatgen>2022.9.21",
+        "seaborn==0.12.1",
+        "matplotlib==3.7.1",
+        "scikit-learn==1.3.0",
+        "umap-learn==0.5.3",
+        "adjustText==0.8",
     ],
     classifiers=[
         "Programming Language :: Python",
-        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Chemistry",
+        "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `ElementEmbeddings-0.1/src/ElementEmbeddings.egg-info/PKG-INFO` & `ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: ElementEmbeddings
-Version: 0.1
+Version: 0.1.1
 Summary: Element Embeddings
 Author: Anthony O. Onwuli
 Author-email: anthony.onwuli16@imperial.ac.uk
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ElementEmbeddings
 ====
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/ElementEmbeddings)](https://github.com/WMD-group/ElementEmbeddings/issues)
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
+[![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
+[![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
+![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
+
 
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
@@ -42,28 +52,31 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
-
+The latest stable release can be installed via pip using:
+```bash
+pip install ElementEmbeddings
+```
 The latest version can be installed using:
 
 ```bash
 pip install git+git://github.com/WMD-group/ElementEmbeddings.git
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
 cd ElementEmbeddings
-pip install --user -e .
+pip install  -e .
 ```
 
 With -e pip will create links to the source folder so that changes to the code will be immediately reflected on the PATH.
 
 Usage
 --------
```

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/composition.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/composition.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/core.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/core.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/element_data/element_group.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_group.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/element_data/element_symbols.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/element_data/periodic-table-lookup.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/magpie.csv` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/magpie_sc.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/mat2vec.csv` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/mat2vec.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/matscholar-embedding.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/matscholar-embedding.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/megnet16.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/megnet16.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/mod_petti.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/mod_petti.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/oliynyk.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/oliynyk_sc.json` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/random_200.csv` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/random_200_new.csv` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200_new.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/data/skipatom_20201009_induced.csv` & `ElementEmbeddings-0.1.1/src/elementembeddings/data/skipatom_20201009_induced.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/plotter.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/plotter.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/tests/test_composition.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/tests/test_core.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/tests/test_plotter.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/tests/test_utils.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1/src/elementembeddings/utils/math.py` & `ElementEmbeddings-0.1.1/src/elementembeddings/utils/math.py`

 * *Files identical despite different names*

