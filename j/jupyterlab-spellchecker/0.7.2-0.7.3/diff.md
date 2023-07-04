# Comparing `tmp/jupyterlab-spellchecker-0.7.2.tar.gz` & `tmp/jupyterlab-spellchecker-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-spellchecker-0.7.2.tar", last modified: Fri Oct  8 10:08:03 2021, max compression
+gzip compressed data, was "jupyterlab-spellchecker-0.7.3.tar", last modified: Wed Feb  8 19:01:58 2023, max compression
```

## Comparing `jupyterlab-spellchecker-0.7.2.tar` & `jupyterlab-spellchecker-0.7.3.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7367 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6175 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)      768 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_de_ALL_frami.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15732 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_en_AU.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15732 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_en_CA.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15740 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_en_GB-ise.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15732 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_en_US.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_es_ES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_fr.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/README_pt_PT.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19218 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_AT_frami.aff
--rw-r--r--   0 runner    (1001) docker     (121)  4422326 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_AT_frami.dic
--rw-r--r--   0 runner    (1001) docker     (121)    19218 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_CH_frami.aff
--rw-r--r--   0 runner    (1001) docker     (121)  4416507 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_CH_frami.dic
--rw-r--r--   0 runner    (1001) docker     (121)    19218 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_DE_frami.aff
--rw-r--r--   0 runner    (1001) docker     (121)  4419933 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/de_DE_frami.dic
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_AU.aff
--rw-r--r--   0 runner    (1001) docker     (121)   553854 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_AU.dic
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_CA.aff
--rw-r--r--   0 runner    (1001) docker     (121)   551079 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_CA.dic
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_GB-ise.aff
--rw-r--r--   0 runner    (1001) docker     (121)   551624 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_GB-ise.dic
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_US.aff
--rw-r--r--   0 runner    (1001) docker     (121)   551260 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/en_US.dic
--rw-r--r--   0 runner    (1001) docker     (121)   167076 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/es_ES.aff
--rw-r--r--   0 runner    (1001) docker     (121)   861168 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/es_ES.dic
--rw-r--r--   0 runner    (1001) docker     (121)   256857 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/fr.aff
--rw-r--r--   0 runner    (1001) docker     (121)  1100397 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/fr.dic
--rw-r--r--   0 runner    (1001) docker     (121)    42765 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/pt_PT.aff
--rw-r--r--   0 runner    (1001) docker     (121)   456494 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/dictionaries/pt_PT.dic
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/install.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.967477 jupyterlab-spellchecker-0.7.2/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyter-config/jupyter_notebook_config.d/jupyterlab_spellchecker.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyter-config/jupyter_server_config.d/jupyterlab_spellchecker.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4734 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.967477 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.967477 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-10-08 10:08:00.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2021-10-08 10:08:00.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)    15108 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/301.f78600de2fee651cf61c.js
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/534.d33b047d412a2047177e.js
--rw-r--r--   0 runner    (1001) docker     (121)     7943 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/581.83daa50633cb94659e90.js
--rw-r--r--   0 runner    (1001) docker     (121)     7377 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/remoteEntry.12cf3b546f44ca3d0354.js
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-10-08 10:08:00.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/style.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.991478 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7367 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 10:07:12.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-10-08 10:08:02.000000 jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/src/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (121)    21181 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/src/loader.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/src/svg.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/style/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/style/base.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 10:08:02.995478 jupyterlab-spellchecker-0.7.2/style/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/style/icons/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/style/icons/ic-baseline-spellcheck.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/style/index.css
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/style/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)   182313 2021-10-08 10:06:28.000000 jupyterlab-spellchecker-0.7.2/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.903931 jupyterlab-spellchecker-0.7.3/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_de_ALL_frami.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_en_AU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_en_CA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_en_GB-ise.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_en_US.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_es_ES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_fr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/README_pt_PT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_AT_frami.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  4422326 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_AT_frami.dic
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_CH_frami.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  4416507 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_CH_frami.dic
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_DE_frami.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  4419933 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/de_DE_frami.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_AU.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   553854 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_AU.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_CA.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   551079 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_CA.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_GB-ise.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   551624 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_GB-ise.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_US.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   551260 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/en_US.dic
+-rw-r--r--   0 runner    (1001) docker     (123)   167076 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/es_ES.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   861168 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/es_ES.dic
+-rw-r--r--   0 runner    (1001) docker     (123)   256857 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/fr.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  1100397 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/fr.dic
+-rw-r--r--   0 runner    (1001) docker     (123)    42765 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/pt_PT.aff
+-rw-r--r--   0 runner    (1001) docker     (123)   456494 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/dictionaries/pt_PT.dic
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.875931 jupyterlab-spellchecker-0.7.3/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyter-config/jupyter_notebook_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyter-config/jupyter_notebook_config.d/jupyterlab_spellchecker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyter-config/jupyter_server_config.d/jupyterlab_spellchecker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.875931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.875931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-08 19:01:56.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-08 19:01:56.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/358.8de52c2073f382b46f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/581.93362237019cb70e1d50.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/747.40ff56e19a50aa8f15aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/remoteEntry.3ff26e696aa2c37cdbc7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-08 19:01:56.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.907931 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 19:01:17.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-08 19:01:58.000000 jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/src/loader.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/src/svg.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/style/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 19:01:58.911931 jupyterlab-spellchecker-0.7.3/style/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/style/icons/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/style/icons/ic-baseline-spellcheck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   179441 2023-02-08 19:00:31.000000 jupyterlab-spellchecker-0.7.3/yarn.lock
```

### Comparing `jupyterlab-spellchecker-0.7.2/LICENSE` & `jupyterlab-spellchecker-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/PKG-INFO` & `jupyterlab-spellchecker-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-spellchecker
-Version: 0.7.2
+Version: 0.7.3
 Summary: A spell checker for JupyterLab.
 Home-page: https://github.com/jupyterlab-contrib/spellchecker
 Author: JupyterLab Spellchecker Development Team
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/spellchecker/issues
 Project-URL: Source Code, https://github.com/jupyterlab-contrib/spellchecker
 Keywords: Jupyter,JupyterLab,JupyterLab3
@@ -196,9 +196,7 @@
 ```
 
 Run tests:
 
 ```bash
 python -m pytest
 ```
-
-
```

### Comparing `jupyterlab-spellchecker-0.7.2/README.md` & `jupyterlab-spellchecker-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_de_ALL_frami.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_de_ALL_frami.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_en_AU.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_en_AU.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_en_CA.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_en_CA.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_en_GB-ise.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_en_GB-ise.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_en_US.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_en_US.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_es_ES.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_es_ES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_fr.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_fr.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/README_pt_PT.txt` & `jupyterlab-spellchecker-0.7.3/dictionaries/README_pt_PT.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_AT_frami.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_AT_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_AT_frami.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_AT_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_CH_frami.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_CH_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_CH_frami.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_CH_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_DE_frami.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_DE_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/de_DE_frami.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/de_DE_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_AU.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_AU.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_AU.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_AU.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_CA.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_CA.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_CA.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_CA.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_GB-ise.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_GB-ise.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_GB-ise.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_GB-ise.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_US.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_US.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/en_US.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/en_US.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/es_ES.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/es_ES.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/es_ES.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/es_ES.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/fr.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/fr.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/fr.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/fr.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/pt_PT.aff` & `jupyterlab-spellchecker-0.7.3/dictionaries/pt_PT.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/dictionaries/pt_PT.dic` & `jupyterlab-spellchecker-0.7.3/dictionaries/pt_PT.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/__init__.py` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/dictionaries.py` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/dictionaries.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/handlers.py` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/package.json` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9706018518518518%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.5.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3ff26e696aa2c37cdbc7.js'}}",*

 * * "'version'": "'0.7.3'"}*

```diff
@@ -21,15 +21,15 @@
         "@jupyterlab/ui-components": "^3.0.2",
         "@lumino/widgets": "^1.16.1",
         "@types/codemirror": "0.0.87",
         "typo-js": "^1.1.0"
     },
     "description": "A spell checker for JupyterLab.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^3.5.0",
         "@jupyterlab/translation": "^3.0.0",
         "@lumino/coreutils": "^1.8.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -45,15 +45,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/spellchecker",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.12cf3b546f44ca3d0354.js",
+            "load": "static/remoteEntry.3ff26e696aa2c37cdbc7.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-spellchecker"
                 },
@@ -95,9 +95,9 @@
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/package.json.orig` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9710648148148147%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.5.0'}", "'version'": "'0.7.3'"}*

```diff
@@ -21,15 +21,15 @@
         "@jupyterlab/ui-components": "^3.0.2",
         "@lumino/widgets": "^1.16.1",
         "@types/codemirror": "0.0.87",
         "typo-js": "^1.1.0"
     },
     "description": "A spell checker for JupyterLab.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^3.5.0",
         "@jupyterlab/translation": "^3.0.0",
         "@lumino/coreutils": "^1.8.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -90,9 +90,9 @@
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/plugin.json` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/plugin.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'properties'": "{'ignore': {'default': {insert: [(5, 'IPython')]}}, 'mimeTypes': {'default': "*

 * *                 "{insert: [(2, 'text/x-rst'), (3, 'text/x-latex')]}}}"}*

```diff
@@ -56,30 +56,33 @@
         "ignore": {
             "$ref": "#/definitions/ignore",
             "default": [
                 "JupyterLab",
                 "Jupyter",
                 "JupyterHub",
                 "Voil\u00e0",
-                "Xeus"
+                "Xeus",
+                "IPython"
             ],
             "description": "Case-sensitive list of words to be ignored",
             "title": "Words to be ignored by the spellchecker"
         },
         "language": {
             "$ref": "#/definitions/language",
             "default": "en-us",
             "description": "Dictionary identifier, e.g. en-us",
             "title": "Language of the spellchecker"
         },
         "mimeTypes": {
             "$ref": "#/definitions/mimeTypes",
             "default": [
                 "text/plain",
-                "text/x-ipythongfm"
+                "text/x-ipythongfm",
+                "text/x-rst",
+                "text/x-latex"
             ],
             "description": "List of MIME types. GFM denotes GitHub Flavored Markdown",
             "title": "MIME types for files/editors for which the spellchecking should be activated"
         },
         "onlineDictionaries": {
             "$ref": "#/definitions/onlineDictionaries",
             "default": [],
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/301.f78600de2fee651cf61c.js` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/358.8de52c2073f382b46f26.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
+"use strict";
 (self.webpackChunk_ijmbarr_jupyterlab_spellchecker = self.webpackChunk_ijmbarr_jupyterlab_spellchecker || []).push([
-    [301], {
-        301: (e, t, n) => {
-            "use strict";
+    [358], {
+        358: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => x,
                 spellcheckIcon: () => f
             });
-            var s = n(314),
-                i = n(604),
-                r = n(786),
-                o = n(759),
-                a = n(706),
-                c = n(765),
-                l = n(509),
-                d = n(222),
-                h = n(364),
-                u = n(396),
-                g = n(251),
+            var s = n(650),
+                i = n(767),
+                r = n(591),
+                o = n(510),
+                a = n(431),
+                c = n(598),
+                l = n(169),
+                d = n(346),
+                h = n(442),
+                u = n(886),
+                g = n(258),
                 p = n(379),
                 m = n.n(p),
                 _ = n(760);
             m()(_.Z, {
                 insert: "head",
                 singleton: !1
             }), _.Z.locals;
@@ -325,27 +325,25 @@
                         const c = new v(e, t, n, s, i, r || h.nullTranslator, o, a);
                         console.log("Spellchecker Loaded ", c)
                     }
                 },
                 x = w
         },
         760: (e, t, n) => {
-            "use strict";
             n.d(t, {
                 Z: () => r
             });
             var s = n(645),
                 i = n.n(s)()((function(e) {
                     return e[1]
                 }));
             i.push([e.id, "body[data-jp-spellchecker-theme='background-box'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  background: rgba(255, 0, 0, .15);\n}\n\nbody[data-jp-spellchecker-theme='background-box'][data-jp-theme-light='false'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  background: rgba(255, 0, 0, .35);\n  text-shadow: 0 0 5px black;\n}\n\nbody[data-jp-spellchecker-theme='wavy-underline'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  text-decoration-line: underline;\n  text-decoration-style: wavy;\n  text-decoration-color: red;\n  /* For Chrome */\n  text-decoration-skip-ink: none;\n}\n\nbody[data-jp-spellchecker-theme='wavy-underline'][data-jp-theme-light='false'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  /* Use bright red for dark themes */\n  text-decoration-color: #ff5722;\n}\n\nbody[data-jp-spellchecker-theme='dotted-underline'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  text-decoration-line: underline;\n  text-decoration-style: dotted;\n  text-decoration-color: red;\n  /* For Chrome */\n  text-decoration-skip-ink: none;\n}\n\nbody[data-jp-spellchecker-theme='dotted-underline'][data-jp-theme-light='false'] .CodeMirror .cm-spell-error:not(.cm-url):not(.cm-tag):not(.cm-word) {\n  /* Use bright red for dark themes */\n    text-decoration-color: #ff5722;\n}\n", ""]);
             const r = i
         },
         645: e => {
-            "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = e(t);
                         return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                     })).join("")
