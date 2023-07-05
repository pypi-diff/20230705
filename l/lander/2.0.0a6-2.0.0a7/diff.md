# Comparing `tmp/lander-2.0.0a6.tar.gz` & `tmp/lander-2.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lander-2.0.0a6.tar", last modified: Mon Feb 15 16:32:07 2021, max compression
+gzip compressed data, was "lander-2.0.0a7.tar", last modified: Thu May 27 16:10:56 2021, max compression
```

## Comparing `lander-2.0.0a6.tar` & `lander-2.0.0a7.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-02-15 16:30:56.000000 lander-2.0.0a6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.669872 lander-2.0.0a6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.669872 lander-2.0.0a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-02-15 16:30:56.000000 lander-2.0.0a6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-02-15 16:30:56.000000 lander-2.0.0a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-02-15 16:30:56.000000 lander-2.0.0a6/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (121)      942 2021-02-15 16:30:56.000000 lander-2.0.0a6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6490 2021-02-15 16:30:56.000000 lander-2.0.0a6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-02-15 16:30:56.000000 lander-2.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-02-15 16:30:56.000000 lander-2.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-02-15 16:30:56.000000 lander-2.0.0a6/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    17903 2021-02-15 16:32:07.677872 lander-2.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6338 2021-02-15 16:30:56.000000 lander-2.0.0a6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-02-15 16:30:56.000000 lander-2.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-02-15 16:32:07.681872 lander-2.0.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-02-15 16:30:56.000000 lander-2.0.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.669872 lander-2.0.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/codemeta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/data/
--rw-r--r--   0 runner    (1001) docker     (121)   186850 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/data/licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/ext/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/ext/parser/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/_cidata.py
--rw-r--r--   0 runner    (1001) docker     (121)     8921 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/_gitdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/ext/parser/pandoc/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/pandoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/pandoc/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/ext/parser/pandoc/filters/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/pandoc/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/pandoc/filters/deparagraph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander/ext/parser/texutils/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/texutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13946 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/texutils/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/parser/texutils/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/ext/theme/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/theme/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/theme/_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/theme/_jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/ext/theme/jinjafilters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/parsers/article/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/parsers/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/parsers/article/_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6642 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/spdx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/base/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/base/js/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/js/lander.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/base/site/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/site/index.html.jinja
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2021-02-15 16:32:06.000000 lander-2.0.0a6/src/lander/themes/base/site/lander.bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/base/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/templates/htmlpage.jinja
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/templates/info_sidebar.jinja
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/templates/pdfviewer.jinja
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/base/webpack.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/minimalist/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/minimalist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/minimalist/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.677872 lander-2.0.0a6/src/lander/themes/minimalist/site/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-02-15 16:30:56.000000 lander-2.0.0a6/src/lander/themes/minimalist/site/index.html.jinja
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 16:32:07.673872 lander-2.0.0a6/src/lander.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17903 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-02-15 16:32:07.000000 lander-2.0.0a6/src/lander.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-02-15 16:30:56.000000 lander-2.0.0a6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-05-27 16:09:53.000000 lander-2.0.0a7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.453417 lander-2.0.0a7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.457417 lander-2.0.0a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3403 2021-05-27 16:09:53.000000 lander-2.0.0a7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-05-27 16:09:53.000000 lander-2.0.0a7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-27 16:09:53.000000 lander-2.0.0a7/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2021-05-27 16:09:53.000000 lander-2.0.0a7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6490 2021-05-27 16:09:53.000000 lander-2.0.0a7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-05-27 16:09:53.000000 lander-2.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2021-05-27 16:09:53.000000 lander-2.0.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-05-27 16:09:53.000000 lander-2.0.0a7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    15092 2021-05-27 16:10:56.465417 lander-2.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6338 2021-05-27 16:09:53.000000 lander-2.0.0a7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-05-27 16:09:53.000000 lander-2.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-05-27 16:10:56.469417 lander-2.0.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-05-27 16:09:53.000000 lander-2.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.453417 lander-2.0.0a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.457417 lander-2.0.0a7/src/lander/
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/codemeta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   186850 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/data/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/parser/
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/_cidata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8921 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4093 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/_gitdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3694 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/parser/pandoc/
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/pandoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/pandoc/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4331 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/pandoc/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/parser/pandoc/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/pandoc/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/pandoc/filters/deparagraph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/parser/texutils/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/texutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13946 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/texutils/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5833 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/parser/texutils/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/ext/theme/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11191 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/theme/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/theme/_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/theme/_jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/ext/theme/jinjafilters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/parsers/article/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/parsers/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/parsers/article/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6642 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/spdx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/themes/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander/themes/base/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/src/lander/themes/base/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/js/lander.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/src/lander/themes/base/site/
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/site/index.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (121)     3803 2021-05-27 16:10:55.000000 lander-2.0.0a7/src/lander/themes/base/site/lander.bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/src/lander/themes/base/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/templates/htmlpage.jinja
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/templates/info_sidebar.jinja
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/templates/pdfviewer.jinja
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/base/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/src/lander/themes/minimalist/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/minimalist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/minimalist/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.465417 lander-2.0.0a7/src/lander/themes/minimalist/site/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-27 16:09:53.000000 lander-2.0.0a7/src/lander/themes/minimalist/site/index.html.jinja
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 16:10:56.461417 lander-2.0.0a7/src/lander.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15092 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-27 16:10:56.000000 lander-2.0.0a7/src/lander.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2021-05-27 16:09:53.000000 lander-2.0.0a7/tox.ini
```

### Comparing `lander-2.0.0a6/.github/workflows/ci.yaml` & `lander-2.0.0a7/.github/workflows/ci.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.7, 3.8]
+        python-version: [3.7, 3.8, 3.9]
 
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
+      - name: Install pandoc
+        run: brew install pandoc
+
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Read .nvmrc
         id: node_version
