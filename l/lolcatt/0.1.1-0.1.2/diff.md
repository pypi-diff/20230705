# Comparing `tmp/lolcatt-0.1.1.tar.gz` & `tmp/lolcatt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.1.1.tar", last modified: Tue Jul  4 18:22:41 2023, max compression
+gzip compressed data, was "lolcatt-0.1.2.tar", last modified: Tue Jul  4 22:04:20 2023, max compression
```

## Comparing `lolcatt-0.1.1.tar` & `lolcatt-0.1.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.067992 lolcatt-0.1.1/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       28 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.coveragerc
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      318 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.editorconfig
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      184 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.flake8
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.059992 lolcatt-0.1.1/.github/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      324 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.059992 lolcatt-0.1.1/.github/workflows/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2695 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.github/workflows/ci.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1589 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.github/workflows/coverage.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1707 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.github/workflows/docs.yml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1221 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.gitignore
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1416 2023-07-02 11:51:34.000000 lolcatt-0.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      708 2023-07-02 11:51:34.000000 lolcatt-0.1.1/Dockerfile
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-07-02 11:51:34.000000 lolcatt-0.1.1/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-07-02 11:51:34.000000 lolcatt-0.1.1/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3735 2023-07-02 11:51:34.000000 lolcatt-0.1.1/Makefile
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 18:22:41.067992 lolcatt-0.1.1/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-04 17:57:06.000000 lolcatt-0.1.1/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.059992 lolcatt-0.1.1/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.055991 lolcatt-0.1.1/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.055991 lolcatt-0.1.1/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-04 17:52:21.000000 lolcatt-0.1.1/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-04 17:52:21.000000 lolcatt-0.1.1/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-04 17:52:21.000000 lolcatt-0.1.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    18676 2023-07-04 17:46:35.000000 lolcatt-0.1.1/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-04 18:00:35.000000 lolcatt-0.1.1/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-07-04 12:57:37.000000 lolcatt-0.1.1/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-04 12:55:04.000000 lolcatt-0.1.1/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-04 17:52:18.000000 lolcatt-0.1.1/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-04 12:55:04.000000 lolcatt-0.1.1/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-04 12:55:04.000000 lolcatt-0.1.1/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-04 17:52:18.000000 lolcatt-0.1.1/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-07-02 11:51:34.000000 lolcatt-0.1.1/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-04 18:16:47.000000 lolcatt-0.1.1/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1142 2023-07-04 12:15:41.000000 lolcatt-0.1.1/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.1/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4701 2023-07-04 16:53:56.000000 lolcatt-0.1.1/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      563 2023-07-04 11:31:02.000000 lolcatt-0.1.1/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.1/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      333 2023-07-04 11:20:23.000000 lolcatt-0.1.1/lolcatt/ui/caster_static.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1442 2023-07-04 15:41:48.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3616 2023-07-04 16:07:21.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      854 2023-07-04 11:20:23.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1551 2023-07-04 16:35:18.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2379 2023-07-04 17:40:58.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      765 2023-07-04 13:34:42.000000 lolcatt-0.1.1/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 12:53:13.000000 lolcatt-0.1.1/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      604 2023-07-04 12:52:53.000000 lolcatt-0.1.1/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.063992 lolcatt-0.1.1/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1527 2023-07-04 18:22:41.000000 lolcatt-0.1.1/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       21 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-04 18:22:40.000000 lolcatt-0.1.1/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-04 18:16:47.000000 lolcatt-0.1.1/pyproject.toml
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.067992 lolcatt-0.1.1/requirements/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      240 2023-07-02 11:51:34.000000 lolcatt-0.1.1/requirements/dev.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       21 2023-07-02 11:51:34.000000 lolcatt-0.1.1/requirements/prod.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       44 2023-07-02 11:51:34.000000 lolcatt-0.1.1/requirements/test.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-04 18:22:41.067992 lolcatt-0.1.1/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-04 18:16:47.000000 lolcatt-0.1.1/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 18:22:41.067992 lolcatt-0.1.1/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-07-02 11:51:34.000000 lolcatt-0.1.1/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      317 2023-07-02 11:51:34.000000 lolcatt-0.1.1/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       28 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.coveragerc
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      318 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.editorconfig
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      184 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.flake8
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/.github/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      324 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/.github/workflows/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2695 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/ci.yml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1589 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/coverage.yml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1707 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.github/workflows/docs.yml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1221 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.gitignore
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1416 2023-07-02 11:51:34.000000 lolcatt-0.1.2/.pre-commit-config.yaml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      708 2023-07-02 11:51:34.000000 lolcatt-0.1.2/Dockerfile
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-07-02 11:51:34.000000 lolcatt-0.1.2/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-07-02 11:51:34.000000 lolcatt-0.1.2/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3735 2023-07-02 11:51:34.000000 lolcatt-0.1.2/Makefile
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 22:04:20.257699 lolcatt-0.1.2/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-04 17:57:06.000000 lolcatt-0.1.2/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.253698 lolcatt-0.1.2/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.249698 lolcatt-0.1.2/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.249698 lolcatt-0.1.2/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-04 21:53:55.000000 lolcatt-0.1.2/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-04 18:00:35.000000 lolcatt-0.1.2/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-04 18:00:35.000000 lolcatt-0.1.2/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-07-04 12:57:37.000000 lolcatt-0.1.2/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-04 21:53:52.000000 lolcatt-0.1.2/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-04 12:55:04.000000 lolcatt-0.1.2/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-04 21:53:52.000000 lolcatt-0.1.2/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-07-02 11:51:34.000000 lolcatt-0.1.2/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-04 21:50:56.000000 lolcatt-0.1.2/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1142 2023-07-04 21:40:08.000000 lolcatt-0.1.2/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.2/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5545 2023-07-04 21:58:28.000000 lolcatt-0.1.2/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1072 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 11:20:23.000000 lolcatt-0.1.2/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      323 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/ui/caster_static.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1442 2023-07-04 15:41:48.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3616 2023-07-04 16:07:21.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1258 2023-07-04 21:27:39.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1548 2023-07-04 21:52:43.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2378 2023-07-04 20:17:28.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      765 2023-07-04 13:34:42.000000 lolcatt-0.1.2/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 12:53:13.000000 lolcatt-0.1.2/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-04 21:45:55.000000 lolcatt-0.1.2/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1527 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-04 22:04:20.000000 lolcatt-0.1.2/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-04 21:50:56.000000 lolcatt-0.1.2/pyproject.toml
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/requirements/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      243 2023-07-04 22:01:38.000000 lolcatt-0.1.2/requirements/dev.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-04 20:19:58.000000 lolcatt-0.1.2/requirements/prod.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       44 2023-07-02 11:51:34.000000 lolcatt-0.1.2/requirements/test.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-04 22:04:20.261699 lolcatt-0.1.2/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-04 21:50:56.000000 lolcatt-0.1.2/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-04 22:04:20.257699 lolcatt-0.1.2/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-07-02 11:51:34.000000 lolcatt-0.1.2/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-04 21:49:29.000000 lolcatt-0.1.2/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.1/.github/workflows/ci.yml` & `lolcatt-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/.github/workflows/coverage.yml` & `lolcatt-0.1.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/.github/workflows/docs.yml` & `lolcatt-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/.gitignore` & `lolcatt-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/.pre-commit-config.yaml` & `lolcatt-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/Dockerfile` & `lolcatt-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/LICENSE` & `lolcatt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/Makefile` & `lolcatt-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/PKG-INFO` & `lolcatt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.1/README.rst` & `lolcatt-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/Makefile` & `lolcatt-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/_build/html/_static/basic.css` & `lolcatt-0.1.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/_build/html/_static/nature.css` & `lolcatt-0.1.2/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/_build/html/_static/pygments.css` & `lolcatt-0.1.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/_static/screenshot.png` & `lolcatt-0.1.2/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/conf.py` & `lolcatt-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/installation.rst` & `lolcatt-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/lolcatt.rst` & `lolcatt-0.1.2/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/lolcatt.ui.rst` & `lolcatt-0.1.2/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/docs/make.bat` & `lolcatt-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/lolcatt/app.py` & `lolcatt-0.1.2/lolcatt/app.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 class LolCatt(App):
     """The main application class for lolcatt."""
 
     CSS_PATH = 'ui/lolcatt.css'
 
     def __init__(self, device_name: str = None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
         self.caster = Caster(device_name)
+        super().__init__(*args, **kwargs)
         self._components = [
             LolCattDeviceInfo(caster=self.caster),
             LolCattPlaybackInfo(caster=self.caster),
             LolCattProgress(caster=self.caster),
             LolCattControls(caster=self.caster, exit_cb=self.exit),
             LolCattUrlInput(caster=self.caster),
         ]
```

### Comparing `lolcatt-0.1.1/lolcatt/casting/caster.py` & `lolcatt-0.1.2/lolcatt/casting/caster.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 import subprocess
+import sys
 import time
 from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 from catt.api import CattDevice
 from catt.api import discover
 from catt.cli import get_config_as_dict
+from catt.error import CastError
 
 
 @dataclass
 class CastState:
     """Dataclass for cast state, encapsulating info dictionaries of a catt controller."""
 
     cast_info: dict
@@ -25,28 +27,45 @@
 
     Provides a simple interface and enables exchange of the CattDevice on the fly.
     """
 
     CATT_ARGS = []
     CAST_ARGS = ['-f']
 
-    def __init__(self, name_or_alias: str = 'default', update_interval: float = 0.5):
+    def __init__(self, name_or_alias: Optional[str] = 'default', update_interval: float = 0.5):
         self._device = None
         self._available_devices = None
         self._catt_call = None
         self._catt_config = get_config_as_dict()
         if name_or_alias == 'default':
             self._device_name = self._catt_config['options'].get('device')
+            if self._device_name is None:
+                print(
+                    'No default device set. '
+                    'Scanning for all available devices and picking first...'
+                )
+                print(
+                    'To skip this in the future, either pass a device name '
+                    'or set a default device in the catt config file.'
+                )
+                possible_devices = self.get_available_devices()
+                if len(possible_devices) > 0:
+                    self._device_name = possible_devices[0].name
         elif name_or_alias is not None:
             self._device_name = self._catt_config['aliases'].get(name_or_alias, name_or_alias)
         else:
             self._device_name = None
 
         if self._device_name is not None:
-            self._device = CattDevice(self._device_name)
+            try:
+                self._device = CattDevice(self._device_name)
+            except CastError:
+                print(f'Selected device "{self._device_name}" was not found on this network.')
+                print('Scan for available devices using "lolcatt --scan".')
+                sys.exit(1)
 
         self._update_interval = update_interval
         self._state_last_updated = time.time()
         self._loading_started = None
         self._is_loading_cast = False
         self._loading_timeout = 8
 
@@ -119,15 +138,15 @@
         """
         Returns a CastState object encapsulating the info dictionaries of the currently active
         CattDevice.
 
         :return: A CastState object
         """
         if self._device is None:
-            raise ValueError('Can\'t get cast state: No device selected.')
+            return CastState({}, {}, False)
 
         if time.time() - self._state_last_updated > self._update_interval:
             self._device.controller._update_status()
             self._state_last_updated = time.time()
 
         if self._is_loading_cast and time.time() - self._loading_started > self._loading_timeout:
             self._loading_started = None
```

### Comparing `lolcatt-0.1.1/lolcatt/ui/lolcatt.css` & `lolcatt-0.1.2/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.1.2/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.1.2/lolcatt/ui/lolcatt_playback_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from textual.containers import Container
-from textual.widgets import Label
 from textual.reactive import reactive
+from textual.widgets import Label
 
 from lolcatt.ui.caster_static import CasterStatic
 from lolcatt.utils.utils import marquee
 
 
 class LolCattPlaybackInfo(CasterStatic):
-
     label_str = reactive('')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.label = Label('', id='title')
         self._marquee_gen = None
 
@@ -21,17 +20,17 @@
         is_loading = self._caster.get_cast_state().is_loading
 
         if playing is not None:
             return f'Playing: "{playing}"'
         elif display_name is not None and display_name != 'Backdrop':
             return f'Displaying: "{display_name}"'
         elif is_loading:
-            return f'Loading...'
+            return 'Loading...'
         else:
-            return f'Nothing is playing.'
+            return 'Nothing is playing.'
 
     def _update_label(self):
         self.label_str = self._get_playback_info() + ' '
         self.label.update(next(self._marquee_gen))
 
     def watch_label_str(self, value):
         self._marquee_gen = marquee(value, self.size.width, 2)
```

### Comparing `lolcatt-0.1.1/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.1.2/lolcatt/ui/lolcatt_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Tuple
 
-from textual.events import Click
+from catt.error import CastError
 from textual.containers import Container
+from textual.events import Click
 from textual.reactive import reactive
 from textual.widgets import Label
 from textual.widgets import ProgressBar
 
-from catt.error import CastError
-
 from lolcatt.ui.caster_static import CasterStatic
 
 
 class LolCattProgress(CasterStatic):
     current = reactive(0)
     duration = reactive(0)
     percent_complete = reactive(0)
```

### Comparing `lolcatt-0.1.1/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.1.2/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.1.2/lolcatt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.1/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.1.2/lolcatt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.1/pyproject.toml` & `lolcatt-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.1.1/setup.py` & `lolcatt-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