@@ -363,15 +361,14 @@
                         var c = [].concat(e[a]);
                         s && i[c[0]] || (n && (c[2] ? c[2] = "".concat(n, " and ").concat(c[2]) : c[2] = n), t.push(c))
                     }
                 }, t
             }
         },
         379: (e, t, n) => {
-            "use strict";
             var s, i = function() {
                     var e = {};
                     return function(t) {
                         if (void 0 === e[t]) {
                             var n = document.querySelector(t);
                             if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                                 n = n.contentDocument.head
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/534.d33b047d412a2047177e.js` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/747.40ff56e19a50aa8f15aa.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,182 +1,179 @@
+"use strict";
 (self.webpackChunk_ijmbarr_jupyterlab_spellchecker = self.webpackChunk_ijmbarr_jupyterlab_spellchecker || []).push([
-    [534], {
-        150: (e, t, n) => {
-            "use strict";
-            n.d(t, {
+    [747], {
+        150: (e, n, t) => {
+            t.d(n, {
                 Z: () => a
             });
-            var r = n(645),
-                i = n.n(r)()((function(e) {
+            var r = t(645),
+                i = t.n(r)()((function(e) {
                     return e[1]
                 }));
             i.push([e.id, "", ""]);
             const a = i
         },
         645: e => {
-            "use strict";
             e.exports = function(e) {
-                var t = [];
-                return t.toString = function() {
-                    return this.map((function(t) {
-                        var n = e(t);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
+                var n = [];
+                return n.toString = function() {
+                    return this.map((function(n) {
+                        var t = e(n);
+                        return n[2] ? "@media ".concat(n[2], " {").concat(t, "}") : t
                     })).join("")
-                }, t.i = function(e, n, r) {
+                }, n.i = function(e, t, r) {
                     "string" == typeof e && (e = [
                         [null, e, ""]
                     ]);
                     var i = {};
                     if (r)
                         for (var a = 0; a < this.length; a++) {
                             var o = this[a][0];
                             null != o && (i[o] = !0)
                         }
                     for (var c = 0; c < e.length; c++) {
                         var s = [].concat(e[c]);
-                        r && i[s[0]] || (n && (s[2] ? s[2] = "".concat(n, " and ").concat(s[2]) : s[2] = n), t.push(s))
+                        r && i[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
                     }
-                }, t
+                }, n
             }
         },
-        379: (e, t, n) => {
-            "use strict";
+        379: (e, n, t) => {
             var r, i = function() {
                     var e = {};
-                    return function(t) {
-                        if (void 0 === e[t]) {
-                            var n = document.querySelector(t);
-                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
-                                n = n.contentDocument.head
+                    return function(n) {
+                        if (void 0 === e[n]) {
+                            var t = document.querySelector(n);
+                            if (window.HTMLIFrameElement && t instanceof window.HTMLIFrameElement) try {
+                                t = t.contentDocument.head
                             } catch (e) {
-                                n = null
+                                t = null
                             }
-                            e[t] = n
+                            e[n] = t
                         }
-                        return e[t]
+                        return e[n]
                     }
                 }(),
                 a = [];
 
             function o(e) {
-                for (var t = -1, n = 0; n < a.length; n++)
-                    if (a[n].identifier === e) {
-                        t = n;
+                for (var n = -1, t = 0; t < a.length; t++)
+                    if (a[t].identifier === e) {
+                        n = t;
                         break
-                    } return t
+                    } return n
             }
 
-            function c(e, t) {
-                for (var n = {}, r = [], i = 0; i < e.length; i++) {
+            function c(e, n) {
+                for (var t = {}, r = [], i = 0; i < e.length; i++) {
                     var c = e[i],
-                        s = t.base ? c[0] + t.base : c[0],
-                        u = n[s] || 0,
+                        s = n.base ? c[0] + n.base : c[0],
+                        u = t[s] || 0,
                         l = "".concat(s, " ").concat(u);
-                    n[s] = u + 1;
+                    t[s] = u + 1;
                     var f = o(l),
                         d = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3]
                         }; - 1 !== f ? (a[f].references++, a[f].updater(d)) : a.push({
                         identifier: l,
-                        updater: v(d, t),
+                        updater: v(d, n),
                         references: 1
                     }), r.push(l)
                 }
                 return r
             }
 
             function s(e) {
-                var t = document.createElement("style"),
+                var n = document.createElement("style"),
                     r = e.attributes || {};
                 if (void 0 === r.nonce) {
-                    var a = n.nc;
+                    var a = t.nc;
                     a && (r.nonce = a)
                 }
                 if (Object.keys(r).forEach((function(e) {
-                        t.setAttribute(e, r[e])
-                    })), "function" == typeof e.insert) e.insert(t);
+                        n.setAttribute(e, r[e])
+                    })), "function" == typeof e.insert) e.insert(n);
                 else {
                     var o = i(e.insert || "head");
                     if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    o.appendChild(t)
+                    o.appendChild(n)
                 }
-                return t
+                return n
             }
-            var u, l = (u = [], function(e, t) {
-                return u[e] = t, u.filter(Boolean).join("\n")
+            var u, l = (u = [], function(e, n) {
+                return u[e] = n, u.filter(Boolean).join("\n")
             });
 
-            function f(e, t, n, r) {
-                var i = n ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
-                if (e.styleSheet) e.styleSheet.cssText = l(t, i);
+            function f(e, n, t, r) {
+                var i = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
+                if (e.styleSheet) e.styleSheet.cssText = l(n, i);
                 else {
                     var a = document.createTextNode(i),
                         o = e.childNodes;
-                    o[t] && e.removeChild(o[t]), o.length ? e.insertBefore(a, o[t]) : e.appendChild(a)
+                    o[n] && e.removeChild(o[n]), o.length ? e.insertBefore(a, o[n]) : e.appendChild(a)
                 }
             }
 
-            function d(e, t, n) {
-                var r = n.css,
-                    i = n.media,
-                    a = n.sourceMap;
+            function d(e, n, t) {
+                var r = t.css,
+                    i = t.media,
+                    a = t.sourceMap;
                 if (i ? e.setAttribute("media", i) : e.removeAttribute("media"), a && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleSheet) e.styleSheet.cssText = r;
                 else {
                     for (; e.firstChild;) e.removeChild(e.firstChild);
                     e.appendChild(document.createTextNode(r))
                 }
             }
             var p = null,
                 h = 0;
 
-            function v(e, t) {
-                var n, r, i;
-                if (t.singleton) {
+            function v(e, n) {
+                var t, r, i;
+                if (n.singleton) {
                     var a = h++;
-                    n = p || (p = s(t)), r = f.bind(null, n, a, !1), i = f.bind(null, n, a, !0)
-                } else n = s(t), r = d.bind(null, n, t), i = function() {
+                    t = p || (p = s(n)), r = f.bind(null, t, a, !1), i = f.bind(null, t, a, !0)
+                } else t = s(n), r = d.bind(null, t, n), i = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
-                    }(n)
+                    }(t)
                 };
                 return r(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            r(e = t)
+                    function(n) {
+                        if (n) {
+                            if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap) return;
+                            r(e = n)
                         } else i()
                     }
             }
-            e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
-                var n = c(e = e || [], t);
+            e.exports = function(e, n) {
+                (n = n || {}).singleton || "boolean" == typeof n.singleton || (n.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
+                var t = c(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var r = 0; r < n.length; r++) {
-                            var i = o(n[r]);
+                        for (var r = 0; r < t.length; r++) {
+                            var i = o(t[r]);
                             a[i].references--
                         }
-                        for (var s = c(e, t), u = 0; u < n.length; u++) {
-                            var l = o(n[u]);
+                        for (var s = c(e, n), u = 0; u < t.length; u++) {
+                            var l = o(t[u]);
                             0 === a[l].references && (a[l].updater(), a.splice(l, 1))
                         }
-                        n = s
+                        t = s
                     }
                 }
             }
         },
-        534: (e, t, n) => {
-            "use strict";
-            n.r(t);
-            var r = n(379),
-                i = n.n(r),
-                a = n(150);
+        747: (e, n, t) => {
+            t.r(n);
+            var r = t(379),
+                i = t.n(r),
+                a = t(150);
             i()(a.Z, {
                 insert: "head",
                 singleton: !1
             }), a.Z.locals
         }
     }
 ]);
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/581.83daa50633cb94659e90.js` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/581.93362237019cb70e1d50.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker/labextension/static/remoteEntry.12cf3b546f44ca3d0354.js` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker/labextension/static/remoteEntry.3ff26e696aa2c37cdbc7.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,127 +1,123 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, s, f, d, p, c, h, b, v, y, g = {
+    var e, r, t, n, a, o, i, l, u, s, d, f, p, c, h, v, b, y, m = {
             34: (e, r, t) => {
-                var a = {
-                        "./index": () => t.e(301).then((() => () => t(301))),
-                        "./extension": () => t.e(301).then((() => () => t(301))),
-                        "./style": () => t.e(534).then((() => () => t(534)))
+                var n = {
+                        "./index": () => t.e(358).then((() => () => t(358))),
+                        "./extension": () => t.e(358).then((() => () => t(358))),
+                        "./style": () => t.e(747).then((() => () => t(747)))
                     },
-                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var a = t.S.default,
-                                n = "default";
+                            var n = "default",
+                                a = t.S[n];
                             if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => n,
+                    get: () => a,
                     init: () => o
                 })
             }
         },
-        m = {};
+        g = {};
 
     function j(e) {
-        var r = m[e];
+        var r = g[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = g[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, j), t.exports
+        return m[e](t, t.exports, j), t.exports
     }
-    j.m = g, j.c = m, j.n = e => {
+    j.m = m, j.c = g, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return j.d(r, {
             a: r
         }), r
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
-        301: "f78600de2fee651cf61c",
-        534: "d33b047d412a2047177e",
-        581: "83daa50633cb94659e90"
+        358: "8de52c2073f382b46f26",
+        581: "93362237019cb70e1d50",
+        747: "40ff56e19a50aa8f15aa"
     } [e] + ".js?v=" + {
-        301: "f78600de2fee651cf61c",
-        534: "d33b047d412a2047177e",
-        581: "83daa50633cb94659e90"
+        358: "8de52c2073f382b46f26",
+        581: "93362237019cb70e1d50",
+        747: "40ff56e19a50aa8f15aa"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@ijmbarr/jupyterlab_spellchecker:", j.l = (t, a, n, o) => {
-        if (e[t]) e[t].push(a);
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@ijmbarr/jupyterlab_spellchecker:", j.l = (t, n, a, o) => {
+        if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== n)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var f = u[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        i = f;
+                    var d = u[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var d = (r, a) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var n = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         j.S = {};
         var e = {},
             r = {};
-        j.I = (t, a) => {
-            a || (a = []);
-            var n = r[t];
-            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
-                if (a.push(n), e[t]) return e[t];
+        j.I = (t, n) => {
+            n || (n = []);
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
                 var o = j.S[t],
                     i = "@ijmbarr/jupyterlab_spellchecker",
-                    l = (e, r, t, a) => {
-                        var n = o[e] = o[e] || {},
-                            l = n[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
+                    l = (e, r, t, n) => {
+                        var a = o[e] = o[e] || {},
+                            l = a[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
-                            eager: !!a
+                            eager: !!n
                         })
                     },
                     u = [];
-                switch (t) {
-                    case "default":
-                        l("@ijmbarr/jupyterlab_spellchecker", "0.7.2", (() => j.e(301).then((() => () => j(301))))), l("typo-js", "1.2.0", (() => j.e(581).then((() => () => j(581)))))
-                }
-                return e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@ijmbarr/jupyterlab_spellchecker", "0.7.3", (() => j.e(358).then((() => () => j(358))))), l("typo-js", "1.2.0", (() => j.e(581).then((() => () => j(581)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -129,74 +125,74 @@
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            a = t[1] ? r(t[1]) : [];
-        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
-    }, a = (e, r) => {
+            n = t[1] ? r(t[1]) : [];
+        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
+    }, n = (e, r) => {
         e = t(e), r = t(r);
-        for (var a = 0;;) {
-            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
-            var n = e[a],
-                o = (typeof n)[0];
-            if (a >= r.length) return "u" == o;
-            var i = r[a],
+        for (var n = 0;;) {
+            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
+            var i = r[n],
                 l = (typeof i)[0];
             if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && n != i) return n < i;
-            a++
+            if ("o" != o && "u" != o && a != i) return a < i;
+            n++
         }
-    }, n = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var a = e[0],
-                n = a < 0;
-            n && (a = -a - 1);
+            var n = e[0],
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
-                if ("u" == f) {
-                    if (!u || "u" != d) return !1
+                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
+                if ("u" == d) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (d == f)
-                        if (l <= a) {
+                    if (f == d)
+                        if (l <= n) {
                             if (s != e[l]) return !1
                         } else {
-                            if (n ? s > e[l] : s < e[l]) return !1;
+                            if (a ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (n || l <= a) return !1;
+                else if ("s" != f && "n" != f) {
+                    if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || f < d != n) return !1;
+                    if (l <= n || d < f != a) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -204,89 +200,92 @@
         return !!c()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", s = (e, r, t, a) => {
-        var n = l(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(t, n, a)), d(e[t][n])
-    }, f = (e, r, t) => {
-        var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, a, n) {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), f(e[t][a])
+    }, d = (e, r, t) => {
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
         var o = j.I(r);
-        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
-        var o = r && j.o(r, t) && f(r, t, a);
-        return o ? d(o) : n()
-    })), b = {}, v = {
-        222: () => c("default", "@jupyterlab/codemirror", [1, 3, 1, 17]),
-        251: () => c("default", "@jupyterlab/services", [1, 6, 1, 17]),
-        314: () => c("default", "@jupyterlab/fileeditor", [1, 3, 1, 17]),
-        364: () => c("default", "@jupyterlab/translation", [1, 3, 1, 17]),
-        396: () => c("default", "@jupyterlab/coreutils", [1, 5, 1, 17]),
+        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+        var o = r && j.o(r, t) && d(r, t, n);
+        return o ? f(o) : a()
+    })), v = {}, b = {
+        169: () => c("default", "@jupyterlab/statusbar", [1, 3, 6, 1]),
+        258: () => c("default", "@jupyterlab/services", [1, 6, 6, 1]),
+        346: () => c("default", "@jupyterlab/codemirror", [1, 3, 6, 1]),
         397: () => h("default", "typo-js", [1, 1, 1, 0], (() => j.e(581).then((() => () => j(581))))),
-        509: () => c("default", "@jupyterlab/statusbar", [1, 3, 1, 17]),
-        604: () => c("default", "@jupyterlab/notebook", [1, 3, 1, 17]),
-        706: () => c("default", "@lumino/widgets", [1, 1, 19, 0]),
-        759: () => c("default", "@jupyterlab/apputils", [1, 3, 1, 17]),
-        765: () => c("default", "@jupyterlab/settingregistry", [1, 3, 1, 17]),
-        786: () => c("default", "@jupyterlab/ui-components", [1, 3, 1, 17])
+        431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
+        442: () => c("default", "@jupyterlab/translation", [1, 3, 6, 1]),
+        510: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
+        591: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
+        598: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 1]),
+        650: () => c("default", "@jupyterlab/fileeditor", [1, 3, 6, 1]),
+        767: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 1]),
+        886: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 1])
     }, y = {
-        301: [222, 251, 314, 364, 396, 397, 509, 604, 706, 759, 765, 786]
+        358: [169, 258, 346, 397, 431, 442, 510, 591, 598, 650, 767, 886]
     }, j.f.consumes = (e, r) => {
         j.o(y, e) && y[e].forEach((e => {
-            if (j.o(b, e)) return r.push(b[e]);
+            if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, j.m[e] = t => {
+                    v[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
-                a = r => {
-                    delete b[e], j.m[e] = t => {
+                n = r => {
+                    delete v[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var n = v[e]();
-                n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
+                var a = b[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
-                a(e)
+                n(e)
             }
         }))
     }, (() => {
         var e = {
             911: 0
         };
         j.f.j = (r, t) => {
-            var a = j.o(e, r) ? e[r] : void 0;
-            if (0 !== a)
-                if (a) t.push(a[2]);
+            var n = j.o(e, r) ? e[r] : void 0;
+            if (0 !== n)
+                if (n) t.push(n[2]);
                 else {
-                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
-                    t.push(a[2] = n);
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
                     var o = j.p + j.u(r),
                         i = new Error;
                     j.l(o, (t => {
-                        if (j.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
-                            var n = t && ("load" === t.type ? "missing" : t.type),
+                        if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var a, n, [o, i, l] = t,
+                var n, a, [o, i, l] = t,
                     u = 0;
-                for (a in i) j.o(i, a) && (j.m[a] = i[a]);
-                for (l && l(j), r && r(t); u < o.length; u++) n = o[u], j.o(e, n) && e[n] && e[n][0](), e[o[u]] = 0
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    l && l(j)
+                }
+                for (r && r(t); u < o.length; u++) a = o[u], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_ijmbarr_jupyterlab_spellchecker = self.webpackChunk_ijmbarr_jupyterlab_spellchecker || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
+    })(), j.nc = void 0;
     var w = j(34);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@ijmbarr/jupyterlab_spellchecker"] = w
 })();
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/PKG-INFO` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-spellchecker
-Version: 0.7.2
+Version: 0.7.3
 Summary: A spell checker for JupyterLab.
 Home-page: https://github.com/jupyterlab-contrib/spellchecker
 Author: JupyterLab Spellchecker Development Team
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/spellchecker/issues
 Project-URL: Source Code, https://github.com/jupyterlab-contrib/spellchecker
 Keywords: Jupyter,JupyterLab,JupyterLab3
@@ -196,9 +196,7 @@
 ```
 
 Run tests:
 
 ```bash
 python -m pytest
 ```
-
-
```

### Comparing `jupyterlab-spellchecker-0.7.2/jupyterlab_spellchecker.egg-info/SOURCES.txt` & `jupyterlab-spellchecker-0.7.3/jupyterlab_spellchecker.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,20 @@
 jupyterlab_spellchecker.egg-info/dependency_links.txt
 jupyterlab_spellchecker.egg-info/not-zip-safe
 jupyterlab_spellchecker.egg-info/requires.txt
 jupyterlab_spellchecker.egg-info/top_level.txt
 jupyterlab_spellchecker/labextension/package.json
 jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/package.json.orig
 jupyterlab_spellchecker/labextension/schemas/@ijmbarr/jupyterlab_spellchecker/plugin.json
-jupyterlab_spellchecker/labextension/static/301.f78600de2fee651cf61c.js
-jupyterlab_spellchecker/labextension/static/534.d33b047d412a2047177e.js
-jupyterlab_spellchecker/labextension/static/581.83daa50633cb94659e90.js
-jupyterlab_spellchecker/labextension/static/remoteEntry.12cf3b546f44ca3d0354.js
+jupyterlab_spellchecker/labextension/static/358.8de52c2073f382b46f26.js
+jupyterlab_spellchecker/labextension/static/581.93362237019cb70e1d50.js
+jupyterlab_spellchecker/labextension/static/747.40ff56e19a50aa8f15aa.js
+jupyterlab_spellchecker/labextension/static/remoteEntry.3ff26e696aa2c37cdbc7.js
 jupyterlab_spellchecker/labextension/static/style.js
+jupyterlab_spellchecker/labextension/static/third-party-licenses.json
 src/handler.ts
 src/index.ts
 src/loader.d.ts
 src/svg.d.ts
 style/base.css
 style/index.css
 style/index.js
```

### Comparing `jupyterlab-spellchecker-0.7.2/package.json` & `jupyterlab-spellchecker-0.7.3/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9710648148148147%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.5.0'}", "'version'": "'0.7.3'"}*

```diff
@@ -21,15 +21,15 @@
         "@jupyterlab/ui-components": "^3.0.2",
         "@lumino/widgets": "^1.16.1",
         "@types/codemirror": "0.0.87",
         "typo-js": "^1.1.0"
     },
     "description": "A spell checker for JupyterLab.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^3.5.0",
         "@jupyterlab/translation": "^3.0.0",
         "@lumino/coreutils": "^1.8.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -90,9 +90,9 @@
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.7.3"
 }
```

### Comparing `jupyterlab-spellchecker-0.7.2/setup.py` & `jupyterlab-spellchecker-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/src/handler.ts` & `jupyterlab-spellchecker-0.7.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/src/index.ts` & `jupyterlab-spellchecker-0.7.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/style/icons/LICENSE` & `jupyterlab-spellchecker-0.7.3/style/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/style/index.css` & `jupyterlab-spellchecker-0.7.3/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/tsconfig.json` & `jupyterlab-spellchecker-0.7.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab-spellchecker-0.7.2/yarn.lock` & `jupyterlab-spellchecker-0.7.3/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,62 @@
   version "0.3.1"
   resolved "https://registry.yarnpkg.com/@hypnosphi/create-react-context/-/create-react-context-0.3.1.tgz#f8bfebdc7665f5d426cba3753e0e9c7d3154d7c6"
   integrity sha512-V1klUed202XahrWJLLOT3EXNeCpFHCcJntdFGI15ntCwau+jfT386w7OFTMaCqOgXUH1fa0w/I1oZs+i/Rfr0A==
   dependencies:
     gud "^1.0.0"
     warning "^4.0.3"
 
+"@jridgewell/gen-mapping@^0.3.0":
+  version "0.3.2"
+  resolved "https://registry.yarnpkg.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz#c1aedc61e853f2bb9f5dfe6d4442d3b565b253b9"
+  integrity sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==
+  dependencies:
+    "@jridgewell/set-array" "^1.0.1"
+    "@jridgewell/sourcemap-codec" "^1.4.10"
+    "@jridgewell/trace-mapping" "^0.3.9"
+
+"@jridgewell/resolve-uri@3.1.0", "@jridgewell/resolve-uri@^3.0.3":
+  version "3.1.0"
+  resolved "https://registry.yarnpkg.com/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz#2203b118c157721addfe69d47b70465463066d78"
+  integrity sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==
+
+"@jridgewell/set-array@^1.0.1":
+  version "1.1.2"
+  resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.1.2.tgz#7c6cf998d6d20b914c0a55a91ae928ff25965e72"
+  integrity sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==
+
+"@jridgewell/source-map@^0.3.2":
+  version "0.3.2"
+  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.2.tgz#f45351aaed4527a298512ec72f81040c998580fb"
+  integrity sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==
+  dependencies:
+    "@jridgewell/gen-mapping" "^0.3.0"
+    "@jridgewell/trace-mapping" "^0.3.9"
+
+"@jridgewell/sourcemap-codec@1.4.14", "@jridgewell/sourcemap-codec@^1.4.10":
+  version "1.4.14"
+  resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz#add4c98d341472a289190b424efbdb096991bb24"
+  integrity sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==
+
+"@jridgewell/trace-mapping@^0.3.14":
+  version "0.3.17"
+  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.17.tgz#793041277af9073b0951a7fe0f0d8c4c98c36985"
+  integrity sha512-MCNzAp77qzKca9+W/+I0+sEpaUnZoeasnghNeVc41VZCEKaCH73Vq3BZZ/SzWIgrqE4H4ceI+p+b6C0mHf9T4g==
+  dependencies:
+    "@jridgewell/resolve-uri" "3.1.0"
+    "@jridgewell/sourcemap-codec" "1.4.14"
+
+"@jridgewell/trace-mapping@^0.3.9":
+  version "0.3.14"
+  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.14.tgz#b231a081d8f66796e475ad588a1ef473112701ed"
+  integrity sha512-bJWEfQ9lPTvm3SneWwRFVLzrh6nhjwqw7TUFFBEMzwvg7t7PCDenf2lDwqo4NQXzdpgBXyFgDWnQA+2vkruksQ==
+  dependencies:
+    "@jridgewell/resolve-uri" "^3.0.3"
+    "@jridgewell/sourcemap-codec" "^1.4.10"
+
 "@jupyterlab/application@^3.0.3":
   version "3.0.11"
   resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.0.11.tgz#01d502656db1aa07afc439a58171897af2a2fdd1"
   integrity sha512-UBqnRcXSy/Iz5vq1dCYkQvSkCFGPqjQdDFvOhvXacGxHklVjiku5Epltdbe2kQl+uhhn7VC4HEh1kzxiYamwcg==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
     "@jupyterlab/apputils" "^3.0.9"
@@ -159,74 +207,55 @@
     "@jupyterlab/nbformat" "^3.0.6"
     "@jupyterlab/observables" "^4.0.6"
     "@jupyterlab/rendermime" "^3.0.10"
     "@jupyterlab/rendermime-interfaces" "^3.0.9"
     "@lumino/disposable" "^1.4.3"
     "@lumino/signaling" "^1.4.3"
 
-"@jupyterlab/builder@^3.0.0":
-  version "3.0.9"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.0.9.tgz#60b184accd63afced196d2369c886f6fe238acc4"
-  integrity sha512-IjWHk/xTgufTyggbT/0tGFeRdsHe3rNMQkOMqDN5+8YqFV4uCTUNokgvyysedgwB7JP+tcPclN/a3QoIPjAq/w==
-  dependencies:
-    "@jupyterlab/buildutils" "^3.0.7"
-    "@lumino/algorithm" "^1.3.3"
-    "@lumino/application" "^1.13.1"
-    "@lumino/commands" "^1.12.0"
-    "@lumino/coreutils" "^1.5.3"
-    "@lumino/disposable" "^1.4.3"
-    "@lumino/domutils" "^1.2.3"
-    "@lumino/dragdrop" "^1.7.1"
-    "@lumino/messaging" "^1.4.3"
-    "@lumino/properties" "^1.2.3"
-    "@lumino/signaling" "^1.4.3"
-    "@lumino/virtualdom" "^1.8.0"
-    "@lumino/widgets" "^1.16.1"
+"@jupyterlab/builder@^3.5.0":
+  version "3.6.1"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.1.tgz#a04bf0312e8679d1f452c27fee2554ba4a6af3f5"
+  integrity sha512-LvHQe6InEXJisEcvAdvSFbEEl8OhTjxBSNz7MrjRB+Ur+Qs898dg8QhDH9Ad5mgK3uh4nEN1BDq9W7C/NomqoA==
+  dependencies:
+    "@lumino/algorithm" "^1.9.0"
+    "@lumino/application" "^1.31.3"
+    "@lumino/commands" "^1.19.0"
+    "@lumino/coreutils" "^1.11.0"
+    "@lumino/disposable" "^1.10.0"
+    "@lumino/domutils" "^1.8.0"
+    "@lumino/dragdrop" "^1.13.0"
+    "@lumino/messaging" "^1.10.0"
+    "@lumino/properties" "^1.8.0"
+    "@lumino/signaling" "^1.10.0"
+    "@lumino/virtualdom" "^1.14.0"
+    "@lumino/widgets" "^1.37.1"
     ajv "^6.12.3"
     commander "~6.0.0"
     css-loader "^5.0.1"
     duplicate-package-checker-webpack-plugin "^3.0.0"
     file-loader "~6.0.0"
     fs-extra "^9.0.1"
     glob "~7.1.6"
+    license-webpack-plugin "^2.3.14"
     mini-css-extract-plugin "~1.3.2"
     path-browserify "^1.0.0"
     process "^0.11.10"
     raw-loader "~4.0.0"
+    source-map-loader "~1.0.2"
     style-loader "~2.0.0"
     supports-color "^7.2.0"
     svg-url-loader "~6.0.0"
     terser-webpack-plugin "^4.1.0"
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
-    webpack "^5.3.1"
+    webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/buildutils@^3.0.7":
-  version "3.0.7"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/buildutils/-/buildutils-3.0.7.tgz#e83d3303b5f2bddd0b6b39fdab81864b67574dec"
-  integrity sha512-V3A9foBIP9CJcblyZTEKHtkY6o/3pRodxNAZqveiDDpBdQhM8xv4uOLBKkkMxroa5Eh5Goub4fw+JHxI2nKGXw==
-  dependencies:
-    "@lumino/coreutils" "^1.5.3"
-    "@yarnpkg/lockfile" "^1.1.0"
-    child_process "~1.0.2"
-    commander "~6.0.0"
-    crypto "~1.0.1"
-    dependency-graph "^0.9.0"
-    fs-extra "^9.0.1"
-    glob "~7.1.6"
-    inquirer "^7.0.0"
-    package-json "^6.5.0"
-    prettier "^2.1.1"
-    semver "^7.3.2"
-    sort-package-json "~1.44.0"
-    typescript "~4.1.3"
-
 "@jupyterlab/cells@^3.0.11", "@jupyterlab/cells@^3.0.3":
   version "3.0.11"
   resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.0.11.tgz#f1e9a4460b4b005ae0adc789c702ad0b392a39fd"
   integrity sha512-mDnHzm2HhY3OZazgC1XIE0HG553nNutX3AESPXvnioLfFZfHz1RzijceUs8+jYx1Hl27UZuL9Ah/1J2NZuDqfg==
   dependencies:
     "@jupyterlab/apputils" "^3.0.9"
     "@jupyterlab/attachments" "^3.0.10"
@@ -654,74 +683,147 @@
     typestyle "^2.0.4"
 
 "@lumino/algorithm@^1.3.3", "@lumino/algorithm@^1.6.0":
   version "1.6.0"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-1.6.0.tgz#771e7896cd94e660f9b58a52f80e1bb255de1d41"
   integrity sha512-NMOcm5Yr9nXz5gokS/K4jHBbUMQYBkvDXl1n51XWdcz0LY+oGuIKPhjazhUgmbNRehzdZBj5hMMd1+htYWeVKQ==
 
+"@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.2":
+  version "1.9.2"
+  resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-1.9.2.tgz#b95e6419aed58ff6b863a51bfb4add0f795141d3"
+  integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
+
 "@lumino/application@^1.13.1":
   version "1.20.0"
   resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.20.0.tgz#b50ca4180bc400589fdfcfcaab08c4af937fccd0"
   integrity sha512-FAoQcq4L3ZswTK0lWfLKnG1ecG26cwqjzg2fyoBeuWGBi1TG9BYjFBdV7ErTFMxW8jE1CLOLuxsZaKFLNErcKA==
   dependencies:
     "@lumino/commands" "^1.15.0"
     "@lumino/coreutils" "^1.8.0"
     "@lumino/widgets" "^1.23.0"
 
+"@lumino/application@^1.31.3":
+  version "1.31.3"
+  resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.3.tgz#c5a9bc84212a2505be8f5d43516e0603d9100965"
+  integrity sha512-XnsXm5PD9QevJRl/pHJziYmhRKqJYjEOTL6Vh9dtKpPPML57uswOj59Pokxx/yCvym1xRF9iDVvujy3KallRwQ==
+  dependencies:
+    "@lumino/commands" "^1.21.1"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/widgets" "^1.37.1"
+
 "@lumino/collections@^1.6.0":
   version "1.6.0"
   resolved "https://registry.yarnpkg.com/@lumino/collections/-/collections-1.6.0.tgz#7d3e94cee26409b0cd719c1934bdda471e6a5662"
   integrity sha512-ZETm0/xF0oUHV03sOXNOfFI1EEpS317HvN5n+fZBJvCNZIrJkWmKD8QuxcfwHb7AChKUhXlVHhDbWlb1LKnd7g==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
 
+"@lumino/collections@^1.9.3":
+  version "1.9.3"
+  resolved "https://registry.yarnpkg.com/@lumino/collections/-/collections-1.9.3.tgz#370dc2d50aa91371288a4f7376bea5a3191fc5dc"
+  integrity sha512-2i2Wf1xnfTgEgdyKEpqM16bcYRIhUOGCDzaVCEZACVG9R1CgYwOe3zfn71slBQOVSjjRgwYrgLXu4MBpt6YK+g==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+
 "@lumino/commands@^1.12.0", "@lumino/commands@^1.15.0":
   version "1.15.0"
   resolved "https://registry.yarnpkg.com/@lumino/commands/-/commands-1.15.0.tgz#06eb94fb4b34cad59f35b1fcaf473e8d2047f779"
   integrity sha512-JOE68KfbR9xw5YTfcwo+9E0PSWidifEMAcOC/aXd7iSzfsCRknMTcMQIUGL277IU7J7CJvoe10DUE5QKwTmX+g==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
     "@lumino/coreutils" "^1.8.0"
     "@lumino/disposable" "^1.7.0"
     "@lumino/domutils" "^1.5.0"
     "@lumino/keyboard" "^1.5.0"
     "@lumino/signaling" "^1.7.0"
     "@lumino/virtualdom" "^1.11.0"
 
+"@lumino/commands@^1.19.0", "@lumino/commands@^1.21.1":
+  version "1.21.1"
+  resolved "https://registry.yarnpkg.com/@lumino/commands/-/commands-1.21.1.tgz#eda8b3cf5ef73b9c8ce93b3b5cf66bb053df2a76"
+  integrity sha512-d1zJmwz5bHU0BM/Rl3tRdZ7/WgXnFB0bM7x7Bf0XDlmX++jnU9k0j3mh6/5JqCGLmIApKCRwVqSaV7jPmSJlcQ==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/domutils" "^1.8.2"
+    "@lumino/keyboard" "^1.8.2"
+    "@lumino/signaling" "^1.11.1"
+    "@lumino/virtualdom" "^1.14.3"
+
+"@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
+  integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
+
 "@lumino/coreutils@^1.5.3", "@lumino/coreutils@^1.8.0":
   version "1.8.0"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.8.0.tgz#4feb3ccbfbc3efc8e395a90f22b5a938fbad959a"
   integrity sha512-OvCsaASUqOE7R6Dxngyk4/b5QMOjyRUNxuZuuL+fx+JvGKZFZ/B2c9LYtAJ9mDmQ1BQiGNV/qSpL4o7x8PCfjw==
 
+"@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4":
+  version "1.10.4"
+  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
+  integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/signaling" "^1.11.1"
+
 "@lumino/disposable@^1.4.3", "@lumino/disposable@^1.7.0":
   version "1.7.0"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.7.0.tgz#539463490cb42e8d2dc46b5ff7cc291f4f1a8d07"
   integrity sha512-3mWi11ko3XVY63BPwvys7MXrbFddA2i+gp72d0wAKM2NDDUopVPikMHhJpjGJcw+otjahzXYiTewxPDEau9dYg==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
     "@lumino/signaling" "^1.7.0"
 
 "@lumino/domutils@^1.2.3", "@lumino/domutils@^1.5.0":
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.5.0.tgz#fdba0cfe404b4817e63aa064f63b3c965655e76e"
   integrity sha512-dZ0Aa+/qhvfPc1aa5kX4LLGE3B6BW1XmJa0R1XVCEpAFY3cZiujuQWmhYHJtZPrOiqn0UtioT2OpqnWdtCWc0A==
 
+"@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
+  integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
+
 "@lumino/dragdrop@^1.10.0", "@lumino/dragdrop@^1.7.1":
   version "1.10.0"
   resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.10.0.tgz#2fddacfee055e660dd33dd9a3cfbd8fbba811673"
   integrity sha512-A3cNLcp09zygOprWmLTkLZCQYNq3dJfN+mhni4IZizqCTkKbTCEzo2/IwoCWvy+ABKft8d/A9Y40wFW6yJ9OyA==
   dependencies:
     "@lumino/coreutils" "^1.8.0"
     "@lumino/disposable" "^1.7.0"
 
+"@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.4":
+  version "1.14.4"
+  resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.4.tgz#b6ec4cf4f470c17a849e31f299d5a24acdc8c7d3"
+  integrity sha512-IHX2M8Yqs2YsFHHXKSKiYLgv9DEuhyyKoDS85Chg34J9OaPC5ocT0AmNVnpeq9T4A50sg3vdL9mSRCZ0f302Gw==
+  dependencies:
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+
 "@lumino/keyboard@^1.5.0":
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.5.0.tgz#c12213822dd2645c412e8689aecd4a2726113ac6"
   integrity sha512-/uF9xqHYVbIkser2Q6UIv7VWrzThr1fxAmSOShjSoKGocL0XHeaBaCOMezSaVxnJ1wm1ciNdhMsjscVM8Inp7g==
 
+"@lumino/keyboard@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.8.2.tgz#714dbe671f0718f516d1ec23188b31a9ccd82fb2"
+  integrity sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==
+
+"@lumino/messaging@^1.10.0", "@lumino/messaging@^1.10.3":
+  version "1.10.3"
+  resolved "https://registry.yarnpkg.com/@lumino/messaging/-/messaging-1.10.3.tgz#b6227bdfc178a8542571625ecb68063691b6af3c"
+  integrity sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/collections" "^1.9.3"
+
 "@lumino/messaging@^1.4.3", "@lumino/messaging@^1.7.0":
   version "1.7.0"
   resolved "https://registry.yarnpkg.com/@lumino/messaging/-/messaging-1.7.0.tgz#32542f9e9a266fd5b3f71842f70cfe141e016d93"
   integrity sha512-QYWf9QGIGD0Oes104zw7mVln4S8yRije2mZhNNRBjkYcDuQlPW+eRSuC5LwAMsFnGymBlUPwPbKOUEO2RbhAtg==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
     "@lumino/collections" "^1.6.0"
@@ -736,28 +838,48 @@
     "@lumino/signaling" "^1.7.0"
 
 "@lumino/properties@^1.2.3", "@lumino/properties@^1.5.0":
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/@lumino/properties/-/properties-1.5.0.tgz#7e8638e84c51bb110c5a69f91ca8b0e40b2c3fca"
   integrity sha512-YqpJE6/1Wkjrie0E+ypu+yzd55B5RlvKYMnQs3Ox+SrJsnNBhA6Oj44EhVf8SUTuHgn1t/mm+LvbswKN5RM4+g==
 
+"@lumino/properties@^1.8.0", "@lumino/properties@^1.8.2":
+  version "1.8.2"
+  resolved "https://registry.yarnpkg.com/@lumino/properties/-/properties-1.8.2.tgz#91131f2ca91a902faa138771eb63341db78fc0fd"
+  integrity sha512-EkjI9Cw8R0U+xC9HxdFSu7X1tz1H1vKu20cGvJ2gU+CXlMB1DvoYJCYxCThByHZ+kURTAap4SE5x8HvKwNPbig==
+
+"@lumino/signaling@^1.10.0", "@lumino/signaling@^1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
+  integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/properties" "^1.8.2"
+
 "@lumino/signaling@^1.4.3", "@lumino/signaling@^1.7.0":
   version "1.7.0"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.7.0.tgz#76da4738bf8f19e7da6de1d457a54220e2140670"
   integrity sha512-a5kd11Sf04jTfpzxCr7TOBD2o5YvItA4IGwiOoG+QR6sPR0Rwmcf47fPItqXo5st58iNIblC3F+c264N+Me+gg==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
 
 "@lumino/virtualdom@^1.11.0", "@lumino/virtualdom@^1.8.0":
   version "1.11.0"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.11.0.tgz#468b4d28a07e2b8988dc583b4aab40e37dc6955e"
   integrity sha512-G0sIx4pLYbgJ4w+SIgsCYQgKP/GBrWgjh8wcumD6XpaYZNivJv4c01xITYYlh7FU61jZmMWMrxtZztArNRDSqg==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
 
+"@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
+  version "1.14.3"
+  resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
+  integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+
 "@lumino/widgets@^1.16.1", "@lumino/widgets@^1.23.0":
   version "1.23.0"
   resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.23.0.tgz#096c7574de75fa67b32bcb914c5dae290fbee6f3"
   integrity sha512-0Akt9ESgc06SJ3EJG3VK1Liw+AAjRWkKMfm8VUTwT/1QJYYGZ8kfHNO97mkBLv+0EkLEkZIeaQb8fIoU6vh7bw==
   dependencies:
     "@lumino/algorithm" "^1.6.0"
     "@lumino/commands" "^1.15.0"
@@ -767,14 +889,31 @@
     "@lumino/dragdrop" "^1.10.0"
     "@lumino/keyboard" "^1.5.0"
     "@lumino/messaging" "^1.7.0"
     "@lumino/properties" "^1.5.0"
     "@lumino/signaling" "^1.7.0"
     "@lumino/virtualdom" "^1.11.0"
 
+"@lumino/widgets@^1.37.1":
+  version "1.37.1"
+  resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.1.tgz#d7a2398b276e15e60aff4fec58c035d46549a75b"
+  integrity sha512-/whz5B/hL0fjv0bR8JYZ+Emx+CH7HBwXc4TqI9PrrHGm3g6+jRJAyIFGZcQubqkPxxHrRE/VxQgoDKGhINw/Gw==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/commands" "^1.21.1"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/domutils" "^1.8.2"
+    "@lumino/dragdrop" "^1.14.4"
+    "@lumino/keyboard" "^1.8.2"
+    "@lumino/messaging" "^1.10.3"
+    "@lumino/properties" "^1.8.2"
+    "@lumino/signaling" "^1.11.1"
+    "@lumino/virtualdom" "^1.14.3"
+
 "@nodelib/fs.scandir@2.1.4":
   version "2.1.4"
   resolved "https://registry.yarnpkg.com/@nodelib/fs.scandir/-/fs.scandir-2.1.4.tgz#d4b3549a5db5de2683e0c1071ab4f140904bbf69"
   integrity sha512-33g3pMJk3bg5nXbL/+CY6I2eJDzZAni49PfJnL5fghPTggPvBd/pFNSgJsdAgWptuFu7qq/ERvOYFlhvsLTCKA==
   dependencies:
     "@nodelib/fs.stat" "2.0.4"
     run-parallel "^1.1.9"
@@ -796,76 +935,61 @@
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@npmcli/move-file/-/move-file-1.1.2.tgz#1a82c3e372f7cae9253eb66d72543d6b8685c674"
   integrity sha512-1SUf/Cg2GzGDyaf15aR9St9TWlb+XvbZXWpDx8YKs7MLzMH/BCeopv+y9vzrzgkfykCGuWOlSu3mZhj2+FQcrg==
   dependencies:
     mkdirp "^1.0.4"
     rimraf "^3.0.2"
 
-"@sindresorhus/is@^0.14.0":
-  version "0.14.0"
-  resolved "https://registry.yarnpkg.com/@sindresorhus/is/-/is-0.14.0.tgz#9fb3a3cf3132328151f353de4632e01e52102bea"
-  integrity sha512-9NET910DNaIPngYnLLPeg+Ogzqsi9uM4mSboU5y6p8S5DzMTVEsJZrawi+BoDNUVBa2DhJqQYUFvMDfgU062LQ==
-
-"@szmarczak/http-timer@^1.1.2":
-  version "1.1.2"
-  resolved "https://registry.yarnpkg.com/@szmarczak/http-timer/-/http-timer-1.1.2.tgz#b1665e2c461a2cd92f4c1bbf50d5454de0d4b421"
-  integrity sha512-XIB2XbzHTN6ieIjfIMV9hlVcfPU26s2vafYWQcZHWXHOxiaRZYEDKEwdl129Zyg50+foYV2jCgtrqSA6qNuNSA==
-  dependencies:
-    defer-to-connect "^1.0.1"
-
 "@types/codemirror@0.0.87":
   version "0.0.87"
   resolved "https://registry.yarnpkg.com/@types/codemirror/-/codemirror-0.0.87.tgz#790b1ef751069074956abeeccd5b1f7fd821fddf"
   integrity sha512-Yv+cw1zckMDK35QJBMMK/z9ZWUHRUpQ2KJI+MCbR95HhDWtSQsS66j/W9OMq3JUqYL7Jb2zHA7fc575/0v1sfA==
   dependencies:
     "@types/tern" "*"
 
 "@types/dom4@^2.0.1":
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/@types/dom4/-/dom4-2.0.1.tgz#506d5781b9bcab81bd9a878b198aec7dee2a6033"
   integrity sha512-kSkVAvWmMZiCYtvqjqQEwOmvKwcH+V4uiv3qPQ8pAh1Xl39xggGEo8gHUqV4waYGHezdFw0rKBR8Jt0CrQSDZA==
 
-"@types/eslint-scope@^3.7.0":
-  version "3.7.0"
-  resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.0.tgz#4792816e31119ebd506902a482caec4951fabd86"
-  integrity sha512-O/ql2+rrCUe2W2rs7wMR+GqPRcgB6UiqN5RhrR5xruFlY7l9YLMn0ZkDzjoHLeiFkR8MCQZVudUuuvQ2BLC9Qw==
+"@types/eslint-scope@^3.7.3":
+  version "3.7.4"
+  resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
+  integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
   version "7.2.10"
   resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-7.2.10.tgz#4b7a9368d46c0f8cd5408c23288a59aa2394d917"
   integrity sha512-kUEPnMKrqbtpCq/KTaGFFKAcz6Ethm2EjCoKIDaCmfRBWLbFuTcOJfTlorwbnboXBzahqWLgUp1BQeKHiJzPUQ==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
-"@types/estree@*", "@types/estree@^0.0.47":
+"@types/estree@*":
   version "0.0.47"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-0.0.47.tgz#d7a51db20f0650efec24cd04994f523d93172ed4"
   integrity sha512-c5ciR06jK8u9BstrmJyO97m+klJrrhCf9u3rLu3DEAJBirxRqSCvDQoYKmxuYwQI5SZChAWu+tq9oVlGRuzPAg==
 
-"@types/glob@^7.1.1":
-  version "7.1.3"
-  resolved "https://registry.yarnpkg.com/@types/glob/-/glob-7.1.3.tgz#e6ba80f36b7daad2c685acd9266382e68985c183"
-  integrity sha512-SEYeGAIQIQX8NN6LDKprLjbrd5dARM5EXsd8GI/A5l0apYI1fGMWgPHSe4ZKL4eozlAyI+doUE9XbYS4xCkQ1w==
-  dependencies:
-    "@types/minimatch" "*"
-    "@types/node" "*"
+"@types/estree@^0.0.51":
+  version "0.0.51"
+  resolved "https://registry.yarnpkg.com/@types/estree/-/estree-0.0.51.tgz#cfd70924a25a3fd32b218e5e420e6897e1ac4f40"
+  integrity sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==
 
 "@types/json-schema@*", "@types/json-schema@^7.0.3", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.6":
   version "7.0.7"
   resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.7.tgz#98a993516c859eb0d5c4c8f098317a9ea68db9ad"
   integrity sha512-cxWFQVseBm6O9Gbw1IWb8r6OS4OhSt3hPZLkFApLjM8TEXROBuQGLAH2i2gZpcXdLBIrpXuTDhH7Vbm1iXmNGA==
 
-"@types/minimatch@*":
-  version "3.0.4"
-  resolved "https://registry.yarnpkg.com/@types/minimatch/-/minimatch-3.0.4.tgz#f0ec25dbf2f0e4b18647313ac031134ca5b24b21"
-  integrity sha512-1z8k4wzFnNjVK/tlxvrWuK5WMt6mydWWP7+zvH5eFep4oj+UkrfiJTRtjCeBXNpwaA/FYqqtb4/QS4ianFpIRA==
+"@types/json-schema@^7.0.8":
+  version "7.0.11"
+  resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.11.tgz#d421b6c527a3037f7c84433fd2c4229e016863d3"
+  integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
 "@types/node@*":
   version "15.3.0"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-15.3.0.tgz#d6fed7d6bc6854306da3dea1af9f874b00783e26"
   integrity sha512-8/bnjSZD86ZfpBsDlCIkNXIvm+h6wi9g7IqL+kmFkQ+Wvu3JrasgLElfiPgoo8V8vVfnEi0QVS12gbl94h9YsQ==
 
 "@types/prop-types@*":
@@ -883,21 +1007,35 @@
     csstype "^3.0.2"
 
 "@types/scheduler@*":
   version "0.16.1"
   resolved "https://registry.yarnpkg.com/@types/scheduler/-/scheduler-0.16.1.tgz#18845205e86ff0038517aab7a18a62a6b9f71275"
   integrity sha512-EaCxbanVeyxDRTQBkdLb3Bvl/HK7PBK6UJjsSixB0iHKoWxE5uu2Q/DgtpOhPIojN0Zl1whvOd7PoHs2P0s5eA==
 
+"@types/source-list-map@*":
+  version "0.1.2"
+  resolved "https://registry.yarnpkg.com/@types/source-list-map/-/source-list-map-0.1.2.tgz#0078836063ffaf17412349bba364087e0ac02ec9"
+  integrity sha512-K5K+yml8LTo9bWJI/rECfIPrGgxdpeNbj+d53lwN4QjW1MCwlkhUms+gtdzigTeUyBr09+u8BwOIY3MXvHdcsA==
+
 "@types/tern@*":
   version "0.23.3"
   resolved "https://registry.yarnpkg.com/@types/tern/-/tern-0.23.3.tgz#4b54538f04a88c9ff79de1f6f94f575a7f339460"
   integrity sha512-imDtS4TAoTcXk0g7u4kkWqedB3E4qpjXzCpD2LU5M5NAXHzCDsypyvXSaG7mM8DKYkCRa7tFp4tS/lp/Wo7Q3w==
   dependencies:
     "@types/estree" "*"
 
+"@types/webpack-sources@^0.1.5":
+  version "0.1.9"
+  resolved "https://registry.yarnpkg.com/@types/webpack-sources/-/webpack-sources-0.1.9.tgz#da69b06eb34f6432e6658acb5a6893c55d983920"
+  integrity sha512-bvzMnzqoK16PQIC8AYHNdW45eREJQMd6WG/msQWX5V2+vZmODCOPb4TJcbgRljTZZTwTM4wUMcsI8FftNA7new==
+  dependencies:
+    "@types/node" "*"
+    "@types/source-list-map" "*"
+    source-map "^0.6.1"
+
 "@typescript-eslint/eslint-plugin@^4.8.1":
   version "4.24.0"
   resolved "https://registry.yarnpkg.com/@typescript-eslint/eslint-plugin/-/eslint-plugin-4.24.0.tgz#03801ffc25b2af9d08f3dc9bccfc0b7ce3780d0f"
   integrity sha512-qbCgkPM7DWTsYQGjx9RTuQGswi+bEt0isqDBeo+CKV0953zqI0Tp7CZ7Fi9ipgFA6mcQqF4NOVNwS/f2r6xShw==
   dependencies:
     "@typescript-eslint/experimental-utils" "4.24.0"
     "@typescript-eslint/scope-manager" "4.24.0"
@@ -960,133 +1098,133 @@
   version "4.24.0"
   resolved "https://registry.yarnpkg.com/@typescript-eslint/visitor-keys/-/visitor-keys-4.24.0.tgz#a8fafdc76cad4e04a681a945fbbac4e35e98e297"
   integrity sha512-4ox1sjmGHIxjEDBnMCtWFFhErXtKA1Ec0sBpuz0fqf3P+g3JFGyTxxbF06byw0FRsPnnbq44cKivH7Ks1/0s6g==
   dependencies:
     "@typescript-eslint/types" "4.24.0"
     eslint-visitor-keys "^2.0.0"
 
-"@webassemblyjs/ast@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.0.tgz#a5aa679efdc9e51707a4207139da57920555961f"
-  integrity sha512-kX2W49LWsbthrmIRMbQZuQDhGtjyqXfEmmHyEi4XWnSZtPmxY0+3anPIzsnRb45VH/J55zlOfWvZuY47aJZTJg==
-  dependencies:
-    "@webassemblyjs/helper-numbers" "1.11.0"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.0"
-
-"@webassemblyjs/floating-point-hex-parser@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.0.tgz#34d62052f453cd43101d72eab4966a022587947c"
-  integrity sha512-Q/aVYs/VnPDVYvsCBL/gSgwmfjeCb4LW8+TMrO3cSzJImgv8lxxEPM2JA5jMrivE7LSz3V+PFqtMbls3m1exDA==
-
-"@webassemblyjs/helper-api-error@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.0.tgz#aaea8fb3b923f4aaa9b512ff541b013ffb68d2d4"
-  integrity sha512-baT/va95eXiXb2QflSx95QGT5ClzWpGaa8L7JnJbgzoYeaA27FCvuBXU758l+KXWRndEmUXjP0Q5fibhavIn8w==
-
-"@webassemblyjs/helper-buffer@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.0.tgz#d026c25d175e388a7dbda9694e91e743cbe9b642"
-  integrity sha512-u9HPBEl4DS+vA8qLQdEQ6N/eJQ7gT7aNvMIo8AAWvAl/xMrcOSiI2M0MAnMCy3jIFke7bEee/JwdX1nUpCtdyA==
-
-"@webassemblyjs/helper-numbers@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.0.tgz#7ab04172d54e312cc6ea4286d7d9fa27c88cd4f9"
-  integrity sha512-DhRQKelIj01s5IgdsOJMKLppI+4zpmcMQ3XboFPLwCpSNH6Hqo1ritgHgD0nqHeSYqofA6aBN/NmXuGjM1jEfQ==
+"@webassemblyjs/ast@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.11.1.tgz#2bfd767eae1a6996f432ff7e8d7fc75679c0b6a7"
+  integrity sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==
+  dependencies:
+    "@webassemblyjs/helper-numbers" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+
+"@webassemblyjs/floating-point-hex-parser@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz#f6c61a705f0fd7a6aecaa4e8198f23d9dc179e4f"
+  integrity sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==
+
+"@webassemblyjs/helper-api-error@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz#1a63192d8788e5c012800ba6a7a46c705288fd16"
+  integrity sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==
+
+"@webassemblyjs/helper-buffer@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz#832a900eb444884cde9a7cad467f81500f5e5ab5"
+  integrity sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==
+
+"@webassemblyjs/helper-numbers@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz#64d81da219fbbba1e3bd1bfc74f6e8c4e10a62ae"
+  integrity sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==
   dependencies:
-    "@webassemblyjs/floating-point-hex-parser" "1.11.0"
-    "@webassemblyjs/helper-api-error" "1.11.0"
+    "@webassemblyjs/floating-point-hex-parser" "1.11.1"
+    "@webassemblyjs/helper-api-error" "1.11.1"
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/helper-wasm-bytecode@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.0.tgz#85fdcda4129902fe86f81abf7e7236953ec5a4e1"
-  integrity sha512-MbmhvxXExm542tWREgSFnOVo07fDpsBJg3sIl6fSp9xuu75eGz5lz31q7wTLffwL3Za7XNRCMZy210+tnsUSEA==
-
-"@webassemblyjs/helper-wasm-section@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.0.tgz#9ce2cc89300262509c801b4af113d1ca25c1a75b"
-  integrity sha512-3Eb88hcbfY/FCukrg6i3EH8H2UsD7x8Vy47iVJrP967A9JGqgBVL9aH71SETPx1JrGsOUVLo0c7vMCN22ytJew==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/helper-buffer" "1.11.0"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.0"
-    "@webassemblyjs/wasm-gen" "1.11.0"
-
-"@webassemblyjs/ieee754@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.0.tgz#46975d583f9828f5d094ac210e219441c4e6f5cf"
-  integrity sha512-KXzOqpcYQwAfeQ6WbF6HXo+0udBNmw0iXDmEK5sFlmQdmND+tr773Ti8/5T/M6Tl/413ArSJErATd8In3B+WBA==
+"@webassemblyjs/helper-wasm-bytecode@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz#f328241e41e7b199d0b20c18e88429c4433295e1"
+  integrity sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==
+
+"@webassemblyjs/helper-wasm-section@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz#21ee065a7b635f319e738f0dd73bfbda281c097a"
+  integrity sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+
+"@webassemblyjs/ieee754@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz#963929e9bbd05709e7e12243a099180812992614"
+  integrity sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==
   dependencies:
     "@xtuc/ieee754" "^1.2.0"
 
-"@webassemblyjs/leb128@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.0.tgz#f7353de1df38aa201cba9fb88b43f41f75ff403b"
-  integrity sha512-aqbsHa1mSQAbeeNcl38un6qVY++hh8OpCOzxhixSYgbRfNWcxJNJQwe2rezK9XEcssJbbWIkblaJRwGMS9zp+g==
+"@webassemblyjs/leb128@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.1.tgz#ce814b45574e93d76bae1fb2644ab9cdd9527aa5"
+  integrity sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==
   dependencies:
     "@xtuc/long" "4.2.2"
 
-"@webassemblyjs/utf8@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.0.tgz#86e48f959cf49e0e5091f069a709b862f5a2cadf"
-  integrity sha512-A/lclGxH6SpSLSyFowMzO/+aDEPU4hvEiooCMXQPcQFPPJaYcPQNKGOCLUySJsYJ4trbpr+Fs08n4jelkVTGVw==
-
-"@webassemblyjs/wasm-edit@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.0.tgz#ee4a5c9f677046a210542ae63897094c2027cb78"
-  integrity sha512-JHQ0damXy0G6J9ucyKVXO2j08JVJ2ntkdJlq1UTiUrIgfGMmA7Ik5VdC/L8hBK46kVJgujkBIoMtT8yVr+yVOQ==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/helper-buffer" "1.11.0"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.0"
-    "@webassemblyjs/helper-wasm-section" "1.11.0"
-    "@webassemblyjs/wasm-gen" "1.11.0"
-    "@webassemblyjs/wasm-opt" "1.11.0"
-    "@webassemblyjs/wasm-parser" "1.11.0"
-    "@webassemblyjs/wast-printer" "1.11.0"
-
-"@webassemblyjs/wasm-gen@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.0.tgz#3cdb35e70082d42a35166988dda64f24ceb97abe"
-  integrity sha512-BEUv1aj0WptCZ9kIS30th5ILASUnAPEvE3tVMTrItnZRT9tXCLW2LEXT8ezLw59rqPP9klh9LPmpU+WmRQmCPQ==
+"@webassemblyjs/utf8@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.1.tgz#d1f8b764369e7c6e6bae350e854dec9a59f0a3ff"
+  integrity sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==
+
+"@webassemblyjs/wasm-edit@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz#ad206ebf4bf95a058ce9880a8c092c5dec8193d6"
+  integrity sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/helper-wasm-section" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+    "@webassemblyjs/wasm-opt" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
+    "@webassemblyjs/wast-printer" "1.11.1"
+
+"@webassemblyjs/wasm-gen@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz#86c5ea304849759b7d88c47a32f4f039ae3c8f76"
+  integrity sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/ieee754" "1.11.1"
+    "@webassemblyjs/leb128" "1.11.1"
+    "@webassemblyjs/utf8" "1.11.1"
+
+"@webassemblyjs/wasm-opt@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz#657b4c2202f4cf3b345f8a4c6461c8c2418985f2"
+  integrity sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-buffer" "1.11.1"
+    "@webassemblyjs/wasm-gen" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
+
+"@webassemblyjs/wasm-parser@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz#86ca734534f417e9bd3c67c7a1c75d8be41fb199"
+  integrity sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==
+  dependencies:
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/helper-api-error" "1.11.1"
+    "@webassemblyjs/helper-wasm-bytecode" "1.11.1"
+    "@webassemblyjs/ieee754" "1.11.1"
+    "@webassemblyjs/leb128" "1.11.1"
+    "@webassemblyjs/utf8" "1.11.1"
+
+"@webassemblyjs/wast-printer@1.11.1":
+  version "1.11.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz#d0c73beda8eec5426f10ae8ef55cee5e7084c2f0"
+  integrity sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==
   dependencies:
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.0"
-    "@webassemblyjs/ieee754" "1.11.0"
-    "@webassemblyjs/leb128" "1.11.0"
-    "@webassemblyjs/utf8" "1.11.0"
-
-"@webassemblyjs/wasm-opt@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.0.tgz#1638ae188137f4bb031f568a413cd24d32f92978"
-  integrity sha512-tHUSP5F4ywyh3hZ0+fDQuWxKx3mJiPeFufg+9gwTpYp324mPCQgnuVKwzLTZVqj0duRDovnPaZqDwoyhIO8kYg==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/helper-buffer" "1.11.0"
-    "@webassemblyjs/wasm-gen" "1.11.0"
-    "@webassemblyjs/wasm-parser" "1.11.0"
-
-"@webassemblyjs/wasm-parser@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.0.tgz#3e680b8830d5b13d1ec86cc42f38f3d4a7700754"
-  integrity sha512-6L285Sgu9gphrcpDXINvm0M9BskznnzJTE7gYkjDbxET28shDqp27wpruyx3C2S/dvEwiigBwLA1cz7lNUi0kw==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/helper-api-error" "1.11.0"
-    "@webassemblyjs/helper-wasm-bytecode" "1.11.0"
-    "@webassemblyjs/ieee754" "1.11.0"
-    "@webassemblyjs/leb128" "1.11.0"
-    "@webassemblyjs/utf8" "1.11.0"
-
-"@webassemblyjs/wast-printer@1.11.0":
-  version "1.11.0"
-  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.0.tgz#680d1f6a5365d6d401974a8e949e05474e1fab7e"
-  integrity sha512-Fg5OX46pRdTgB7rKIUojkh9vXaVN6sGYCnEiJN1GYkb0RPwShZXp6KTDqmoMdQPKhcroOXh3fEzmkWmCYaKYhQ==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.0"
+    "@webassemblyjs/ast" "1.11.1"
     "@xtuc/long" "4.2.2"
 
 "@webpack-cli/configtest@^1.0.3":
   version "1.0.3"
   resolved "https://registry.yarnpkg.com/@webpack-cli/configtest/-/configtest-1.0.3.tgz#204bcff87cda3ea4810881f7ea96e5f5321b87b9"
   integrity sha512-WQs0ep98FXX2XBAfQpRbY0Ma6ADw8JR6xoIkaIiJIzClGOMqVRvPCWqndTxf28DgFopWan0EKtHtg/5W1h0Zkw==
 
@@ -1108,33 +1246,43 @@
   integrity sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==
 
 "@xtuc/long@4.2.2":
   version "4.2.2"
   resolved "https://registry.yarnpkg.com/@xtuc/long/-/long-4.2.2.tgz#d291c6a4e97989b5c61d9acf396ae4fe133a718d"
   integrity sha512-NuHqBY1PB/D8xU6s/thBgOAiAP7HOYDQ32+BFZILJ8ivkUkAHQnWfn6WhL79Owj1qmUnoN/YPhktdIoucipkAQ==
 
-"@yarnpkg/lockfile@^1.1.0":
-  version "1.1.0"
-  resolved "https://registry.yarnpkg.com/@yarnpkg/lockfile/-/lockfile-1.1.0.tgz#e77a97fbd345b76d83245edcd17d393b1b41fb31"
-  integrity sha512-GpSwvyXOcOOlV70vbnzjj4fW5xW/FdUF6nQEt1ENy7m4ZCczi1+/buVUPAqmGfqznsORNFzUMjctTIp8a9tuCQ==
+abab@^2.0.3:
+  version "2.0.6"
+  resolved "https://registry.yarnpkg.com/abab/-/abab-2.0.6.tgz#41b80f2c871d19686216b82309231cfd3cb3d291"
+  integrity sha512-j2afSsaIENvHZN2B8GOpF566vZ5WVk5opAiMTvWgaQT8DkbOqsTfvNAvHoRGU2zzP8cPoqys+xHTRDWW8L+/BA==
+
+acorn-import-assertions@^1.7.6:
+  version "1.8.0"
+  resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz#ba2b5939ce62c238db6d93d81c9b111b29b855e9"
+  integrity sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==
 
 acorn-jsx@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/acorn-jsx/-/acorn-jsx-5.3.1.tgz#fc8661e11b7ac1539c47dbfea2e72b3af34d267b"
   integrity sha512-K0Ptm/47OKfQRpNQ2J/oIN/3QYiK6FwW+eJbILhsdxh2WTLdl+30o8aGdTbm5JbffpFFAg/g+zi1E+jvJha5ng==
 
 acorn@^7.4.0:
   version "7.4.1"
   resolved "https://registry.yarnpkg.com/acorn/-/acorn-7.4.1.tgz#feaed255973d2e77555b83dbc08851a6c63520fa"
   integrity sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==
 
-acorn@^8.2.1:
-  version "8.2.4"
-  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.2.4.tgz#caba24b08185c3b56e3168e97d15ed17f4d31fd0"
-  integrity sha512-Ibt84YwBDDA890eDiDCEqcbwvHlBvzzDkU2cGBBDDI1QWT12jTiXIOn2CIw5KK4i6N5Z2HUxwYjzriDyqaqqZg==
+acorn@^8.5.0:
+  version "8.7.1"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.7.1.tgz#0197122c843d1bf6d0a5e83220a788f278f63c30"
+  integrity sha512-Xx54uLJQZ19lKygFXOWsscKUbsBZW0CPykPhVQdhIeIwrbPmJzqeASDInc8nKBnp/JT6igTs82qPXz069H8I/A==
+
+acorn@^8.7.1:
+  version "8.8.2"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.2.tgz#1b2f25db02af965399b9776b0c2c391276d37c4a"
+  integrity sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==
 
 aggregate-error@^3.0.0:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/aggregate-error/-/aggregate-error-3.1.0.tgz#92670ff50f5359bdb7a3e0d40d0ec30c5737687a"
   integrity sha512-4I7Td01quW/RpocfNayFdFVk1qSuoh0E7JrbRJ16nH01HhKFQ88INq9Sd+nd72zqRySlr9BmDA8xlEJ6vJMrYA==
   dependencies:
     clean-stack "^2.0.0"
@@ -1166,21 +1314,14 @@
     uri-js "^4.2.2"
 
 ansi-colors@^4.1.1:
   version "4.1.1"
   resolved "https://registry.yarnpkg.com/ansi-colors/-/ansi-colors-4.1.1.tgz#cbb9ae256bf750af1eab344f229aa27fe94ba348"
   integrity sha512-JoX0apGbHaUJBNl6yF+p6JAFYZ666/hhCGKN5t9QFjbJQKUU/g8MNbFDbvfrgKXvI1QpZplPOnwIo99lX/AAmA==
 
-ansi-escapes@^4.2.1:
-  version "4.3.2"
-  resolved "https://registry.yarnpkg.com/ansi-escapes/-/ansi-escapes-4.3.2.tgz#6b2291d1db7d98b6521d5f1efa42d0f3a9feb65e"
-  integrity sha512-gKXj5ALrKWQLsYG9jlTRmR/xKluxHV+Z9QEwNIgCfM1/uwPMCuzVVnh5mwTd+OuBZcwSIMbqssNWRm1lE51QaQ==
-  dependencies:
-    type-fest "^0.21.3"
-
 ansi-regex@^5.0.0:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/ansi-regex/-/ansi-regex-5.0.1.tgz#082cb2c89c9fe8659a311a53bd6a4dc5301db304"
   integrity sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==
 
 ansi-styles@^3.2.1:
   version "3.2.1"
@@ -1256,17 +1397,17 @@
     caniuse-lite "^1.0.30001219"
     colorette "^1.2.2"
     electron-to-chromium "^1.3.723"
     escalade "^3.1.1"
     node-releases "^1.1.71"
 
 buffer-from@^1.0.0:
-  version "1.1.1"
-  resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.1.tgz#32713bc028f75c02fdb710d7c7bcec1f2c6070ef"
-  integrity sha512-MQcXEUbCKtEo7bhqEs6560Hyd4XaovZlO/k9V3hjVUF/zwW7KBVdSK4gIt/bzwS9MbR5qob+F5jusZsb0YQK2A==
+  version "1.1.2"
+  resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
+  integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
 buffer@^5.6.0:
   version "5.7.1"
   resolved "https://registry.yarnpkg.com/buffer/-/buffer-5.7.1.tgz#ba62e7c13133053582197160851a8f648e99eed0"
   integrity sha512-EHcyIPBQ4BSGlvjB16k5KgAJ27CIsHY/2JBmCRReo48y9rQ3MaUzWX3KVlBa4U7MyX02HdVj0K7C3WaB3ju7FQ==
   dependencies:
     base64-js "^1.3.1"
@@ -1291,27 +1432,14 @@
     p-map "^4.0.0"
     promise-inflight "^1.0.1"
     rimraf "^3.0.2"
     ssri "^8.0.1"
     tar "^6.0.2"
     unique-filename "^1.1.1"
 
-cacheable-request@^6.0.0:
-  version "6.1.0"
-  resolved "https://registry.yarnpkg.com/cacheable-request/-/cacheable-request-6.1.0.tgz#20ffb8bd162ba4be11e9567d823db651052ca912"
-  integrity sha512-Oj3cAGPCqOZX7Rz64Uny2GYAZNliQSqfbePrgAQ1wKAihYmCUnraBtJtKcGR4xz7wF+LoJC+ssFZvv5BgF9Igg==
-  dependencies:
-    clone-response "^1.0.2"
-    get-stream "^5.1.0"
-    http-cache-semantics "^4.0.0"
-    keyv "^3.0.0"
-    lowercase-keys "^2.0.0"
-    normalize-url "^4.1.0"
-    responselike "^1.0.2"
-
 call-bind@^1.0.0, call-bind@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/call-bind/-/call-bind-1.0.2.tgz#b1d4e89e688119c3c9a903ad30abb2f6a919be3c"
   integrity sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==
   dependencies:
     function-bind "^1.1.1"
     get-intrinsic "^1.0.2"
@@ -1336,32 +1464,22 @@
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
     escape-string-regexp "^1.0.5"
     supports-color "^5.3.0"
 
-chalk@^4.0.0, chalk@^4.1.0:
+chalk@^4.0.0:
   version "4.1.1"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-4.1.1.tgz#c80b3fab28bf6371e6863325eee67e618b77e6ad"
   integrity sha512-diHzdDKxcU+bAsUboHLPEDQiw0qEe0qd7SYUn3HgcFlWgbDcfLGswOHYeGrHKzG9z6UYf01d9VFMfZxPM1xZSg==
   dependencies:
     ansi-styles "^4.1.0"
     supports-color "^7.1.0"
 
-chardet@^0.7.0:
-  version "0.7.0"
-  resolved "https://registry.yarnpkg.com/chardet/-/chardet-0.7.0.tgz#90094849f0937f2eedc2425d0d28a9e5f0cbad9e"
-  integrity sha512-mT8iDcrh03qDGRRmoA2hmBJnxpllMR+0/0qlzjqZES6NdiWDcZkCNAk4rPFZ9Q85r27unkiNNg8ZOiwZXBHwcA==
-
-child_process@~1.0.2:
-  version "1.0.2"
-  resolved "https://registry.yarnpkg.com/child_process/-/child_process-1.0.2.tgz#b1f7e7fc73d25e7fd1d455adc94e143830182b5a"
-  integrity sha1-sffn/HPSXn/R1FWtyU4UODAYK1o=
-
 chownr@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/chownr/-/chownr-2.0.0.tgz#15bfbe53d2eab4cf70f18a8cd68ebe5b3cb1dece"
   integrity sha512-bIomtDF5KGpdogkLd9VspvFzk9KfpyyGlS8YFVZl7TGPBHL5snIOnxeshwVgPteQ9b4Eydl+pVbIyE1DcvCWgQ==
 
 chrome-trace-event@^1.0.2:
   version "1.0.3"
@@ -1374,42 +1492,23 @@
   integrity sha512-OlQdbZ7gLfGarSqxesMesDa5uz7KFbID8Kpq/SxIoNGDqY8lSYs0D+hhtBXhcdB3rcbXArFr7vlHheLk1voeNA==
 
 clean-stack@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/clean-stack/-/clean-stack-2.2.0.tgz#ee8472dbb129e727b31e8a10a427dee9dfe4008b"
   integrity sha512-4diC9HaTE+KRAMWhDhrGOECgWZxoevMc5TlkObMqNSsVU62PYzXZ/SMTjzyGAFF1YusgxGcSWTEXBhp0CPwQ1A==
 
-cli-cursor@^3.1.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/cli-cursor/-/cli-cursor-3.1.0.tgz#264305a7ae490d1d03bf0c9ba7c925d1753af307"
-  integrity sha512-I/zHAwsKf9FqGoXM4WWRACob9+SNukZTd94DWF57E4toouRulbCxcUh6RKUEOQlYTHJnzkPMySvPNaaSLNfLZw==
-  dependencies:
-    restore-cursor "^3.1.0"
-
-cli-width@^3.0.0:
-  version "3.0.0"
-  resolved "https://registry.yarnpkg.com/cli-width/-/cli-width-3.0.0.tgz#a2f48437a2caa9a22436e794bf071ec9e61cedf6"
-  integrity sha512-FxqpkPPwu1HjuN93Omfm4h8uIanXofW0RxVEW3k5RKx+mJJYSthzNhp32Kzxxy3YAEZ/Dc/EWN1vZRY0+kOhbw==
-
 clone-deep@^4.0.1:
   version "4.0.1"
   resolved "https://registry.yarnpkg.com/clone-deep/-/clone-deep-4.0.1.tgz#c19fd9bdbbf85942b4fd979c84dcf7d5f07c2387"
   integrity sha512-neHB9xuzh/wk0dIHweyAXv2aPGZIVk3pLMe+/RNzINf17fe0OG96QroktYAUm7SM1PBnzTabaLboqqxDyMU+SQ==
   dependencies:
     is-plain-object "^2.0.4"
     kind-of "^6.0.2"
     shallow-clone "^3.0.0"
 
-clone-response@^1.0.2:
-  version "1.0.2"
-  resolved "https://registry.yarnpkg.com/clone-response/-/clone-response-1.0.2.tgz#d1dc973920314df67fbeb94223b4ee350239e96b"
-  integrity sha1-0dyXOSAxTfZ/vrlCI7TuNQI56Ws=
-  dependencies:
-    mimic-response "^1.0.0"
-
 codemirror@~5.58.0:
   version "5.58.3"
   resolved "https://registry.yarnpkg.com/codemirror/-/codemirror-5.58.3.tgz#3f0689854ecfbed5d4479a98b96148b2c3b79796"
   integrity sha512-KBhB+juiyOOgn0AqtRmWyAT3yoElkuvWTI6hsHa9E6GQrl6bk/fdAYcvuqW1/upO9T9rtEtapWdw4XYcNiVDEA==
 
 color-convert@^1.9.0:
   version "1.9.3"
@@ -1459,15 +1558,15 @@
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/commondir/-/commondir-1.0.1.tgz#ddd800da0c66127393cca5950ea968a3aaf1253b"
   integrity sha1-3dgA2gxmEnOTzKWVDqloo6rxJTs=
 
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
-  integrity sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=
+  integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
 cross-spawn@^6.0.5:
   version "6.0.5"
   resolved "https://registry.yarnpkg.com/cross-spawn/-/cross-spawn-6.0.5.tgz#4a5ec7c64dfae22c3a14124dbacdee846d80cbc4"
   integrity sha512-eTVLrBSt7fjbDygz805pMnstIs2VTBNkRm0qxZd+M7A5XDdxVRWO5MxGBXZhjY4cqLYLdtrGqRf8mBPmzwSpWQ==
   dependencies:
     nice-try "^1.0.4"
@@ -1481,19 +1580,14 @@
   resolved "https://registry.yarnpkg.com/cross-spawn/-/cross-spawn-7.0.3.tgz#f73a85b9d5d41d045551c177e2882d4ac85728a6"
   integrity sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==
   dependencies:
     path-key "^3.1.0"
     shebang-command "^2.0.0"
     which "^2.0.1"
 
-crypto@~1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/crypto/-/crypto-1.0.1.tgz#2af1b7cad8175d24c8a1b0778255794a21803037"
-  integrity sha512-VxBKmeNcqQdiUQUW2Tzq0t377b54N2bMtXO/qiLa+6eRRmmC4qT3D4OnTGoT/U6O9aklQ/jTwbOtRMTTY8G0Ig==
-
 css-loader@^5.0.1:
   version "5.2.4"
   resolved "https://registry.yarnpkg.com/css-loader/-/css-loader-5.2.4.tgz#e985dcbce339812cb6104ef3670f08f9893a1536"
   integrity sha512-OFYGyINCKkdQsTrSYxzGSFnGS4gNjcXkKkQgWxK138jgnPt+lepxdjSZNc8sHAl5vP3DhsJUxufWIjOwI8PMMw==
   dependencies:
     camelcase "^6.2.0"
     icss-utils "^5.1.0"
@@ -1518,82 +1612,59 @@
   integrity sha512-xz39Sb4+OaTsULgUERcCk+TJj8ylkL4aSVDQiX/ksxbELSqwkgt4d4RD7fovIdgJGSuNYqwZEiVjYY5l0ask+Q==
 
 csstype@^3.0.2, csstype@~3.0.3:
   version "3.0.8"
   resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.0.8.tgz#d2266a792729fb227cd216fb572f43728e1ad340"
   integrity sha512-jXKhWqXPmlUeoQnF/EhTtTl4C9SnrxSH/jZUih3jmO6lBKr99rP3/+FmrMj4EFpOXzMtXHAZkd3x0E6h6Fgflw==
 
+data-urls@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.yarnpkg.com/data-urls/-/data-urls-2.0.0.tgz#156485a72963a970f5d5821aaf642bef2bf2db9b"
+  integrity sha512-X5eWTSXO/BJmpdIKCRuKUgSCgAN0OwliVK3yPKbwIWU1Tdw5BRajxlzMidvh+gwko9AfQ9zIj52pzF91Q3YAvQ==
+  dependencies:
+    abab "^2.0.3"
+    whatwg-mimetype "^2.3.0"
+    whatwg-url "^8.0.0"
+
 debug@^4.0.1, debug@^4.1.1:
   version "4.3.1"
   resolved "https://registry.yarnpkg.com/debug/-/debug-4.3.1.tgz#f0d229c505e0c6d8c49ac553d1b13dc183f6b2ee"
   integrity sha512-doEwdvm4PCeK4K3RQN2ZC2BYUBaxwLARCqZmMjtF8a51J2Rb0xpVloFRnCODwqjpwnAoao4pelN8l3RJdv3gRQ==
   dependencies:
     ms "2.1.2"
 
-decompress-response@^3.3.0:
-  version "3.3.0"
-  resolved "https://registry.yarnpkg.com/decompress-response/-/decompress-response-3.3.0.tgz#80a4dd323748384bfa248083622aedec982adff3"
-  integrity sha1-gKTdMjdIOEv6JICDYirt7Jgq3/M=
-  dependencies:
-    mimic-response "^1.0.0"
-
 deep-equal@^1.1.1:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/deep-equal/-/deep-equal-1.1.1.tgz#b5c98c942ceffaf7cb051e24e1434a25a2e6076a"
   integrity sha512-yd9c5AdiqVcR+JjcwUQb9DkhJc8ngNr0MahEBGvDiJw8puWab2yZlh+nkasOnZP+EGTAP6rRp2JzJhJZzvNF8g==
   dependencies:
     is-arguments "^1.0.4"
     is-date-object "^1.0.1"
     is-regex "^1.0.4"
     object-is "^1.0.1"
     object-keys "^1.1.1"
     regexp.prototype.flags "^1.2.0"
 
-deep-extend@^0.6.0:
-  version "0.6.0"
-  resolved "https://registry.yarnpkg.com/deep-extend/-/deep-extend-0.6.0.tgz#c4fa7c95404a17a9c3e8ca7e1537312b736330ac"
-  integrity sha512-LOHxIOaPYdHlJRtCQfDIVZtfw/ufM8+rVj649RIHzcm/vGwQRXFt6OPqIFWsm2XEMrNIEtWR64sY1LEKD2vAOA==
-
 deep-is@^0.1.3:
   version "0.1.3"
   resolved "https://registry.yarnpkg.com/deep-is/-/deep-is-0.1.3.tgz#b369d6fb5dbc13eecf524f91b070feedc357cf34"
   integrity sha1-s2nW+128E+7PUk+RsHD+7cNXzzQ=
 
 deepmerge@^4.2.2:
   version "4.2.2"
   resolved "https://registry.yarnpkg.com/deepmerge/-/deepmerge-4.2.2.tgz#44d2ea3679b8f4d4ffba33f03d865fc1e7bf4955"
   integrity sha512-FJ3UgI4gIl+PHZm53knsuSFpE+nESMr7M4v9QcgB7S63Kj/6WqMiFQJpBBYz1Pt+66bZpP3Q7Lye0Oo9MPKEdg==
 
-defer-to-connect@^1.0.1:
-  version "1.1.3"
-  resolved "https://registry.yarnpkg.com/defer-to-connect/-/defer-to-connect-1.1.3.tgz#331ae050c08dcf789f8c83a7b81f0ed94f4ac591"
-  integrity sha512-0ISdNousHvZT2EiFlZeZAHBUvSxmKswVCEf8hW7KWgG4a8MVEu/3Vb6uWYozkjylyCxe0JBIiRB1jV45S70WVQ==
-
 define-properties@^1.1.3:
   version "1.1.3"
   resolved "https://registry.yarnpkg.com/define-properties/-/define-properties-1.1.3.tgz#cf88da6cbee26fe6db7094f61d870cbd84cee9f1"
   integrity sha512-3MqfYKj2lLzdMSf8ZIZE/V+Zuy+BgD6f164e8K2w7dgnpKArBDerGYpM46IYYcjnkdPNMjPk9A6VFB8+3SKlXQ==
   dependencies:
     object-keys "^1.0.12"
 
-dependency-graph@^0.9.0:
-  version "0.9.0"
-  resolved "https://registry.yarnpkg.com/dependency-graph/-/dependency-graph-0.9.0.tgz#11aed7e203bc8b00f48356d92db27b265c445318"
-  integrity sha512-9YLIBURXj4DJMFALxXw9K3Y3rwb5Fk0X5/8ipCzaN84+gKxoHK43tVKRNakCQbiEx07E8Uwhuq21BpUagFhZ8w==
-
-detect-indent@^6.0.0:
-  version "6.0.0"
-  resolved "https://registry.yarnpkg.com/detect-indent/-/detect-indent-6.0.0.tgz#0abd0f549f69fc6659a254fe96786186b6f528fd"
-  integrity sha512-oSyFlqaTHCItVRGK5RmrmjB+CmaMOW7IaNA/kdxqhoa6d17j/5ce9O9eWXmV/KEdRwqpQA+Vqe8a8Bsybu4YnA==
-
-detect-newline@3.1.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/detect-newline/-/detect-newline-3.1.0.tgz#576f5dfc63ae1a192ff192d8ad3af6308991b651"
-  integrity sha512-TLz+x/vEXm/Y7P7wn1EJFNLxYpUD4TgMosxY6fAVJUnJMbupHBOncxyWUG9OpTaH9EBD7uFI5LfEgmMOc54DsA==
-
 dir-glob@^3.0.1:
   version "3.0.1"
   resolved "https://registry.yarnpkg.com/dir-glob/-/dir-glob-3.0.1.tgz#56dbf73d992a4a93ba1584f4534063fd2e41717f"
   integrity sha512-WkrWp9GR4KXfKGYzOLmTuGVi1UWFfws377n9cc55/tb6DuqyF6pcQ5AbiHEshaDpY9v6oaSr2XCDidGmMwdzIA==
   dependencies:
     path-type "^4.0.0"
 
@@ -1642,19 +1713,14 @@
   resolved "https://registry.yarnpkg.com/domutils/-/domutils-2.6.0.tgz#2e15c04185d43fb16ae7057cb76433c6edb938b7"
   integrity sha512-y0BezHuy4MDYxh6OvolXYsH+1EMGmFbwv5FKW7ovwMG6zTPWqNPq3WF9ayZssFq+UlKdffGLbOEaghNdaOm1WA==
   dependencies:
     dom-serializer "^1.0.1"
     domelementtype "^2.2.0"
     domhandler "^4.2.0"
 
-duplexer3@^0.1.4:
-  version "0.1.4"
-  resolved "https://registry.yarnpkg.com/duplexer3/-/duplexer3-0.1.4.tgz#ee01dd1cac0ed3cbc7fdbea37dc0a8f1ce002ce2"
-  integrity sha1-7gHdHKwO08vH/b6jfcCo8c4ALOI=
-
 duplicate-package-checker-webpack-plugin@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/duplicate-package-checker-webpack-plugin/-/duplicate-package-checker-webpack-plugin-3.0.0.tgz#78bb89e625fa7cf8c2a59c53f62b495fda9ba287"
   integrity sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
@@ -1672,25 +1738,18 @@
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/emojis-list/-/emojis-list-3.0.0.tgz#5570662046ad29e2e916e71aae260abdff4f6a78"
   integrity sha512-/kyM18EfinwXZbno9FyUGeFh87KC8HRQBQGildHZbEuRyWFOmv1U10o9BBp8XVZDVNNuQKyIGIu5ZYAAXJ0V2Q==
 
-end-of-stream@^1.1.0:
-  version "1.4.4"
-  resolved "https://registry.yarnpkg.com/end-of-stream/-/end-of-stream-1.4.4.tgz#5ae64a5f45057baf3626ec14da0ca5e4b2431eb0"
-  integrity sha512-+uw1inIHVPQoaVuHzRyXd21icM+cnt4CzD5rW+NC1wjOUSTOs+Te7FOv7AhN7vS9x/oIyhLP5PR1H+phQAHu5Q==
-  dependencies:
-    once "^1.4.0"
-
-enhanced-resolve@^5.8.0:
-  version "5.8.2"
-  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.8.2.tgz#15ddc779345cbb73e97c611cd00c01c1e7bf4d8b"
-  integrity sha512-F27oB3WuHDzvR2DOGNTaYy0D5o0cnrv8TeI482VM4kYgQd/FT9lUQwuNsJ0oOHtBUq7eiW5ytqzp7nBFknL+GA==
+enhanced-resolve@^5.10.0:
+  version "5.12.0"
+  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz#300e1c90228f5b570c4d35babf263f6da7155634"
+  integrity sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 enquirer@^2.3.5:
   version "2.3.6"
   resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.3.6.tgz#2a7fe5dd634a1e4125a975ec994ff5456dc3734d"
@@ -1733,18 +1792,18 @@
     object-inspect "^1.9.0"
     object-keys "^1.1.1"
     object.assign "^4.1.2"
     string.prototype.trimend "^1.0.4"
     string.prototype.trimstart "^1.0.4"
     unbox-primitive "^1.0.0"
 
-es-module-lexer@^0.4.0:
-  version "0.4.1"
-  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-0.4.1.tgz#dda8c6a14d8f340a24e34331e0fab0cb50438e0e"
-  integrity sha512-ooYciCUtfw6/d2w56UVeqHPcoCFAiJdz5XOkYpv/Txl1HMUozpXjz/2RIQgqwKdXNDPSF1W7mJCFse3G+HDyAA==
+es-module-lexer@^0.9.0:
+  version "0.9.3"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-0.9.3.tgz#6f13db00cc38417137daf74366f535c8eb438f19"
+  integrity sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==
 
 es-to-primitive@^1.2.1:
   version "1.2.1"
   resolved "https://registry.yarnpkg.com/es-to-primitive/-/es-to-primitive-1.2.1.tgz#e55cd4c9cdc188bcefb03b366c736323fc5c898a"
   integrity sha512-QCOllgZJtaUo9miYBcLChTUaHNjJF3PYs1VidD7AwiEj1kYxKeQTctLAezAOH5ZKRH0g2IgPn6KwB4IT8iRpvA==
   dependencies:
     is-callable "^1.1.4"
@@ -1776,15 +1835,15 @@
 eslint-plugin-prettier@^3.1.4:
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/eslint-plugin-prettier/-/eslint-plugin-prettier-3.4.0.tgz#cdbad3bf1dbd2b177e9825737fe63b476a08f0c7"
   integrity sha512-UDK6rJT6INSfcOo545jiaOwB701uAIt2/dR7WnFQoGCVl1/EMqdANBmwUaqqQ45aXprsTGzSa39LI1PyuRBxxw==
   dependencies:
     prettier-linter-helpers "^1.0.0"
 
-eslint-scope@^5.0.0, eslint-scope@^5.1.1:
+eslint-scope@5.1.1, eslint-scope@^5.0.0, eslint-scope@^5.1.1:
   version "5.1.1"
   resolved "https://registry.yarnpkg.com/eslint-scope/-/eslint-scope-5.1.1.tgz#e786e59a66cb92b3f6c1fb0d508aab174848f48c"
   integrity sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==
   dependencies:
     esrecurse "^4.3.0"
     estraverse "^4.1.1"
 
@@ -1907,34 +1966,25 @@
     is-stream "^2.0.0"
     merge-stream "^2.0.0"
     npm-run-path "^4.0.1"
     onetime "^5.1.2"
     signal-exit "^3.0.3"
     strip-final-newline "^2.0.0"
 
-external-editor@^3.0.3:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/external-editor/-/external-editor-3.1.0.tgz#cb03f740befae03ea4d283caed2741a83f335495"
-  integrity sha512-hMQ4CX1p1izmuLYyZqLMO/qGNw10wSv9QDCPfzXfyFrOaCSSoRfqE1Kf1s5an66J5JZC62NewG+mK49jOCtQew==
-  dependencies:
-    chardet "^0.7.0"
-    iconv-lite "^0.4.24"
-    tmp "^0.0.33"
-
 fast-deep-equal@^3.1.1:
   version "3.1.3"
   resolved "https://registry.yarnpkg.com/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz#3a7d56b559d6cbc3eb512325244e619a65c6c525"
   integrity sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==
 
 fast-diff@^1.1.2:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/fast-diff/-/fast-diff-1.2.0.tgz#73ee11982d86caaf7959828d519cfe927fac5f03"
   integrity sha512-xJuoT5+L99XlZ8twedaRf6Ax2TgQVxvgZOYoPKqZufmJib0tL2tegPBOZb1pVNgIhlqDlA0eO0c3wBvQcmzx4w==
 
-fast-glob@^3.0.3, fast-glob@^3.1.1:
+fast-glob@^3.1.1:
   version "3.2.5"
   resolved "https://registry.yarnpkg.com/fast-glob/-/fast-glob-3.2.5.tgz#7939af2a656de79a4f1901903ee8adcaa7cb9661"
   integrity sha512-2DtFcgT68wiTTiwZ2hNdJfcHNke9XOfnwmBRWXhmeKM8rF0TGwmC/Qto3S7RoZKp5cilZbxzO5iTNTQsJ+EeDg==
   dependencies:
     "@nodelib/fs.stat" "^2.0.2"
     "@nodelib/fs.walk" "^1.2.3"
     glob-parent "^5.1.0"
@@ -1960,21 +2010,14 @@
 fastq@^1.6.0:
   version "1.11.0"
   resolved "https://registry.yarnpkg.com/fastq/-/fastq-1.11.0.tgz#bb9fb955a07130a918eb63c1f5161cc32a5d0858"
   integrity sha512-7Eczs8gIPDrVzT+EksYBcupqMyxSHXXrHOLRRxU2/DicV8789MRBRR8+Hc2uWzUupOs4YS4JzBmBxjjCVBxD/g==
   dependencies:
     reusify "^1.0.4"
 
-figures@^3.0.0:
-  version "3.2.0"
-  resolved "https://registry.yarnpkg.com/figures/-/figures-3.2.0.tgz#625c18bd293c604dc4a8ddb2febf0c88341746af"
-  integrity sha512-yaduQFRKLXYOGgEn6AZau90j3ggSOyiqXU0F9JZfeXYhNa+Jk4X+s45A2zg5jns87GAFa34BBm2kXw4XpNcbdg==
-  dependencies:
-    escape-string-regexp "^1.0.5"
-
 file-entry-cache@^6.0.1:
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/file-entry-cache/-/file-entry-cache-6.0.1.tgz#211b2dd9659cb0394b073e7323ac3c933d522027"
   integrity sha512-7Gps/XWymbLk2QLYK4NzpMOrYjMhdIxXuIvy2QBsLE6ljuodKvdkWs/cpyJJ3CVIVpH0Oi1Hvg1ovbMzLdFBBg==
   dependencies:
     flat-cache "^3.0.4"
 
@@ -2075,38 +2118,19 @@
     has-symbols "^1.0.1"
 
 get-stdin@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/get-stdin/-/get-stdin-6.0.0.tgz#9e09bf712b360ab9225e812048f71fde9c89657b"
   integrity sha512-jp4tHawyV7+fkkSKyvjuLZswblUtz+SQKzSWnBbii16BuZksJlU1wuBYXY75r+duh/llF1ur6oNwi+2ZzjKZ7g==
 
-get-stream@^4.1.0:
-  version "4.1.0"
-  resolved "https://registry.yarnpkg.com/get-stream/-/get-stream-4.1.0.tgz#c1b255575f3dc21d59bfc79cd3d2b46b1c3a54b5"
-  integrity sha512-GMat4EJ5161kIy2HevLlr4luNjBgvmj413KaQA7jt4V8B4RDsfpHk7WQ9GVqfYyyx8OS/L66Kox+rJRNklLK7w==
-  dependencies:
-    pump "^3.0.0"
-
-get-stream@^5.1.0:
-  version "5.2.0"
-  resolved "https://registry.yarnpkg.com/get-stream/-/get-stream-5.2.0.tgz#4966a1795ee5ace65e706c4b7beb71257d6e22d3"
-  integrity sha512-nBF+F1rAZVCu/p7rjzgA+Yb4lfYXrpl7a6VmJrU8wF9I1CKvP/QwPNZHnOlwbTkY6dvtFIzFMSyQXbLoTQPRpA==
-  dependencies:
-    pump "^3.0.0"
-
 get-stream@^6.0.0:
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/get-stream/-/get-stream-6.0.1.tgz#a262d8eef67aced57c2852ad6167526a43cbf7b7"
   integrity sha512-ts6Wi+2j3jQjqi70w5AlN8DFnkSwC+MqmxEzdEALB2qXZYV3X/b1CTfgPLGJNMeAWxdPfU8FO1ms3NUfaHCPYg==
 
-git-hooks-list@1.0.3:
-  version "1.0.3"
-  resolved "https://registry.yarnpkg.com/git-hooks-list/-/git-hooks-list-1.0.3.tgz#be5baaf78203ce342f2f844a9d2b03dba1b45156"
-  integrity sha512-Y7wLWcrLUXwk2noSka166byGCvhMtDRpgHdzCno1UQv/n/Hegp++a2xBWJL1lJarnKD3SWaljD+0z1ztqxuKyQ==
-
 glob-parent@^5.0.0, glob-parent@^5.1.0:
   version "5.1.2"
   resolved "https://registry.yarnpkg.com/glob-parent/-/glob-parent-5.1.2.tgz#869832c58034fe68a4093c17dc15e8340d8401c4"
   integrity sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==
   dependencies:
     is-glob "^4.0.1"
 
@@ -2137,62 +2161,36 @@
 globals@^13.6.0:
   version "13.8.0"
   resolved "https://registry.yarnpkg.com/globals/-/globals-13.8.0.tgz#3e20f504810ce87a8d72e55aecf8435b50f4c1b3"
   integrity sha512-rHtdA6+PDBIjeEvA91rpqzEvk/k3/i7EeNQiryiWuJH0Hw9cpyJMAt2jtbAwUaRdhD+573X4vWw6IcjKPasi9Q==
   dependencies:
     type-fest "^0.20.2"
 
-globby@10.0.0:
-  version "10.0.0"
-  resolved "https://registry.yarnpkg.com/globby/-/globby-10.0.0.tgz#abfcd0630037ae174a88590132c2f6804e291072"
-  integrity sha512-3LifW9M4joGZasyYPz2A1U74zbC/45fvpXUvO/9KbSa+VV0aGZarWkfdgKyR9sExNP0t0x0ss/UMJpNpcaTspw==
-  dependencies:
-    "@types/glob" "^7.1.1"
-    array-union "^2.1.0"
-    dir-glob "^3.0.1"
-    fast-glob "^3.0.3"
-    glob "^7.1.3"
-    ignore "^5.1.1"
-    merge2 "^1.2.3"
-    slash "^3.0.0"
-
 globby@^11.0.1:
   version "11.0.3"
   resolved "https://registry.yarnpkg.com/globby/-/globby-11.0.3.tgz#9b1f0cb523e171dd1ad8c7b2a9fb4b644b9593cb"
   integrity sha512-ffdmosjA807y7+lA1NM0jELARVmYul/715xiILEjo3hBLPTcirgQNnXECn5g3mtR8TOLCVbkfua1Hpen25/Xcg==
   dependencies:
     array-union "^2.1.0"
     dir-glob "^3.0.1"
     fast-glob "^3.1.1"
     ignore "^5.1.4"
     merge2 "^1.3.0"
     slash "^3.0.0"
 
-got@^9.6.0:
-  version "9.6.0"
-  resolved "https://registry.yarnpkg.com/got/-/got-9.6.0.tgz#edf45e7d67f99545705de1f7bbeeeb121765ed85"
-  integrity sha512-R7eWptXuGYxwijs0eV+v3o6+XH1IqVK8dJOEecQfTmkncw9AV4dcw/Dhxi8MdlqPthxxpZyizMzyg8RTmEsG+Q==
-  dependencies:
-    "@sindresorhus/is" "^0.14.0"
-    "@szmarczak/http-timer" "^1.1.2"
-    cacheable-request "^6.0.0"
-    decompress-response "^3.3.0"
-    duplexer3 "^0.1.4"
-    get-stream "^4.1.0"
-    lowercase-keys "^1.0.1"
-    mimic-response "^1.0.1"
-    p-cancelable "^1.0.0"
-    to-readable-stream "^1.0.0"
-    url-parse-lax "^3.0.0"
-
 graceful-fs@^4.1.2, graceful-fs@^4.1.6, graceful-fs@^4.2.0, graceful-fs@^4.2.4:
   version "4.2.6"
   resolved "https://registry.yarnpkg.com/graceful-fs/-/graceful-fs-4.2.6.tgz#ff040b2b0853b23c3d31027523706f1885d76bee"
   integrity sha512-nTnJ528pbqxYanhpDYsi4Rd8MAeaBA67+RZ10CM1m3bTAVFEDcd5AuA4a6W5YkGZ1iNXHzZz8T6TBKLeBuNriQ==
 
+graceful-fs@^4.2.9:
+  version "4.2.10"
+  resolved "https://registry.yarnpkg.com/graceful-fs/-/graceful-fs-4.2.10.tgz#147d3a006da4ca3ce14728c7aefc287c367d7a6c"
+  integrity sha512-9ByhssR2fPVsNZj478qUUbKfmL0+t5BDVyjShtyZZLiK7ZDAArFFfopyOTj0M05wE2tJPisA4iTnnXl2YoPvOA==
+
 gud@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/gud/-/gud-1.0.0.tgz#a489581b17e6a70beca9abe3ae57de7a499852c0"
   integrity sha512-zGEOVKFM5sVPPrYs7J5/hYEw2Pof8KCyOwyhG8sAF26mCAeUFAcYPu1mwB7hhpIP29zOIBaDqwuHdLp0jvZXjw==
 
 has-bigints@^1.0.1:
   version "1.0.1"
@@ -2232,30 +2230,25 @@
   integrity sha512-gyyPk6rgonLFEDGoeRgQNaEUvdJ4ktTmmUh/h2t7s+M8oPpIPxgNACWa+6ESR57kXstwqPiCut0V8NRpcwgU7A==
   dependencies:
     domelementtype "^2.0.1"
     domhandler "^4.0.0"
     domutils "^2.5.2"
     entities "^2.0.0"
 
-http-cache-semantics@^4.0.0:
-  version "4.1.0"
-  resolved "https://registry.yarnpkg.com/http-cache-semantics/-/http-cache-semantics-4.1.0.tgz#49e91c5cbf36c9b94bcfcd71c23d5249ec74e390"
-  integrity sha512-carPklcUh7ROWRK7Cv27RPtdhYhUsela/ue5/jKzjegVvXDqM2ILE9Q2BGn9JZJh1g87cp56su/FgQSzcWS8cQ==
-
 human-signals@^2.1.0:
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/human-signals/-/human-signals-2.1.0.tgz#dc91fcba42e4d06e4abaed33b3e7a3c02f514ea0"
   integrity sha512-B4FFZ6q/T2jhhksgkbEW3HBvWIfDW85snkQgawt07S7J5QXTk6BkNV+0yAeZrM5QpMAdYlocGoljn0sJ/WQkFw==
 
-iconv-lite@^0.4.24:
-  version "0.4.24"
-  resolved "https://registry.yarnpkg.com/iconv-lite/-/iconv-lite-0.4.24.tgz#2022b4b25fbddc21d2f524974a474aafe733908b"
-  integrity sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==
+iconv-lite@^0.6.2:
+  version "0.6.3"
+  resolved "https://registry.yarnpkg.com/iconv-lite/-/iconv-lite-0.6.3.tgz#a52f80bf38da1952eb5c681790719871a1a72501"
+  integrity sha512-4fCk79wshMdzMp2rH06qWrJE4iolqLhCUH+OiuIgU++RB0+94NlDL81atO7GX55uUKueo0txHNtvEyI6D7WdMw==
   dependencies:
-    safer-buffer ">= 2.1.2 < 3"
+    safer-buffer ">= 2.1.2 < 3.0.0"
 
 icss-utils@^5.0.0, icss-utils@^5.1.0:
   version "5.1.0"
   resolved "https://registry.yarnpkg.com/icss-utils/-/icss-utils-5.1.0.tgz#c6be6858abd013d768e98366ae47e25d5887b1ae"
   integrity sha512-soFhflCVWLfRNOPU3iv5Z9VUdT44xFRbzjLsEzSr5AQmgqPMTHdU3PMT1Cf1ssx8fLNJDA1juftYl+PUcv3MqA==
 
 ieee754@^1.1.13:
@@ -2264,15 +2257,15 @@
   integrity sha512-dcyqhDvX1C46lXZcVqCpK+FtMRQVdIMN6/Df5js2zouUsqG7I6sFxitIC+7KYK29KdXOLHdu9zL4sFnoVQnqaA==
 
 ignore@^4.0.6:
   version "4.0.6"
   resolved "https://registry.yarnpkg.com/ignore/-/ignore-4.0.6.tgz#750e3db5862087b4737ebac8207ffd1ef27b25fc"
   integrity sha512-cyFDKrqc/YdcWFniJhzI42+AzS+gNwmUzOSFcRCQYwySuBBBy/KjuxWLZ/FHEH6Moq1NizMOBWyTcv8O4OZIMg==
 
-ignore@^5.1.1, ignore@^5.1.4:
+ignore@^5.1.4:
   version "5.1.8"
   resolved "https://registry.yarnpkg.com/ignore/-/ignore-5.1.8.tgz#f150a8b50a34289b33e22f5889abd4d8016f0e57"
   integrity sha512-BMpfD7PpiETpBl/A6S498BaIJ6Y/ABT93ETbby2fP00v4EbvPBXWEoaR1UBPKs3iR53pJY7EtZk5KACI57i1Uw==
 
 import-fresh@^3.0.0, import-fresh@^3.2.1:
   version "3.3.0"
   resolved "https://registry.yarnpkg.com/import-fresh/-/import-fresh-3.3.0.tgz#37162c25fcb9ebaa2e6e53d5b4d88ce17d9e0c2b"
@@ -2313,38 +2306,14 @@
     wrappy "1"
 
 inherits@2:
   version "2.0.4"
   resolved "https://registry.yarnpkg.com/inherits/-/inherits-2.0.4.tgz#0fa2c64f932917c3433a0ded55363aae37416b7c"
   integrity sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==
 
-ini@~1.3.0:
-  version "1.3.8"
-  resolved "https://registry.yarnpkg.com/ini/-/ini-1.3.8.tgz#a29da425b48806f34767a4efce397269af28432c"
-  integrity sha512-JV/yugV2uzW5iMRSiZAyDtQd+nxtUnjeLt0acNdw98kKLrvuRVyB80tsREOE7yvGVgalhZ6RNXCmEHkUKBKxew==
-
-inquirer@^7.0.0:
-  version "7.3.3"
-  resolved "https://registry.yarnpkg.com/inquirer/-/inquirer-7.3.3.tgz#04d176b2af04afc157a83fd7c100e98ee0aad003"
-  integrity sha512-JG3eIAj5V9CwcGvuOmoo6LB9kbAYT8HXffUl6memuszlwDC/qvFAJw49XJ5NROSFNPxp3iQg1GqkFhaY/CR0IA==
-  dependencies:
-    ansi-escapes "^4.2.1"
-    chalk "^4.1.0"
-    cli-cursor "^3.1.0"
-    cli-width "^3.0.0"
-    external-editor "^3.0.3"
-    figures "^3.0.0"
-    lodash "^4.17.19"
-    mute-stream "0.0.8"
-    run-async "^2.4.0"
-    rxjs "^6.6.0"
-    string-width "^4.1.0"
-    strip-ansi "^6.0.0"
-    through "^2.3.6"
-
 interpret@^2.2.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/interpret/-/interpret-2.2.0.tgz#1a78a0b5965c40a5416d007ad6f50ad27c417df9"
   integrity sha512-Ju0Bz/cEia55xDwUWEa8+olFpCiQoypjnQySseKtmjNrnps3P+xfpUmGr90T7yjlVJmOtybRvPXhKMbHr+fWnw==
 
 is-arguments@^1.0.4:
   version "1.1.0"
@@ -2415,19 +2384,14 @@
   integrity sha512-RU0lI/n95pMoUKu9v1BZP5MBcZuNSVJkMkAG2dJqC4z2GlkGUNeH68SuHuBKBD/XFe+LHZ+f9BKkLET60Niedw==
 
 is-number@^7.0.0:
   version "7.0.0"
   resolved "https://registry.yarnpkg.com/is-number/-/is-number-7.0.0.tgz#7535345b896734d5f80c4d06c50955527a14f12b"
   integrity sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==
 
-is-plain-obj@2.1.0:
-  version "2.1.0"
-  resolved "https://registry.yarnpkg.com/is-plain-obj/-/is-plain-obj-2.1.0.tgz#45e42e37fccf1f40da8e5f76ee21515840c09287"
-  integrity sha512-YWnfyRwxL/+SsrWYfOpUtz5b3YD+nyfkHvjbcanzk8zgyO4ASD67uVMRt8k5bM4lLMDnXfriRhOpemw+NfT1eA==
-
 is-plain-object@^2.0.4:
   version "2.0.4"
   resolved "https://registry.yarnpkg.com/is-plain-object/-/is-plain-object-2.0.4.tgz#2c163b3fafb1b606d9d17928f05c2a1c38e07677"
   integrity sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==
   dependencies:
     isobject "^3.0.1"
 
@@ -2467,46 +2431,55 @@
   integrity sha1-6PvzdNxVb/iUehDcsFctYz8s+hA=
 
 isobject@^3.0.1:
   version "3.0.1"
   resolved "https://registry.yarnpkg.com/isobject/-/isobject-3.0.1.tgz#4e431e92b11a9731636aa1f9c8d1ccbcfdab78df"
   integrity sha1-TkMekrEalzFjaqH5yNHMvP2reN8=
 
-jest-worker@^26.5.0, jest-worker@^26.6.2:
+jest-worker@^26.5.0:
   version "26.6.2"
   resolved "https://registry.yarnpkg.com/jest-worker/-/jest-worker-26.6.2.tgz#7f72cbc4d643c365e27b9fd775f9d0eaa9c7a8ed"
   integrity sha512-KWYVV1c4i+jbMpaBC+U++4Va0cp8OisU185o73T1vo99hqi7w8tSJfUXYswwqqrjzwxa6KpRK54WhPvwf5w6PQ==
   dependencies:
     "@types/node" "*"
     merge-stream "^2.0.0"
     supports-color "^7.0.0"
 
+jest-worker@^27.4.5:
+  version "27.5.1"
+  resolved "https://registry.yarnpkg.com/jest-worker/-/jest-worker-27.5.1.tgz#8d146f0900e8973b106b6f73cc1e9a8cb86f8db0"
+  integrity sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==
+  dependencies:
+    "@types/node" "*"
+    merge-stream "^2.0.0"
+    supports-color "^8.0.0"
+
 "js-tokens@^3.0.0 || ^4.0.0", js-tokens@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/js-tokens/-/js-tokens-4.0.0.tgz#19203fb59991df98e3a287050d4647cdeaf32499"
   integrity sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==
 
 js-yaml@^3.13.1:
   version "3.14.1"
   resolved "https://registry.yarnpkg.com/js-yaml/-/js-yaml-3.14.1.tgz#dae812fdb3825fa306609a8717383c50c36a0537"
   integrity sha512-okMH7OXXJ7YrN9Ok3/SXrnu4iX9yOk+25nqX4imS2npuvTYDmo/QEZoqwZkYaIDk3jVvBOTOIEgEhaLOynBS9g==
   dependencies:
     argparse "^1.0.7"
     esprima "^4.0.0"
 
-json-buffer@3.0.0:
-  version "3.0.0"
-  resolved "https://registry.yarnpkg.com/json-buffer/-/json-buffer-3.0.0.tgz#5b1f397afc75d677bde8bcfc0e47e1f9a3d9a898"
-  integrity sha1-Wx85evx11ne96Lz8Dkfh+aPZqJg=
-
-json-parse-better-errors@^1.0.1, json-parse-better-errors@^1.0.2:
+json-parse-better-errors@^1.0.1:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/json-parse-better-errors/-/json-parse-better-errors-1.0.2.tgz#bb867cfb3450e69107c131d1c514bab3dc8bcaa9"
   integrity sha512-mrqyZKfX5EhL7hvqcV6WG1yYjnjeuYDzDhhcAAUrq8Po85NBQBJP+ZDUT75qZQ98IkUoBqdkExkukOU7Ts2wrw==
 
+json-parse-even-better-errors@^2.3.1:
+  version "2.3.1"
+  resolved "https://registry.yarnpkg.com/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz#7c47805a94319928e05777405dc12e1f7a4ee02d"
+  integrity sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==
+
 json-schema-traverse@^0.4.1:
   version "0.4.1"
   resolved "https://registry.yarnpkg.com/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz#69f6a87d9513ab8bb8fe63bdb0979c448e684660"
   integrity sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==
 
 json-schema-traverse@^1.0.0:
   version "1.0.0"
@@ -2515,17 +2488,17 @@
 
 json-stable-stringify-without-jsonify@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/json-stable-stringify-without-jsonify/-/json-stable-stringify-without-jsonify-1.0.1.tgz#9db7b59496ad3f3cfef30a75142d2d930ad72651"
   integrity sha1-nbe1lJatPzz+8wp1FC0tkwrXJlE=
 
 json5@^1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.1.tgz#779fb0018604fa854eacbf6252180d83543e3dbe"
-  integrity sha512-aKS4WQjPenRxiQsC93MNfjx+nbF4PAdYzmd/1JIj8HYzqfbu86beTuNgXDzPknWk0n0uARlyewZo4s++ES36Ow==
+  version "1.0.2"
+  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.2.tgz#63d98d60f21b313b77c4d6da18bfa69d80e1d593"
+  integrity sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==
   dependencies:
     minimist "^1.2.0"
 
 json5@^2.1.1, json5@^2.1.2:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/json5/-/json5-2.2.0.tgz#2dfefe720c6ba525d9ebd909950f0515316c89a3"
   integrity sha512-f+8cldu7X/y7RAJurMEJmdoKXGB/X550w2Nr3tTbezL6RwEE/iMcm+tZnXeoZtKuOq6ft8+CqzEkrIgx1fPoQA==
@@ -2537,21 +2510,14 @@
   resolved "https://registry.yarnpkg.com/jsonfile/-/jsonfile-6.1.0.tgz#bc55b2634793c679ec6403094eb13698a6ec0aae"
   integrity sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==
   dependencies:
     universalify "^2.0.0"
   optionalDependencies:
     graceful-fs "^4.1.6"
 
-keyv@^3.0.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/keyv/-/keyv-3.1.0.tgz#ecc228486f69991e49e9476485a5be1e8fc5c4d9"
-  integrity sha512-9ykJ/46SN/9KPM/sichzQ7OvXyGDYKGTaDlKMGCAlg2UK8KRy4jb0d8sFc+0Tt0YYnThq8X2RZgCg74RPxgcVA==
-  dependencies:
-    json-buffer "3.0.0"
-
 kind-of@^6.0.2:
   version "6.0.3"
   resolved "https://registry.yarnpkg.com/kind-of/-/kind-of-6.0.3.tgz#07c05034a6c349fa06e24fa35aa76db4580ce4dd"
   integrity sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==
 
 klona@^2.0.3:
   version "2.0.4"
@@ -2562,14 +2528,22 @@
   version "0.4.1"
   resolved "https://registry.yarnpkg.com/levn/-/levn-0.4.1.tgz#ae4562c007473b932a6200d403268dd2fffc6ade"
   integrity sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==
   dependencies:
     prelude-ls "^1.2.1"
     type-check "~0.4.0"
 
+license-webpack-plugin@^2.3.14:
+  version "2.3.21"
+  resolved "https://registry.yarnpkg.com/license-webpack-plugin/-/license-webpack-plugin-2.3.21.tgz#152f5e82d5f51f8bab78905731f2b8042aa5691b"
+  integrity sha512-rVaYU9TddZN3ao8M/0PrRSCdTp2EW6VQymlgsuScld1vef0Ou7fALx3ePe83KLP3xAEDcPK5fkqUVqGBnbz1zQ==
+  dependencies:
+    "@types/webpack-sources" "^0.1.5"
+    webpack-sources "^1.2.0"
+
 load-json-file@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/load-json-file/-/load-json-file-4.0.0.tgz#2f5f45ab91e33216234fd53adab668eb4ec0993b"
   integrity sha1-L19Fq5HjMhYjT9U62rZo607AmTs=
   dependencies:
     graceful-fs "^4.1.2"
     parse-json "^4.0.0"
@@ -2578,17 +2552,17 @@
 
 loader-runner@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/loader-runner/-/loader-runner-4.2.0.tgz#d7022380d66d14c5fb1d496b89864ebcfd478384"
   integrity sha512-92+huvxMvYlMzMt0iIOukcwYBFpkYJdpl2xsZ7LrlayO7E8SOv+JJUEK17B/dJIHAOLMfh2dZZ/Y18WgmGtYNw==
 
 loader-utils@^1.0.0:
-  version "1.4.0"
-  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-1.4.0.tgz#c579b5e34cb34b1a74edc6c1fb36bfa371d5a613"
-  integrity sha512-qH0WSMBtn/oHuwjy/NucEgbx5dbxxnxup9s4PVXJUDHZBQY+s0NWA9rJf53RBnQZxfch7euUui7hpoAPvALZdA==
+  version "1.4.2"
+  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-1.4.2.tgz#29a957f3a63973883eb684f10ffd3d151fec01a3"
+  integrity sha512-I5d00Pd/jwMD2QCduo657+YM/6L3KZu++pmX9VFncxaxvHcru9jx1lBaFft+r4Mt2jK0Yhp41XlRAihzPxHNCg==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^1.0.1"
 
 loader-utils@^2.0.0, loader-utils@~2.0.0:
   version "2.0.0"
@@ -2617,36 +2591,26 @@
   integrity sha1-yQRGkMIeBClL6qUXcS/e0fqI3pg=
 
 lodash.truncate@^4.4.2:
   version "4.4.2"
   resolved "https://registry.yarnpkg.com/lodash.truncate/-/lodash.truncate-4.4.2.tgz#5a350da0b1113b837ecfffd5812cbe58d6eae193"
   integrity sha1-WjUNoLERO4N+z//VgSy+WNbq4ZM=
 
-lodash@^4.17.15, lodash@^4.17.19, lodash@^4.17.21, lodash@^4.17.4:
+lodash@^4.17.15, lodash@^4.17.21, lodash@^4.17.4, lodash@^4.7.0:
   version "4.17.21"
   resolved "https://registry.yarnpkg.com/lodash/-/lodash-4.17.21.tgz#679591c564c3bffaae8454cf0b3df370c3d6911c"
   integrity sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==
 
 loose-envify@^1.0.0, loose-envify@^1.1.0, loose-envify@^1.4.0:
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/loose-envify/-/loose-envify-1.4.0.tgz#71ee51fa7be4caec1a63839f7e682d8132d30caf"
   integrity sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==
   dependencies:
     js-tokens "^3.0.0 || ^4.0.0"
 
-lowercase-keys@^1.0.0, lowercase-keys@^1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/lowercase-keys/-/lowercase-keys-1.0.1.tgz#6f9e30b47084d971a7c820ff15a6c5167b74c26f"
-  integrity sha512-G2Lj61tXDnVFFOi8VZds+SoQjtQC3dgokKdDG2mTm1tx4m50NUHBOZSBwQQHyy0V12A0JTG4icfZQH+xPyh8VA==
-
-lowercase-keys@^2.0.0:
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/lowercase-keys/-/lowercase-keys-2.0.0.tgz#2603e78b7b4b0006cbca2fbcc8a3202558ac9479"
-  integrity sha512-tqNXrS78oMOE73NMxK4EMLQsQowWf8jKooH9g7xPavRT706R6bkQJ6DY2Te7QukaZsulxa30wQ7bk0pm4XiHmA==
-
 lru-cache@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/lru-cache/-/lru-cache-6.0.0.tgz#6d6fe6570ebd96aaf90fcad1dafa3b2566db3a94"
   integrity sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==
   dependencies:
     yallist "^4.0.0"
 
@@ -2668,15 +2632,15 @@
   integrity sha1-htcJCzDORV1j+64S3aUaR93K+bI=
 
 merge-stream@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/merge-stream/-/merge-stream-2.0.0.tgz#52823629a14dd00c9770fb6ad47dc6310f2c1f60"
   integrity sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==
 
-merge2@^1.2.3, merge2@^1.3.0:
+merge2@^1.3.0:
   version "1.4.1"
   resolved "https://registry.yarnpkg.com/merge2/-/merge2-1.4.1.tgz#4368892f885e907455a6fd7dc55c0c9d404990ae"
   integrity sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==
 
 micromatch@^4.0.2:
   version "4.0.4"
   resolved "https://registry.yarnpkg.com/micromatch/-/micromatch-4.0.4.tgz#896d519dfe9db25fce94ceb7a500919bf881ebf9"
@@ -2698,39 +2662,34 @@
     mime-db "1.47.0"
 
 mimic-fn@^2.1.0:
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/mimic-fn/-/mimic-fn-2.1.0.tgz#7ed2c2ccccaf84d3ffcb7a69b57711fc2083401b"
   integrity sha512-OqbOk5oEQeAZ8WXWydlu9HJjz9WVdEIvamMCcXmuqUYjTknH/sqsWvhQ3vgwKFRR1HpjvNBKQ37nbJgYzGqGcg==
 
-mimic-response@^1.0.0, mimic-response@^1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/mimic-response/-/mimic-response-1.0.1.tgz#4923538878eef42063cb8a3e3b0798781487ab1b"
-  integrity sha512-j5EctnkH7amfV/q5Hgmoal1g2QHFJRraOtmx0JpIqkxhBhI/lJSl1nMpQ45hVarwNETOoWEimndZ4QK0RHxuxQ==
-
 mini-css-extract-plugin@~1.3.2:
   version "1.3.9"
   resolved "https://registry.yarnpkg.com/mini-css-extract-plugin/-/mini-css-extract-plugin-1.3.9.tgz#47a32132b0fd97a119acd530e8421e8f6ab16d5e"
   integrity sha512-Ac4s+xhVbqlyhXS5J/Vh/QXUz3ycXlCqoCPpg0vdfhsIBH9eg/It/9L1r1XhSCH737M1lqcWnMuWL13zcygn5A==
   dependencies:
     loader-utils "^2.0.0"
     schema-utils "^3.0.0"
     webpack-sources "^1.1.0"
 
 minimatch@^3.0.4:
-  version "3.0.4"
-  resolved "https://registry.yarnpkg.com/minimatch/-/minimatch-3.0.4.tgz#5166e286457f03306064be5497e8dbb0c3d32083"
-  integrity sha512-yJHVQEhyqPLUTgt9B83PXu6W3rx4MvvHvSUvToogpwoGDOUQ+yDrR0HRot+yOCdCO7u4hX3pWft6kWBBcqh0UA==
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/minimatch/-/minimatch-3.1.2.tgz#19cd194bfd3e428f049a70817c038d89ab4be35b"
+  integrity sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==
   dependencies:
     brace-expansion "^1.1.7"
 
 minimist@^1.2.0, minimist@^1.2.5, minimist@~1.2.0:
-  version "1.2.5"
-  resolved "https://registry.yarnpkg.com/minimist/-/minimist-1.2.5.tgz#67d66014b66a6a8aaa0c083c5fd58df4e4e97602"
-  integrity sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==
+  version "1.2.7"
+  resolved "https://registry.yarnpkg.com/minimist/-/minimist-1.2.7.tgz#daa1c4d91f507390437c6a8bc01078e7000c4d18"
+  integrity sha512-bzfL1YUZsP41gmu/qjrEk0Q6i2ix/cVeAhbCbqH9u3zYutS1cLg00qhrD0M2MVdCcx4Sc0UpP2eBWo9rotpq6g==
 
 minipass-collect@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/minipass-collect/-/minipass-collect-1.0.2.tgz#22b813bf745dc6edba2576b940022ad6edc8c617"
   integrity sha512-6T6lH0H8OG9kITm/Jm6tdooIbogG9e0tLgpY6mphXSm/A9u8Nq1ryBG+Qspiub9LjWlBPsPS3tWQ/Botq4FdxA==
   dependencies:
     minipass "^3.0.0"
@@ -2766,32 +2725,27 @@
 
 mkdirp@^1.0.3, mkdirp@^1.0.4:
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/mkdirp/-/mkdirp-1.0.4.tgz#3eb5ed62622756d79a5f0e2a221dfebad75c2f7e"
   integrity sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==
 
 moment@^2.24.0:
-  version "2.29.1"
-  resolved "https://registry.yarnpkg.com/moment/-/moment-2.29.1.tgz#b2be769fa31940be9eeea6469c075e35006fa3d3"
-  integrity sha512-kHmoybcPV8Sqy59DwNDY3Jefr64lK/by/da0ViFcuA4DH0vQg5Q6Ze5VimxkfQNSC+Mls/Kx53s7TjP1RhFEDQ==
+  version "2.29.4"
+  resolved "https://registry.yarnpkg.com/moment/-/moment-2.29.4.tgz#3dbe052889fe7c1b2ed966fcb3a77328964ef108"
+  integrity sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==
 
 ms@2.1.2:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/ms/-/ms-2.1.2.tgz#d09d1f357b443f493382a8eb3ccd183872ae6009"
   integrity sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==
 
-mute-stream@0.0.8:
-  version "0.0.8"
-  resolved "https://registry.yarnpkg.com/mute-stream/-/mute-stream-0.0.8.tgz#1630c42b2251ff81e2a283de96a5497ea92e5e0d"
-  integrity sha512-nnbWWOkoWyUsTjKrhgD0dcz22mdkSnpYqbEjIm2nhwhuxlSkpywJmBo8h0ZqJdkp73mb90SssHkN4rsRaBAfAA==
-
 nanoid@^3.1.23:
-  version "3.1.23"
-  resolved "https://registry.yarnpkg.com/nanoid/-/nanoid-3.1.23.tgz#f744086ce7c2bc47ee0a8472574d5c78e4183a81"
-  integrity sha512-FiB0kzdP0FFVGDKlRLEQ1BgDzU87dy5NnzjeW9YZNt+/c3+q82EQDUwniSAUxp/F0gFNI1ZhKU1FqYsMuqZVnw==
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/nanoid/-/nanoid-3.2.0.tgz#62667522da6673971cca916a6d3eff3f415ff80c"
+  integrity sha512-fmsZYa9lpn69Ad5eDn7FMcnnSR+8R34W9qJEijxYhTbfOWzr22n1QxCMzXLK+ODyW2973V3Fux959iQoUxzUIA==
 
 natural-compare@^1.4.0:
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/natural-compare/-/natural-compare-1.4.0.tgz#4abebfeed7541f2c27acfb29bdbbd15c8d5ba4f7"
   integrity sha1-Sr6/7tdUHywnrPspvbvRXI1bpPc=
 
 neo-async@^2.6.2:
@@ -2801,17 +2755,19 @@
 
 nice-try@^1.0.4:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/nice-try/-/nice-try-1.0.5.tgz#a3378a7696ce7d223e88fc9b764bd7ef1089e366"
   integrity sha512-1nh45deeb5olNY7eX82BkPO7SSxR5SSYJiPTrTdFUVYwAl8CKMA5N9PjTYkHiRjisVcxcQ1HXdLhx2qxxJzLNQ==
 
 node-fetch@^2.6.0:
-  version "2.6.1"
-  resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.1.tgz#045bd323631f76ed2e2b55573394416b639a0052"
-  integrity sha512-V4aYg89jEoVRxRb2fJdAg8FHvI7cEyYdVAh94HH0UIK8oJxUfkjlDQN9RbMx+bEjP7+ggMiFRprSti032Oipxw==
+  version "2.6.7"
+  resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.7.tgz#24de9fba827e3b4ae44dc8b20256a379160052ad"
+  integrity sha512-ZjMPFEfVx5j+y2yF35Kzx5sF7kDzxuDj6ziH4FFbOp87zKDZNx8yExJIb05OGF4Nlt9IHFIMBkRl41VdvcNdbQ==
+  dependencies:
+    whatwg-url "^5.0.0"
 
 node-releases@^1.1.71:
   version "1.1.72"
   resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-1.1.72.tgz#14802ab6b1039a79a0c7d662b610a5bbd76eacbe"
   integrity sha512-LLUo+PpH3dU6XizX3iVoubUNheF/owjXCZZ5yACDxNnPtgFuludV1ZL3ayK1kVep42Rmm0+R9/Y60NQbZ2bifw==
 
 normalize-package-data@^2.3.2:
@@ -2820,19 +2776,14 @@
   integrity sha512-/5CMN3T0R4XTj4DcGaexo+roZSdSFW/0AOOTROrjxzCG1wrWXEsGbRKevjlIL+ZDE4sZlJr5ED4YW0yqmkK+eA==
   dependencies:
     hosted-git-info "^2.1.4"
     resolve "^1.10.0"
     semver "2 || 3 || 4 || 5"
     validate-npm-package-license "^3.0.1"
 
-normalize-url@^4.1.0:
-  version "4.5.1"
-  resolved "https://registry.yarnpkg.com/normalize-url/-/normalize-url-4.5.1.tgz#0dd90cf1288ee1d1313b87081c9a5932ee48518a"
-  integrity sha512-9UZCFRHQdNrfTpGg8+1INIg93B6zE0aXMVFkw1WFwvO4SlZywU6aLg5Of0Ap/PgcbSw4LNxvMWXMeugwMCX0AA==
-
 normalize.css@^8.0.1:
   version "8.0.1"
   resolved "https://registry.yarnpkg.com/normalize.css/-/normalize.css-8.0.1.tgz#9b98a208738b9cc2634caacbc42d131c97487bf3"
   integrity sha512-qizSNPO93t1YUuUhP22btGOo3chcvDFqFaj2TRybP0DMxkHOCTYwp3n34fel4a31ORXy4m1Xq0Gyqpb5m33qIg==
 
 npm-run-all@^4.1.5:
   version "4.1.5"
@@ -2885,22 +2836,22 @@
   integrity sha512-ixT2L5THXsApyiUPYKmW+2EHpXXe5Ii3M+f4e+aJFAHao5amFRW6J0OO6c/LU8Be47utCx2GL89hxGB6XSmKuQ==
   dependencies:
     call-bind "^1.0.0"
     define-properties "^1.1.3"
     has-symbols "^1.0.1"
     object-keys "^1.1.1"
 
-once@^1.3.0, once@^1.3.1, once@^1.4.0:
+once@^1.3.0:
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/once/-/once-1.4.0.tgz#583b1aa775961d4b113ac17d9c50baef9dd76bd1"
   integrity sha1-WDsap3WWHUsROsF9nFC6753Xa9E=
   dependencies:
     wrappy "1"
 
-onetime@^5.1.0, onetime@^5.1.2:
+onetime@^5.1.2:
   version "5.1.2"
   resolved "https://registry.yarnpkg.com/onetime/-/onetime-5.1.2.tgz#d0e96ebb56b07476df1dd9c4806e5237985ca45e"
   integrity sha512-kbpaSSGJTWdAY5KPVeMOKXSrPtr8C8C7wodJbcsd51jRnmD+GZu8Y0VoU6Dm5Z4vWr0Ig/1NKuWRKf7j5aaYSg==
   dependencies:
     mimic-fn "^2.1.0"
 
 optionator@^0.9.1:
@@ -2911,32 +2862,22 @@
     deep-is "^0.1.3"
     fast-levenshtein "^2.0.6"
     levn "^0.4.1"
     prelude-ls "^1.2.1"
     type-check "^0.4.0"
     word-wrap "^1.2.3"
 
-os-tmpdir@~1.0.2:
-  version "1.0.2"
-  resolved "https://registry.yarnpkg.com/os-tmpdir/-/os-tmpdir-1.0.2.tgz#bbe67406c79aa85c5cfec766fe5734555dfa1274"
-  integrity sha1-u+Z0BseaqFxc/sdm/lc0VV36EnQ=
-
-p-cancelable@^1.0.0:
-  version "1.1.0"
-  resolved "https://registry.yarnpkg.com/p-cancelable/-/p-cancelable-1.1.0.tgz#d078d15a3af409220c886f1d9a0ca2e441ab26cc"
-  integrity sha512-s73XxOZ4zpt1edZYZzvhqFa6uvQc1vwUa0K0BdtIZgQMAJj9IbebH+JkgKZc9h+B05PKHLOTl4ajG1BmNrVZlw==
-
 p-limit@^2.2.0:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/p-limit/-/p-limit-2.3.0.tgz#3dd33c647a214fdfffd835933eb086da0dc21db1"
   integrity sha512-//88mFWSJx8lxCzwdAABTJL2MyWB12+eIY7MDL2SqLmAkeKU9qxRvWuSyTjm3FUmpBEMuFfckAIqEaVGUDxb6w==
   dependencies:
     p-try "^2.0.0"
 
-p-limit@^3.0.2, p-limit@^3.1.0:
+p-limit@^3.0.2:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/p-limit/-/p-limit-3.1.0.tgz#e1daccbe78d0d1388ca18c64fea38e3e57e3706b"
   integrity sha512-TYOanM3wGwNGsZN2cVTYPArw454xnXj5qmWF1bEoAc4+cU/ol7GVh7odevjp1FNHduHc3KZMcFduxU5Xc6uJRQ==
   dependencies:
     yocto-queue "^0.1.0"
 
 p-locate@^4.1.0:
@@ -2954,24 +2895,14 @@
     aggregate-error "^3.0.0"
 
 p-try@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/p-try/-/p-try-2.2.0.tgz#cb2868540e313d61de58fafbe35ce9004d5540e6"
   integrity sha512-R4nPAVTAU0B9D35/Gk3uJf/7XYbQcyohSKdvAxIRSNghFl4e71hVoGnBNQz9cWaXxO2I10KTC+3jMdvvoKw6dQ==
 
-package-json@^6.5.0:
-  version "6.5.0"
-  resolved "https://registry.yarnpkg.com/package-json/-/package-json-6.5.0.tgz#6feedaca35e75725876d0b0e64974697fed145b0"
-  integrity sha512-k3bdm2n25tkyxcjSKzB5x8kfVxlMdgsbPr0GkZcwHsLpba6cBjqCt1KlcChKEvxHIcTB1FVMuwoijZ26xex5MQ==
-  dependencies:
-    got "^9.6.0"
-    registry-auth-token "^4.0.0"
-    registry-url "^5.0.0"
-    semver "^6.2.0"
-
 parent-module@^1.0.0:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/parent-module/-/parent-module-1.0.1.tgz#691d2709e78c79fae3a156622452d00762caaaa2"
   integrity sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==
   dependencies:
     callsites "^3.0.0"
 
@@ -3108,19 +3039,14 @@
     source-map "^0.6.1"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
   resolved "https://registry.yarnpkg.com/prelude-ls/-/prelude-ls-1.2.1.tgz#debc6489d7a6e6b0e7611888cec880337d316396"
   integrity sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==
 
-prepend-http@^2.0.0:
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/prepend-http/-/prepend-http-2.0.0.tgz#e92434bfa5ea8c19f41cdfd401d741a3c819d897"
-  integrity sha1-6SQ0v6XqjBn0HN/UAddBo8gZ2Jc=
-
 prettier-linter-helpers@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/prettier-linter-helpers/-/prettier-linter-helpers-1.0.0.tgz#d23d41fe1375646de2d0104d3454a3008802cf7b"
   integrity sha512-GbK2cP9nraSSUF9N2XwUwqfzlAFlMNYYl+ShE/V+H8a9uNl/oUqB1w2EL54Jh0OlyRSd8RfWYJ3coVS4TROP2w==
   dependencies:
     fast-diff "^1.1.2"
 
@@ -3149,32 +3075,29 @@
   resolved "https://registry.yarnpkg.com/prop-types/-/prop-types-15.7.2.tgz#52c41e75b8c87e72b9d9360e0206b99dcbffa6c5"
   integrity sha512-8QQikdH7//R2vurIJSutZ1smHYTcLpRWEOlHnzcWHmBYrOGUysKwSsrC89BCiFj3CbrfJ/nXFdJepOVrY1GCHQ==
   dependencies:
     loose-envify "^1.4.0"
     object-assign "^4.1.1"
     react-is "^16.8.1"
 
-pump@^3.0.0:
-  version "3.0.0"
-  resolved "https://registry.yarnpkg.com/pump/-/pump-3.0.0.tgz#b4a2116815bde2f4e1ea602354e8c75565107a64"
-  integrity sha512-LwZy+p3SFs1Pytd/jYct4wpv49HiYCqd9Rlc5ZVdk0V+8Yzv6jR5Blk3TRmPL1ft69TxP0IMZGJ+WPFU2BFhww==
-  dependencies:
-    end-of-stream "^1.1.0"
-    once "^1.3.1"
-
 punycode@1.3.2:
   version "1.3.2"
   resolved "https://registry.yarnpkg.com/punycode/-/punycode-1.3.2.tgz#9653a036fb7c1ee42342f2325cceefea3926c48d"
   integrity sha1-llOgNvt8HuQjQvIyXM7v6jkmxI0=
 
 punycode@^2.1.0:
   version "2.1.1"
   resolved "https://registry.yarnpkg.com/punycode/-/punycode-2.1.1.tgz#b58b010ac40c22c5657616c8d2c2c02c7bf479ec"
   integrity sha512-XRsRjdf+j5ml+y/6GKHPZbrF/8p2Yga0JPtdqTIY2Xe5ohJPD9saDJJLPvp9+NSBprVvevdXZybnj2cv8OEd0A==
 
+punycode@^2.1.1:
+  version "2.3.0"
+  resolved "https://registry.yarnpkg.com/punycode/-/punycode-2.3.0.tgz#f67fa67c94da8f4d0cfff981aee4118064199b8f"
+  integrity sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==
+
 querystring@0.2.0:
   version "0.2.0"
   resolved "https://registry.yarnpkg.com/querystring/-/querystring-0.2.0.tgz#b209849203bb25df820da756e747005878521620"
   integrity sha1-sgmEkgO7Jd+CDadW50cAWHhSFiA=
 
 querystringify@^2.1.1:
   version "2.2.0"
@@ -3197,24 +3120,14 @@
   version "4.0.2"
   resolved "https://registry.yarnpkg.com/raw-loader/-/raw-loader-4.0.2.tgz#1aac6b7d1ad1501e66efdac1522c73e59a584eb6"
   integrity sha512-ZnScIV3ag9A4wPX/ZayxL/jZH+euYb6FcUinPcgiQW0+UBtEv0O6Q3lGd3cqJ+GHH+rksEv3Pj99oxJ3u3VIKA==
   dependencies:
     loader-utils "^2.0.0"
     schema-utils "^3.0.0"
 
-rc@^1.2.8:
-  version "1.2.8"
-  resolved "https://registry.yarnpkg.com/rc/-/rc-1.2.8.tgz#cd924bf5200a075b83c188cd6b9e211b7fc0d3ed"
-  integrity sha512-y3bGgqKj3QBdxLbLkomlohkvsA8gdAiUQlSBJnBhfn+BPxg4bc62d8TcBW15wavDfgexCgccckhcZvywyQYPOw==
-  dependencies:
-    deep-extend "^0.6.0"
-    ini "~1.3.0"
-    minimist "^1.2.0"
-    strip-json-comments "~2.0.1"
-
 react-dom@^17.0.1:
   version "17.0.2"
   resolved "https://registry.yarnpkg.com/react-dom/-/react-dom-17.0.2.tgz#ecffb6845e3ad8dbfcdc498f0d0a939736502c23"
   integrity sha512-s4h96KtLDUQlsENhMn1ar8t2bEa+q/YAtj8pPPdIjPDGBDIVNsrD9aXNWqspUe6AzKCIG0C1HZZLqLV7qpOBGA==
   dependencies:
     loose-envify "^1.1.0"
     object-assign "^4.1.1"
@@ -3291,28 +3204,14 @@
     define-properties "^1.1.3"
 
 regexpp@^3.0.0, regexpp@^3.1.0:
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/regexpp/-/regexpp-3.1.0.tgz#206d0ad0a5648cffbdb8ae46438f3dc51c9f78e2"
   integrity sha512-ZOIzd8yVsQQA7j8GCSlPGXwg5PfmA1mrq0JP4nGhh54LaKN3xdai/vHUDu74pKwV8OxseMS65u2NImosQcSD0Q==
 
-registry-auth-token@^4.0.0:
-  version "4.2.1"
-  resolved "https://registry.yarnpkg.com/registry-auth-token/-/registry-auth-token-4.2.1.tgz#6d7b4006441918972ccd5fedcd41dc322c79b250"
-  integrity sha512-6gkSb4U6aWJB4SF2ZvLb76yCBjcvufXBqvvEx1HbmKPkutswjW1xNVRY0+daljIYRbogN7O0etYSlbiaEQyMyw==
-  dependencies:
-    rc "^1.2.8"
-
-registry-url@^5.0.0:
-  version "5.1.0"
-  resolved "https://registry.yarnpkg.com/registry-url/-/registry-url-5.1.0.tgz#e98334b50d5434b81136b44ec638d9c2009c5009"
-  integrity sha512-8acYXXTI0AkQv6RAOjE3vOaIXZkT9wo4LOFbBKYQEEnnMNBpKqdUrI6S4NT0KPIo/WVvJ5tE/X5LF/TQUf0ekw==
-  dependencies:
-    rc "^1.2.8"
-
 require-from-string@^2.0.2:
   version "2.0.2"
   resolved "https://registry.yarnpkg.com/require-from-string/-/require-from-string-2.0.2.tgz#89a7fdd938261267318eafe14f9c32e598c36909"
   integrity sha512-Xf0nWe6RseziFMu+Ap9biiUbmplq6S9/p+7w7YXP/JBHhrUDDUhwa+vANyubuqfZWTveU//DYVGsDG7RKL/vEw==
 
 requires-port@^1.0.0:
   version "1.0.0"
@@ -3345,66 +3244,39 @@
   version "1.20.0"
   resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.20.0.tgz#629a013fb3f70755d6f0b7935cc1c2c5378b1975"
   integrity sha512-wENBPt4ySzg4ybFQW2TT1zMQucPK95HSh/nq2CFTZVOGut2+pQvSsgtda4d26YrYcr067wjbmzOG8byDPBX63A==
   dependencies:
     is-core-module "^2.2.0"
     path-parse "^1.0.6"
 
-responselike@^1.0.2:
-  version "1.0.2"
-  resolved "https://registry.yarnpkg.com/responselike/-/responselike-1.0.2.tgz#918720ef3b631c5642be068f15ade5a46f4ba1e7"
-  integrity sha1-kYcg7ztjHFZCvgaPFa3lpG9Loec=
-  dependencies:
-    lowercase-keys "^1.0.0"
-
-restore-cursor@^3.1.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/restore-cursor/-/restore-cursor-3.1.0.tgz#39f67c54b3a7a58cea5236d95cf0034239631f7e"
-  integrity sha512-l+sSefzHpj5qimhFSE5a8nufZYAM3sBSVMAPtYkmC+4EH2anSGaEMXSD0izRQbu9nfyQ9y5JrVmp7E8oZrUjvA==
-  dependencies:
-    onetime "^5.1.0"
-    signal-exit "^3.0.2"
-
 reusify@^1.0.4:
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/reusify/-/reusify-1.0.4.tgz#90da382b1e126efc02146e90845a88db12925d76"
   integrity sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==
 
 rimraf@^3.0.2:
   version "3.0.2"
   resolved "https://registry.yarnpkg.com/rimraf/-/rimraf-3.0.2.tgz#f1a5402ba6220ad52cc1282bac1ae3aa49fd061a"
   integrity sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==
   dependencies:
     glob "^7.1.3"
 
-run-async@^2.4.0:
-  version "2.4.1"
-  resolved "https://registry.yarnpkg.com/run-async/-/run-async-2.4.1.tgz#8440eccf99ea3e70bd409d49aab88e10c189a455"
-  integrity sha512-tvVnVv01b8c1RrA6Ep7JkStj85Guv/YrMcwqYQnwjsAS2cTmmPGBBjAjpCW7RrSodNSoE2/qg9O4bceNvUuDgQ==
-
 run-parallel@^1.1.9:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/run-parallel/-/run-parallel-1.2.0.tgz#66d1368da7bdf921eb9d95bd1a9229e7f21a43ee"
   integrity sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==
   dependencies:
     queue-microtask "^1.2.2"
 
-rxjs@^6.6.0:
-  version "6.6.7"
-  resolved "https://registry.yarnpkg.com/rxjs/-/rxjs-6.6.7.tgz#90ac018acabf491bf65044235d5863c4dab804c9"
-  integrity sha512-hTdwr+7yYNIT5n4AMYp85KA6yw2Va0FLa3Rguvbpa4W3I5xynaBZo41cM3XM+4Q6fRMj3sBYIR1VAmZMXYJvRQ==
-  dependencies:
-    tslib "^1.9.0"
-
 safe-buffer@^5.1.0:
   version "5.2.1"
   resolved "https://registry.yarnpkg.com/safe-buffer/-/safe-buffer-5.2.1.tgz#1eaf9fa9bdb1fdd4ec75f58f9cdb4e6b7827eec6"
   integrity sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==
 
-"safer-buffer@>= 2.1.2 < 3":
+"safer-buffer@>= 2.1.2 < 3.0.0":
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/safer-buffer/-/safer-buffer-2.1.2.tgz#44fa161b0187b9549dd84bb91802f9bd8385cd6a"
   integrity sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==
 
 sanitize-html@~2.3.3:
   version "2.3.3"
   resolved "https://registry.yarnpkg.com/sanitize-html/-/sanitize-html-2.3.3.tgz#3db382c9a621cce4c46d90f10c64f1e9da9e8353"
@@ -3422,15 +3294,15 @@
   version "0.20.2"
   resolved "https://registry.yarnpkg.com/scheduler/-/scheduler-0.20.2.tgz#4baee39436e34aa93b4874bddcbf0fe8b8b50e91"
   integrity sha512-2eWfGgAqqWFGqtdMmcL5zCMK1U8KlXv8SQFGglL3CEtd0aDVDWgeF/YoCmvln55m5zSk3J/20hTaSBeSObsQDQ==
   dependencies:
     loose-envify "^1.1.0"
     object-assign "^4.1.1"
 
-schema-utils@^2.6.5:
+schema-utils@^2.6.5, schema-utils@^2.7.0:
   version "2.7.1"
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-2.7.1.tgz#1ca4f32d1b24c590c203b8e7a50bf0ea4cd394d7"
   integrity sha512-SHiNtMOUGWBQJwzISiVYKu82GiV4QYGePp3odlY1tuKO7gPtphAT5R/py0fA6xtbgLL/RvtJZnU9b8s0F1q0Xg==
   dependencies:
     "@types/json-schema" "^7.0.5"
     ajv "^6.12.4"
     ajv-keywords "^3.5.2"
@@ -3440,20 +3312,29 @@
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.0.0.tgz#67502f6aa2b66a2d4032b4279a2944978a0913ef"
   integrity sha512-6D82/xSzO094ajanoOSbe4YvXWMfn2A//8Y1+MUqFAJul5Bs+yn36xbK9OtNDcRVSBJ9jjeoXftM6CfztsjOAA==
   dependencies:
     "@types/json-schema" "^7.0.6"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
 
+schema-utils@^3.1.0, schema-utils@^3.1.1:
+  version "3.1.1"
+  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.1.tgz#bc74c4b6b6995c1d88f76a8b77bea7219e0c8281"
+  integrity sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==
+  dependencies:
+    "@types/json-schema" "^7.0.8"
+    ajv "^6.12.5"
+    ajv-keywords "^3.5.2"
+
 "semver@2 || 3 || 4 || 5", semver@^5.4.1, semver@^5.5.0:
   version "5.7.1"
   resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.1.tgz#a954f931aeba508d307bbf069eff0c01c96116f7"
   integrity sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==
 
-semver@^6.0.0, semver@^6.2.0:
+semver@^6.0.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.0.tgz#ee0a64c8af5e8ceea67687b133761e1becbd1d3d"
   integrity sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==
 
 semver@^7.2.1, semver@^7.3.2, semver@^7.3.5:
   version "7.3.5"
   resolved "https://registry.yarnpkg.com/semver/-/semver-7.3.5.tgz#0b621c879348d8998e4b0e4be94b3f12e6018ef7"
@@ -3464,14 +3345,21 @@
 serialize-javascript@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-5.0.1.tgz#7886ec848049a462467a97d3d918ebb2aaf934f4"
   integrity sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==
   dependencies:
     randombytes "^2.1.0"
 
+serialize-javascript@^6.0.0:
+  version "6.0.1"
+  resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-6.0.1.tgz#b206efb27c3da0b0ab6b52f48d170b7996458e5c"
+  integrity sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==
+  dependencies:
+    randombytes "^2.1.0"
+
 shallow-clone@^3.0.0:
   version "3.0.1"
   resolved "https://registry.yarnpkg.com/shallow-clone/-/shallow-clone-3.0.1.tgz#8f2981ad92531f55035b01fb230769a40e02efa3"
   integrity sha512-/6KqX+GVUdqPuPPd2LxDDxzX6CAbjJehAAOKlNpqqUpAqPM6HeL8f+o3a+JsyGjn2lv0WY8UsTgUJjU9Ok55NA==
   dependencies:
     kind-of "^6.0.2"
 
@@ -3496,19 +3384,19 @@
 
 shebang-regex@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/shebang-regex/-/shebang-regex-3.0.0.tgz#ae16f1644d873ecad843b0307b143362d4c42172"
   integrity sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==
 
 shell-quote@^1.6.1:
-  version "1.7.2"
-  resolved "https://registry.yarnpkg.com/shell-quote/-/shell-quote-1.7.2.tgz#67a7d02c76c9da24f99d20808fcaded0e0e04be2"
-  integrity sha512-mRz/m/JVscCrkMyPqHc/bczi3OQHkLTqXHEFu0zDhK/qfv3UcOA4SVmRCLmos4bhjr9ekVQubj/R7waKapmiQg==
+  version "1.7.3"
+  resolved "https://registry.yarnpkg.com/shell-quote/-/shell-quote-1.7.3.tgz#aa40edac170445b9a431e17bb62c0b881b9c4123"
+  integrity sha512-Vpfqwm4EnqGdlsBFNmHhxhElJYrdfcxPThu+ryKS5J8L/fhAwLazFZtq+S+TWZ9ANj2piSQLGj6NQg+lKPmxrw==
 
-signal-exit@^3.0.2, signal-exit@^3.0.3:
+signal-exit@^3.0.3:
   version "3.0.3"
   resolved "https://registry.yarnpkg.com/signal-exit/-/signal-exit-3.0.3.tgz#a1410c2edd8f077b08b4e253c8eacfcaf057461c"
   integrity sha512-VUJ49FC8U1OxwZLxIbTTrDvLnf/6TDgxZcK8wxR8zs13xpx7xbG60ndBlhNrFi2EMuFRoeDoJO7wthSLq42EjA==
 
 slash@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/slash/-/slash-3.0.0.tgz#6539be870c165adbd5240220dbe361f1bc4d4634"
@@ -3519,54 +3407,43 @@
   resolved "https://registry.yarnpkg.com/slice-ansi/-/slice-ansi-4.0.0.tgz#500e8dd0fd55b05815086255b3195adf2a45fe6b"
   integrity sha512-qMCMfhY040cVHT43K9BFygqYbUPFZKHOg7K73mtTWJRb8pyP3fzf4Ixd5SzdEJQ6MRUg/WBnOLxghZtKKurENQ==
   dependencies:
     ansi-styles "^4.0.0"
     astral-regex "^2.0.0"
     is-fullwidth-code-point "^3.0.0"
 
-sort-object-keys@^1.1.3:
-  version "1.1.3"
-  resolved "https://registry.yarnpkg.com/sort-object-keys/-/sort-object-keys-1.1.3.tgz#bff833fe85cab147b34742e45863453c1e190b45"
-  integrity sha512-855pvK+VkU7PaKYPc+Jjnmt4EzejQHyhhF33q31qG8x7maDzkeFhAAThdCYay11CISO+qAMwjOBP+fPZe0IPyg==
-
-sort-package-json@~1.44.0:
-  version "1.44.0"
-  resolved "https://registry.yarnpkg.com/sort-package-json/-/sort-package-json-1.44.0.tgz#470330be868f8a524a4607b26f2a0233e93d8b6d"
-  integrity sha512-u9GUZvpavUCXV5SbEqXu9FRbsJrYU6WM10r3zA0gymGPufK5X82MblCLh9GW9l46pXKEZvK+FA3eVTqC4oMp4A==
-  dependencies:
-    detect-indent "^6.0.0"
-    detect-newline "3.1.0"
-    git-hooks-list "1.0.3"
-    globby "10.0.0"
-    is-plain-obj "2.1.0"
-    sort-object-keys "^1.1.3"
-
-source-list-map@^2.0.0, source-list-map@^2.0.1:
+source-list-map@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/source-list-map/-/source-list-map-2.0.1.tgz#3993bd873bfc48479cca9ea3a547835c7c154b34"
   integrity sha512-qnQ7gVMxGNxsiL4lEuJwe/To8UnK7fAnmbGEEH8RpLouuKbeEm0lhbQVFIrNSuB+G7tVrAlVsZgETT5nljf+Iw==
 
-source-map-support@~0.5.19:
-  version "0.5.19"
-  resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.19.tgz#a98b62f86dcaf4f67399648c085291ab9e8fed61"
-  integrity sha512-Wonm7zOCIJzBGQdB+thsPar0kYuCIzYvxZwlBa87yi/Mdjv7Tip2cyVbLj5o0cFPN4EVkuTwb3GDDyUx2DGnGw==
+source-map-loader@~1.0.2:
+  version "1.0.2"
+  resolved "https://registry.yarnpkg.com/source-map-loader/-/source-map-loader-1.0.2.tgz#b0a6582b2eaa387ede1ecf8061ae0b93c23f9eb0"
+  integrity sha512-oX8d6ndRjN+tVyjj6PlXSyFPhDdVAPsZA30nD3/II8g4uOv8fCz0DMn5sy8KtVbDfKQxOpGwGJnK3xIW3tauDw==
+  dependencies:
+    data-urls "^2.0.0"
+    iconv-lite "^0.6.2"
+    loader-utils "^2.0.0"
+    schema-utils "^2.7.0"
+    source-map "^0.6.1"
+
+source-map-support@~0.5.20:
+  version "0.5.21"
+  resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.21.tgz#04fe7c7f9e1ed2d662233c28cb2b35b9f63f6e4f"
+  integrity sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==
   dependencies:
     buffer-from "^1.0.0"
     source-map "^0.6.0"
 
 source-map@^0.6.0, source-map@^0.6.1, source-map@~0.6.1:
   version "0.6.1"
   resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.6.1.tgz#74722af32e9614e9c287a8d0bbde48b5e2f1a263"
   integrity sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==
 
-source-map@~0.7.2:
-  version "0.7.3"
-  resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.7.3.tgz#5302f8169031735226544092e64981f751750383"
-  integrity sha512-CkCj6giN3S+n9qrYiBTX5gystlENnRW5jZeNLHpe6aue+SrHcG5VYwujhW9s4dY31mEGsxBDrHR6oI69fTXsaQ==
-
 spdx-correct@^3.0.0:
   version "3.1.1"
   resolved "https://registry.yarnpkg.com/spdx-correct/-/spdx-correct-3.1.1.tgz#dece81ac9c1e6713e5f7d1b6f17d468fa53d89a9"
   integrity sha512-cOYcUWwhCuHCXi49RhFRCyJEK3iPj1Ziz9DpViV3tbZOwXD49QzIN3MpOLJNxh2qwq2lJJZaKMVw9qNi4jTC0w==
   dependencies:
     spdx-expression-parse "^3.0.0"
     spdx-license-ids "^3.0.0"
@@ -3597,15 +3474,15 @@
 ssri@^8.0.1:
   version "8.0.1"
   resolved "https://registry.yarnpkg.com/ssri/-/ssri-8.0.1.tgz#638e4e439e2ffbd2cd289776d5ca457c4f51a2af"
   integrity sha512-97qShzy1AiyxvPNIkLWoGua7xoQzzPjQ0HAH4B0rWKo7SZ6USuPcrUiAFrws0UH8RrbWmgq3LMTObhPIHbbBeQ==
   dependencies:
     minipass "^3.1.1"
 
-string-width@^4.1.0, string-width@^4.2.0:
+string-width@^4.2.0:
   version "4.2.2"
   resolved "https://registry.yarnpkg.com/string-width/-/string-width-4.2.2.tgz#dafd4f9559a7585cfba529c6a0a4f73488ebd4c5"
   integrity sha512-XBJbT3N4JhVumXE0eoLU9DCjcaF92KLNqTmFCnG1pf8duUxFGwtP6AD6nkjw9a3IdiRtL3E2w3JDiE/xi3vOeA==
   dependencies:
     emoji-regex "^8.0.0"
     is-fullwidth-code-point "^3.0.0"
     strip-ansi "^6.0.0"
@@ -3653,19 +3530,14 @@
   integrity sha512-BrpvfNAE3dcvq7ll3xVumzjKjZQ5tI1sEUIKr3Uoks0XUl45St3FlatVqef9prk4jRDzhW6WZg+3bk93y6pLjA==
 
 strip-json-comments@^3.1.0, strip-json-comments@^3.1.1:
   version "3.1.1"
   resolved "https://registry.yarnpkg.com/strip-json-comments/-/strip-json-comments-3.1.1.tgz#31f1281b3832630434831c310c01cccda8cbe006"
   integrity sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==
 
-strip-json-comments@~2.0.1:
-  version "2.0.1"
-  resolved "https://registry.yarnpkg.com/strip-json-comments/-/strip-json-comments-2.0.1.tgz#3c531942e908c2697c0ec344858c286c7ca0a60a"
-  integrity sha1-PFMZQukIwml8DsNEhYwobHygpgo=
-
 style-loader@~2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/style-loader/-/style-loader-2.0.0.tgz#9669602fd4690740eaaec137799a03addbbc393c"
   integrity sha512-Z0gYUJmzZ6ZdRUqpg1r8GsaFKypE+3xAzuFeMuoHgjc9KZv3wMyCRjQIWEbhoFSq7+7yoHXySDJyyWQaPajeiQ==
   dependencies:
     loader-utils "^2.0.0"
     schema-utils "^3.0.0"
@@ -3680,14 +3552,21 @@
 supports-color@^7.0.0, supports-color@^7.1.0, supports-color@^7.2.0:
   version "7.2.0"
   resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-7.2.0.tgz#1b7dcdcb32b8138801b3e478ba6a51caa89648da"
   integrity sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==
   dependencies:
     has-flag "^4.0.0"
 
+supports-color@^8.0.0:
+  version "8.1.1"
+  resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-8.1.1.tgz#cd6fc17e28500cff56c1b86c0a7fd4a54a73005c"
+  integrity sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==
+  dependencies:
+    has-flag "^4.0.0"
+
 svg-url-loader@~6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/svg-url-loader/-/svg-url-loader-6.0.0.tgz#b94861d9f6badfb8ca3e7d3ec4655c1bf732ac5d"
   integrity sha512-Qr5SCKxyxKcRnvnVrO3iQj9EX/v40UiGEMshgegzV7vpo3yc+HexELOdtWcA3MKjL8IyZZ1zOdcILmDEa/8JJQ==
   dependencies:
     file-loader "~6.0.0"
     loader-utils "~2.0.0"
@@ -3732,72 +3611,77 @@
     p-limit "^3.0.2"
     schema-utils "^3.0.0"
     serialize-javascript "^5.0.1"
     source-map "^0.6.1"
     terser "^5.3.4"
     webpack-sources "^1.4.3"
 
-terser-webpack-plugin@^5.1.1:
-  version "5.1.2"
-  resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.1.2.tgz#51d295eb7cc56785a67a372575fdc46e42d5c20c"
-  integrity sha512-6QhDaAiVHIQr5Ab3XUWZyDmrIPCHMiqJVljMF91YKyqwKkL5QHnYMkrMBy96v9Z7ev1hGhSEw1HQZc2p/s5Z8Q==
+terser-webpack-plugin@^5.1.3:
+  version "5.3.6"
+  resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.3.6.tgz#5590aec31aa3c6f771ce1b1acca60639eab3195c"
+  integrity sha512-kfLFk+PoLUQIbLmB1+PZDMRSZS99Mp+/MHqDNmMA6tOItzRt+Npe3E+fsMs5mfcM0wCtrrdU387UnV+vnSffXQ==
+  dependencies:
+    "@jridgewell/trace-mapping" "^0.3.14"
+    jest-worker "^27.4.5"
+    schema-utils "^3.1.1"
+    serialize-javascript "^6.0.0"
+    terser "^5.14.1"
+
+terser@^5.14.1:
+  version "5.16.3"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.16.3.tgz#3266017a9b682edfe019b8ecddd2abaae7b39c6b"
+  integrity sha512-v8wWLaS/xt3nE9dgKEWhNUFP6q4kngO5B8eYFUuebsu7Dw/UNAnpUod6UHo04jSSkv8TzKHjZDSd7EXdDQAl8Q==
   dependencies:
-    jest-worker "^26.6.2"
-    p-limit "^3.1.0"
-    schema-utils "^3.0.0"
-    serialize-javascript "^5.0.1"
-    source-map "^0.6.1"
-    terser "^5.7.0"
+    "@jridgewell/source-map" "^0.3.2"
+    acorn "^8.5.0"
+    commander "^2.20.0"
+    source-map-support "~0.5.20"
 
-terser@^5.3.4, terser@^5.7.0:
-  version "5.7.0"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.7.0.tgz#a761eeec206bc87b605ab13029876ead938ae693"
-  integrity sha512-HP5/9hp2UaZt5fYkuhNBR8YyRcT8juw8+uFbAme53iN9hblvKnLUTKkmwJG6ocWpIKf8UK4DoeWG4ty0J6S6/g==
+terser@^5.3.4:
+  version "5.14.2"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.14.2.tgz#9ac9f22b06994d736174f4091aa368db896f1c10"
+  integrity sha512-oL0rGeM/WFQCUd0y2QrWxYnq7tfSuKBiqTjRPWrRgB46WD/kiwHwF8T23z78H6Q6kGCuuHcPB+KULHRdxvVGQA==
   dependencies:
+    "@jridgewell/source-map" "^0.3.2"
+    acorn "^8.5.0"
     commander "^2.20.0"
-    source-map "~0.7.2"
-    source-map-support "~0.5.19"
+    source-map-support "~0.5.20"
 
 text-table@^0.2.0:
   version "0.2.0"
   resolved "https://registry.yarnpkg.com/text-table/-/text-table-0.2.0.tgz#7f5ee823ae805207c00af2df4a84ec3fcfa570b4"
   integrity sha1-f17oI66AUgfACvLfSoTsP8+lcLQ=
 
-through@^2.3.6:
-  version "2.3.8"
-  resolved "https://registry.yarnpkg.com/through/-/through-2.3.8.tgz#0dd4c9ffaabc357960b1b724115d7e0e86a2e1f5"
-  integrity sha1-DdTJ/6q8NXlgsbckEV1+Doai4fU=
-
-tmp@^0.0.33:
-  version "0.0.33"
-  resolved "https://registry.yarnpkg.com/tmp/-/tmp-0.0.33.tgz#6d34335889768d21b2bcda0aa277ced3b1bfadf9"
-  integrity sha512-jRCJlojKnZ3addtTOjdIqoRuPEKBvNXcGYqzO6zWZX8KfKEpnGY5jfggJQ3EjKuu8D4bJRr0y+cYJFmYbImXGw==
-  dependencies:
-    os-tmpdir "~1.0.2"
-
-to-readable-stream@^1.0.0:
-  version "1.0.0"
-  resolved "https://registry.yarnpkg.com/to-readable-stream/-/to-readable-stream-1.0.0.tgz#ce0aa0c2f3df6adf852efb404a783e77c0475771"
-  integrity sha512-Iq25XBt6zD5npPhlLVXGFN3/gyR2/qODcKNNyTMd4vbm39HUaOiAM4PMq0eMVC/Tkxz+Zjdsc55g9yyz+Yq00Q==
-
 to-regex-range@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/to-regex-range/-/to-regex-range-5.0.1.tgz#1648c44aae7c8d988a326018ed72f5b4dd0392e4"
   integrity sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==
   dependencies:
     is-number "^7.0.0"
 
 to-string-loader@^1.1.6:
   version "1.1.6"
   resolved "https://registry.yarnpkg.com/to-string-loader/-/to-string-loader-1.1.6.tgz#230529ccc63dd0ecca052a85e1fb82afe946b0ab"
   integrity sha512-VNg62//PS1WfNwrK3n7t6wtK5Vdtx/qeYLLEioW46VMlYUwAYT6wnfB+OwS2FMTCalIHu0tk79D3RXX8ttmZTQ==
   dependencies:
     loader-utils "^1.0.0"
 
-tslib@^1.8.1, tslib@^1.9.0:
+tr46@^2.1.0:
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/tr46/-/tr46-2.1.0.tgz#fa87aa81ca5d5941da8cbf1f9b749dc969a4e240"
+  integrity sha512-15Ih7phfcdP5YxqiB+iDtLoaTz4Nd35+IiAv0kQ5FNKHzXgdWqPoTIqEDDJmXceQt4JZk6lVPT8lnDlPpGDppw==
+  dependencies:
+    punycode "^2.1.1"
+
+tr46@~0.0.3:
+  version "0.0.3"
+  resolved "https://registry.yarnpkg.com/tr46/-/tr46-0.0.3.tgz#8184fd347dac9cdc185992f3a6622e14b9d9ab6a"
+  integrity sha1-gYT9NH2snNwYWZLzpmIuFLnZq2o=
+
+tslib@^1.8.1:
   version "1.14.1"
   resolved "https://registry.yarnpkg.com/tslib/-/tslib-1.14.1.tgz#cf2d38bdc34a134bcaf1091c41f6619e2f672d00"
   integrity sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==
 
 tslib@~1.13.0:
   version "1.13.0"
   resolved "https://registry.yarnpkg.com/tslib/-/tslib-1.13.0.tgz#c881e13cc7015894ed914862d276436fa9a47043"
@@ -3818,19 +3702,14 @@
     prelude-ls "^1.2.1"
 
 type-fest@^0.20.2:
   version "0.20.2"
   resolved "https://registry.yarnpkg.com/type-fest/-/type-fest-0.20.2.tgz#1bf207f4b28f91583666cb5fbd327887301cd5f4"
   integrity sha512-Ne+eE4r0/iWnpAxD852z3A+N0Bt5RN//NjJwRd2VFHEmrywxf5vsZlh4R6lixl6B+wz/8d+maTSAkN1FIkI3LQ==
 
-type-fest@^0.21.3:
-  version "0.21.3"
-  resolved "https://registry.yarnpkg.com/type-fest/-/type-fest-0.21.3.tgz#d260a24b0198436e133fa26a524a6d65fa3b2e37"
-  integrity sha512-t0rzBq87m3fVcduHDUFhKmyyX+9eo6WQjZvf51Ea/M0Q7+T374Jp1aUiyUl0GKxp8M/OETVHSDvmkyPgvX+X2w==
-
 type-fest@^0.8.1:
   version "0.8.1"
   resolved "https://registry.yarnpkg.com/type-fest/-/type-fest-0.8.1.tgz#09e249ebde851d3b1e48d27c105444667f17b83d"
   integrity sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==
 
 typed-styles@^0.0.7:
   version "0.0.7"
@@ -3896,25 +3775,18 @@
   resolved "https://registry.yarnpkg.com/url-loader/-/url-loader-4.1.1.tgz#28505e905cae158cf07c92ca622d7f237e70a4e2"
   integrity sha512-3BTV812+AVHHOJQO8O5MkWgZ5aosP7GnROJwvzLS9hWDj00lZ6Z0wNak423Lp9PBZN05N+Jk/N5Si8jRAlGyWA==
   dependencies:
     loader-utils "^2.0.0"
     mime-types "^2.1.27"
     schema-utils "^3.0.0"
 
-url-parse-lax@^3.0.0:
-  version "3.0.0"
-  resolved "https://registry.yarnpkg.com/url-parse-lax/-/url-parse-lax-3.0.0.tgz#16b5cafc07dbe3676c1b1999177823d6503acb0c"
-  integrity sha1-FrXK/Afb42dsGxmZF3gj1lA6yww=
-  dependencies:
-    prepend-http "^2.0.0"
-
 url-parse@~1.5.1:
-  version "1.5.3"
-  resolved "https://registry.yarnpkg.com/url-parse/-/url-parse-1.5.3.tgz#71c1303d38fb6639ade183c2992c8cc0686df862"
-  integrity sha512-IIORyIQD9rvj0A4CLWsHkBBJuNqWpFQe224b6j9t/ABmquIS0qDU2pY6kl6AuOrL5OkCXHMCFNe1jBcuAggjvQ==
+  version "1.5.10"
+  resolved "https://registry.yarnpkg.com/url-parse/-/url-parse-1.5.10.tgz#9d3c2f736c1d75dd3bd2be507dcc111f1e2ea9c1"
+  integrity sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==
   dependencies:
     querystringify "^2.1.1"
     requires-port "^1.0.0"
 
 url@^0.11.0:
   version "0.11.0"
   resolved "https://registry.yarnpkg.com/url/-/url-0.11.0.tgz#3838e97cfc60521eb73c525a8e55bfdd9e2e28f1"
@@ -3944,22 +3816,32 @@
 warning@^4.0.2, warning@^4.0.3:
   version "4.0.3"
   resolved "https://registry.yarnpkg.com/warning/-/warning-4.0.3.tgz#16e9e077eb8a86d6af7d64aa1e05fd85b4678ca3"
   integrity sha512-rpJyN222KWIvHJ/F53XSZv0Zl/accqHR8et1kpaMTD/fLCRxtV8iX8czMzY7sVZupTI3zcUTg8eycS2kNF9l6w==
   dependencies:
     loose-envify "^1.0.0"
 
-watchpack@^2.0.0:
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/watchpack/-/watchpack-2.1.1.tgz#e99630550fca07df9f90a06056987baa40a689c7"
-  integrity sha512-Oo7LXCmc1eE1AjyuSBmtC3+Wy4HcV8PxWh2kP6fOl8yTlNS7r0K9l1ao2lrrUza7V39Y3D/BbJgY8VeSlc5JKw==
+watchpack@^2.4.0:
+  version "2.4.0"
+  resolved "https://registry.yarnpkg.com/watchpack/-/watchpack-2.4.0.tgz#fa33032374962c78113f93c7f2fb4c54c9862a5d"
+  integrity sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==
   dependencies:
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.1.2"
 
+webidl-conversions@^3.0.0:
+  version "3.0.1"
+  resolved "https://registry.yarnpkg.com/webidl-conversions/-/webidl-conversions-3.0.1.tgz#24534275e2a7bc6be7bc86611cc16ae0a5654871"
+  integrity sha1-JFNCdeKnvGvnvIZhHMFq4KVlSHE=
+
+webidl-conversions@^6.1.0:
+  version "6.1.0"
+  resolved "https://registry.yarnpkg.com/webidl-conversions/-/webidl-conversions-6.1.0.tgz#9111b4d7ea80acd40f5270d666621afa78b69514"
+  integrity sha512-qBIvFLGiBpLjfwmYAaHPXsn+ho5xZnGvyGvsarywGNc8VyQJUMHJ8OBKGGrPER0okBeMDaan4mNBlgBROxuI8w==
+
 webpack-cli@^4.1.0:
   version "4.7.0"
   resolved "https://registry.yarnpkg.com/webpack-cli/-/webpack-cli-4.7.0.tgz#3195a777f1f802ecda732f6c95d24c0004bc5a35"
   integrity sha512-7bKr9182/sGfjFm+xdZSwgQuFjgEcy0iCTIBxRUeteJ2Kr8/Wz0qNJX+jw60LU36jApt4nmMkep6+W5AKhok6g==
   dependencies:
     "@discoveryjs/json-ext" "^0.5.0"
     "@webpack-cli/configtest" "^1.0.3"
@@ -3979,58 +3861,78 @@
   version "5.7.3"
   resolved "https://registry.yarnpkg.com/webpack-merge/-/webpack-merge-5.7.3.tgz#2a0754e1877a25a8bbab3d2475ca70a052708213"
   integrity sha512-6/JUQv0ELQ1igjGDzHkXbVDRxkfA57Zw7PfiupdLFJYrgFqY5ZP8xxbpp2lU3EPwYx89ht5Z/aDkD40hFCm5AA==
   dependencies:
     clone-deep "^4.0.1"
     wildcard "^2.0.0"
 
-webpack-sources@^1.1.0, webpack-sources@^1.4.3:
+webpack-sources@^1.1.0, webpack-sources@^1.2.0, webpack-sources@^1.4.3:
   version "1.4.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-1.4.3.tgz#eedd8ec0b928fbf1cbfe994e22d2d890f330a933"
   integrity sha512-lgTS3Xhv1lCOKo7SA5TjKXMjpSM4sBjNV5+q2bqesbSPs5FjGmU6jjtBSkX9b4qW87vDIsCIlUPOEhbZrMdjeQ==
   dependencies:
     source-list-map "^2.0.0"
     source-map "~0.6.1"
 
-webpack-sources@^2.1.1:
-  version "2.2.0"
-  resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-2.2.0.tgz#058926f39e3d443193b6c31547229806ffd02bac"
-  integrity sha512-bQsA24JLwcnWGArOKUxYKhX3Mz/nK1Xf6hxullKERyktjNMC4x8koOeaDNTA2fEJ09BdWLbM/iTW0ithREUP0w==
-  dependencies:
-    source-list-map "^2.0.1"
-    source-map "^0.6.1"
-
-webpack@^5.3.1:
-  version "5.37.1"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.37.1.tgz#2deb5acd350583c1ab9338471f323381b0b0c14b"
-  integrity sha512-btZjGy/hSjCAAVHw+cKG+L0M+rstlyxbO2C+BOTaQ5/XAnxkDrP5sVbqWhXgo4pL3X2dcOib6rqCP20Zr9PLow==
-  dependencies:
-    "@types/eslint-scope" "^3.7.0"
-    "@types/estree" "^0.0.47"
-    "@webassemblyjs/ast" "1.11.0"
-    "@webassemblyjs/wasm-edit" "1.11.0"
-    "@webassemblyjs/wasm-parser" "1.11.0"
-    acorn "^8.2.1"
+webpack-sources@^3.2.3:
+  version "3.2.3"
+  resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
+  integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
+
+webpack@^5.41.1:
+  version "5.75.0"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.75.0.tgz#1e440468647b2505860e94c9ff3e44d5b582c152"
+  integrity sha512-piaIaoVJlqMsPtX/+3KTTO6jfvrSYgauFVdt8cr9LTHKmcq/AMd4mhzsiP7ZF/PGRNPGA8336jldh9l2Kt2ogQ==
+  dependencies:
+    "@types/eslint-scope" "^3.7.3"
+    "@types/estree" "^0.0.51"
+    "@webassemblyjs/ast" "1.11.1"
+    "@webassemblyjs/wasm-edit" "1.11.1"
+    "@webassemblyjs/wasm-parser" "1.11.1"
+    acorn "^8.7.1"
+    acorn-import-assertions "^1.7.6"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.8.0"
-    es-module-lexer "^0.4.0"
-    eslint-scope "^5.1.1"
+    enhanced-resolve "^5.10.0"
+    es-module-lexer "^0.9.0"
+    eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
-    graceful-fs "^4.2.4"
-    json-parse-better-errors "^1.0.2"
+    graceful-fs "^4.2.9"
+    json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
-    schema-utils "^3.0.0"
+    schema-utils "^3.1.0"
     tapable "^2.1.1"
-    terser-webpack-plugin "^5.1.1"
-    watchpack "^2.0.0"
-    webpack-sources "^2.1.1"
+    terser-webpack-plugin "^5.1.3"
+    watchpack "^2.4.0"
+    webpack-sources "^3.2.3"
+
+whatwg-mimetype@^2.3.0:
+  version "2.3.0"
+  resolved "https://registry.yarnpkg.com/whatwg-mimetype/-/whatwg-mimetype-2.3.0.tgz#3d4b1e0312d2079879f826aff18dbeeca5960fbf"
+  integrity sha512-M4yMwr6mAnQz76TbJm914+gPpB/nCwvZbJU28cUD6dR004SAxDLOOSUaB1JDRqLtaOV/vi0IC5lEAGFgrjGv/g==
+
+whatwg-url@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.yarnpkg.com/whatwg-url/-/whatwg-url-5.0.0.tgz#966454e8765462e37644d3626f6742ce8b70965d"
+  integrity sha1-lmRU6HZUYuN2RNNib2dCzotwll0=
+  dependencies:
+    tr46 "~0.0.3"
+    webidl-conversions "^3.0.0"
+
+whatwg-url@^8.0.0:
+  version "8.7.0"
+  resolved "https://registry.yarnpkg.com/whatwg-url/-/whatwg-url-8.7.0.tgz#656a78e510ff8f3937bc0bcbe9f5c0ac35941b77"
+  integrity sha512-gAojqb/m9Q8a5IV96E3fHJM70AzCkgt4uXYX2O7EmuyOnLrViCQlsEBmF9UQIu3/aeAIp2U17rtbpZWNntQqdg==
+  dependencies:
+    lodash "^4.7.0"
+    tr46 "^2.1.0"
+    webidl-conversions "^6.1.0"
 
 which-boxed-primitive@^1.0.2:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/which-boxed-primitive/-/which-boxed-primitive-1.0.2.tgz#13757bc89b209b049fe5d86430e21cf40a89a8e6"
   integrity sha512-bwZdv0AKLpplFY2KZRX6TvyuN7ojjr7lwkg6ml0roIy9YeuSr7JS372qlNW18UQYzgYK9ziGcerWqZOmEn9VNg==
   dependencies:
     is-bigint "^1.0.1"
```

