# Comparing `tmp/mly_pipeline-0.5.2.tar.gz` & `tmp/mly_pipeline-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.2.tar", last modified: Tue Jul  4 14:07:20 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.3.tar", last modified: Wed Jul  5 16:41:05 2023, max compression
```

## Comparing `mly_pipeline-0.5.2.tar` & `mly_pipeline-0.5.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.584667 mly_pipeline-0.5.2/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.2/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.2/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.2/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-04 14:07:20.584667 mly_pipeline-0.5.2/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.2/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.059661 mly_pipeline-0.5.2/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.051661 mly_pipeline-0.5.2/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.285664 mly_pipeline-0.5.2/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.2/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.2/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.2/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.382665 mly_pipeline-0.5.2/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.406665 mly_pipeline-0.5.2/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.2/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.419665 mly_pipeline-0.5.2/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.510666 mly_pipeline-0.5.2/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.2/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.2/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.532666 mly_pipeline-0.5.2/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.2/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.2/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.2/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.2/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.566666 mly_pipeline-0.5.2/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.2/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.2/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.2/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31499 2023-06-29 14:15:00.000000 mly_pipeline-0.5.2/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.2/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.2/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5825 2023-06-06 08:44:31.000000 mly_pipeline-0.5.2/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.2/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16742 2023-06-30 11:44:45.000000 mly_pipeline-0.5.2/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49651 2023-06-30 11:52:05.000000 mly_pipeline-0.5.2/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.582666 mly_pipeline-0.5.2/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.2/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.2/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.579666 mly_pipeline-0.5.2/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-04 14:07:20.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-04 12:43:13.000000 mly_pipeline-0.5.2/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-04 14:07:20.585667 mly_pipeline-0.5.2/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.843629 mly_pipeline-0.5.3/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.3/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.3/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.3/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-05 16:41:05.842629 mly_pipeline-0.5.3/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.3/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.353625 mly_pipeline-0.5.3/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.344625 mly_pipeline-0.5.3/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.581627 mly_pipeline-0.5.3/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.3/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.3/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.3/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.673628 mly_pipeline-0.5.3/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.694628 mly_pipeline-0.5.3/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.3/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.699628 mly_pipeline-0.5.3/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.785629 mly_pipeline-0.5.3/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.3/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.3/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.792629 mly_pipeline-0.5.3/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.3/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.3/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.3/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.3/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.833629 mly_pipeline-0.5.3/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.3/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.3/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.3/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31499 2023-06-29 14:15:00.000000 mly_pipeline-0.5.3/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.3/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.3/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6330 2023-07-05 16:37:33.000000 mly_pipeline-0.5.3/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.3/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16735 2023-07-05 16:36:01.000000 mly_pipeline-0.5.3/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49651 2023-06-30 11:52:05.000000 mly_pipeline-0.5.3/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.841629 mly_pipeline-0.5.3/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.3/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.3/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.839629 mly_pipeline-0.5.3/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-05 16:39:50.000000 mly_pipeline-0.5.3/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-05 16:41:05.843629 mly_pipeline-0.5.3/setup.cfg
```

### Comparing `mly_pipeline-0.5.2/.gitlab-ci.yml` & `mly_pipeline-0.5.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/LICENSE` & `mly_pipeline-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/PKG-INFO` & `mly_pipeline-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.2
+Version: 0.5.3
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.2/README.md` & `mly_pipeline-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/Makefile` & `mly_pipeline-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.5.3/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.5.3/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.3/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.3/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/How to use.html` & `mly_pipeline-0.5.3/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.3/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/Installation.html` & `mly_pipeline-0.5.3/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.3/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.3/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.3/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.3/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.3/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.3/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.3/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.3/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.3/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/doctools.js` & `mly_pipeline-0.5.3/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.3/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.3/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.3/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.3/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.3/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.3/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.3/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.3/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/genindex.html` & `mly_pipeline-0.5.3/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.3/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/howtouse.html` & `mly_pipeline-0.5.3/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/index.html` & `mly_pipeline-0.5.3/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/installation.html` & `mly_pipeline-0.5.3/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/objects.inv` & `mly_pipeline-0.5.3/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.3/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/runningasearch.html` & `mly_pipeline-0.5.3/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/search.html` & `mly_pipeline-0.5.3/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/searchindex.js` & `mly_pipeline-0.5.3/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.3/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/source/conf.py` & `mly_pipeline-0.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/source/index.rst` & `mly_pipeline-0.5.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/source/installation.rst` & `mly_pipeline-0.5.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/source/runningasearch.rst` & `mly_pipeline-0.5.3/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.3/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/__init__.py` & `mly_pipeline-0.5.3/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.3/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.5.3/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/initialization.py` & `mly_pipeline-0.5.3/mly_pipeline/initialization.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.3/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/manager.py` & `mly_pipeline-0.5.3/mly_pipeline/manager.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.3/mly_pipeline/mly_to_grace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #! /usr/bin/env python3
+
+import os, json, time
+
+# Scipy and numpy env parameters that limit the threads
+os.environ["MKL_NUM_THREADS"] = "1"
+os.environ["NUMEXPR_NUM_THREADS"] = "1"
+os.environ["OMP_NUM_THREADS"] = "1"
+
 import pickle
