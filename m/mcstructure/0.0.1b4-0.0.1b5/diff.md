# Comparing `tmp/mcstructure-0.0.1b4.tar.gz` & `tmp/mcstructure-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcstructure-0.0.1b4.tar", last modified: Wed Feb  1 17:11:36 2023, max compression
+gzip compressed data, was "mcstructure-0.0.1b5.tar", last modified: Wed Jul  5 21:43:36 2023, max compression
```

## Comparing `mcstructure-0.0.1b4.tar` & `mcstructure-0.0.1b5.tar`

### file list

```diff
@@ -1,235 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/
--rw-r--r--   0 root         (0) root         (0)       66 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/.gitattributes
--rw-r--r--   0 root         (0) root         (0)     3265 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2660 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1909 2023-02-01 16:22:03.000000 mcstructure-0.0.1b4/README.md
--rw-r--r--   0 root         (0) root         (0)     2235 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/README_CN.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/_example_structures/
--rw-r--r--   0 root         (0) root         (0)     4914 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/_example_structures/awe.mcstructure
--rw-r--r--   0 root         (0) root         (0)      344 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/_example_structures/cube_const.mcstructure
--rw-r--r--   0 root         (0) root         (0)      344 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/_example_structures/cube_creates.mcstructure
--rw-r--r--   0 root         (0) root         (0)     2237 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/_example_structures/example_result.mcstructure
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/docs/
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/.buildinfo
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs/.nojekyll
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    14692 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/_static/basic.css
--rw-r--r--   0 root         (0) root         (0)    10766 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      429 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/file.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/docs/_static/images/
--rw-r--r--   0 root         (0) root         (0)     1186 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/images/logo_binder.svg
--rw-r--r--   0 root         (0) root         (0)     7601 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/images/logo_colab.png
--rw-r--r--   0 root         (0) root         (0)      681 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/images/logo_deepnote.svg
--rw-r--r--   0 root         (0) root         (0)     1758 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 root         (0) root         (0)   287630 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 root         (0) root         (0)    89476 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/jquery.js
--rw-r--r--   0 root         (0) root         (0)    10854 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/_static/language_data.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/docs/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1608 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/bg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.343488 mcstructure-0.0.1b4/docs/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1789 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/bn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1231 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1449 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1343 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1444 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1816 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/eo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1438 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/et/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1391 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1469 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1449 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/id/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1360 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1447 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/iw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1490 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.323488 mcstructure-0.0.1b4/docs/_static/locales/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1518 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ko/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1406 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/lt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ml/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1890 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/mr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1675 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1398 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/no/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1357 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1420 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ro/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1441 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1797 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/sk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1441 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/sr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1760 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1391 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ta/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1968 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/te/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1834 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/tg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1710 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/th/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1860 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/tl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.353488 mcstructure-0.0.1b4/docs/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1259 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1405 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1756 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/ur/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1460 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/vi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1487 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/zh_CN/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1279 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/locales/zh_TW/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     5510 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)      419 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/scripts/
--rw-r--r--   0 root         (0) root         (0)    87299 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 root         (0) root         (0)     3388 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 root         (0) root         (0)    15106 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 root         (0) root         (0)    16634 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/searchtools.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/styles/
--rw-r--r--   0 root         (0) root         (0)   162094 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 root         (0) root         (0)    20970 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 root         (0) root         (0)     5488 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/styles/theme.css
--rw-r--r--   0 root         (0) root         (0)    68420 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 root         (0) root         (0)    19530 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/underscore.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.363489 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/css/
--rw-r--r--   0 root         (0) root         (0)    58578 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/css/all.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.373489 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/
--rw-r--r--   0 root         (0) root         (0)   133034 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
--rw-r--r--   0 root         (0) root         (0)   715890 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
--rw-r--r--   0 root         (0) root         (0)   132728 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 root         (0) root         (0)    89824 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
--rw-r--r--   0 root         (0) root         (0)    76612 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 root         (0) root         (0)    34390 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
--rw-r--r--   0 root         (0) root         (0)   144322 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
--rw-r--r--   0 root         (0) root         (0)    34092 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 root         (0) root         (0)    16800 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
--rw-r--r--   0 root         (0) root         (0)    13584 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 root         (0) root         (0)   202902 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
--rw-r--r--   0 root         (0) root         (0)   897426 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
--rw-r--r--   0 root         (0) root         (0)   202616 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 root         (0) root         (0)   103300 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
--rw-r--r--   0 root         (0) root         (0)    79444 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 root         (0) root         (0)     1361 2023-01-30 17:44:23.000000 mcstructure-0.0.1b4/docs/_static/webpack-macros.html
--rw-r--r--   0 root         (0) root         (0)    28705 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/index.html
--rw-r--r--   0 root         (0) root         (0)      430 2023-01-30 17:44:42.000000 mcstructure-0.0.1b4/docs/objects.inv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/docs_src/
--rw-r--r--   0 root         (0) root         (0)      700 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs_src/Makefile
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs_src/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/docs_src/source/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-01-30 17:40:20.000000 mcstructure-0.0.1b4/docs_src/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs_src/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/docs_src/source/resources/
--rwxr-xr-x   0 root         (0) root         (0)     4592 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs_src/source/resources/mcstructure_logo.png
--rwxr-xr-x   0 root         (0) root         (0)     6159 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/docs_src/source/resources/mcstructure_logo_3d.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/examples/
--rw-r--r--   0 root         (0) root         (0)     1295 2023-02-01 17:06:01.000000 mcstructure-0.0.1b4/examples/barrel.mcstructure
--rw-r--r--   0 root         (0) root         (0)     6561 2023-02-01 17:06:01.000000 mcstructure-0.0.1b4/examples/caged_villager.mcstructure
--rw-r--r--   0 root         (0) root         (0)     1551 2023-02-01 17:06:01.000000 mcstructure-0.0.1b4/examples/dirt_house.mcstructure
--rw-r--r--   0 root         (0) root         (0)      129 2023-02-01 16:24:50.000000 mcstructure-0.0.1b4/examples/read_and_display.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-02-01 17:06:01.000000 mcstructure-0.0.1b4/examples/scarecrow.mcstructure
--rw-r--r--   0 root         (0) root         (0)      571 2023-02-01 16:49:12.000000 mcstructure-0.0.1b4/examples.py
--rwxr-xr-x   0 root         (0) root         (0)     6159 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/logo.png
--rw-r--r--   0 root         (0) root         (0)      947 2023-02-01 17:02:18.000000 mcstructure-0.0.1b4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.333488 mcstructure-0.0.1b4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/src/mcstructure/
--rw-r--r--   0 root         (0) root         (0)    14240 2023-02-01 16:58:23.000000 mcstructure-0.0.1b4/src/mcstructure/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-30 17:39:37.000000 mcstructure-0.0.1b4/src/mcstructure/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/src/mcstructure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2660 2023-02-01 17:11:36.000000 mcstructure-0.0.1b4/src/mcstructure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5069 2023-02-01 17:11:36.000000 mcstructure-0.0.1b4/src/mcstructure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 17:11:36.000000 mcstructure-0.0.1b4/src/mcstructure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-02-01 17:11:36.000000 mcstructure-0.0.1b4/src/mcstructure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-01 17:11:36.000000 mcstructure-0.0.1b4/src/mcstructure.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 17:11:36.383489 mcstructure-0.0.1b4/tests/
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-01 16:51:51.000000 mcstructure-0.0.1b4/tests/test_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.742893 mcstructure-0.0.1b5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.682893 mcstructure-0.0.1b5/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.702893 mcstructure-0.0.1b5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-02 17:04:38.000000 mcstructure-0.0.1b5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-02 17:04:38.000000 mcstructure-0.0.1b5/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-02 17:04:38.000000 mcstructure-0.0.1b5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.702893 mcstructure-0.0.1b5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-02 17:04:38.000000 mcstructure-0.0.1b5/.github/workflows/black.yaml
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-05 21:43:36.732893 mcstructure-0.0.1b5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/README.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/README_CN.md
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/README_DE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.712893 mcstructure-0.0.1b5/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/api.md
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-07-02 16:54:28.000000 mcstructure-0.0.1b5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/contributing.md
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)      800 2023-07-02 16:35:44.000000 mcstructure-0.0.1b5/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/docs/quickstart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.712893 mcstructure-0.0.1b5/examples/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-05 20:40:30.000000 mcstructure-0.0.1b5/examples/README.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/examples/area.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-05 20:55:54.000000 mcstructure-0.0.1b5/examples/diagonal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.712893 mcstructure-0.0.1b5/examples/pack/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-05 20:46:23.000000 mcstructure-0.0.1b5/examples/pack/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-07-05 20:55:54.000000 mcstructure-0.0.1b5/examples/pack/makepack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.712893 mcstructure-0.0.1b5/examples/pack/src/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-03 15:34:25.000000 mcstructure-0.0.1b5/examples/pack/src/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.712893 mcstructure-0.0.1b5/examples/pack/src/structures/
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-07-03 15:32:46.000000 mcstructure-0.0.1b5/examples/pack/src/structures/barrel.mcstructure
+-rw-r--r--   0 root         (0) root         (0)     6561 2023-07-03 15:32:46.000000 mcstructure-0.0.1b5/examples/pack/src/structures/caged_villager.mcstructure
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-07-03 15:32:46.000000 mcstructure-0.0.1b5/examples/pack/src/structures/dirt_house.mcstructure
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-03 15:32:46.000000 mcstructure-0.0.1b5/examples/pack/src/structures/scarecrow.mcstructure
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-02 16:46:06.000000 mcstructure-0.0.1b5/examples/read_and_display.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/examples/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.732893 mcstructure-0.0.1b5/examples/structures/
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/examples/structures/barrel.mcstructure
+-rw-r--r--   0 root         (0) root         (0)     6561 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/examples/structures/caged_villager.mcstructure
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/examples/structures/dirt_house.mcstructure
+-rw-r--r--   0 root         (0) root         (0)      573 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/examples/structures/scarecrow.mcstructure
+-rwxr-xr-x   0 root         (0) root         (0)     6159 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/logo.png
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-05 20:09:22.000000 mcstructure-0.0.1b5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 21:43:36.742893 mcstructure-0.0.1b5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.682893 mcstructure-0.0.1b5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.732893 mcstructure-0.0.1b5/src/mcstructure/
+-rw-r--r--   0 root         (0) root         (0)    16041 2023-07-05 21:41:37.000000 mcstructure-0.0.1b5/src/mcstructure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-08 16:31:53.000000 mcstructure-0.0.1b5/src/mcstructure/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.732893 mcstructure-0.0.1b5/src/mcstructure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-05 21:43:36.000000 mcstructure-0.0.1b5/src/mcstructure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-05 21:43:36.000000 mcstructure-0.0.1b5/src/mcstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 21:43:36.000000 mcstructure-0.0.1b5/src/mcstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-05 21:43:36.000000 mcstructure-0.0.1b5/src/mcstructure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-05 21:43:36.000000 mcstructure-0.0.1b5/src/mcstructure.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:43:36.732893 mcstructure-0.0.1b5/tests/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-02 16:54:28.000000 mcstructure-0.0.1b5/tests/test_block.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-05 21:27:24.000000 mcstructure-0.0.1b5/tests/test_structure.py
```

### Comparing `mcstructure-0.0.1b4/.gitignore` & `mcstructure-0.0.1b5/.gitignore`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/LICENSE.md` & `mcstructure-0.0.1b5/LICENSE.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 The-phoenixR
+Copyright (c) 2023 Jonas da Silva
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `mcstructure-0.0.1b4/PKG-INFO` & `mcstructure-0.0.1b5/README_DE.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,60 @@
-Metadata-Version: 2.1
-Name: mcstructure
-Version: 0.0.1b4
-Summary: Read and write Minecraft .mcstructure files.
-License: MIT
-Project-URL: Documentation, https://phoenixr-codes.github.io/mcstructure/
-Project-URL: Source Code, https://github.com/phoenixr-codes/mcstructure/
-Keywords: mcstructure,Minecraft
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Games/Entertainment
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE.md
-
 <p align="center">
   <img
     src="https://raw.githubusercontent.com/phoenixr-codes/mcstructure/main/logo.png"
     width="120px"
     align="center" alt="mcstructure logo"
   />
   <h1 align="center">mcstructure</h1>
   <p align="center">