@@ -42,25 +45,76 @@
 
       - name: Build assets
         run: gulp assets
 
       - name: Run tests
         run: tox -e py,lint,typing
 
+  demo:
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v2
+        with:
+          fetch-depth: 0 # full history for setuptools_scm
+
+      - name: Install pandoc
+        run: brew install pandoc
+
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.9
+
+      - name: Read .nvmrc
+        id: node_version
+        run: echo ::set-output name=NODE_VERSION::$(cat .nvmrc)
+
+      - name: Set up node
+        uses: actions/setup-node@v2
+        with:
+          node-version: ${{ steps.node_version.outputs.NODE_VERSION }}
+
+      - name: NPM install
+        run: |
+          npm install -g gulp-cli
+          npm install
+
+      - name: Python install
+        run: |
+          python -m pip install --upgrade pip
+          pip install .[dev]
+          pip install tox
+
+      - name: Build assets
+        run: gulp assets
+
+      - name: Build demo pages
+        run: tox -e demo
+
+      - name: Upload demo artifact
+        uses: actions/upload-artifact@v2
+        with:
+          name: article-demo
+          path: _build/article-demo
+
   pypi:
 
     runs-on: ubuntu-latest
     needs: [test]
     if: startsWith(github.ref, 'refs/tags/')
 
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
+      - name: Install pandoc
+        run: brew install pandoc
+
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: 3.8
 
       - name: Read .nvmrc
         id: node_version
```

### Comparing `lander-2.0.0a6/.gitignore` & `lander-2.0.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/.pre-commit-config.yaml` & `lander-2.0.0a7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/CHANGELOG.rst` & `lander-2.0.0a7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/LICENSE` & `lander-2.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/README.rst` & `lander-2.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/pyproject.toml` & `lander-2.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/setup.cfg` & `lander-2.0.0a7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Intended Audience :: Developers
 	Natural Language :: English
 	Operating System :: POSIX
 keywords = 
 	lsst
 
 [options]
@@ -36,16 +37,15 @@
 	importlib_metadata; python_version < "3.8"
 	python-dateutil>=2.6.0
 	Jinja2>=2.10.1
 	pydantic
 	email-validator # for pydantic
 	bleach
 	pypandoc
-	py-pandoc<2.10 # match panflut compatibility matrix
-	panflute~=1.2  # https://github.com/sergiocorreia/panflute#supported-pandoc-versions
+	panflute>=2  # https://github.com/sergiocorreia/panflute#supported-pandoc-versions
 	GitPython
 	typer
 	base32-lib
 
 [options.packages.find]
 where = src
```

### Comparing `lander-2.0.0a6/src/lander/cli.py` & `lander-2.0.0a7/src/lander/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Optional
 
 import typer
 
+from lander.ext.parser.pandoc import print_pandoc_version
 from lander.plugins import parsers, themes
 from lander.settings import BuildSettings
 
 __all__ = ["app"]
 
 app = typer.Typer()
 
@@ -26,14 +27,16 @@
     ),
     parser: Optional[str] = typer.Option(None, help="Metadata parsing plugin"),
     theme: Optional[str] = typer.Option(None, help="Theme plugin."),
     canonical_url: Optional[str] = typer.Option(
         None, "--url", help="Canonical URL where the landing page is hosted."
     ),
 ) -> None:
