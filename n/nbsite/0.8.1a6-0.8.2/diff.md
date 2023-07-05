# Comparing `tmp/nbsite-0.8.1a6.tar.gz` & `tmp/nbsite-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsite-0.8.1a6.tar", last modified: Tue Jun 20 16:35:15 2023, max compression
+gzip compressed data, was "nbsite-0.8.2.tar", last modified: Wed Jul  5 11:45:11 2023, max compression
```

## Comparing `nbsite-0.8.1a6.tar` & `nbsite-0.8.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.251068 nbsite-0.8.1a6/nbsite/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/holoviz-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/github-stars-button.html
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.251068 nbsite-0.8.1a6/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.731871 nbsite-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-05 11:44:01.000000 nbsite-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 11:44:01.000000 nbsite-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-05 11:45:11.731871 nbsite-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-05 11:44:01.000000 nbsite-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.719871 nbsite-0.8.2/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.723871 nbsite-0.8.2/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/holoviz-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.723871 nbsite-0.8.2/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_templates/github-stars-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/_shared_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.723871 nbsite-0.8.2/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31073 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.727871 nbsite-0.8.2/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.727871 nbsite-0.8.2/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.715871 nbsite-0.8.2/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.727871 nbsite-0.8.2/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.727871 nbsite-0.8.2/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.731871 nbsite-0.8.2/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 11:44:01.000000 nbsite-0.8.2/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.719871 nbsite-0.8.2/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 11:45:11.000000 nbsite-0.8.2/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-05 11:44:01.000000 nbsite-0.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:45:11.731871 nbsite-0.8.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-05 11:44:01.000000 nbsite-0.8.2/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-07-05 11:44:01.000000 nbsite-0.8.2/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-07-05 11:44:01.000000 nbsite-0.8.2/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-07-05 11:44:01.000000 nbsite-0.8.2/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-05 11:44:01.000000 nbsite-0.8.2/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-05 11:45:11.731871 nbsite-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-05 11:44:01.000000 nbsite-0.8.2/setup.py
```

### Comparing `nbsite-0.8.1a6/LICENSE.txt` & `nbsite-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/PKG-INFO` & `nbsite-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a6
+Version: 0.8.2
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.1a6/README.md` & `nbsite-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/__main__.py` & `nbsite-0.8.2/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/alert.css` & `nbsite-0.8.2/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.2/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.2/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.2/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.2/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/notebook.css` & `nbsite-0.8.2/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_static/scroller.css` & `nbsite-0.8.2/nbsite/_shared_static/scroller.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.2/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/_shared_templates/layout.html` & `nbsite-0.8.2/nbsite/_shared_templates/layout.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/cmd.py` & `nbsite-0.8.2/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/gallery/gen.py` & `nbsite-0.8.2/nbsite/gallery/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,17 @@
     old_size = im.size  # old_size[0] is in (width, height) format
 
     ratio = float(desired_size)/max(old_size)
     new_size = tuple([int(x*ratio) for x in old_size])
     w = (desired_size-new_size[0])//2
     h = (desired_size-new_size[1])//2
 
-    im = im.resize(new_size, Image.ANTIALIAS)
+    # LANCZOS replaced ANTIALIAS in PIL 10
+    im_filter = getattr(Image, "LANCZOS", None) or getattr(Image, "ANTIALIAS", None)
+    im = im.resize(new_size, im_filter)
     new_im = Image.new("RGBA", (desired_size, desired_size), color=(0, 0, 0, 0))
     new_im.paste(im, (w, h))
     new_im.save(im_pth)
 
 
 def generate_gallery(app, page):
     """
```

### Comparing `nbsite-0.8.1a6/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.2/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/nbbuild.py` & `nbsite-0.8.2/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/paramdoc.py` & `nbsite-0.8.2/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.2/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.2/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.2/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/__init__.py` & `nbsite-0.8.2/nbsite/pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.2/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.2/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.2/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/shared_conf.py` & `nbsite-0.8.2/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/templates/basic/conf.py` & `nbsite-0.8.2/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.2/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/tests/test_cmd.py` & `nbsite-0.8.2/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/tests/test_util.py` & `nbsite-0.8.2/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite/util.py` & `nbsite-0.8.2/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.2/nbsite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a6
+Version: 0.8.2
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.1a6/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.2/nbsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/pyproject.toml` & `nbsite-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.2/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/scripts/nbsite_fix_links.py` & `nbsite-0.8.2/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/scripts/nbsite_generate_modules.py` & `nbsite-0.8.2/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.2/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/setup.cfg` & `nbsite-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a6/setup.py` & `nbsite-0.8.2/setup.py`

 * *Files identical despite different names*

