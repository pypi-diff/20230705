# Comparing `tmp/jupyterlab_spellchecker-0.8.0.tar.gz` & `tmp/jupyterlab_spellchecker-0.8.2.tar.gz`

## Comparing `jupyterlab_spellchecker-0.8.0.tar` & `jupyterlab_spellchecker-0.8.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.eslintrc.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.yarnrc.yml
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/demo.gif
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/install.json
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/tsconfig.json
--rw-r--r--   0        0        0   206920 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/yarn.lock
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README.txt
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_de_ALL_frami.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_en_AU.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_en_CA.txt
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_en_GB-ise.txt
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_en_US.txt
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_es_ES.txt
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_fr.txt
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/README_pt_PT.txt
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_AT_frami.aff
--rw-r--r--   0        0        0  4422326 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_AT_frami.dic
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_CH_frami.aff
--rw-r--r--   0        0        0  4416507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_CH_frami.dic
--rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_DE_frami.aff
--rw-r--r--   0        0        0  4419933 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/de_DE_frami.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_AU.aff
--rw-r--r--   0        0        0   553854 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_AU.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_CA.aff
--rw-r--r--   0        0        0   551079 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_CA.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_GB-ise.aff
--rw-r--r--   0        0        0   551624 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_GB-ise.dic
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_US.aff
--rw-r--r--   0        0        0   551260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/en_US.dic
--rw-r--r--   0        0        0   167076 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/es_ES.aff
--rw-r--r--   0        0        0   861168 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/es_ES.dic
--rw-r--r--   0        0        0   256857 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/fr.aff
--rw-r--r--   0        0        0  1100397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/fr.dic
--rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/pt_PT.aff
--rw-r--r--   0        0        0   456494 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/dictionaries/pt_PT.dic
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyter-config/nb-config/jupyterlab-spellchecker.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyter-config/server-config/jupyterlab-spellchecker.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/_version.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/dictionaries.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/handlers.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/package.json
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json
--rw-r--r--   0        0        0    12308 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/567.8d6cd80dc97bed24045f.js
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/remoteEntry.0c6332c849276aede6e7.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/style.js
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/tests/test_dictionaries.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/schema/plugin.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/src/handler.ts
--rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/src/index.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/src/loader.d.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/src/svg.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/style/base.css
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/style/icons/LICENSE
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/style/icons/ic-baseline-spellcheck.svg
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/.gitignore
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/LICENSE
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/README.md
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.eslintrc.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.yarnrc.yml
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/demo.gif
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/install.json
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/tsconfig.json
+-rw-r--r--   0        0        0   206920 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/yarn.lock
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README.txt
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_de_ALL_frami.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_en_AU.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_en_CA.txt
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_en_GB-ise.txt
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_en_US.txt
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_es_ES.txt
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_fr.txt
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/README_pt_PT.txt
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_AT_frami.aff
+-rw-r--r--   0        0        0  4422326 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_AT_frami.dic
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_CH_frami.aff
+-rw-r--r--   0        0        0  4416507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_CH_frami.dic
+-rw-r--r--   0        0        0    19218 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_DE_frami.aff
+-rw-r--r--   0        0        0  4419933 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/de_DE_frami.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_AU.aff
+-rw-r--r--   0        0        0   553854 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_AU.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_CA.aff
+-rw-r--r--   0        0        0   551079 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_CA.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_GB-ise.aff
+-rw-r--r--   0        0        0   551624 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_GB-ise.dic
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_US.aff
+-rw-r--r--   0        0        0   551260 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/en_US.dic
+-rw-r--r--   0        0        0   167076 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/es_ES.aff
+-rw-r--r--   0        0        0   861168 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/es_ES.dic
+-rw-r--r--   0        0        0   256857 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/fr.aff
+-rw-r--r--   0        0        0  1100397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/fr.dic
+-rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/pt_PT.aff
+-rw-r--r--   0        0        0   456494 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/dictionaries/pt_PT.dic
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyter-config/nb-config/jupyterlab-spellchecker.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyter-config/server-config/jupyterlab-spellchecker.json
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/_version.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/dictionaries.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/handlers.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/package.json
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json
+-rw-r--r--   0        0        0    12308 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/567.8d6cd80dc97bed24045f.js
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/remoteEntry.3b7ed715d30be884a69e.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/style.js
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/tests/test_dictionaries.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/schema/plugin.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/src/handler.ts
+-rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/src/index.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/src/loader.d.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/src/svg.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/style/base.css
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/style/icons/LICENSE
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/style/icons/ic-baseline-spellcheck.svg
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/README.md
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 jupyterlab_spellchecker-0.8.2/PKG-INFO
```

### Comparing `jupyterlab_spellchecker-0.8.0/.eslintrc.js` & `jupyterlab_spellchecker-0.8.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/CHANGELOG.md` & `jupyterlab_spellchecker-0.8.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 0.8.2 (2023-06-04)
+
+- fix server extension loading (#131)
+
 ### 0.8.1 (2023-06-04)
 
 - fix for PyPI upload (#130)
 
 ### 0.8.0 (2023-06-04)
 
 - support JupyterLab 4.0 (#128)
```

### Comparing `jupyterlab_spellchecker-0.8.0/demo.gif` & `jupyterlab_spellchecker-0.8.2/demo.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/package.json` & `jupyterlab_spellchecker-0.8.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'0.8.2'"}*

```diff
@@ -120,9 +120,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.8.2"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.0/tsconfig.json` & `jupyterlab_spellchecker-0.8.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/yarn.lock` & `jupyterlab_spellchecker-0.8.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_de_ALL_frami.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_de_ALL_frami.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_en_AU.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_en_AU.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_en_CA.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_en_CA.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_en_GB-ise.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_en_GB-ise.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_en_US.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_en_US.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_es_ES.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_es_ES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_fr.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_fr.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/README_pt_PT.txt` & `jupyterlab_spellchecker-0.8.2/dictionaries/README_pt_PT.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_AT_frami.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_AT_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_AT_frami.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_AT_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_CH_frami.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_CH_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_CH_frami.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_CH_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_DE_frami.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_DE_frami.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/de_DE_frami.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/de_DE_frami.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_AU.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_AU.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_AU.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_AU.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_CA.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_CA.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_CA.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_CA.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_GB-ise.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_GB-ise.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_GB-ise.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_GB-ise.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_US.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_US.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/en_US.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/en_US.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/es_ES.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/es_ES.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/es_ES.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/es_ES.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/fr.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/fr.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/fr.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/fr.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/pt_PT.aff` & `jupyterlab_spellchecker-0.8.2/dictionaries/pt_PT.aff`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/dictionaries/pt_PT.dic` & `jupyterlab_spellchecker-0.8.2/dictionaries/pt_PT.dic`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/__init__.py` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,21 @@
     # Fallback when using the package in dev mode without installing
     # in editable mode with pip. It is highly recommended to install
     # the package from a stable release or in editable mode: https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs
     import warnings
     warnings.warn("Importing 'jupyterlab-spellchecker' outside a proper installation.")
     __version__ = "dev"
 
-import json
-from pathlib import Path
-
 from .handlers import setup_handlers
 
-HERE = Path(__file__).parent.resolve()
-
-with (HERE / "labextension" / "package.json").open() as fid:
-    data = json.load(fid)
 
 def _jupyter_labextension_paths():
     return [{
         "src": "labextension",
-        "dest": data["name"]
+        "dest": "@jupyterlab-contrib/spellchecker"
     }]
 
 
 def _jupyter_server_extension_points():
     return [{"module": "jupyterlab_spellchecker"}]
```

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/dictionaries.py` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/dictionaries.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/handlers.py` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/package.json` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.8.2'"}*

```diff
@@ -64,19 +64,14 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/spellchecker",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.0c6332c849276aede6e7.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-spellchecker"
                 },
                 "managers": [
                     "pip",
@@ -125,9 +120,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.8.2"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/package.json.orig` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.3b7ed715d30be884a69e.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.8.2'"}*

```diff
@@ -64,14 +64,19 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/spellchecker",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.3b7ed715d30be884a69e.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-spellchecker"
                 },
                 "managers": [
                     "pip",
@@ -120,9 +125,9 @@
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.8.2"
 }
```

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/schemas/@jupyterlab-contrib/spellchecker/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/567.8d6cd80dc97bed24045f.js` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/567.8d6cd80dc97bed24045f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/581.7b781918df8ce52c9a8f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/747.2f89d796d954e37784cd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/995.266a0ca9063d6df0c41f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/remoteEntry.0c6332c849276aede6e7.js` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/remoteEntry.3b7ed715d30be884a69e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -111,15 +111,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-contrib/spellchecker", "0.8.0", (() => Promise.all([w.e(995), w.e(567)]).then((() => () => w(552))))), l("typo-js", "1.2.0", (() => w.e(581).then((() => () => w(581)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-contrib/spellchecker", "0.8.2", (() => Promise.all([w.e(995), w.e(567)]).then((() => () => w(552))))), l("typo-js", "1.2.0", (() => w.e(581).then((() => () => w(581)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/labextension/static/third-party-licenses.json` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/jupyterlab_spellchecker/tests/test_dictionaries.py` & `jupyterlab_spellchecker-0.8.2/jupyterlab_spellchecker/tests/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/schema/plugin.json` & `jupyterlab_spellchecker-0.8.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/src/handler.ts` & `jupyterlab_spellchecker-0.8.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/src/index.ts` & `jupyterlab_spellchecker-0.8.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/style/index.css` & `jupyterlab_spellchecker-0.8.2/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/style/icons/LICENSE` & `jupyterlab_spellchecker-0.8.2/style/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/.gitignore` & `jupyterlab_spellchecker-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/LICENSE` & `jupyterlab_spellchecker-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/README.md` & `jupyterlab_spellchecker-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/pyproject.toml` & `jupyterlab_spellchecker-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_spellchecker-0.8.0/PKG-INFO` & `jupyterlab_spellchecker-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-spellchecker
-Version: 0.8.0
+Version: 0.8.2
 Summary: A spell checker for JupyterLab.
 Project-URL: Source, https://github.com/jupyterlab-contrib/spellchecker
 Project-URL: Issues, https://github.com/jupyterlab-contrib/spellchecker/issues
 Author: JupyterLab Spellchecker Development Team
 License: BSD 3-Clause License
         
         Copyright (c) 2020, ijmbarr All rights reserved.
```