+    print_pandoc_version()
+
     settings = BuildSettings.load(
         output_dir=output,
         source_path=source,
         pdf=pdf,
         parser=parser,
         theme=theme,
         canonical_url=canonical_url,
```

### Comparing `lander-2.0.0a6/src/lander/codemeta.py` & `lander-2.0.0a7/src/lander/codemeta.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/data/licenses.json` & `lander-2.0.0a7/src/lander/data/licenses.json`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/__init__.py` & `lander-2.0.0a7/src/lander/ext/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/_cidata.py` & `lander-2.0.0a7/src/lander/ext/parser/_cidata.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/_datamodel.py` & `lander-2.0.0a7/src/lander/ext/parser/_datamodel.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/_discovery.py` & `lander-2.0.0a7/src/lander/ext/parser/_discovery.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/_gitdata.py` & `lander-2.0.0a7/src/lander/ext/parser/_gitdata.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/_parser.py` & `lander-2.0.0a7/src/lander/ext/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/pandoc/_convert.py` & `lander-2.0.0a7/src/lander/ext/parser/pandoc/_convert.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,16 +22,32 @@
     @functools.wraps(func)
     def _install_and_run(*args: Any, **kwargs: Any) -> Any:
         try:
             # First try to run pypandoc function
             result = func(*args, **kwargs)
         except OSError:
             # Install pandoc and retry
-            message = "Pandoc is required but not found."
-            logger.warning(message)
+            logger.warning(
+                "Pandoc is required but not found. Lander is going to try to "
+                "install it for you right now."
+            )
+
+            try:
+                pypandoc.download_pandoc()
+                logger.info(
+                    "Pandoc version %s installation complete",
+                    pypandoc.get_pandoc_version(),
+                )
+            except Exception:
+                logger.exception("Failed to download pandoc.")
+                raise RuntimeError(
+                    "Could not install Pandoc. Please pre-install pandoc on "
+                    "your system and try again. See "
+                    "https://pandoc.org/installing.html."
+                )
 
             result = func(*args, **kwargs)
 
         return result
 
     return _install_and_run
```

### Comparing `lander-2.0.0a6/src/lander/ext/parser/pandoc/filters/deparagraph.py` & `lander-2.0.0a7/src/lander/ext/parser/pandoc/filters/deparagraph.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/texutils/extract.py` & `lander-2.0.0a7/src/lander/ext/parser/texutils/extract.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/parser/texutils/normalize.py` & `lander-2.0.0a7/src/lander/ext/parser/texutils/normalize.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/theme/_base.py` & `lander-2.0.0a7/src/lander/ext/theme/_base.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/theme/_discovery.py` & `lander-2.0.0a7/src/lander/ext/theme/_discovery.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/theme/_jinjaloader.py` & `lander-2.0.0a7/src/lander/ext/theme/_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/ext/theme/jinjafilters.py` & `lander-2.0.0a7/src/lander/ext/theme/jinjafilters.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/parsers/article/_parser.py` & `lander-2.0.0a7/src/lander/parsers/article/_parser.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/renderer.py` & `lander-2.0.0a7/src/lander/renderer.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/settings.py` & `lander-2.0.0a7/src/lander/settings.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/spdx.py` & `lander-2.0.0a7/src/lander/spdx.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/_plugin.py` & `lander-2.0.0a7/src/lander/themes/base/_plugin.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/js/lander.js` & `lander-2.0.0a7/src/lander/themes/base/js/lander.js`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/site/index.html.jinja` & `lander-2.0.0a7/src/lander/themes/base/site/index.html.jinja`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/site/lander.bundle.js` & `lander-2.0.0a7/src/lander/themes/base/site/lander.bundle.js`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/templates/htmlpage.jinja` & `lander-2.0.0a7/src/lander/themes/base/templates/htmlpage.jinja`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/templates/info_sidebar.jinja` & `lander-2.0.0a7/src/lander/themes/base/templates/info_sidebar.jinja`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/base/webpack.config.js` & `lander-2.0.0a7/src/lander/themes/base/webpack.config.js`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander/themes/minimalist/_plugin.py` & `lander-2.0.0a7/src/lander/themes/minimalist/_plugin.py`

 * *Files identical despite different names*

### Comparing `lander-2.0.0a6/src/lander.egg-info/SOURCES.txt` & `lander-2.0.0a7/src/lander.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/lander/ext/parser/__init__.py
 src/lander/ext/parser/_cidata.py
 src/lander/ext/parser/_datamodel.py
 src/lander/ext/parser/_discovery.py
 src/lander/ext/parser/_gitdata.py
 src/lander/ext/parser/_parser.py
 src/lander/ext/parser/pandoc/__init__.py
+src/lander/ext/parser/pandoc/_compatibility.py
 src/lander/ext/parser/pandoc/_convert.py
 src/lander/ext/parser/pandoc/filters/__init__.py
 src/lander/ext/parser/pandoc/filters/deparagraph.py
 src/lander/ext/parser/texutils/__init__.py
 src/lander/ext/parser/texutils/extract.py
 src/lander/ext/parser/texutils/normalize.py
 src/lander/ext/theme/__init__.py
```

