# Comparing `tmp/gentle_mxml-0.3.1.tar.gz` & `tmp/gentle_mxml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentle_mxml-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gentle_mxml-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gentle_mxml-0.3.1.tar` & `gentle_mxml-0.4.0.tar`

### file list

```diff
@@ -1,199 +1,256 @@
--rw-r--r--   0        0        0      177 2023-07-01 23:16:33.075157 gentle_mxml-0.3.1/.bumpversion.cfg
--rw-r--r--   0        0        0       85 2023-06-25 13:58:30.249547 gentle_mxml-0.3.1/.bumpversion.cfg.license
--rw-r--r--   0        0        0      384 2023-06-26 18:36:20.326251 gentle_mxml-0.3.1/.drone.yml
--rw-r--r--   0        0        0      153 2023-07-01 23:15:07.469678 gentle_mxml-0.3.1/.gitignore
--rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.3.1/LICENSE
--rw-r--r--   0        0        0    34020 2023-06-21 17:54:08.857916 gentle_mxml-0.3.1/LICENSES/AGPL-3.0-only.txt
--rw-r--r--   0        0        0    10280 2023-06-07 19:43:48.069665 gentle_mxml-0.3.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     1460 2023-06-21 23:16:06.355684 gentle_mxml-0.3.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0        0        0     7048 2022-11-14 10:12:41.100101 gentle_mxml-0.3.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-06-25 12:08:33.459576 gentle_mxml-0.3.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     1078 2023-06-07 16:20:14.601959 gentle_mxml-0.3.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0      432 2022-11-14 10:12:40.671121 gentle_mxml-0.3.1/LICENSES/WTFPL.txt
--rw-r--r--   0        0        0     2343 2023-06-26 18:30:42.288936 gentle_mxml-0.3.1/README.md
--rw-r--r--   0        0        0      230 2023-06-25 13:09:13.402778 gentle_mxml-0.3.1/docs/_build/.buildinfo
--rw-r--r--   0        0        0     9939 2023-06-25 13:09:12.274825 gentle_mxml-0.3.1/docs/_build/.doctrees/contributing.doctree
--rw-r--r--   0        0        0   119130 2023-06-25 13:09:12.772805 gentle_mxml-0.3.1/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0        0        0     4893 2023-06-25 13:09:12.284825 gentle_mxml-0.3.1/docs/_build/.doctrees/getting-started.doctree
--rw-r--r--   0        0        0     5207 2023-06-25 13:09:12.293825 gentle_mxml-0.3.1/docs/_build/.doctrees/index.doctree
--rw-r--r--   0        0        0     6471 2023-06-25 13:09:12.307824 gentle_mxml-0.3.1/docs/_build/.doctrees/installation.doctree
--rw-r--r--   0        0        0    43744 2023-06-25 13:09:12.755805 gentle_mxml-0.3.1/docs/_build/.doctrees/reference.doctree
--rw-r--r--   0        0        0     4901 2023-06-25 13:09:12.765805 gentle_mxml-0.3.1/docs/_build/.doctrees/toc.doctree
--rw-r--r--   0        0        0     8129 2023-06-25 13:09:13.319782 gentle_mxml-0.3.1/docs/_build/404.html
--rw-r--r--   0        0        0     1458 2023-06-25 12:55:03.457995 gentle_mxml-0.3.1/docs/_build/_sources/contributing.rst.txt
--rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.3.1/docs/_build/_sources/getting-started.rst.txt
--rw-r--r--   0        0        0      456 2023-06-25 12:43:37.704408 gentle_mxml-0.3.1/docs/_build/_sources/index.rst.txt
--rw-r--r--   0        0        0      619 2023-06-25 12:45:58.431577 gentle_mxml-0.3.1/docs/_build/_sources/installation.rst.txt
--rw-r--r--   0        0        0      301 2023-06-25 13:09:09.222952 gentle_mxml-0.3.1/docs/_build/_sources/reference.rst.txt
--rw-r--r--   0        0        0      321 2023-06-25 13:05:45.723384 gentle_mxml-0.3.1/docs/_build/_sources/toc.rst.txt
--rw-r--r--   0        0        0    14813 2023-06-25 13:09:13.360780 gentle_mxml-0.3.1/docs/_build/_static/basic.css
--rw-r--r--   0        0        0     4472 2023-06-20 06:40:23.406098 gentle_mxml-0.3.1/docs/_build/_static/doctools.js
--rw-r--r--   0        0        0      417 2023-06-25 13:09:13.349781 gentle_mxml-0.3.1/docs/_build/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-20 06:40:23.406098 gentle_mxml-0.3.1/docs/_build/_static/file.png
--rw-r--r--   0        0        0     1249 2023-06-25 13:09:13.379779 gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar-readthedocs.css
--rw-r--r--   0        0        0    10567 2023-06-25 13:09:13.375780 gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar.js
--rw-r--r--   0        0        0    22222 2023-06-25 13:09:13.401779 gentle_mxml-0.3.1/docs/_build/_static/insipid.css
--rw-r--r--   0        0        0     5269 2023-05-08 04:53:11.827459 gentle_mxml-0.3.1/docs/_build/_static/insipid.js
--rw-r--r--   0        0        0     4758 2023-06-25 13:09:13.354781 gentle_mxml-0.3.1/docs/_build/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.3.1/docs/_build/_static/minus.png
--rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.3.1/docs/_build/_static/plus.png
--rw-r--r--   0        0        0     4846 2023-06-25 13:09:13.343781 gentle_mxml-0.3.1/docs/_build/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-20 06:40:23.408098 gentle_mxml-0.3.1/docs/_build/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-20 06:40:23.408098 gentle_mxml-0.3.1/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    17289 2023-06-25 13:09:13.115790 gentle_mxml-0.3.1/docs/_build/contributing.html
--rw-r--r--   0        0        0    12858 2023-06-25 13:09:13.286783 gentle_mxml-0.3.1/docs/_build/genindex.html
--rw-r--r--   0        0        0    13806 2023-06-25 13:09:13.132790 gentle_mxml-0.3.1/docs/_build/getting-started.html
--rw-r--r--   0        0        0    13514 2023-06-25 13:09:13.148789 gentle_mxml-0.3.1/docs/_build/index.html
--rw-r--r--   0        0        0    14768 2023-06-25 13:09:13.164788 gentle_mxml-0.3.1/docs/_build/installation.html
--rw-r--r--   0        0        0      508 2023-06-25 13:09:13.405779 gentle_mxml-0.3.1/docs/_build/objects.inv
--rw-r--r--   0        0        0     8996 2023-06-25 13:09:13.312782 gentle_mxml-0.3.1/docs/_build/py-modindex.html
--rw-r--r--   0        0        0    28930 2023-06-25 13:09:13.221786 gentle_mxml-0.3.1/docs/_build/reference.html
--rw-r--r--   0        0        0     7918 2023-06-25 13:09:13.341781 gentle_mxml-0.3.1/docs/_build/search.html
--rw-r--r--   0        0        0     7181 2023-06-25 13:09:13.404778 gentle_mxml-0.3.1/docs/_build/searchindex.js
--rw-r--r--   0        0        0      702 2023-06-25 13:09:13.407778 gentle_mxml-0.3.1/docs/_build/sitemap.xml
--rw-r--r--   0        0        0    15966 2023-06-25 13:09:13.248785 gentle_mxml-0.3.1/docs/_build/toc.html
--rw-r--r--   0        0        0        0 2023-06-25 12:32:02.812195 gentle_mxml-0.3.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-25 12:32:06.444044 gentle_mxml-0.3.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      217 2023-06-26 13:39:30.085763 gentle_mxml-0.3.1/docs/api/gentle.generators.bower.rst
--rw-r--r--   0        0        0      217 2023-06-26 13:39:30.096762 gentle_mxml-0.3.1/docs/api/gentle.generators.cargo.rst
--rw-r--r--   0        0        0      229 2023-06-26 13:39:30.105762 gentle_mxml-0.3.1/docs/api/gentle.generators.composer.rst
--rw-r--r--   0        0        0      213 2023-06-26 13:39:30.118761 gentle_mxml-0.3.1/docs/api/gentle.generators.doap.rst
--rw-r--r--   0        0        0      217 2023-06-26 13:39:30.129761 gentle_mxml-0.3.1/docs/api/gentle.generators.hpack.rst
--rw-r--r--   0        0        0      209 2023-06-26 13:39:30.139761 gentle_mxml-0.3.1/docs/api/gentle.generators.npm.rst
--rw-r--r--   0        0        0      230 2023-06-26 13:39:30.149760 gentle_mxml-0.3.1/docs/api/gentle.generators.pkg_info.rst
--rw-r--r--   0        0        0      233 2023-06-26 13:39:30.159760 gentle_mxml-0.3.1/docs/api/gentle.generators.pyproject.rst
--rw-r--r--   0        0        0      521 2023-06-26 13:39:30.047764 gentle_mxml-0.3.1/docs/api/gentle.generators.rst
--rw-r--r--   0        0        0      221 2023-06-26 13:39:30.170759 gentle_mxml-0.3.1/docs/api/gentle.generators.shards.rst
--rw-r--r--   0        0        0      326 2023-06-26 13:39:30.059764 gentle_mxml-0.3.1/docs/api/gentle.metadata.rst
--rw-r--r--   0        0        0      241 2023-06-26 13:39:30.178759 gentle_mxml-0.3.1/docs/api/gentle.metadata.utils.rst
--rw-r--r--   0        0        0      204 2023-06-26 13:39:29.750777 gentle_mxml-0.3.1/docs/api/gentle.rst
--rw-r--r--   0        0        0     1722 2023-07-01 23:16:33.074157 gentle_mxml-0.3.1/docs/conf.py
--rw-r--r--   0        0        0     1614 2023-06-26 18:32:13.013266 gentle_mxml-0.3.1/docs/contributing.rst
--rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.3.1/docs/getting-started.rst
--rw-r--r--   0        0        0      456 2023-06-25 12:43:37.704408 gentle_mxml-0.3.1/docs/index.rst
--rw-r--r--   0        0        0      546 2023-06-26 18:21:56.391213 gentle_mxml-0.3.1/docs/installation.rst
--rw-r--r--   0        0        0      197 2023-06-26 13:35:46.178048 gentle_mxml-0.3.1/docs/reference.rst
--rw-r--r--   0        0        0      305 2023-07-01 22:50:55.661323 gentle_mxml-0.3.1/docs/release-notes.rst
--rw-r--r--   0        0        0      338 2023-07-01 22:51:29.247945 gentle_mxml-0.3.1/docs/toc.rst
--rw-r--r--   0        0        0      162 2023-07-01 23:16:33.074157 gentle_mxml-0.3.1/gentle/__init__.py
--rw-r--r--   0        0        0     2512 2023-07-01 22:40:42.721486 gentle_mxml-0.3.1/gentle/__main__.py
--rw-r--r--   0        0        0      967 2023-06-28 15:28:10.118254 gentle_mxml-0.3.1/gentle/generators/__init__.py
--rw-r--r--   0        0        0     1661 2023-06-28 22:07:13.223836 gentle_mxml-0.3.1/gentle/generators/bower.py
--rw-r--r--   0        0        0     3061 2023-06-23 06:42:42.354791 gentle_mxml-0.3.1/gentle/generators/cargo.py
--rw-r--r--   0        0        0     2429 2023-06-28 22:08:17.555203 gentle_mxml-0.3.1/gentle/generators/composer.py
--rw-r--r--   0        0        0     2157 2023-06-28 22:08:38.229357 gentle_mxml-0.3.1/gentle/generators/doap.py
--rw-r--r--   0        0        0     2528 2023-06-28 22:08:52.124788 gentle_mxml-0.3.1/gentle/generators/hpack.py
--rw-r--r--   0        0        0     2705 2023-06-28 22:09:13.317921 gentle_mxml-0.3.1/gentle/generators/npm.py
--rw-r--r--   0        0        0      376 2023-06-26 11:47:57.742065 gentle_mxml-0.3.1/gentle/generators/python/__init__.py
--rw-r--r--   0        0        0     2625 2023-06-26 11:53:28.465383 gentle_mxml-0.3.1/gentle/generators/python/pkg_info.py
--rw-r--r--   0        0        0     2385 2023-06-28 22:07:44.380561 gentle_mxml-0.3.1/gentle/generators/python/pyproject.py
--rw-r--r--   0        0        0     1922 2023-06-11 14:05:23.291217 gentle_mxml-0.3.1/gentle/generators/shards.py
--rw-r--r--   0        0        0     3642 2023-06-28 22:03:01.445140 gentle_mxml-0.3.1/gentle/metadata/__init__.py
--rw-r--r--   0        0        0     1555 2023-06-28 21:25:57.964830 gentle_mxml-0.3.1/gentle/metadata/types.py
--rw-r--r--   0        0        0     3206 2023-06-26 13:40:45.503635 gentle_mxml-0.3.1/gentle/metadata/utils.py
--rw-r--r--   0        0        0        0 2023-07-01 22:18:06.920291 gentle_mxml-0.3.1/gentle/pms/__init__.py
--rw-r--r--   0        0        0     3051 2023-07-01 22:16:34.191111 gentle_mxml-0.3.1/gentle/pms/portagepm.py
--rw-r--r--   0        0        0        0 2023-06-23 06:33:13.040427 gentle_mxml-0.3.1/gentle/py.typed
--rw-r--r--   0        0        0     1762 2023-06-26 18:38:20.296348 gentle_mxml-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.3.1/tests/bower/__init__.py
--rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.3.1/tests/bower/aurelia/bower.json
--rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.3.1/tests/bower/aurelia/bower.json.license
--rw-r--r--   0        0        0      151 2023-06-14 11:53:43.708296 gentle_mxml-0.3.1/tests/bower/aurelia/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.3.1/tests/bower/aurelia/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.1/tests/bower/pkg_empty/bower.json
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.1/tests/bower/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.3.1/tests/bower/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.3.1/tests/cargo/__init__.py
--rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml
--rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml.license
--rw-r--r--   0        0        0      163 2023-06-21 17:42:36.044548 gentle_mxml-0.3.1/tests/cargo/lemmy/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.3.1/tests/cargo/lemmy/metadata.xml.license
--rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml
--rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml.license
--rw-r--r--   0        0        0      189 2023-06-07 19:42:12.112203 gentle_mxml-0.3.1/tests/cargo/orjson/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.3.1/tests/cargo/orjson/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.1/tests/cargo/pkg_empty/Cargo.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.1/tests/cargo/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.3.1/tests/cargo/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.3.1/tests/composer/__init__.py
--rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.3.1/tests/composer/composer/composer.json
--rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.3.1/tests/composer/composer/composer.json.license
--rw-r--r--   0        0        0      318 2023-06-11 14:01:02.564058 gentle_mxml-0.3.1/tests/composer/composer/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.3.1/tests/composer/composer/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.1/tests/composer/pkg_empty/composer.json
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.1/tests/composer/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.3.1/tests/composer/test_generator.py
--rw-r--r--   0        0        0      346 2023-06-28 22:01:32.014811 gentle_mxml-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.439617 gentle_mxml-0.3.1/tests/doap/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-25 11:59:51.296133 gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap
--rw-r--r--   0        0        0      193 2023-06-25 12:01:58.282890 gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap.license
--rw-r--r--   0        0        0      329 2023-06-25 12:03:47.156396 gentle_mxml-0.3.1/tests/doap/gnome-calls/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-25 12:00:30.912497 gentle_mxml-0.3.1/tests/doap/gnome-calls/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.441617 gentle_mxml-0.3.1/tests/doap/pkg_empty/null.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:58:21.257850 gentle_mxml-0.3.1/tests/doap/pkg_multiple/one.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:58:24.041735 gentle_mxml-0.3.1/tests/doap/pkg_multiple/two.doap
--rw-r--r--   0        0        0        0 2023-06-25 11:57:38.444617 gentle_mxml-0.3.1/tests/doap/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1243 2023-06-25 11:59:31.351956 gentle_mxml-0.3.1/tests/doap/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.776769 gentle_mxml-0.3.1/tests/hpack/__init__.py
--rw-r--r--   0        0        0      197 2023-06-21 23:10:21.212904 gentle_mxml-0.3.1/tests/hpack/hpack/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 23:09:22.249333 gentle_mxml-0.3.1/tests/hpack/hpack/metadata.xml.license
--rw-r--r--   0        0        0     1398 2023-06-21 23:08:08.575369 gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml
--rw-r--r--   0        0        0       90 2023-06-21 23:09:09.245869 gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml.license
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.780768 gentle_mxml-0.3.1/tests/hpack/pkg_empty/package.yaml
--rw-r--r--   0        0        0        0 2023-06-21 23:06:21.783768 gentle_mxml-0.3.1/tests/hpack/pkg_none/.gitkeep
--rw-r--r--   0        0        0      117 2023-06-21 23:11:51.765173 gentle_mxml-0.3.1/tests/hpack/stack/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 23:10:32.554437 gentle_mxml-0.3.1/tests/hpack/stack/metadata.xml.license
--rw-r--r--   0        0        0    10727 2023-06-21 23:11:25.944237 gentle_mxml-0.3.1/tests/hpack/stack/package.yaml
--rw-r--r--   0        0        0       91 2023-06-21 23:16:13.343396 gentle_mxml-0.3.1/tests/hpack/stack/package.yaml.license
--rw-r--r--   0        0        0     1117 2023-06-21 23:07:37.239659 gentle_mxml-0.3.1/tests/hpack/test_generator.py
--rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.3.1/tests/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.3.1/tests/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.3.1/tests/npm/__init__.py
--rw-r--r--   0        0        0      234 2023-06-08 00:13:02.172234 gentle_mxml-0.3.1/tests/npm/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.3.1/tests/npm/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json
--rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.3.1/tests/npm/pkg_empty/package.json
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.3.1/tests/npm/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.3.1/tests/npm/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.866553 gentle_mxml-0.3.1/tests/pkg_info/__init__.py
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO
--rw-r--r--   0        0        0      103 2023-06-24 18:59:44.869553 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO.license
--rw-r--r--   0        0        0      303 2023-06-24 19:09:17.624922 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-24 18:59:44.869553 gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.1/tests/pkg_info/pkg_empty/PKG-INFO
--rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.1/tests/pkg_info/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1883 2023-02-18 15:55:47.929912 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO
--rw-r--r--   0        0        0       92 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO.license
--rw-r--r--   0        0        0      214 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-24 18:59:44.868553 gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/metadata.xml.license
--rw-r--r--   0        0        0     1149 2023-06-26 11:51:52.074371 gentle_mxml-0.3.1/tests/pkg_info/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.3.1/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      330 2023-06-07 19:13:56.979345 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml
--rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.1/tests/pyproject/pkg_empty/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.1/tests/pyproject/pkg_none/.gitkeep
--rw-r--r--   0        0        0      214 2023-06-07 18:58:47.333338 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/metadata.xml.license
--rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml
--rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml.license
--rw-r--r--   0        0        0     1158 2023-06-26 11:51:38.121948 gentle_mxml-0.3.1/tests/pyproject/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.3.1/tests/shards/__init__.py
--rw-r--r--   0        0        0      262 2023-06-07 16:08:13.258065 gentle_mxml-0.3.1/tests/shards/athena-spec/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.3.1/tests/shards/athena-spec/metadata.xml.license
--rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.3.1/tests/shards/athena-spec/shard.yml
--rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.3.1/tests/shards/athena-spec/shard.yml.license
--rw-r--r--   0        0        0      254 2023-06-07 18:34:22.044597 gentle_mxml-0.3.1/tests/shards/exception_page/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.3.1/tests/shards/exception_page/metadata.xml.license
--rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.3.1/tests/shards/exception_page/shard.yml
--rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.3.1/tests/shards/exception_page/shard.yml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.3.1/tests/shards/pkg_empty/shard.yml
--rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.3.1/tests/shards/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.3.1/tests/shards/test_generator.py
--rw-r--r--   0        0        0     1239 2023-06-28 22:09:49.764429 gentle_mxml-0.3.1/tests/test_metadata.py
--rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.3.1/tests/utils.py
--rw-r--r--   0        0        0      619 2023-06-26 18:38:06.720903 gentle_mxml-0.3.1/tox.ini
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 gentle_mxml-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2023-07-05 14:01:37.568840 gentle_mxml-0.4.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       85 2023-06-25 13:58:30.249547 gentle_mxml-0.4.0/.bumpversion.cfg.license
+-rw-r--r--   0        0        0      384 2023-06-26 18:36:20.326251 gentle_mxml-0.4.0/.drone.yml
+-rw-r--r--   0        0        0      171 2023-07-05 00:47:18.753056 gentle_mxml-0.4.0/.gitignore
+-rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.4.0/LICENSE
+-rw-r--r--   0        0        0    34020 2023-06-21 17:54:08.857916 gentle_mxml-0.4.0/LICENSES/AGPL-3.0-only.txt
+-rw-r--r--   0        0        0    10280 2023-06-07 19:43:48.069665 gentle_mxml-0.4.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     1460 2023-06-21 23:16:06.355684 gentle_mxml-0.4.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0     7048 2022-11-14 10:12:41.100101 gentle_mxml-0.4.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-06-25 12:08:33.459576 gentle_mxml-0.4.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-06-07 16:20:14.601959 gentle_mxml-0.4.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2855 2023-07-02 01:35:13.743401 gentle_mxml-0.4.0/LICENSES/PHP-3.01.txt
+-rw-r--r--   0        0        0      432 2022-11-14 10:12:40.671121 gentle_mxml-0.4.0/LICENSES/WTFPL.txt
+-rw-r--r--   0        0        0     3213 2023-07-05 13:35:44.620545 gentle_mxml-0.4.0/README.md
+-rw-r--r--   0        0        0      230 2023-06-25 13:09:13.402778 gentle_mxml-0.4.0/docs/_build/.buildinfo
+-rw-r--r--   0        0        0     9939 2023-06-25 13:09:12.274825 gentle_mxml-0.4.0/docs/_build/.doctrees/contributing.doctree
+-rw-r--r--   0        0        0   119130 2023-06-25 13:09:12.772805 gentle_mxml-0.4.0/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     4893 2023-06-25 13:09:12.284825 gentle_mxml-0.4.0/docs/_build/.doctrees/getting-started.doctree
+-rw-r--r--   0        0        0     5207 2023-06-25 13:09:12.293825 gentle_mxml-0.4.0/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0        0        0     6471 2023-06-25 13:09:12.307824 gentle_mxml-0.4.0/docs/_build/.doctrees/installation.doctree
+-rw-r--r--   0        0        0    43744 2023-06-25 13:09:12.755805 gentle_mxml-0.4.0/docs/_build/.doctrees/reference.doctree
+-rw-r--r--   0        0        0     4901 2023-06-25 13:09:12.765805 gentle_mxml-0.4.0/docs/_build/.doctrees/toc.doctree
+-rw-r--r--   0        0        0     8129 2023-06-25 13:09:13.319782 gentle_mxml-0.4.0/docs/_build/404.html
+-rw-r--r--   0        0        0     1458 2023-06-25 12:55:03.457995 gentle_mxml-0.4.0/docs/_build/_sources/contributing.rst.txt
+-rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.4.0/docs/_build/_sources/getting-started.rst.txt
+-rw-r--r--   0        0        0      456 2023-06-25 12:43:37.704408 gentle_mxml-0.4.0/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0        0        0      619 2023-06-25 12:45:58.431577 gentle_mxml-0.4.0/docs/_build/_sources/installation.rst.txt
+-rw-r--r--   0        0        0      301 2023-06-25 13:09:09.222952 gentle_mxml-0.4.0/docs/_build/_sources/reference.rst.txt
+-rw-r--r--   0        0        0      321 2023-06-25 13:05:45.723384 gentle_mxml-0.4.0/docs/_build/_sources/toc.rst.txt
+-rw-r--r--   0        0        0    14813 2023-06-25 13:09:13.360780 gentle_mxml-0.4.0/docs/_build/_static/basic.css
+-rw-r--r--   0        0        0     4472 2023-06-20 06:40:23.406098 gentle_mxml-0.4.0/docs/_build/_static/doctools.js
+-rw-r--r--   0        0        0      417 2023-06-25 13:09:13.349781 gentle_mxml-0.4.0/docs/_build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-20 06:40:23.406098 gentle_mxml-0.4.0/docs/_build/_static/file.png
+-rw-r--r--   0        0        0     1249 2023-06-25 13:09:13.379779 gentle_mxml-0.4.0/docs/_build/_static/insipid-sidebar-readthedocs.css
+-rw-r--r--   0        0        0    10567 2023-06-25 13:09:13.375780 gentle_mxml-0.4.0/docs/_build/_static/insipid-sidebar.js
+-rw-r--r--   0        0        0    22222 2023-06-25 13:09:13.401779 gentle_mxml-0.4.0/docs/_build/_static/insipid.css
+-rw-r--r--   0        0        0     5269 2023-05-08 04:53:11.827459 gentle_mxml-0.4.0/docs/_build/_static/insipid.js
+-rw-r--r--   0        0        0     4758 2023-06-25 13:09:13.354781 gentle_mxml-0.4.0/docs/_build/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.4.0/docs/_build/_static/minus.png
+-rw-r--r--   0        0        0       90 2023-06-20 06:40:23.407098 gentle_mxml-0.4.0/docs/_build/_static/plus.png
+-rw-r--r--   0        0        0     4846 2023-06-25 13:09:13.343781 gentle_mxml-0.4.0/docs/_build/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-20 06:40:23.408098 gentle_mxml-0.4.0/docs/_build/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-20 06:40:23.408098 gentle_mxml-0.4.0/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    17289 2023-06-25 13:09:13.115790 gentle_mxml-0.4.0/docs/_build/contributing.html
+-rw-r--r--   0        0        0    12858 2023-06-25 13:09:13.286783 gentle_mxml-0.4.0/docs/_build/genindex.html
+-rw-r--r--   0        0        0    13806 2023-06-25 13:09:13.132790 gentle_mxml-0.4.0/docs/_build/getting-started.html
+-rw-r--r--   0        0        0    13514 2023-06-25 13:09:13.148789 gentle_mxml-0.4.0/docs/_build/index.html
+-rw-r--r--   0        0        0    14768 2023-06-25 13:09:13.164788 gentle_mxml-0.4.0/docs/_build/installation.html
+-rw-r--r--   0        0        0      508 2023-06-25 13:09:13.405779 gentle_mxml-0.4.0/docs/_build/objects.inv
+-rw-r--r--   0        0        0     8996 2023-06-25 13:09:13.312782 gentle_mxml-0.4.0/docs/_build/py-modindex.html
+-rw-r--r--   0        0        0    28930 2023-06-25 13:09:13.221786 gentle_mxml-0.4.0/docs/_build/reference.html
+-rw-r--r--   0        0        0     7918 2023-06-25 13:09:13.341781 gentle_mxml-0.4.0/docs/_build/search.html
+-rw-r--r--   0        0        0     7181 2023-06-25 13:09:13.404778 gentle_mxml-0.4.0/docs/_build/searchindex.js
+-rw-r--r--   0        0        0      702 2023-06-25 13:09:13.407778 gentle_mxml-0.4.0/docs/_build/sitemap.xml
+-rw-r--r--   0        0        0    15966 2023-06-25 13:09:13.248785 gentle_mxml-0.4.0/docs/_build/toc.html
+-rw-r--r--   0        0        0        0 2023-06-25 12:32:02.812195 gentle_mxml-0.4.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-25 12:32:06.444044 gentle_mxml-0.4.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1722 2023-07-05 14:01:37.567840 gentle_mxml-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0     1614 2023-06-26 18:32:13.013266 gentle_mxml-0.4.0/docs/contributing.rst
+-rw-r--r--   0        0        0      450 2023-06-25 12:49:53.056856 gentle_mxml-0.4.0/docs/getting-started.rst
+-rw-r--r--   0        0        0      727 2023-07-04 20:31:53.391263 gentle_mxml-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0      588 2023-07-04 23:39:17.982630 gentle_mxml-0.4.0/docs/installation.rst
+-rw-r--r--   0        0        0      197 2023-06-26 13:35:46.178048 gentle_mxml-0.4.0/docs/reference.rst
+-rw-r--r--   0        0        0      747 2023-07-05 01:17:56.733580 gentle_mxml-0.4.0/docs/release-notes.rst
+-rw-r--r--   0        0        0      338 2023-07-01 22:51:29.247945 gentle_mxml-0.4.0/docs/toc.rst
+-rw-r--r--   0        0        0      162 2023-07-05 14:01:37.568840 gentle_mxml-0.4.0/gentle/__init__.py
+-rw-r--r--   0        0        0     3127 2023-07-05 01:16:44.943529 gentle_mxml-0.4.0/gentle/__main__.py
+-rw-r--r--   0        0        0     1031 2023-07-04 22:17:22.939422 gentle_mxml-0.4.0/gentle/generators/__init__.py
+-rw-r--r--   0        0        0     2247 2023-07-05 13:58:47.674809 gentle_mxml-0.4.0/gentle/generators/autoconf.py
+-rw-r--r--   0        0        0     1661 2023-06-28 22:07:13.223836 gentle_mxml-0.4.0/gentle/generators/bower.py
+-rw-r--r--   0        0        0     3061 2023-06-23 06:42:42.354791 gentle_mxml-0.4.0/gentle/generators/cargo.py
+-rw-r--r--   0        0        0     2429 2023-06-28 22:08:17.555203 gentle_mxml-0.4.0/gentle/generators/composer.py
+-rw-r--r--   0        0        0     2157 2023-06-28 22:08:38.229357 gentle_mxml-0.4.0/gentle/generators/doap.py
+-rw-r--r--   0        0        0     2528 2023-06-28 22:08:52.124788 gentle_mxml-0.4.0/gentle/generators/hpack.py
+-rw-r--r--   0        0        0     2705 2023-06-28 22:09:13.317921 gentle_mxml-0.4.0/gentle/generators/npm.py
+-rw-r--r--   0        0        0     1589 2023-07-05 00:44:05.351997 gentle_mxml-0.4.0/gentle/generators/nuspec.py
+-rw-r--r--   0        0        0     1840 2023-07-05 00:43:35.516222 gentle_mxml-0.4.0/gentle/generators/pear.py
+-rw-r--r--   0        0        0     2674 2023-07-05 00:42:43.349364 gentle_mxml-0.4.0/gentle/generators/pom.py
+-rw-r--r--   0        0        0     1859 2023-07-03 19:25:07.088581 gentle_mxml-0.4.0/gentle/generators/pubspec.py
+-rw-r--r--   0        0        0      620 2023-07-05 13:57:30.826961 gentle_mxml-0.4.0/gentle/generators/python/__init__.py
+-rw-r--r--   0        0        0     2732 2023-07-04 21:55:29.566346 gentle_mxml-0.4.0/gentle/generators/python/pkg_info.py
+-rw-r--r--   0        0        0     2389 2023-07-04 19:20:24.854278 gentle_mxml-0.4.0/gentle/generators/python/pyproject.py
+-rw-r--r--   0        0        0     2343 2023-07-04 19:53:38.344474 gentle_mxml-0.4.0/gentle/generators/python/setuptools.py
+-rw-r--r--   0        0        0     3479 2023-07-04 22:16:59.414388 gentle_mxml-0.4.0/gentle/generators/python/wheel.py
+-rw-r--r--   0        0        0     1918 2023-07-04 14:54:40.135657 gentle_mxml-0.4.0/gentle/generators/shards.py
+-rw-r--r--   0        0        0     3698 2023-07-05 12:50:39.155577 gentle_mxml-0.4.0/gentle/metadata/__init__.py
+-rw-r--r--   0        0        0     2255 2023-07-05 00:20:58.760934 gentle_mxml-0.4.0/gentle/metadata/types.py
+-rw-r--r--   0        0        0     3699 2023-07-05 01:25:37.650653 gentle_mxml-0.4.0/gentle/metadata/utils.py
+-rw-r--r--   0        0        0        0 2023-07-01 22:18:06.920291 gentle_mxml-0.4.0/gentle/pms/__init__.py
+-rw-r--r--   0        0        0     3051 2023-07-01 22:16:34.191111 gentle_mxml-0.4.0/gentle/pms/portagepm.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:33:13.040427 gentle_mxml-0.4.0/gentle/py.typed
+-rw-r--r--   0        0        0      292 2023-07-05 00:41:09.620213 gentle_mxml-0.4.0/gentle/utils.py
+-rw-r--r--   0        0        0     1915 2023-07-05 01:27:02.093185 gentle_mxml-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 18:19:11.866860 gentle_mxml-0.4.0/tests/autoconf/__init__.py
+-rwxr-xr-x   0        0        0   140927 2021-01-28 21:06:02.000000 gentle_mxml-0.4.0/tests/autoconf/autoconf/configure
+-rw-r--r--   0        0        0       97 2023-07-04 18:25:49.214563 gentle_mxml-0.4.0/tests/autoconf/autoconf/configure.license
+-rw-r--r--   0        0        0      131 2023-07-04 23:45:15.409953 gentle_mxml-0.4.0/tests/autoconf/autoconf/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-04 18:26:01.159073 gentle_mxml-0.4.0/tests/autoconf/autoconf/metadata.xml.license
+-rwxr-xr-x   0        0        0   504593 2023-07-04 18:38:22.408675 gentle_mxml-0.4.0/tests/autoconf/libsecp256k1/configure
+-rw-r--r--   0        0        0       73 2023-07-04 18:39:28.118980 gentle_mxml-0.4.0/tests/autoconf/libsecp256k1/configure.license
+-rw-r--r--   0        0        0      214 2023-07-04 23:45:18.338833 gentle_mxml-0.4.0/tests/autoconf/libsecp256k1/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-04 18:36:53.047339 gentle_mxml-0.4.0/tests/autoconf/libsecp256k1/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-07-04 18:19:11.871860 gentle_mxml-0.4.0/tests/autoconf/pkg_empty/configure
+-rw-r--r--   0        0        0        0 2023-07-04 18:19:11.873860 gentle_mxml-0.4.0/tests/autoconf/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1142 2023-07-04 18:36:38.811923 gentle_mxml-0.4.0/tests/autoconf/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.4.0/tests/bower/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.4.0/tests/bower/aurelia/bower.json
+-rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.4.0/tests/bower/aurelia/bower.json.license
+-rw-r--r--   0        0        0      179 2023-07-04 23:45:20.940726 gentle_mxml-0.4.0/tests/bower/aurelia/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.4.0/tests/bower/aurelia/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.4.0/tests/bower/pkg_empty/bower.json
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.4.0/tests/bower/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.4.0/tests/bower/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.4.0/tests/cargo/__init__.py
+-rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.4.0/tests/cargo/lemmy/Cargo.toml
+-rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.4.0/tests/cargo/lemmy/Cargo.toml.license
+-rw-r--r--   0        0        0      191 2023-07-04 23:45:23.484621 gentle_mxml-0.4.0/tests/cargo/lemmy/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.4.0/tests/cargo/lemmy/metadata.xml.license
+-rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.4.0/tests/cargo/orjson/Cargo.toml
+-rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.4.0/tests/cargo/orjson/Cargo.toml.license
+-rw-r--r--   0        0        0      217 2023-07-04 23:45:26.684490 gentle_mxml-0.4.0/tests/cargo/orjson/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.4.0/tests/cargo/orjson/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.4.0/tests/cargo/pkg_empty/Cargo.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.4.0/tests/cargo/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.4.0/tests/cargo/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.4.0/tests/composer/__init__.py
+-rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.4.0/tests/composer/composer/composer.json
+-rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.4.0/tests/composer/composer/composer.json.license
+-rw-r--r--   0        0        0      346 2023-07-04 23:45:29.884359 gentle_mxml-0.4.0/tests/composer/composer/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.4.0/tests/composer/composer/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.4.0/tests/composer/pkg_empty/composer.json
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.4.0/tests/composer/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.4.0/tests/composer/test_generator.py
+-rw-r--r--   0        0        0      346 2023-06-28 22:01:32.014811 gentle_mxml-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.439617 gentle_mxml-0.4.0/tests/doap/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-25 11:59:51.296133 gentle_mxml-0.4.0/tests/doap/gnome-calls/calls.doap
+-rw-r--r--   0        0        0      193 2023-06-25 12:01:58.282890 gentle_mxml-0.4.0/tests/doap/gnome-calls/calls.doap.license
+-rw-r--r--   0        0        0      357 2023-07-04 23:45:32.532250 gentle_mxml-0.4.0/tests/doap/gnome-calls/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-25 12:00:30.912497 gentle_mxml-0.4.0/tests/doap/gnome-calls/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.441617 gentle_mxml-0.4.0/tests/doap/pkg_empty/null.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:21.257850 gentle_mxml-0.4.0/tests/doap/pkg_multiple/one.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:24.041735 gentle_mxml-0.4.0/tests/doap/pkg_multiple/two.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.444617 gentle_mxml-0.4.0/tests/doap/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1243 2023-06-25 11:59:31.351956 gentle_mxml-0.4.0/tests/doap/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.776769 gentle_mxml-0.4.0/tests/hpack/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-04 23:45:37.686038 gentle_mxml-0.4.0/tests/hpack/hpack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:09:22.249333 gentle_mxml-0.4.0/tests/hpack/hpack/metadata.xml.license
+-rw-r--r--   0        0        0     1398 2023-06-21 23:08:08.575369 gentle_mxml-0.4.0/tests/hpack/hpack/package.yaml
+-rw-r--r--   0        0        0       90 2023-06-21 23:09:09.245869 gentle_mxml-0.4.0/tests/hpack/hpack/package.yaml.license
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.780768 gentle_mxml-0.4.0/tests/hpack/pkg_empty/package.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.783768 gentle_mxml-0.4.0/tests/hpack/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      145 2023-07-04 23:45:40.610918 gentle_mxml-0.4.0/tests/hpack/stack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:10:32.554437 gentle_mxml-0.4.0/tests/hpack/stack/metadata.xml.license
+-rw-r--r--   0        0        0    10727 2023-06-21 23:11:25.944237 gentle_mxml-0.4.0/tests/hpack/stack/package.yaml
+-rw-r--r--   0        0        0       91 2023-06-21 23:16:13.343396 gentle_mxml-0.4.0/tests/hpack/stack/package.yaml.license
+-rw-r--r--   0        0        0     1117 2023-06-21 23:07:37.239659 gentle_mxml-0.4.0/tests/hpack/test_generator.py
+-rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.4.0/tests/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.4.0/tests/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.4.0/tests/npm/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-04 23:45:43.491800 gentle_mxml-0.4.0/tests/npm/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.4.0/tests/npm/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.4.0/tests/npm/mkdocs-material/package.json
+-rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.4.0/tests/npm/mkdocs-material/package.json.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.4.0/tests/npm/pkg_empty/package.json
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.4.0/tests/npm/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.4.0/tests/npm/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:52.317293 gentle_mxml-0.4.0/tests/nuspec/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:52.319293 gentle_mxml-0.4.0/tests/nuspec/pkg_empty/null.nuspec
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:52.319293 gentle_mxml-0.4.0/tests/nuspec/pkg_multiple/one.nuspec
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:52.319293 gentle_mxml-0.4.0/tests/nuspec/pkg_multiple/two.nuspec
+-rw-r--r--   0        0        0        0 2023-07-04 14:58:52.320293 gentle_mxml-0.4.0/tests/nuspec/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      784 2023-07-04 15:00:56.648183 gentle_mxml-0.4.0/tests/nuspec/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-02 00:33:54.789465 gentle_mxml-0.4.0/tests/pear/__init__.py
+-rw-r--r--   0        0        0      867 2023-07-04 23:45:45.733708 gentle_mxml-0.4.0/tests/pear/pear/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-02 00:38:54.802152 gentle_mxml-0.4.0/tests/pear/pear/metadata.xml.license
+-rw-r--r--   0        0        0    55403 2023-07-02 00:35:58.869372 gentle_mxml-0.4.0/tests/pear/pear/package2.xml
+-rw-r--r--   0        0        0      462 2023-07-02 01:15:53.753044 gentle_mxml-0.4.0/tests/pear/pear/package2.xml.license
+-rw-r--r--   0        0        0      456 2023-07-04 23:45:48.396598 gentle_mxml-0.4.0/tests/pear/pecl-redis/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-02 01:25:37.027087 gentle_mxml-0.4.0/tests/pear/pecl-redis/metadata.xml.license
+-rw-r--r--   0        0        0    51276 2023-07-02 01:25:02.174518 gentle_mxml-0.4.0/tests/pear/pecl-redis/package.xml
+-rw-r--r--   0        0        0      257 2023-07-02 01:35:33.683582 gentle_mxml-0.4.0/tests/pear/pecl-redis/package.xml.license
+-rw-r--r--   0        0        0        0 2023-07-02 00:33:54.792465 gentle_mxml-0.4.0/tests/pear/pkg_empty/package.xml
+-rw-r--r--   0        0        0        0 2023-07-02 00:33:54.793465 gentle_mxml-0.4.0/tests/pear/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1117 2023-07-02 01:24:49.525038 gentle_mxml-0.4.0/tests/pear/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:18:08.266397 gentle_mxml-0.4.0/tests/pom/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-04 23:45:51.164485 gentle_mxml-0.4.0/tests/pom/maven/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-02 22:20:03.256676 gentle_mxml-0.4.0/tests/pom/maven/metadata.xml.license
+-rw-r--r--   0        0        0    25887 2023-07-02 22:19:54.555033 gentle_mxml-0.4.0/tests/pom/maven/pom.xml
+-rw-r--r--   0        0        0       93 2023-07-02 22:31:45.443845 gentle_mxml-0.4.0/tests/pom/maven/pom.xml.license
+-rw-r--r--   0        0        0        0 2023-07-02 22:18:08.271397 gentle_mxml-0.4.0/tests/pom/pkg_empty/pom.xml
+-rw-r--r--   0        0        0        0 2023-07-02 22:18:08.271397 gentle_mxml-0.4.0/tests/pom/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1099 2023-07-02 22:18:38.839142 gentle_mxml-0.4.0/tests/pom/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:50:56.509848 gentle_mxml-0.4.0/tests/pubspec/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:50:56.511848 gentle_mxml-0.4.0/tests/pubspec/pkg_empty/pubspec.yaml
+-rw-r--r--   0        0        0        0 2023-07-04 14:50:56.514848 gentle_mxml-0.4.0/tests/pubspec/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      652 2023-07-04 15:01:06.350784 gentle_mxml-0.4.0/tests/pubspec/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 20:57:51.000321 gentle_mxml-0.4.0/tests/python/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.866553 gentle_mxml-0.4.0/tests/python/pkg_info/__init__.py
+-rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gentle_mxml-0.4.0/tests/python/pkg_info/mkdocs-material/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-06-24 18:59:44.869553 gentle_mxml-0.4.0/tests/python/pkg_info/mkdocs-material/PKG-INFO.license
+-rw-r--r--   0        0        0      327 2023-07-04 23:46:08.433776 gentle_mxml-0.4.0/tests/python/pkg_info/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.869553 gentle_mxml-0.4.0/tests/python/pkg_info/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.4.0/tests/python/pkg_info/pkg_empty/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.4.0/tests/python/pkg_info/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1883 2023-02-18 15:55:47.929912 gentle_mxml-0.4.0/tests/python/pkg_info/pkgcraft/PKG-INFO
+-rw-r--r--   0        0        0       92 2023-06-24 18:59:44.868553 gentle_mxml-0.4.0/tests/python/pkg_info/pkgcraft/PKG-INFO.license
+-rw-r--r--   0        0        0      242 2023-07-04 23:46:10.884675 gentle_mxml-0.4.0/tests/python/pkg_info/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.868553 gentle_mxml-0.4.0/tests/python/pkg_info/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     1149 2023-06-26 11:51:52.074371 gentle_mxml-0.4.0/tests/python/pkg_info/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.4.0/tests/python/pyproject/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-04 23:46:13.181581 gentle_mxml-0.4.0/tests/python/pyproject/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.4.0/tests/python/pyproject/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.4.0/tests/python/pyproject/mkdocs-material/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.4.0/tests/python/pyproject/mkdocs-material/pyproject.toml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.4.0/tests/python/pyproject/pkg_empty/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.4.0/tests/python/pyproject/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      242 2023-07-04 23:46:15.468487 gentle_mxml-0.4.0/tests/python/pyproject/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.4.0/tests/python/pyproject/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.4.0/tests/python/pyproject/pkgcraft/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.4.0/tests/python/pyproject/pkgcraft/pyproject.toml.license
+-rw-r--r--   0        0        0     1158 2023-06-26 11:51:38.121948 gentle_mxml-0.4.0/tests/python/pyproject/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:00.332211 gentle_mxml-0.4.0/tests/python/setuptools/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-04 23:46:20.860265 gentle_mxml-0.4.0/tests/python/setuptools/django/metadata.xml
+-rw-r--r--   0        0        0       85 2023-07-04 19:42:43.349359 gentle_mxml-0.4.0/tests/python/setuptools/django/metadata.xml.license
+-rw-r--r--   0        0        0     2191 2023-07-04 19:39:14.825918 gentle_mxml-0.4.0/tests/python/setuptools/django/setup.cfg
+-rw-r--r--   0        0        0      126 2023-07-04 19:42:28.173982 gentle_mxml-0.4.0/tests/python/setuptools/django/setup.cfg.license
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:00.336211 gentle_mxml-0.4.0/tests/python/setuptools/pkg_empty/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:00.338211 gentle_mxml-0.4.0/tests/python/setuptools/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1141 2023-07-04 19:33:59.606854 gentle_mxml-0.4.0/tests/python/setuptools/test_generator.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:10:15.244768 gentle_mxml-0.4.0/tests/python/wheel/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-05 14:00:45.244986 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/pyproject.toml/UNKNOWN.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-07-05 14:00:45.251986 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/pyproject.toml/UNKNOWN.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-05 14:00:45.245986 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/pyproject.toml/UNKNOWN.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2023-07-05 14:00:45.245986 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/pyproject.toml/UNKNOWN.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2023-07-04 21:11:25.803871 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/pyproject.toml/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 21:11:35.819460 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/setup.cfg/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-04 21:11:30.978659 gentle_mxml-0.4.0/tests/python/wheel/pkg_empty/setup.py/setup.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:10:15.246768 gentle_mxml-0.4.0/tests/python/wheel/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      772 2023-07-04 21:22:09.965427 gentle_mxml-0.4.0/tests/python/wheel/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.4.0/tests/shards/__init__.py
+-rw-r--r--   0        0        0      290 2023-07-04 23:45:53.753378 gentle_mxml-0.4.0/tests/shards/athena-spec/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.4.0/tests/shards/athena-spec/metadata.xml.license
+-rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.4.0/tests/shards/athena-spec/shard.yml
+-rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.4.0/tests/shards/athena-spec/shard.yml.license
+-rw-r--r--   0        0        0      282 2023-07-04 23:45:56.515265 gentle_mxml-0.4.0/tests/shards/exception_page/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.4.0/tests/shards/exception_page/metadata.xml.license
+-rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.4.0/tests/shards/exception_page/shard.yml
+-rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.4.0/tests/shards/exception_page/shard.yml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.4.0/tests/shards/pkg_empty/shard.yml
+-rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.4.0/tests/shards/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.4.0/tests/shards/test_generator.py
+-rw-r--r--   0        0        0     1228 2023-07-04 23:47:12.466146 gentle_mxml-0.4.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.4.0/tests/utils.py
+-rw-r--r--   0        0        0      644 2023-07-05 00:39:05.410313 gentle_mxml-0.4.0/tox.ini
+-rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 gentle_mxml-0.4.0/PKG-INFO
```