-    Read and write Minecraft <code>.mcstructure</code> files.
+    Lesen und Schreiben von Minecraft <code>.mcstructure</code>-Dateien.
   </p>
 </p>
 
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-_In the entire project (and officially since 
-the "Better Together Update") the term
-"Minecraft" refers to the edition of Minecraft
-that is also known as "Bedrock Edition"._
+Diese README-Datei ist auch in den folgenden
+Sprachen verfügbar:
+
+* [🇨🇳 Chinesisch](./README_CN.md)
+* [🇬🇧 Englisch](./README.md)
+
+_Im gesamten Projekt (und offiziell seit dem
+"Better Together Update") ist mit "Minecraft"
+die Version gemeint, welche auch als "Bedrock
+Edition" bekannt ist._
 
-_Features that this library provide are only
-useful for the above named edition of Minecraft._
+_Features dieser Bibliothek sind nur in der
+oben genannten Edition von Minecraft nützlich._
 
 > **Warning**
-> This project is currently in BETA Version. Most
-> features will probably not work.
+> Dieses Projekt ist momentan in der BETA Version.
+> Die meisten Features sind somit instabil.
 
-This library lets you programmatically create
-and edit Minecraft structures. You are able to
-save these as ``.mcstructure`` files and for
-example use them in behavior packs.
-
-You may aswell read them to identify blocks and
-and entities that were saved with a Structure
-Block in-game.
+Diese Bibliothek ermöglicht es innerhalb eines
+Programmes Minecraft Strukturen zu editieren.
+Diese können dann als ``.mcstructure``-Datei
+gespeichert werden und beispielsweise in einem
+Verhaltenspaket genutzt werden.
+
+Es ist auch möglich, Blöcke und Entitäten zu
+identifizieren, welche mit einem Konstruktionsblock
+innerhalb des Spiels gespeichert wurden.
 
 
 Installation
 ------------
 
 ```bash
 pip install mcstructure
 ```
 
 