-import os
-import sys
-import json
 import argparse
 import ast
 import numpy as np
 
-# Sourcing the submodule of mly in a very unpythonic way 
-sys.path.append("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
 from mly.datatools import DataPod
-
-
 from lal import gpstime
 from ligo.gracedb.rest import GraceDb
 
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = [
     "trigger_destination",
     "skymap_directory",
     "triggerfile",
     "triggerplot_directory",
     "skymap",
-    "config"
 ]
 
 #Construct argument parser
 parser = argparse.ArgumentParser()
 [parser.add_argument(f"--{argument}") for argument in arguments]
 
 # Pass arguments
@@ -36,17 +36,18 @@
 
 # Store arguments in dictionary
 kwargs = {}
 for argument in arguments:
     kwargs[argument] = getattr(args, argument)
 
 # Config file is inherited by the search script updated
+with open('config.json') as json_file:
+    config = json.load(json_file)
 
-config = ast.literal_eval(kwargs['config'])      
-#def main(**kwargs):
+# config = ast.literal_eval(kwargs['config'])  
     
     
 """This function issues a GraceDB event provided with a json file.
 
 Parameters
 ----------
 
@@ -122,39 +123,45 @@
 
 # Loading the pod that has all the data that produced the trigger
 with open(triggerfile[:-4]+'pkl','rb') as obj:
     thepod = pickle.load(obj)
 
 with open(f"{triggerfile[:-5]}_buffer.pkl", 'rb') as obj:
     buffer = pickle.load(obj)
-    
 if kwargs['skymap']==None:
-    kwargs['skymap']=False
-if isinstance(kwargs['skymap'],str):
-    kwargs['skymap']=bool(kwargs['skymap'])
+    kwargs['skymap']=0
+else:
+    kwargs['skymap'] = int(kwargs['skymap'])
 
-    
-    
-# Probably this could go below skymap generation?    
+# if isinstance(kwargs['skymap'],str):
+#     if kwargs['skymap'].lower=='true':
+#         kwargs['skymap']==True
+#     elif kwargs['skymap'].lower=='false':
+#         kwargs['skymap']==False
+#     else:
+#         print(kwargs['skymap'])
+
+
+
+# # Probably this could go below skymap generation?    
 if kwargs['triggerplot_directory'] != 'None':
     
-    print('triggerplot_checkpoint')
     # Creating a directory for each event using the graceid from the event creation.
     # Not always works.
     try:
         eventDirectory = graceEventDict['graceid']+'-'+triggerfile.split('_')[-2]+'-'+triggerfile.split('_')[-1].split('.')[0]
     except Exception as e:
         print(e)
         eventDirectory = 'NoGraceID'+'-'+triggerfile.split('_')[-2]+'-'+triggerfile.split('_')[-1].split('.')[0]
     
     # Making an event directory
     os.mkdir(f"{kwargs['triggerplot_directory']}/{eventDirectory}")
+    print('triggerplot_checkpoint')
 
 
-    
 if kwargs['skymap']:
 
     from mly.null_energy_map import *
     from ligo.skymap.io import fits
 
     # Create skymap plugin:
     sky_map_plugin = createSkymapPlugin(
@@ -170,14 +177,15 @@
     with open(skymap_path, "w") as f:
         fits.write_sky_map(f.name, skymap_fits, nest=False)
     
     # Upload skymap to grace db:
     if kwargs['trigger_destination'] != 'None':
 
         client.writeLog(graceEventDict['graceid'], 'skymap',  filename=skymap_path, tg_name='sky_loc')
+    print('skymap checkpoint')
 
 if kwargs['triggerplot_directory'] != 'None':
 
     import matplotlib.pyplot as plt
     
     gpsstring=triggerfile.split('_')[1]
     detectors=triggerfile.split('_')[-1][-5]
@@ -187,19 +195,24 @@
     plt.savefig(f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_strain.png")
     
     # Creating the correlation plot
     thepod.plot(type_="correlation")
     plt.savefig(
         f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_correlation.png")
 
+    thepod.plot('tf_map')
+    plt.savefig(
+        f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_tfmap.png")
+
     # And if skymap is created we save the plot as png too.
     if kwargs['skymap']==True:
         buffer.plot(type_="skymap")
         plt.savefig(f"{kwargs['triggerplot_directory']}/{eventDirectory}/T_{triggerfile.split('_')[-2]}_{triggerfile.split('_')[-1][:-5]}_skymap.png")
 
+    print('plots checkpoint')
 raise SystemExit()
 
 # if __name__ == "__main__":
 
 
 #     main(**kwargs)
```

### Comparing `mly_pipeline-0.5.2/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.3/mly_pipeline/offline_search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/search.py` & `mly_pipeline-0.5.3/mly_pipeline/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
         # Perform time- and frequency-domain parameter estimation.
         # It adds parameter estimation to events.
         pe_t0 = time.time()
         mly_output = runTimeFrequencyParameterEstimation(thepod,  mly_output)
         logger.info(f"PE time {time.time()- pe_t0}s")
         # If result us above threshold, do all even relate actions 
-        if mly_output["scores"]["combined"] >= threshold:
+        if mly_output["scores"]["combined"] >= 1e-8:#threshold:
 
 
 
             # Saving trigger into the trigger_directory
             with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
                 json.dump(mly_output, mly_json,indent=4)
                 mly_json.close()
@@ -337,24 +337,24 @@
             # Saving trigger background DataPod into the trigger_directory
             with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}_buffer.pkl", 'wb') as mly_pkl:
                 pickle.dump(buffer_pod, mly_pkl, 4)
                                 
             # Sending trigger to GraceDB 
             logger.debug(f"PROCESSES before run mlytograce: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']])}")
 
+            print(config['skymap'],type(config['skymap']))
+
             with open( f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.out"
             ,"wb") as out:
-
                 # Using subprocess to create mly_to grace function and run it independently.
-                p = subprocess.Popen(["python", config["mlyPipelineSource"]+"/mly_to_grace.py", "--triggerfile"
+                p = subprocess.Popen(["python","-m","mly_pipeline.mly_to_grace", "--triggerfile"
                                       ,f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json"
                                       ,"--trigger_destination", str(config['trigger_destination'])
                                       ,"--triggerplot_directory",config['triggerplot_directory']
-                                      ,"--config",str(config)
-                                      ,"--skymap", str(config['skymap'])]
+                                      ,"--skymap", str(int(config['skymap']))]
                                       #+" > "+f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.out &"
                                       ,stdout=out, stderr=out,shell=False)
             
             logger.info(f"S{config['script_index']} - TRIGGER follow-up script initialised for: "+str(mly_output['gpstime']))
                 
 
             # Saving output to output directory. Notice that the name starts with T_ for triggers
```

### Comparing `mly_pipeline-0.5.2/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.3/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.3/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.3/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.3/mly_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.2
+Version: 0.5.3
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.2/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.3/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.2/pyproject.toml` & `mly_pipeline-0.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