### Comparing `gentle_mxml-0.3.1/LICENSES/AGPL-3.0-only.txt` & `gentle_mxml-0.4.0/LICENSES/AGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/LICENSES/Apache-2.0.txt` & `gentle_mxml-0.4.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/LICENSES/BSD-3-Clause.txt` & `gentle_mxml-0.4.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/LICENSES/CC0-1.0.txt` & `gentle_mxml-0.4.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/LICENSES/GPL-3.0-or-later.txt` & `gentle_mxml-0.4.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/LICENSES/MIT.txt` & `gentle_mxml-0.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/README.md` & `gentle_mxml-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,36 +4,50 @@
 gentle
 ======
 
 [![Build Status](https://drone.tildegit.org/api/badges/CyberTaIlor/gentle/status.svg)](https://drone.tildegit.org/CyberTaIlor/gentle)
 
 **Gent**oo **L**azy **E**ntry — a `metadata.xml` generator.
 
+If you need a distro-agnostic solution, try [upstream-ontologist][u-o]!
+
+[u-o]: https://github.com/jelmer/upstream-ontologist
+
 
 Supported generators
 --------------------
 
-* [Bower](https://github.com/bower/spec/blob/master/json.md)
 * Crystal ([Shards](https://github.com/crystal-lang/shards/blob/master/docs/shard.yml.adoc))
-* [DOAP](https://github.com/ewilderj/doap/wiki)
+* Dart ([Pub](https://dart.dev/tools/pub/pubspec))
 * Haskell ([Hpack](https://github.com/sol/hpack/blob/main/README.md))
-* Node.js ([npm](https://docs.npmjs.com/files/package.json/))
-* PHP ([Composer](https://getcomposer.org/doc/04-schema.md))
-* Python ([PEP 621](https://peps.python.org/pep-0621/) and [PEP 643](https://peps.python.org/pep-0643/))
+* Java ([Maven](https://maven.apache.org/pom.html))
+* .NET ([NuGet](https://learn.microsoft.com/en-us/nuget/reference/nuspec))
+* Node.js ([npm](https://docs.npmjs.com/files/package.json/), [Bower](https://github.com/bower/spec/blob/master/json.md))
+* PHP ([Composer](https://getcomposer.org/doc/04-schema.md), [PEAR/PECL](https://pear.php.net/manual/en/guide.developers.package2.php))
+* Python ([PEP 621](https://peps.python.org/pep-0621/), [PEP 643](https://peps.python.org/pep-0643/), [Setuptools](https://setuptools.pypa.io/en/latest/userguide/declarative_config.html))
 * Rust ([Cargo](https://doc.rust-lang.org/cargo/reference/manifest.html))
 
+Language-independent:
+
+* [DOAP](https://github.com/ewilderj/doap/wiki)
+* [GNU Autoconf](https://www.gnu.org/savannah-checkouts/gnu/autoconf/manual/autoconf-2.71/html_node/Initializing-configure.html)
+
 
 Dependencies
 ------------
 
-* [Portage](https://pypi.org/project/portage/)
-* [pkginfo](https://pypi.org/project/pkginfo/) *(optional)*
-* [PyYAML](https://pyyaml.org/) *(optional)*
-* [rdflib](https://pypi.org/project/rdflib/) *(optional)*
-* [Tomli](https://pypi.org/project/tomli/) *(optional)*
+* Required:
+  * [Portage](https://pypi.org/project/portage/)
+  * [lxml](https://lxml.de/)
+* Optional:
+  * [GNU Autoconf](https://www.gnu.org/software/autoconf/)
+  * [pkginfo](https://pypi.org/project/pkginfo/)
+  * [PyYAML](https://pyyaml.org/)
+  * [rdflib](https://pypi.org/project/rdflib/)
+  * [Tomli](https://pypi.org/project/tomli/)
 
 
 Installing
 ----------
 
 ### Gentoo
 
@@ -76,11 +90,21 @@
 ```
 
 [1]: https://git-send-email.io/
 [2]: https://git-scm.com/docs/git-request-pull
 [gh]: http://github.com/cybertailor/gentle
 
 
+IRC
+---
+
+You can join the `#gentle` channel either on [Libera Chat][libera] or
+[via Matrix][matrix].
+
+[libera]: https://libera.chat/
+[matrix]: https://matrix.to/#/#gentle:libera.chat
+
+
 License
 -------
 
 WTFPL
```

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/contributing.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/contributing.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/environment.pickle` & `gentle_mxml-0.4.0/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/getting-started.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/getting-started.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/index.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/installation.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/reference.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/.doctrees/toc.doctree` & `gentle_mxml-0.4.0/docs/_build/.doctrees/toc.doctree`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/404.html` & `gentle_mxml-0.4.0/docs/_build/404.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_sources/contributing.rst.txt` & `gentle_mxml-0.4.0/docs/_build/_sources/contributing.rst.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_sources/installation.rst.txt` & `gentle_mxml-0.4.0/docs/_build/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/basic.css` & `gentle_mxml-0.4.0/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/doctools.js` & `gentle_mxml-0.4.0/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar-readthedocs.css` & `gentle_mxml-0.4.0/docs/_build/_static/insipid-sidebar-readthedocs.css`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/insipid-sidebar.js` & `gentle_mxml-0.4.0/docs/_build/_static/insipid-sidebar.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/insipid.css` & `gentle_mxml-0.4.0/docs/_build/_static/insipid.css`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/insipid.js` & `gentle_mxml-0.4.0/docs/_build/_static/insipid.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/language_data.js` & `gentle_mxml-0.4.0/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/pygments.css` & `gentle_mxml-0.4.0/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/searchtools.js` & `gentle_mxml-0.4.0/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/_static/sphinx_highlight.js` & `gentle_mxml-0.4.0/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/contributing.html` & `gentle_mxml-0.4.0/docs/_build/contributing.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/genindex.html` & `gentle_mxml-0.4.0/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/getting-started.html` & `gentle_mxml-0.4.0/docs/_build/getting-started.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/index.html` & `gentle_mxml-0.4.0/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/installation.html` & `gentle_mxml-0.4.0/docs/_build/installation.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/py-modindex.html` & `gentle_mxml-0.4.0/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/reference.html` & `gentle_mxml-0.4.0/docs/_build/reference.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/search.html` & `gentle_mxml-0.4.0/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/searchindex.js` & `gentle_mxml-0.4.0/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/sitemap.xml` & `gentle_mxml-0.4.0/docs/_build/sitemap.xml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/_build/toc.html` & `gentle_mxml-0.4.0/docs/_build/toc.html`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/conf.py` & `gentle_mxml-0.4.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'gentle'
 copyright = '2022-2023, Anna <cyber@sysrq.in>'
 author = 'Anna <cyber@sysrq.in>'
-release = '0.3.1'
+release = '0.4.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autosummary',
     'sphinx.ext.autodoc',
```

### Comparing `gentle_mxml-0.3.1/docs/contributing.rst` & `gentle_mxml-0.4.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/docs/installation.rst` & `gentle_mxml-0.4.0/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 Installation
 ============
 
 Prerequisites
 -------------
 
-The only hard dependency is `Portage`_.
+The only hard dependencies are `Portage`_ and `lxml`_.
 
 All other dependencies are optional, you can find them in the
 :file:`pyproject.toml` file.
 
 .. _Portage: https://pypi.org/project/portage/
+.. _lxml: https://lxml.de/
 
 Gentoo
 ------
 
 gentle is packaged in the Gentoo repository.
 
 .. prompt:: bash #
```

### Comparing `gentle_mxml-0.3.1/gentle/__main__.py` & `gentle_mxml-0.4.0/gentle/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2022-2023 Anna <cyber@sysrq.in>
 # No warranty
 
+# pylint: disable=unused-import
+
 import argparse
 import importlib.util
 import logging
 import os
 import sys
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import gentle
 from gentle.generators import AbstractGenerator, GeneratorClass
 from gentle.metadata import MetadataXML
 
+import gentle.generators.autoconf
 import gentle.generators.bower
 import gentle.generators.cargo
 import gentle.generators.composer
 import gentle.generators.doap
 import gentle.generators.hpack
 import gentle.generators.npm
-import gentle.generators.python.pkg_info
+import gentle.generators.nuspec
+import gentle.generators.pear
+import gentle.generators.pubspec
 import gentle.generators.python.pyproject
+import gentle.generators.python.setuptools
+import gentle.generators.python.pkg_info
+import gentle.generators.python.wheel
 import gentle.generators.shards
 
 _HAS_PORTAGE = importlib.util.find_spec("portage") is not None
 
+_HAS_BUILD = importlib.util.find_spec("build") is not None
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("main")
 
 
 def main() -> None:
     """
     Parse command-line arguments and run the program.
@@ -38,20 +48,26 @@
     pm = []
     if _HAS_PORTAGE:
         pm.append("portage")
 
     if len(pm) == 0:
         raise RuntimeError("No package manager installed. Aborting")
 
+    py_api = ["simple"]
+    if _HAS_BUILD:
+        py_api.insert(0, "wheel")
+
     parser = argparse.ArgumentParser("gentle", description=gentle.__doc__)
     parser.add_argument("ebuild", type=Path, help="path to the ebuild file")
     parser.add_argument("--api", "-a", choices=pm, default=pm[0],
                         help="package manager API to use")
     parser.add_argument("--prefix", "-p",
                         help="value of EPREFIX")
+    parser.add_argument("--quick", "-q", action="store_true",
+                        help="skip slow generators")
     parser.add_argument("-v", action="version", version=gentle.__version__)
     args = parser.parse_args()
 
     if args.prefix is not None:
         os.environ["PORTAGE_OVERRIDE_EPREFIX"] = args.prefix
 
     with TemporaryDirectory(prefix="gentle-") as tmpdir:
@@ -67,15 +83,20 @@
             logger.error("Ebuild's metadata.xml file is missing, create it before running gentle")
             sys.exit(1)
 
         srcdir = src_unpack(args.ebuild, tmpdir)
         cls: GeneratorClass
         for cls in AbstractGenerator.get_generator_subclasses():
             generator = cls(srcdir)
-            if generator.active:
-                logger.info("Starting %s", cls.__name__)
-                generator.update_metadata_xml(mxml)
-    mxml.dump()
+            if not generator.active:
+                continue
+            if args.quick and generator.slow:
+                continue
+            logger.info("Starting %s", cls.__name__)
+            generator.update_metadata_xml(mxml)
+
+    if mxml.modified:
+        mxml.dump()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gentle_mxml-0.3.1/gentle/generators/__init__.py` & `gentle_mxml-0.4.0/gentle/generators/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,13 @@
         ...
 
     @property
     @abstractmethod
     def active(self) -> bool:
         ...
 
+    @property
+    def slow(self) -> bool:
+        return False
+
 
 GeneratorClass = Type[AbstractGenerator]
```

### Comparing `gentle_mxml-0.3.1/gentle/generators/bower.py` & `gentle_mxml-0.4.0/gentle/generators/bower.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/cargo.py` & `gentle_mxml-0.4.0/gentle/generators/cargo.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/composer.py` & `gentle_mxml-0.4.0/gentle/generators/composer.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/doap.py` & `gentle_mxml-0.4.0/gentle/generators/doap.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/hpack.py` & `gentle_mxml-0.4.0/gentle/generators/hpack.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/npm.py` & `gentle_mxml-0.4.0/gentle/generators/npm.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/gentle/generators/python/pkg_info.py` & `gentle_mxml-0.4.0/gentle/generators/python/pkg_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class PkgInfoGenerator(AbstractGenerator):
     def __init__(self, srcdir: Path):
         self.srcdir = srcdir
         self.pkg_info = srcdir / "PKG-INFO"
 
+    # pylint: disable=too-many-branches
     def update_metadata_xml(self, mxml: MetadataXML) -> None:
         package = pkginfo.UnpackedSDist(str(self.srcdir))
 
         maint_keys = (package.maintainer, package.maintainer_email)
         if maint_keys == (None, None):
             maint_keys = (package.author, package.author_email)
 
@@ -57,20 +58,21 @@
         for maint in map(extract_name_email, maintainers):
             if maint is None:
                 continue
             logger.info("Found upstream maintainer: %s", maint)
             mxml.add_upstream_maintainer(maint)
 
         if package.home_page is not None:
+            logger.info("Found homepage: %s", package.home_page)
             if (remote_id := extract_remote_id(package.home_page)) is not None:
                 mxml.add_upstream_remote_id(remote_id)
 
-        for url in package.project_urls:
-            name, value = [entry.strip()
-                           for entry in url.split(",", maxsplit=1)]
+        for entry in package.project_urls:
+            name, value = [item.strip()
+                           for item in entry.split(",", maxsplit=1)]
             logger.info("Found %s: %s", name, value)
             if name.lower() in BUG_TRACKER_LABELS:
                 mxml.set_upstream_bugs_to(value)
             elif name.lower() in CHANGELOG_LABELS:
                 mxml.set_upstream_changelog(value)
             elif name.lower() in DOCS_LABELS:
                 mxml.set_upstream_doc(value)
```

### Comparing `gentle_mxml-0.3.1/gentle/generators/python/pyproject.py` & `gentle_mxml-0.4.0/gentle/generators/python/pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         for maint in project.get(maint_key, {}):
             person = Person(name=maint.get("name", ""), email=maint.get("email", ""))
             logger.info("Found upstream maintainer: %s", person)
             if not person.name:
                 continue
             mxml.add_upstream_maintainer(person)
 
-        for name, value in project.get("urls").items():
+        for name, value in project.get("urls", {}).items():
             logger.info("Found %s: %s", name, value)
             if name.lower() in BUG_TRACKER_LABELS:
                 mxml.set_upstream_bugs_to(value)
             elif name.lower() in CHANGELOG_LABELS:
                 mxml.set_upstream_changelog(value)
             elif name.lower() in DOCS_LABELS:
                 mxml.set_upstream_doc(value)
```

### Comparing `gentle_mxml-0.3.1/gentle/generators/shards.py` & `gentle_mxml-0.4.0/gentle/generators/shards.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class ShardsGenerator(AbstractGenerator):
     def __init__(self, srcdir: Path):
         self.shard_yml = srcdir / "shard.yml"
 
     def update_metadata_xml(self, mxml: MetadataXML) -> None:
         with open(self.shard_yml) as file:
             if (shard := yaml.load(file, CLoader)) is None:
-                shard = {}
+                return
 
         for author in map(extract_name_email, shard.get("authors", [])):
             if author is None:
                 continue
             logger.info("Found upstream maintainer: %s", author)
             mxml.add_upstream_maintainer(author)
```

### Comparing `gentle_mxml-0.3.1/gentle/metadata/__init__.py` & `gentle_mxml-0.4.0/gentle/metadata/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
 """ Metadata routines """
 
 import logging
-import textwrap
-import xml.etree.ElementTree as ET
 from pathlib import Path
 from typing import Callable
 
+import lxml.etree as ET
+
 from gentle.metadata.types import Person, RemoteID, Upstream
 
 logger = logging.getLogger("metadata")
 
 
 class MetadataXML:
     """ Modify :file:`metadata.xml` files """
 
     def __init__(self, xmlfile: Path, parser: Callable[[Path], Upstream]):
         """
         :param xmlfile: Path to the :file:`metadata.xml` file
         :param upstream: Pre-parsed :class:`Upstream` object
         """
         self.xmlfile: Path = xmlfile
-        self.xml: ET.ElementTree = ET.parse(self.xmlfile)
+        self.xml: ET._ElementTree = ET.parse(self.xmlfile)
 
         self.upstream: Upstream = parser(xmlfile)
+        self.modified: bool = False
 
     def dump(self) -> None:
         """ Write :file:`metadata.xml` file """
         logger.info("Writing metadata.xml")
         ET.indent(self.xml, space="\t", level=0)
-        with open(self.xmlfile, "w") as file:
-            file.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "https://www.gentoo.org/dtd/metadata.dtd">
-            """))
-            self.xml.write(file, encoding="unicode")
-            file.write("\n")
+        self.xml.write(self.xmlfile,
+                       xml_declaration=True,
+                       pretty_print=True,
+                       encoding="UTF-8")
 
     def dumps(self) -> str:
         """ Convert the object to text """
         ET.indent(self.xml, space="\t", level=0)
         return ET.tostring(self.xml.getroot(), encoding="unicode")
 
     def add_upstream_maintainer(self, person: Person) -> None:
@@ -51,58 +49,69 @@
             return
 
         logger.info("Adding upstream maintainer: %s", person)
         self.upstream.maintainers.append(person)
         upstream = self._make_upstream_element()
         upstream.append(person.to_xml())
 
+        self.modified = True
+
     def add_upstream_remote_id(self, remote_id: RemoteID) -> None:
         """ Add an item to the list of remote ids """
-        if remote_id in self.upstream.remote_ids:
-            return
+        for old_remote_id in self.upstream.remote_ids:
+            if remote_id.attr == old_remote_id.attr:
+                return
 
         logger.info("Adding remote id: %s", remote_id)
         self.upstream.remote_ids.append(remote_id)
         upstream = self._make_upstream_element()
         upstream.append(remote_id.to_xml())
 
+        self.modified = True
+
     def set_upstream_bugs_to(self, url: str) -> None:
         """ Set upstream bugs-to URL """
         if self.upstream.bugs_to:
             return
 
         logger.info("Setting upstream bug tracker to %s", url)
         self.upstream.bugs_to = url
 
         upstream = self._make_upstream_element()
         bugs_to = ET.SubElement(upstream, "bugs-to")
         bugs_to.text = url
 
+        self.modified = True
+
     def set_upstream_changelog(self, url: str) -> None:
         """ Set upstream changelog URL """
         if self.upstream.changelog:
             return
 
         logger.info("Setting upstream changelog to %s", url)
         self.upstream.changelog = url
 
         upstream = self._make_upstream_element()
         changelog = ET.SubElement(upstream, "changelog")
         changelog.text = url
 
+        self.modified = True
+
     def set_upstream_doc(self, url: str) -> None:
         """ Set upstream documentation URL """
         if self.upstream.doc:
             return
 
         logger.info("Setting upstream documentation to %s", url)
         self.upstream.doc = url
 
         upstream = self._make_upstream_element()
         doc = ET.SubElement(upstream, "doc")
         doc.text = url
 
-    def _make_upstream_element(self) -> ET.Element:
+        self.modified = True
+
+    def _make_upstream_element(self) -> ET._Element:
         if (upstream := self.xml.find("upstream")) is None:
             pkgmetadata = self.xml.getroot()
             upstream = ET.SubElement(pkgmetadata, "upstream")
         return upstream
```

### Comparing `gentle_mxml-0.3.1/gentle/metadata/types.py` & `gentle_mxml-0.4.0/gentle/metadata/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
 """ Types for working with Gentoo package metadata """
 
-import xml.etree.ElementTree as ET
 from dataclasses import dataclass, field
+from enum import Enum, auto
+
+import lxml.etree as ET
+
+
+class MaintainerStatus(Enum):
+    """ Maintainer status enum """
+
+    NONE = auto()
+    ACTIVE = auto()
+    INACTIVE = auto()
 
 
 @dataclass
 class Person:
     """ Representation of a person"""
 
     name: str = field(default="", compare=False)
     email: str = ""
+    status: MaintainerStatus = MaintainerStatus.NONE
+
+    def __str__(self) -> str:
+        if self.name and self.email:
+            return f"{self.name} <{self.email}>"
 
-    def to_xml(self, attrib: dict | None = None) -> ET.Element:
+        if self.email:
+            return self.email
+
+        return self.name
+
+    def to_xml(self, attrib: dict | None = None) -> ET._Element:
         """
         :param attrib: attributes for the ``<maintainer>`` tag
         :return: :file:`metadata.xml` respresentation of a person
         """
-        result = ET.Element("maintainer", attrib=attrib or {})
+        attrib = attrib or {}
+        match self.status:
+            case MaintainerStatus.ACTIVE:
+                attrib["status"] = "active"
+            case MaintainerStatus.INACTIVE:
+                attrib["status"] = "inactive"
+
+        result = ET.Element("maintainer", attrib=attrib)
         if self.name:
             name_elem = ET.SubElement(result, "name")
             name_elem.text = self.name
         if self.email:
             email_elem = ET.SubElement(result, "email")
             email_elem.text = self.email
 
@@ -34,15 +61,18 @@
 @dataclass
 class RemoteID:
     """ Representation of a remote ID """
 
     attr: str
     value: str
 
-    def to_xml(self) -> ET.Element:
+    def __str__(self) -> str:
+        return f"{self.attr}:{self.value}"
+
+    def to_xml(self) -> ET._Element:
         """
         :return: :file:`metadata.xml` respresentation of a remote id
         """
         remote_elem = ET.Element("remote-id", type=self.attr)
         remote_elem.text = self.value
         return remote_elem
```

### Comparing `gentle_mxml-0.3.1/gentle/pms/portagepm.py` & `gentle_mxml-0.4.0/gentle/pms/portagepm.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/pyproject.toml` & `gentle_mxml-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 authors = [
     {name = "Anna", email = "cyber@sysrq.in"}
 ]
 dynamic = ["version", "description"]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
-dependencies = ["portage"]
+dependencies = [
+    "portage",
+    "lxml"
+]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: DFSG approved",
     "Operating System :: POSIX",
     "Topic :: System :: Software Distribution",
     "Topic :: Utilities"
 ]
@@ -28,15 +31,17 @@
 [project.optional-dependencies]
 # PKG-INFO
 pkginfo = ["pkginfo"]
 # DOAP
 rdf = ["rdflib"]
 # Cargo.toml, pyproject.toml
 toml = ["tomli; python_version <= '3.11'"]
-# package.yaml, shard.yml
+# Python packaging
+wheel = ["build"]
+# package.yaml, pubspec.yaml, shard.yml
 yaml = ["PyYAML"]
 
 docs = [
     "insipid-sphinx-theme",
     "sphinx",
     "sphinx-prompt"
 ]
@@ -48,23 +53,27 @@
 [project.scripts]
 gentle = "gentle.__main__:main"
 
 [project.urls]
 Home = "https://gentle.sysrq.in"
 Source = "https://git.sysrq.in/gentle"
 Issues = "https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=gentle"
+Changelog = "https://gentle.sysrq.in/release-notes.html"
 
 [tool.flit.module]
 name = "gentle"
 
 [tool.flit.sdist]
 include = [
     "docs/",
     "tests/"
 ]
+exclude = [
+    "docs/api/"
+]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 [tool.mypy]
 disallow_untyped_defs = true
 no_implicit_optional = true
@@ -77,11 +86,11 @@
 disallow_untyped_defs = false
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
     "portage.*",
     "tomllib.*",
-    "xml.sax._exceptions.*",
+    "xml.sax._exceptions",
     "xmldiff.*"
 ]
 ignore_missing_imports = true
```

### Comparing `gentle_mxml-0.3.1/tests/bower/aurelia/bower.json` & `gentle_mxml-0.4.0/tests/bower/aurelia/bower.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/bower/test_generator.py` & `gentle_mxml-0.4.0/tests/bower/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/cargo/lemmy/Cargo.toml` & `gentle_mxml-0.4.0/tests/cargo/lemmy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/cargo/orjson/Cargo.toml` & `gentle_mxml-0.4.0/tests/cargo/orjson/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/cargo/test_generator.py` & `gentle_mxml-0.4.0/tests/cargo/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/composer/composer/composer.json` & `gentle_mxml-0.4.0/tests/composer/composer/composer.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/composer/test_generator.py` & `gentle_mxml-0.4.0/tests/composer/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/doap/gnome-calls/calls.doap` & `gentle_mxml-0.4.0/tests/doap/gnome-calls/calls.doap`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/doap/test_generator.py` & `gentle_mxml-0.4.0/tests/doap/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/hpack/hpack/package.yaml` & `gentle_mxml-0.4.0/tests/hpack/hpack/package.yaml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/hpack/stack/package.yaml` & `gentle_mxml-0.4.0/tests/hpack/stack/package.yaml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/hpack/test_generator.py` & `gentle_mxml-0.4.0/tests/hpack/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/npm/mkdocs-material/package.json` & `gentle_mxml-0.4.0/tests/npm/mkdocs-material/package.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/npm/test_generator.py` & `gentle_mxml-0.4.0/tests/npm/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pkg_info/mkdocs-material/PKG-INFO` & `gentle_mxml-0.4.0/tests/python/pkg_info/mkdocs-material/PKG-INFO`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pkg_info/pkgcraft/PKG-INFO` & `gentle_mxml-0.4.0/tests/python/pkg_info/pkgcraft/PKG-INFO`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pkg_info/test_generator.py` & `gentle_mxml-0.4.0/tests/python/pkg_info/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pyproject/mkdocs-material/pyproject.toml` & `gentle_mxml-0.4.0/tests/python/pyproject/mkdocs-material/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pyproject/pkgcraft/pyproject.toml` & `gentle_mxml-0.4.0/tests/python/pyproject/pkgcraft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/pyproject/test_generator.py` & `gentle_mxml-0.4.0/tests/python/pyproject/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/shards/test_generator.py` & `gentle_mxml-0.4.0/tests/shards/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.3.1/tests/test_metadata.py` & `gentle_mxml-0.4.0/tests/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
-import xml.etree.ElementTree as ET
+import lxml.etree as ET
 
 from gentle.metadata.types import Person, RemoteID
 
 
 def test_person_to_xml():
     person = Person(name="Larry the Cow", email="larry@gentoo.org")
     assert (
```

### Comparing `gentle_mxml-0.3.1/tox.ini` & `gentle_mxml-0.4.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     lint
     py310
     py311
 
 [testenv]
 description = run the tests with pytest
 deps =
+    lxml-stubs
     mypy
     types-PyYAML
 extras =
     pkginfo
     rdf
     test
+    wheel
     yaml
 commands =
     pytest -vv {tty:--color=yes} {posargs}
     mypy {posargs:gentle tests}
 
 [testenv:lint]
 description = run the linters
```

### Comparing `gentle_mxml-0.3.1/PKG-INFO` & `gentle_mxml-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 Metadata-Version: 2.1
 Name: gentle-mxml
-Version: 0.3.1
+Version: 0.4.0
 Summary: Gentoo Metadata XML generator 
 Author-email: Anna <cyber@sysrq.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: Operating System :: POSIX
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Dist: portage
+Requires-Dist: lxml
 Requires-Dist: insipid-sphinx-theme ; extra == "docs"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-prompt ; extra == "docs"
 Requires-Dist: pkginfo ; extra == "pkginfo"
 Requires-Dist: rdflib ; extra == "rdf"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: xmldiff ; extra == "test"
 Requires-Dist: tomli ; extra == "toml" and ( python_version <= '3.11')
+Requires-Dist: build ; extra == "wheel"
 Requires-Dist: PyYAML ; extra == "yaml"
+Project-URL: Changelog, https://gentle.sysrq.in/release-notes.html
 Project-URL: Home, https://gentle.sysrq.in
 Project-URL: Issues, https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=gentle
 Project-URL: Source, https://git.sysrq.in/gentle
 Provides-Extra: docs
 Provides-Extra: pkginfo
 Provides-Extra: rdf
 Provides-Extra: test
 Provides-Extra: toml
+Provides-Extra: wheel
 Provides-Extra: yaml
 
 <!-- SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in> -->
 <!-- SPDX-License-Identifier: CC0-1.0 -->
 
 gentle
 ======
 
 [![Build Status](https://drone.tildegit.org/api/badges/CyberTaIlor/gentle/status.svg)](https://drone.tildegit.org/CyberTaIlor/gentle)
 
 **Gent**oo **L**azy **E**ntry — a `metadata.xml` generator.
 
+If you need a distro-agnostic solution, try [upstream-ontologist][u-o]!
+
+[u-o]: https://github.com/jelmer/upstream-ontologist
+
 
 Supported generators
 --------------------
 
-* [Bower](https://github.com/bower/spec/blob/master/json.md)
 * Crystal ([Shards](https://github.com/crystal-lang/shards/blob/master/docs/shard.yml.adoc))
-* [DOAP](https://github.com/ewilderj/doap/wiki)
+* Dart ([Pub](https://dart.dev/tools/pub/pubspec))
 * Haskell ([Hpack](https://github.com/sol/hpack/blob/main/README.md))
-* Node.js ([npm](https://docs.npmjs.com/files/package.json/))
-* PHP ([Composer](https://getcomposer.org/doc/04-schema.md))
-* Python ([PEP 621](https://peps.python.org/pep-0621/) and [PEP 643](https://peps.python.org/pep-0643/))
+* Java ([Maven](https://maven.apache.org/pom.html))
+* .NET ([NuGet](https://learn.microsoft.com/en-us/nuget/reference/nuspec))
+* Node.js ([npm](https://docs.npmjs.com/files/package.json/), [Bower](https://github.com/bower/spec/blob/master/json.md))
+* PHP ([Composer](https://getcomposer.org/doc/04-schema.md), [PEAR/PECL](https://pear.php.net/manual/en/guide.developers.package2.php))
+* Python ([PEP 621](https://peps.python.org/pep-0621/), [PEP 643](https://peps.python.org/pep-0643/), [Setuptools](https://setuptools.pypa.io/en/latest/userguide/declarative_config.html))
 * Rust ([Cargo](https://doc.rust-lang.org/cargo/reference/manifest.html))
 
+Language-independent:
+
+* [DOAP](https://github.com/ewilderj/doap/wiki)
+* [GNU Autoconf](https://www.gnu.org/savannah-checkouts/gnu/autoconf/manual/autoconf-2.71/html_node/Initializing-configure.html)
+
 
 Dependencies
 ------------
 
-* [Portage](https://pypi.org/project/portage/)
-* [pkginfo](https://pypi.org/project/pkginfo/) *(optional)*
-* [PyYAML](https://pyyaml.org/) *(optional)*
-* [rdflib](https://pypi.org/project/rdflib/) *(optional)*
-* [Tomli](https://pypi.org/project/tomli/) *(optional)*
+* Required:
+  * [Portage](https://pypi.org/project/portage/)
+  * [lxml](https://lxml.de/)
+* Optional:
+  * [GNU Autoconf](https://www.gnu.org/software/autoconf/)
+  * [pkginfo](https://pypi.org/project/pkginfo/)
+  * [PyYAML](https://pyyaml.org/)
+  * [rdflib](https://pypi.org/project/rdflib/)
+  * [Tomli](https://pypi.org/project/tomli/)
 
 
 Installing
 ----------
 
 ### Gentoo
 
@@ -110,12 +128,22 @@
 ```
 
 [1]: https://git-send-email.io/
 [2]: https://git-scm.com/docs/git-request-pull
 [gh]: http://github.com/cybertailor/gentle
 
 
+IRC
+---
+
+You can join the `#gentle` channel either on [Libera Chat][libera] or
+[via Matrix][matrix].
+
+[libera]: https://libera.chat/
+[matrix]: https://matrix.to/#/#gentle:libera.chat
+
+
 License
 -------
 
 WTFPL
```