-Basic Usage
------------
+Demonstration
+-------------
 
 ```python
 from mcstructure import Block, Structure
 
 struct = Structure(
     (7, 7, 7),
     Block("minecraft:wool", color = "red")
@@ -81,20 +67,32 @@
     .set_block((4, 4, 4), Block("minecraft:grass"))
     .set_block((5, 5, 5), Block("minecraft:grass"))
     .set_block((6, 6, 6), Block("minecraft:grass"))
 )
 
 with open("house.mcstructure", "wb") as f:
     struct.dump(f)
-
 ```
 
 ```python
 with open("house.mcstructure", "rb") as f:
     struct = Structure.load(f)
-
 ```
 
+
+Nützliche Links
+---------------
+
+* [👋 Einführung zu Konstruktionsblöcken](https://learn.microsoft.com/en-us/minecraft/creator/documents/introductiontostructureblocks)
+* [📖 Bedrock Wiki](https://wiki.bedrock.dev/nbt/mcstructure.html#file-format)
+* [📖 Dokumentation](https://mcstructure.readthedocs.io/en/latest/)
+* [📁 Quellcode](https://github.com/phoenixr-codes/mcstructure)
+* [🐍 PyPI](https://pypi.org/project/mcstructure/)
+
 --------------------------------------------
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
+
+KEIN OFFIZIELLES MINECRAFT PRODUKT.
+NICHT VON MOJANG GENEHMIGT ODER MIT MOJANG
+ASSOZIIERT.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mcstructure-0.0.1b4/README.md` & `mcstructure-0.0.1b5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,37 +6,52 @@
   />
   <h1 align="center">mcstructure</h1>
   <p align="center">
     Read and write Minecraft <code>.mcstructure</code> files.
   </p>
 </p>
 
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+🌍 This README is also available in the following
+languages:
+
+* [🇨🇳 Chinese](./README_CN.md)
+* [🇩🇪 German](./README_DE.md)
+
+<!-- Not really accessible ♿️ but we get a better line
+than the default "<hr/>" or "---" --> 
+<h2></h2>
+
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/mcstructure/badge/?style=for-the-badge&version=latest)](https://mcstructure.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/mcstructure?style=for-the-badge)](https://pypi.org/project/mcstructure)
 
 _In the entire project (and officially since 
 the "Better Together Update") the term
 "Minecraft" refers to the edition of Minecraft
 that is also known as "Bedrock Edition"._
 
 _Features that this library provide are only
 useful for the above named edition of Minecraft._
 
 > **Warning**
-> This project is currently in BETA Version. Most
-> features will probably not work.
+> This project is currently in the **BETA** version. Some
+> features may not work as expected.
+
+<!-- start elevator-pitch -->
 
 This library lets you programmatically create
 and edit Minecraft structures. You are able to
 save these as ``.mcstructure`` files and for
 example use them in behavior packs.
 
-You may aswell read them to identify blocks and
+You may as well read them to identify blocks and
 and entities that were saved with a Structure
 Block in-game.
 
+<!-- end elevator-pitch -->
 
 Installation
 ------------
 
 ```bash
 pip install mcstructure
 ```
@@ -60,20 +75,28 @@
     .set_block((4, 4, 4), Block("minecraft:grass"))
     .set_block((5, 5, 5), Block("minecraft:grass"))
     .set_block((6, 6, 6), Block("minecraft:grass"))
 )
 
 with open("house.mcstructure", "wb") as f:
     struct.dump(f)
-
 ```
 
 ```python
 with open("house.mcstructure", "rb") as f:
     struct = Structure.load(f)
-
 ```
 
+
+Useful Links
+------------
+
+* [👋 Introduction to Structure Blocks](https://learn.microsoft.com/en-us/minecraft/creator/documents/introductiontostructureblocks)
+* [📖 Bedrock Wiki](https://wiki.bedrock.dev/nbt/mcstructure.html#file-format)
+* [📖 Documentation](https://mcstructure.readthedocs.io/en/latest/)
+* [📁 Source Code](https://github.com/phoenixr-codes/mcstructure)
+* [🐍 PyPI](https://pypi.org/project/mcstructure/)
+
 --------------------------------------------
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mcstructure-0.0.1b4/README_CN.md` & `mcstructure-0.0.1b5/README_CN.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 	/>
 	<h1 align="center">mcstructure</h1>
 	<p align="center">
 		对于《我的世界》<code>.mcstructure</code> 文件的读写操作库
 	</p>
 </p>
 
-*在此项目中（且更官方地是在“大一统更新”("Better Together Update")之后）专有名词《我的世界》("Minecraft")所指代的均为基岩版("Bedrock Edition")。*
+[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+此介绍文件亦可见翻译：
+
+* [🇪🇳 英文](./README.md)
+* [🇩🇪 德文](./README_DE.md)
+
+*在整个项目中（且更官方地是在“大一统更新”("Better Together Update")之后）专有名词《我的世界》("Minecraft")所指代的均为基岩版("Bedrock Edition")。*
 
 _此项目中的所有特性也是仅仅针对基岩版的。_
 
 > **请注意**
 > 此项目目前仍属于 BETA版本，因此很多的特性可能无法实现。
 
 此库可以让您以代码实现对 *《我的世界》* 结构文件的创建与编辑。
@@ -68,15 +75,25 @@
 
 	```python
 	with open("house.mcstructure", "rb") as f:
 		struct = Structure.load(f)
 
 	```
 
+妙用链接
+------------
+
+* [👋 结构方块的简介](https://learn.microsoft.com/en-us/minecraft/creator/documents/introductiontostructureblocks)
+* [📖 基岩版维基](https://wiki.bedrock.dev/nbt/mcstructure.html#file-format)
+_译注：文件结构文档已经被我翻译了，详见[我的译本](https://gitee.com/TriM-Organization/mcstructure/blob/main/docs/mcstructure%E6%96%87%E4%BB%B6%E7%BB%93%E6%9E%84.md)_
+* [📖 此项目之文档](https://mcstructure.readthedocs.io/en/latest/)
+* [📁 此项目之源码](https://github.com/phoenixr-codes/mcstructure)
+* [🐍 PyPI](https://pypi.org/project/mcstructure/)
+
 --------------------------------------------
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
 
 此项目并非一个官方 《我的世界》（*Minecraft*）项目
 
-此项目不隶属或关联于 Mojang Studios
+此项目不隶属或关联于 Mojang Studios
```

### Comparing `mcstructure-0.0.1b4/docs_src/Makefile` & `mcstructure-0.0.1b5/docs/Makefile`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
+SOURCEDIR     = .
+BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
-github:
-	@make singlehtml
-	@cp -a build/singlehtml/. ../docs
-
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mcstructure-0.0.1b4/docs_src/make.bat` & `mcstructure-0.0.1b5/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=source
-set BUILDDIR=build
+set SOURCEDIR=.
+set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `mcstructure-0.0.1b4/docs_src/source/resources/mcstructure_logo_3d.png` & `mcstructure-0.0.1b5/logo.png`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/examples/barrel.mcstructure` & `mcstructure-0.0.1b5/examples/pack/src/structures/barrel.mcstructure`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/examples/caged_villager.mcstructure` & `mcstructure-0.0.1b5/examples/pack/src/structures/caged_villager.mcstructure`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/examples/dirt_house.mcstructure` & `mcstructure-0.0.1b5/examples/pack/src/structures/dirt_house.mcstructure`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/examples/scarecrow.mcstructure` & `mcstructure-0.0.1b5/examples/pack/src/structures/scarecrow.mcstructure`

 * *Files identical despite different names*

### Comparing `mcstructure-0.0.1b4/pyproject.toml` & `mcstructure-0.0.1b5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mcstructure"
-version = "0.0.1b4"
+version = "0.0.1b5"
 description = "Read and write Minecraft .mcstructure files."
 dependencies = [
     "numpy>=1.21",
     "pynbt>=2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
@@ -26,16 +26,18 @@
 keywords = [
     "mcstructure",
     "Minecraft",
 ]
 
 [project.optional-dependencies]
 docs = [
-    "Sphinx<5,>3",
-    "sphinx-book-theme>=0.3",
+    "furo",
+    "myst-parser>=2",
+    "Sphinx>=7",
+    "sphinx-copybutton>=0",
 ]
 
 [project.urls]
-"Documentation" = "https://phoenixr-codes.github.io/mcstructure/"
+"Documentation" = "https://mcstructure.readthedocs.io/en/latest/"
 "Source Code" = "https://github.com/phoenixr-codes/mcstructure/"
```

### Comparing `mcstructure-0.0.1b4/src/mcstructure/__init__.py` & `mcstructure-0.0.1b5/src/mcstructure/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 """
-Read and write Minecraft .mcstructure files.
+Read and write Minecraft ``.mcstructure`` files.
 """
 
 # TODO: coordinates might be in wrong order (XYZ -> ZYX)
+# TODO: maybe make Block attributes properties
+# TODO: rename structure attr to blocks or something similar
 # TODO: make Structure._structure public
-# TODO: test mirror
-# TODO: test rotate
 # TODO: second layer (waterlogged blocks)
 # TODO: additional block data
 # TODO: entities
 # TODO: rename set_blocks to fill_blocks or create alias
 # TODO: export as 3d model (might be extension)
 # TODO: add shadow to logo
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import partial
 from itertools import repeat
 import json
-from typing import Any, BinaryIO, Optional, Tuple
+from typing import Any, BinaryIO, Tuple
 
 import numpy as np
 from numpy.typing import NDArray
 from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String  # type: ignore
 
+
 Coordinate = Tuple[int, int, int]
 
 
 COMPABILITY_VERSION: int = 17959425
+"""
+The compability version for a block. The four bytes making up this
+integer determine the game version number. For example, ``17879555`` is
+``01 10 D2 03`` in hex meaning ``1.16.210.03``.
+"""
+
+STRUCTURE_MAX_SIZE: tuple[int, int, int] = (64, 384, 64)
+"""The maximum size a structure can have."""
 
 
+# TODO: cover all tags
 def _into_pyobj(tag: BaseTag) -> Any:
     """
     Turns an NBT tree into a python tree.
     """
     if isinstance(tag, (TAG_Compound, dict)):
         res = {}
         for key, value in tag.items():
@@ -53,14 +63,15 @@
 
     if isinstance(tag, BaseTag):
         return tag.value
 
     return tag
 
 
+# TODO: cover all types
 def _into_tag(obj: Any) -> BaseTag:
     """
     Turn a python tree into an NBT tree.
     """
     if isinstance(obj, int):
         return TAG_Int(obj)
 
@@ -87,146 +98,226 @@
     """
     if with_prefix:
         name = name.replace(":", "", 1)
 
     return all((char.isalnum() and char in "-_") for char in name)
 
 
+def has_valid_size(size: tuple[int, int, int]) -> bool:
+    """Returns ``False`` if ``size`` is too big.
+
+    .. seealso:: :const:`STRUCTURE_MAX_SIZE`
+    """
+    return all(map(lambda n: n[0] <= n[1], zip(size, STRUCTURE_MAX_SIZE)))
+
+
 @dataclass(init=False)
 class Block:
     """
     Attributes
     ----------
     name
         The name of the block.
 
     states
         The states of the block.
 
-    Example
-    -------
+    Examples
+    --------
     .. code-block::
 
-        Block("minecraft:wool", color = "red")
+        Block("minecraft:wool", color="red")
+        Block("minecraft:grass")
+
     """
 
     identifier: str
     states: dict[str, Any]
 
     def __init__(self, identifier: str, **states: Any):
         """
         Parameters
         ----------
         identifier
             The identifier of the block (e.g. "minecraft:wool").
 
         states
-            The block states such as "color" or "stone_type".
+            The block states such as ``color`` or ``stone_type``.
             This varies by every block.
+
+            .. seealso:: https://learn.microsoft.com/en-us/minecraft/creator/reference/content/blockreference/examples/blockstateslist
         """
         self.identifier = identifier
         self.states = states
 
     def __str__(self) -> str:
         return self.stringify()
 
     def stringify(
         self,
         *,
         with_namespace: bool = True,
         with_states: bool = True,
     ) -> str:
+        """Returns a human-readable representation of the structure.
+
+        Parameters
+        ----------
+        with_namespace
+            Whether to include the block's namespace.
+
+        with_states
+            Whether to include the block's states.
+        """
         result = ""
-        if with_namespace and (ns := self.get_namespace()) is not None:
+        if with_namespace and (ns := self.namespace) is not None:
             result += ns + ":"
-        result += self.get_name()
+        result += self.name
         if with_states:
             result += f" [{json.dumps(self.states)[1:-1]}]"
         return result
 
-    def get_namespace_and_name(self) -> tuple[Optional[str], str]:
-        """
-        Returns the namespace and the name of the block.
+    @property
+    def namespace_and_name(self) -> tuple[str | None, str]:
+        """The namespace and the name of the block.
+
+        Examples
+        --------
+        .. code-block:: python
+
+            >>> from mcstructure import Block
+            >>>
+            >>> block = Block("minecraft:wool", color="red")
+            >>> block.namespace_and_name
+            ("minecraft", "wool")
+            >>>
+            >>> block = Block("foobar")
+            >>> block.namespace_and_name
+            (None, "foobar")
+
         """
         if ":" in self.identifier:
             ns, name = self.identifier.split(":", 1)
             return ns, name
 
         return (None, self.identifier)
 
-    def get_name(self) -> str:
-        """
-        Returns the name of the block.
-        """
-        return self.get_namespace_and_name()[1]
+    @property
+    def name(self) -> str:
+        """The name of the block.
+
+        Examples
+        --------
+        .. code-block:: python
+
+                >>> from mcstructure import Block
+                >>>
+                >>> block = Block("minecraft:wool", color="red")
+                >>> block.name
+                "wool"
+                >>>
+                >>> block = Block("foobar")
+                >>> block.name
+                "foobar"
 
-    def get_namespace(self) -> Optional[str]:
         """
-        Returns the namespace of the block.
+        return self.namespace_and_name[1]
+
+    @property
+    def namespace(self) -> str | None:
+        """The namespace of the block.
+
+        Examples
+        --------
+        .. code-block:: python
+
+                >>> from mcstructure import Block
+                >>>
+                >>> block = Block("minecraft:wool", color="red")
+                >>> block.namespace
+                "minecraft"
+                >>>
+                >>> block = Block("foobar")
+                >>> (block.namespace,)
+                (None,)
+
         """
-        return self.get_namespace_and_name()[0]
+        return self.namespace_and_name[0]
 
 
 class Structure:
-    """
-    Class representing a Minecraft structure that
-    consists of blocks and entities.
+    """Class representing a Minecraft structure that consists of blocks and entities.
 
     Attributes
     ----------
-    size
-        The size of the structure.
+    structure
+        The numpy array representing the blocks in the structure. Each entry is an ID
+        associated with a block present in :meth:`palette`.
     """
 
     def __init__(
-        self, size: tuple[int, int, int], fill: Optional[Block] = Block("minecraft:air")
-    ):
+        self,
+        size: tuple[int, int, int],
+        fill: Block | None = Block("minecraft:air"),
+    ) -> None:
         """
         Parameters
         ----------
         size
             The size of the structure.
 
         fill
             Fill the structure with this block at
             creation of a new structure object.
 
             If this is set to ``None`` the structure
             is filled with "Structure Void" blocks.
 
-            "minecraft:air" is used as default.
+            ``'minecraft:air'`` is used as default.
         """
-        self._structure: NDArray[np.intc]
+        if not has_valid_size(size):
+            raise ValueError(f"structure too large, max size: {STRUCTURE_MAX_SIZE}")
+
+        self.structure: NDArray[np.intc]
 
         self._size = size
         self._palette: list[Block] = []
 
         if fill is None:
-            self._structure = np.full(size, -1, dtype=np.intc)
+            self.structure = np.full(size, -1, dtype=np.intc)
 
         else:
-            self._structure = np.zeros(size, dtype=np.intc)
+            self.structure = np.zeros(size, dtype=np.intc)
             self._palette.append(fill)
 
     @classmethod
     def load(cls, file: BinaryIO):
         """
-        Loads an mcstructure file.
+        Loads a structure from a file.
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from mcstructure import Structure
+
+            with open("house.mcstructure", "rb") as f:
+                struct = Structure.load(f)
 
         Parameters
         ----------
         file
             File object to read.
         """
         nbt = NBTFile(file, little_endian=True)
         size: tuple[int, int, int] = tuple(x.value for x in nbt["size"])  # type: ignore
 
         struct = cls(size)
 
-        struct._structure = np.array(
+        struct.structure = np.array(
             [_into_pyobj(x) for x in nbt["structure"]["block_indices"][0]],
             dtype=np.intc,
         ).reshape(size)
 
         struct._palette.extend(
             [
                 Block(block["name"].value, **_into_pyobj(block["states"].value))
@@ -234,16 +325,23 @@
             ]
         )
 
         return struct
 
     @property
     def size(self) -> tuple[int, int, int]:
+        """The size of the structure."""
         return self._size
 
+    @property
+    def palette(self) -> list[Block]:
+        """A copy of the palette."""
+        palette = self._palette.copy()
+        return palette
+
     def __repr__(self) -> str:
         return repr(self._get_str_array())
 
     def __str__(self) -> str:
         return str(self._get_str_array())
 
     def _get_str_array(
@@ -265,15 +363,15 @@
         vec = np.vectorize(
             partial(
                 Block.stringify, with_namespace=with_namespace, with_states=with_states
             )
         )
         return vec(arr)
 
-    def _add_block_to_palette(self, block: Optional[Block]) -> int:
+    def _add_block_to_palette(self, block: Block | None) -> int:
         """
         Adds a block to the palette.
 
         Parameters
         ----------
         block
             The block to add. If this is set to ``None``
@@ -295,23 +393,33 @@
 
     def get_structure(self) -> NDArray[Any]:
         """
         Returns the structure as a numpy array filled
         with the corresponding block objects.
         """
         arr = np.full(
-            self._structure.shape, Block("minecraft:structure_void"), dtype=object
+            self.structure.shape, Block("minecraft:structure_void"), dtype=object
         )
         for key, block in enumerate(self._palette):
-            arr[self._structure == key] = block
+            arr[self.structure == key] = block
         return arr
 
     def dump(self, file: BinaryIO) -> None:
         """
-        Serialize the structure as a ``mcstructure``.
+        Serialize the structure as a NBT file.
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from mcstructure import Structure
+
+            struct = Structure((5, 5, 5), None)
+            with open("house.mcstructure", "wb") as f:
+                struct.dump(f)
 
         Parameters
         ----------
         file
             File object to write to.
         """
         nbt = NBTFile(
@@ -320,19 +428,19 @@
                 size=TAG_List(TAG_Int, map(TAG_Int, self._size)),
                 structure=TAG_Compound(
                     dict(
                         block_indices=TAG_List(
                             TAG_List,
                             [
                                 TAG_List(
-                                    TAG_Int, map(TAG_Int, self._structure.flatten())
+                                    TAG_Int, map(TAG_Int, self.structure.flatten())
                                 ),
                                 TAG_List(
                                     TAG_Int,
-                                    map(TAG_Int, repeat(-1, self._structure.size)),
+                                    map(TAG_Int, repeat(-1, self.structure.size)),
                                 ),
                             ],
                         ),
                         entities=TAG_List(TAG_Compound, []),
                         palette=TAG_Compound(
                             dict(
                                 default=TAG_Compound(
@@ -370,100 +478,62 @@
                 ),
                 structure_world_origin=TAG_List(TAG_Int, [0, 0, 0]),
             ),
             little_endian=True,
         )
         nbt.save(file, little_endian=True)
 
-    def mirror(self, axis: str) -> Structure:
-        """
-        Flips the structure.
-
-        Parameters
-        ----------
-        axis
-            Turn the structure either the ``X`` or ``Z`` axis.
-            Use ``"X"``, ``"x"``,``"Z"`` or ``"z"``.
-        """
-        if axis in "Xx":
-            self._structure = self._structure[::-1, :, :]
-        elif axis in "Zz":
-            self._structure = self._structure[:, :, ::-1]
-        else:
-            raise ValueError(f"invalid argument for 'rotation' ({axis!r})")
-        return self
-
-    def rotate(self, by: int) -> Structure:
-        """
-        Rotates the structure.
-
-        Parameters
-        ----------
-        by
-            Rotates the structure by ``90``, ``180``
-            or ``270`` degrees.
-        """
-        if by == 90:
-            self._structure = np.rot90(self._structure, k=1, axes=(0, 1))
-        elif by == 180:
-            self._structure = np.rot90(self._structure, k=2, axes=(0, 1))
-        elif by == 270:
-            self._structure = np.rot90(self._structure, k=3, axes=(0, 1))
-        else:
-            raise ValueError(f"invalid argument for 'by' ({by!r})")
-        return self
-
-    def get_block(self, coordinate: Coordinate) -> Optional[Block]:
+    def get_block(self, coordinate: Coordinate) -> Block | None:
         """
         Returns the block in a specific position.
 
         Parameters
         ----------
         coordinate
             The coordinte of the block.
         """
         x, y, z = coordinate
-        return self._palette[self._structure[x, y, z]]
+        return self._palette[self.structure[x, y, z]]
 
     def set_block(
         self,
         coordinate: Coordinate,
-        block: Optional[Block],
+        block: Block | None,
     ) -> Structure:
         """
-        Puts a block into the structure.
+        Places a block in the structure.
 
         Parameters
         ----------
         coordinate
             Relative coordinates of the block's position.
 
         block
             The block to place. If this is set to ``None``
             "Structure Void" blocks will be used.
         """
         x, y, z = coordinate
 
         ident = self._add_block_to_palette(block)
 
-        self._structure[x, y, z] = ident
+        self.structure[x, y, z] = ident
         return self
 
     def set_blocks(
         self,
         from_coordinate: Coordinate,
         to_coordinate: Coordinate,
         block: Block,
     ) -> Structure:
         """
-        Puts multiple blocks into the structure.
+        Fills an area in the structure with blocks.
 
         Notes
         -----
-        Both start and end points are filled.
+        Both start and end points are included.
 
         Parameters
         ----------
         from_coordinate
             Relative coordinates of the start edge.
 
         to_coordinate
@@ -473,16 +543,15 @@
             The block to place. If this is set to ``None``
             "STructure Void" blocks will be used to fill.
         """
         fx, fy, fz = from_coordinate
         tx, ty, tz = to_coordinate
 
         ident = self._add_block_to_palette(block)
-        # print([[[ident for k in range(abs(fz-tz)+1) ]for j in range(abs(fy-ty)+1)]for i in range(abs(fx-tx)+1)])
-        self._structure[fx : tx + 1, fy : ty + 1, fz : tz + 1] = np.array(
+        self.structure[fx : tx + 1, fy : ty + 1, fz : tz + 1] = np.array(
             [
                 [
                     [ident for k in range(abs(fz - tz) + 1)]
                     for j in range(abs(fy - ty) + 1)
                 ]
                 for i in range(abs(fx - tx) + 1)
             ],
```

### Comparing `mcstructure-0.0.1b4/src/mcstructure.egg-info/PKG-INFO` & `mcstructure-0.0.1b5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 Metadata-Version: 2.1
 Name: mcstructure
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Read and write Minecraft .mcstructure files.
 License: MIT
-Project-URL: Documentation, https://phoenixr-codes.github.io/mcstructure/
+Project-URL: Documentation, https://mcstructure.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/phoenixr-codes/mcstructure/
 Keywords: mcstructure,Minecraft
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-License-File: LICENSE.md
+License-File: LICENSE.txt
 
 <p align="center">
   <img
     src="https://raw.githubusercontent.com/phoenixr-codes/mcstructure/main/logo.png"
     width="120px"
     align="center" alt="mcstructure logo"
   />
   <h1 align="center">mcstructure</h1>
   <p align="center">
     Read and write Minecraft <code>.mcstructure</code> files.
   </p>
 </p>
 
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+🌍 This README is also available in the following
+languages:
+
+* [🇨🇳 Chinese](./README_CN.md)
+* [🇩🇪 German](./README_DE.md)
+
+<!-- Not really accessible ♿️ but we get a better line
+than the default "<hr/>" or "---" --> 
+<h2></h2>
+
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/mcstructure/badge/?style=for-the-badge&version=latest)](https://mcstructure.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/mcstructure?style=for-the-badge)](https://pypi.org/project/mcstructure)
 
 _In the entire project (and officially since 
 the "Better Together Update") the term
 "Minecraft" refers to the edition of Minecraft
 that is also known as "Bedrock Edition"._
 
 _Features that this library provide are only
 useful for the above named edition of Minecraft._
 
 > **Warning**
-> This project is currently in BETA Version. Most
-> features will probably not work.
+> This project is currently in the **BETA** version. Some
+> features may not work as expected.
+
+<!-- start elevator-pitch -->
 
 This library lets you programmatically create
 and edit Minecraft structures. You are able to
 save these as ``.mcstructure`` files and for
 example use them in behavior packs.
 
-You may aswell read them to identify blocks and
+You may as well read them to identify blocks and
 and entities that were saved with a Structure
 Block in-game.
 
+<!-- end elevator-pitch -->
 
 Installation
 ------------
 
 ```bash
 pip install mcstructure
 ```
@@ -81,20 +96,28 @@
     .set_block((4, 4, 4), Block("minecraft:grass"))
     .set_block((5, 5, 5), Block("minecraft:grass"))
     .set_block((6, 6, 6), Block("minecraft:grass"))
 )
 
 with open("house.mcstructure", "wb") as f:
     struct.dump(f)
-
 ```
 
 ```python
 with open("house.mcstructure", "rb") as f:
     struct = Structure.load(f)
-
 ```
 
+
+Useful Links
+------------
+
+* [👋 Introduction to Structure Blocks](https://learn.microsoft.com/en-us/minecraft/creator/documents/introductiontostructureblocks)
+* [📖 Bedrock Wiki](https://wiki.bedrock.dev/nbt/mcstructure.html#file-format)
+* [📖 Documentation](https://mcstructure.readthedocs.io/en/latest/)
+* [📁 Source Code](https://github.com/phoenixr-codes/mcstructure)
+* [🐍 PyPI](https://pypi.org/project/mcstructure/)
+
 --------------------------------------------
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

