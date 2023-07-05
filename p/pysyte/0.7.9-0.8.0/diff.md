# Comparing `tmp/pysyte-0.7.9.tar.gz` & `tmp/pysyte-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysyte-0.7.9.tar", last modified: Tue May  7 00:21:04 2019, max compression
+gzip compressed data, was "pysyte-0.8.0.tar", last modified: Wed Jul  5 16:44:41 2023, max compression
```

## Comparing `pysyte-0.7.9.tar` & `pysyte-0.8.0.tar`

### file list

```diff
@@ -1,80 +1,138 @@
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/
--rw-r--r--   0 jab        (501) staff       (20)      895 2019-05-07 00:21:04.000000 pysyte-0.7.9/PKG-INFO
--rw-r--r--   0 jab        (501) staff       (20)      788 2019-01-24 20:25:22.000000 pysyte-0.7.9/README.rst
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/bin/
--rwxr-xr-x   0 jab        (501) staff       (20)     2823 2019-05-06 23:49:01.000000 pysyte-0.7.9/bin/kat
--rwxr-xr-x   0 jab        (501) staff       (20)     4206 2019-05-06 23:03:02.000000 pysyte-0.7.9/bin/short_dir
--rwxr-xr-x   0 jab        (501) staff       (20)      656 2019-01-24 20:25:22.000000 pysyte-0.7.9/bin/try
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte/
--rw-r--r--   0 jab        (501) staff       (20)       81 2019-05-07 00:15:56.000000 pysyte-0.7.9/pysyte/__init__.py
--rw-r--r--   0 jab        (501) staff       (20)     3759 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/args.py
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte/bash/
--rw-r--r--   0 jab        (501) staff       (20)        0 2019-04-22 23:56:07.000000 pysyte-0.7.9/pysyte/bash/__init__.py
--rw-r--r--   0 jab        (501) staff       (20)      472 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/bash/cmnds.py
--rw-r--r--   0 jab        (501) staff       (20)    24326 2019-03-21 23:16:57.000000 pysyte-0.7.9/pysyte/bash/git.py
--rw-r--r--   0 jab        (501) staff       (20)      837 2019-03-21 04:56:19.000000 pysyte-0.7.9/pysyte/bash/git.test
--rw-r--r--   0 jab        (501) staff       (20)     1612 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/bash/shell.py
--rw-r--r--   0 jab        (501) staff       (20)      232 2018-01-14 23:28:35.000000 pysyte-0.7.9/pysyte/code.py
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte/colours/
--rw-r--r--   0 jab        (501) staff       (20)        0 2018-01-14 23:28:35.000000 pysyte-0.7.9/pysyte/colours/__init__.py
--rw-r--r--   0 jab        (501) staff       (20)     1843 2018-01-14 23:28:35.000000 pysyte-0.7.9/pysyte/colours/ansi_escapes.py
--rw-r--r--   0 jab        (501) staff       (20)      543 2019-04-21 23:29:17.000000 pysyte-0.7.9/pysyte/colours/ansi_escapes.test
--rw-r--r--   0 jab        (501) staff       (20)      943 2018-01-14 23:28:35.000000 pysyte-0.7.9/pysyte/colours/colour_names.py
--rw-r--r--   0 jab        (501) staff       (20)      942 2019-04-21 23:30:20.000000 pysyte-0.7.9/pysyte/colours/colour_names.test
--rw-r--r--   0 jab        (501) staff       (20)     4572 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/colours/colour_numbers.py
--rw-r--r--   0 jab        (501) staff       (20)     2503 2019-04-21 23:30:40.000000 pysyte-0.7.9/pysyte/colours/colour_numbers.test
--rw-r--r--   0 jab        (501) staff       (20)     4025 2019-04-21 23:30:53.000000 pysyte-0.7.9/pysyte/colours/colour_numbers.tests
--rw-r--r--   0 jab        (501) staff       (20)     1034 2018-05-30 00:38:38.000000 pysyte-0.7.9/pysyte/colours/main.py
--rw-r--r--   0 jab        (501) staff       (20)     2086 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/colours/texts.py
--rw-r--r--   0 jab        (501) staff       (20)      789 2019-04-08 01:08:04.000000 pysyte-0.7.9/pysyte/colours/texts.test
--rw-r--r--   0 jab        (501) staff       (20)      247 2019-04-08 01:08:04.000000 pysyte-0.7.9/pysyte/colours/texts.tests
--rw-r--r--   0 jab        (501) staff       (20)     2686 2019-04-22 23:20:29.000000 pysyte-0.7.9/pysyte/colours/x11_colour_names.py
--rw-r--r--   0 jab        (501) staff       (20)      226 2019-04-22 23:56:07.000000 pysyte-0.7.9/pysyte/colours/x11_colour_names.test
--rw-r--r--   0 jab        (501) staff       (20)       57 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/darwin.py
--rw-r--r--   0 jab        (501) staff       (20)     4749 2018-11-02 05:05:00.000000 pysyte-0.7.9/pysyte/debuggers.py
--rw-r--r--   0 jab        (501) staff       (20)     4460 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/decorators.py
--rw-r--r--   0 jab        (501) staff       (20)     2803 2019-05-06 21:01:54.000000 pysyte-0.7.9/pysyte/dictionaries.py
--rw-r--r--   0 jab        (501) staff       (20)      862 2019-04-21 23:37:21.000000 pysyte-0.7.9/pysyte/dictionaries.test
--rw-r--r--   0 jab        (501) staff       (20)     7835 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/getch.py
--rw-r--r--   0 jab        (501) staff       (20)     4742 2019-04-21 23:03:32.000000 pysyte-0.7.9/pysyte/imports.py
--rw-r--r--   0 jab        (501) staff       (20)     1145 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/iteration.py
--rw-r--r--   0 jab        (501) staff       (20)      635 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/keyboard.py
--rw-r--r--   0 jab        (501) staff       (20)       45 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/linux.py
--rw-r--r--   0 jab        (501) staff       (20)      285 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/lists.py
--rw-r--r--   0 jab        (501) staff       (20)     1839 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/literals.py
--rw-r--r--   0 jab        (501) staff       (20)    25165 2019-04-22 00:14:47.000000 pysyte-0.7.9/pysyte/paths.py
--rw-r--r--   0 jab        (501) staff       (20)     5819 2019-05-06 22:36:32.000000 pysyte-0.7.9/pysyte/paths.test
--rw-r--r--   0 jab        (501) staff       (20)      459 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/platforms.py
--rw-r--r--   0 jab        (501) staff       (20)      133 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/pp.py
--rw-r--r--   0 jab        (501) staff       (20)      127 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/randoms.py
--rw-r--r--   0 jab        (501) staff       (20)     2585 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/scripts.py
--rw-r--r--   0 jab        (501) staff       (20)     4922 2018-01-14 23:28:36.000000 pysyte-0.7.9/pysyte/splits.py
--rw-r--r--   0 jab        (501) staff       (20)      479 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/splits.test
--rw-r--r--   0 jab        (501) staff       (20)      730 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/streams.py
--rw-r--r--   0 jab        (501) staff       (20)      353 2019-04-08 01:10:36.000000 pysyte-0.7.9/pysyte/streams.test
--rw-r--r--   0 jab        (501) staff       (20)      416 2019-04-22 23:56:07.000000 pysyte-0.7.9/pysyte/term.py
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte/testing/
--rw-r--r--   0 jab        (501) staff       (20)        0 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/testing/__init__.py
--rw-r--r--   0 jab        (501) staff       (20)    10481 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/testing/files_for_test.py
--rw-r--r--   0 jab        (501) staff       (20)     2378 2019-04-22 00:58:38.000000 pysyte-0.7.9/pysyte/testing/files_for_test.test
--rw-r--r--   0 jab        (501) staff       (20)     3993 2019-05-06 23:50:00.000000 pysyte-0.7.9/pysyte/testing/files_for_test.tests
--rw-r--r--   0 jab        (501) staff       (20)    10167 2019-04-22 00:30:05.000000 pysyte-0.7.9/pysyte/testing/see.py
--rw-r--r--   0 jab        (501) staff       (20)      924 2019-04-22 01:02:44.000000 pysyte-0.7.9/pysyte/testing/see.test
--rw-r--r--   0 jab        (501) staff       (20)      514 2019-04-21 23:38:48.000000 pysyte-0.7.9/pysyte/testing/see.tests
--rw-r--r--   0 jab        (501) staff       (20)      371 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/testing/try_plugins.py
--rw-r--r--   0 jab        (501) staff       (20)      432 2019-04-21 23:40:20.000000 pysyte-0.7.9/pysyte/testing/try_plugins.test
--rw-r--r--   0 jab        (501) staff       (20)    10846 2019-05-06 23:03:02.000000 pysyte-0.7.9/pysyte/testing/trying.py
--rw-r--r--   0 jab        (501) staff       (20)     2065 2019-05-06 22:48:30.000000 pysyte-0.7.9/pysyte/testing/trying.test
--rw-r--r--   0 jab        (501) staff       (20)     2134 2019-01-24 20:25:22.000000 pysyte-0.7.9/pysyte/text_streams.py
--rw-r--r--   0 jab        (501) staff       (20)      962 2018-01-14 23:28:35.000000 pysyte-0.7.9/pysyte/tracebacks.py
--rw-r--r--   0 jab        (501) staff       (20)      622 2019-04-23 01:45:11.000000 pysyte-0.7.9/pysyte/words.py
--rw-r--r--   0 jab        (501) staff       (20)      526 2019-04-23 01:45:12.000000 pysyte-0.7.9/pysyte/words.test
--rw-r--r--   0 jab        (501) staff       (20)     3732 2019-05-06 21:56:01.000000 pysyte-0.7.9/pysyte/words.tests
-drwxr-xr-x   0 jab        (501) staff       (20)        0 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/
--rw-r--r--   0 jab        (501) staff       (20)      895 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/PKG-INFO
--rw-r--r--   0 jab        (501) staff       (20)     1629 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/SOURCES.txt
--rw-r--r--   0 jab        (501) staff       (20)        1 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/dependency_links.txt
--rw-r--r--   0 jab        (501) staff       (20)       52 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/requires.txt
--rw-r--r--   0 jab        (501) staff       (20)        7 2019-05-07 00:21:04.000000 pysyte-0.7.9/pysyte.egg-info/top_level.txt
--rw-r--r--   0 jab        (501) staff       (20)      109 2019-05-07 00:21:04.000000 pysyte-0.7.9/setup.cfg
--rw-r--r--   0 jab        (501) staff       (20)     1933 2019-05-06 22:52:03.000000 pysyte-0.7.9/setup.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.206595 pysyte-0.8.0/
+-rw-r--r--   0 jab        (501) wheel        (0)     1106 2023-03-01 23:03:27.000000 pysyte-0.8.0/LICENSE
+-rw-r--r--   0 jab        (501) wheel        (0)      691 2023-07-05 16:44:41.206751 pysyte-0.8.0/PKG-INFO
+-rw-r--r--   0 jab        (501) wheel        (0)     1038 2023-07-03 12:36:32.000000 pysyte-0.8.0/README.rst
+-rw-r--r--   0 jab        (501) wheel        (0)      111 2023-03-01 23:03:27.000000 pysyte-0.8.0/pyproject.toml
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.167862 pysyte-0.8.0/pysyte/
+-rw-r--r--   0 jab        (501) wheel        (0)       52 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/__init__.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.170582 pysyte-0.8.0/pysyte/bash/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2022-11-08 03:15:23.000000 pysyte-0.8.0/pysyte/bash/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      530 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/bash/screen.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1277 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/bash/shell.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.171069 pysyte-0.8.0/pysyte/bash/test/
+-rw-r--r--   0 jab        (501) wheel        (0)     1018 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/bash/test/shell.test
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.175113 pysyte-0.8.0/pysyte/cli/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2022-11-08 03:15:23.000000 pysyte-0.8.0/pysyte/cli/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      701 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/cli/app.py
+-rw-r--r--   0 jab        (501) wheel        (0)     6508 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/cli/arguments.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1592 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/cli/config.py
+-rw-r--r--   0 jab        (501) wheel        (0)      354 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/cli/exceptions.py
+-rw-r--r--   0 jab        (501) wheel        (0)     3241 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/cli/lines.py
+-rw-r--r--   0 jab        (501) wheel        (0)     3463 2023-07-03 12:36:32.000000 pysyte-0.8.0/pysyte/cli/main.py
+-rw-r--r--   0 jab        (501) wheel        (0)      769 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/cli/paths.py
+-rw-r--r--   0 jab        (501) wheel        (0)     2035 2023-07-03 12:36:32.000000 pysyte-0.8.0/pysyte/cli/streams.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.176360 pysyte-0.8.0/pysyte/cli/test/
+-rw-r--r--   0 jab        (501) wheel        (0)     1630 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/cli/test/arguments.test
+-rw-r--r--   0 jab        (501) wheel        (0)      388 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/cli/test/config.test
+-rw-r--r--   0 jab        (501) wheel        (0)      959 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/cli/test/main.test
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.178727 pysyte-0.8.0/pysyte/colours/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2022-11-08 03:15:23.000000 pysyte-0.8.0/pysyte/colours/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1992 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/ansi_escapes.py
+-rw-r--r--   0 jab        (501) wheel        (0)      935 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/colour_names.py
+-rw-r--r--   0 jab        (501) wheel        (0)     4840 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/colour_numbers.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.181306 pysyte-0.8.0/pysyte/colours/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      543 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/test/ansi_escapes.test
+-rw-r--r--   0 jab        (501) wheel        (0)      977 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/colours/test/colour_names.test
+-rw-r--r--   0 jab        (501) wheel        (0)     2445 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/colours/test/colour_numbers.test
+-rw-r--r--   0 jab        (501) wheel        (0)     4290 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/colours/test/colour_numbers.tests
+-rw-r--r--   0 jab        (501) wheel        (0)     1022 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/colours/test/texts.test
+-rw-r--r--   0 jab        (501) wheel        (0)      290 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/test/x11_colour_names.test
+-rw-r--r--   0 jab        (501) wheel        (0)      432 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/colours/test/x11_colour_names.tests
+-rw-r--r--   0 jab        (501) wheel        (0)     2664 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/texts.py
+-rw-r--r--   0 jab        (501) wheel        (0)     2528 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/colours/x11_colour_names.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.182880 pysyte-0.8.0/pysyte/config/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/config/__init__.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.184119 pysyte-0.8.0/pysyte/config/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      351 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/config/test/types.test
+-rw-r--r--   0 jab        (501) wheel        (0)      857 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/config/test/urator.test
+-rw-r--r--   0 jab        (501) wheel        (0)      559 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/config/test/xdg.test
+-rw-r--r--   0 jab        (501) wheel        (0)     2136 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/config/types.py
+-rw-r--r--   0 jab        (501) wheel        (0)      451 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/config/urator.py
+-rw-r--r--   0 jab        (501) wheel        (0)      176 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/config/xdg.py
+-rw-r--r--   0 jab        (501) wheel        (0)     5590 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/importers.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.184651 pysyte-0.8.0/pysyte/imports/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/imports/__init__.py
+-rwxr-xr-x   0 jab        (501) wheel        (0)     2413 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/imports/__main__.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1442 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/iteration.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.185349 pysyte-0.8.0/pysyte/kat/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/kat/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      585 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/kat/__main__.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.186074 pysyte-0.8.0/pysyte/keys/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/keys/__init__.py
+-rwxr-xr-x   0 jab        (501) wheel        (0)      757 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/keys/__main__.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.140353 pysyte-0.8.0/pysyte/net/
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.186672 pysyte-0.8.0/pysyte/net/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      587 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/net/test/hosts.test
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.189175 pysyte-0.8.0/pysyte/oss/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2022-11-08 03:15:23.000000 pysyte-0.8.0/pysyte/oss/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)       87 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/darwin.py
+-rw-r--r--   0 jab        (501) wheel        (0)     8901 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/getch.py
+-rw-r--r--   0 jab        (501) wheel        (0)      639 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/keyboard.py
+-rw-r--r--   0 jab        (501) wheel        (0)      677 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/linux.py
+-rw-r--r--   0 jab        (501) wheel        (0)      447 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/platforms.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.190073 pysyte-0.8.0/pysyte/oss/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      710 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/oss/test/linux.test
+-rw-r--r--   0 jab        (501) wheel        (0)      425 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/oss/test/platforms.test
+-rw-r--r--   0 jab        (501) wheel        (0)       35 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/pysyte.yaml
+-rw-r--r--   0 jab        (501) wheel        (0)      325 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/randoms.py
+-rw-r--r--   0 jab        (501) wheel        (0)     3233 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/similarities.py
+-rw-r--r--   0 jab        (501) wheel        (0)     5505 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/splits.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1713 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/streams.py
+-rw-r--r--   0 jab        (501) wheel        (0)      565 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/term.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.193309 pysyte-0.8.0/pysyte/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      435 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/test/importers.test
+-rw-r--r--   0 jab        (501) wheel        (0)     1039 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/test/iteration.test
+-rw-r--r--   0 jab        (501) wheel        (0)      364 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/test/similarities.test
+-rw-r--r--   0 jab        (501) wheel        (0)      479 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/test/splits.test
+-rw-r--r--   0 jab        (501) wheel        (0)      533 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/test/streams.test
+-rw-r--r--   0 jab        (501) wheel        (0)      823 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/test/tracebacks.test
+-rw-r--r--   0 jab        (501) wheel        (0)      554 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/test/words.test
+-rw-r--r--   0 jab        (501) wheel        (0)     4147 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/test/words.tests
+-rw-r--r--   0 jab        (501) wheel        (0)      995 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/tracebacks.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.197249 pysyte-0.8.0/pysyte/types/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2022-11-08 03:15:23.000000 pysyte-0.8.0/pysyte/types/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      335 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/colours.py
+-rw-r--r--   0 jab        (501) wheel        (0)     4750 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/dictionaries.py
+-rw-r--r--   0 jab        (501) wheel        (0)     3052 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/lines.py
+-rw-r--r--   0 jab        (501) wheel        (0)     2933 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/lists.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.200119 pysyte-0.8.0/pysyte/types/literals/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      725 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/ansi.py
+-rw-r--r--   0 jab        (501) wheel        (0)      109 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/control.py
+-rw-r--r--   0 jab        (501) wheel        (0)      180 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/digits.py
+-rw-r--r--   0 jab        (501) wheel        (0)       84 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/nones.py
+-rw-r--r--   0 jab        (501) wheel        (0)      105 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/numbers.py
+-rw-r--r--   0 jab        (501) wheel        (0)      635 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/punctuation.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.202435 pysyte-0.8.0/pysyte/types/literals/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      293 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/test/ansi.test
+-rw-r--r--   0 jab        (501) wheel        (0)      469 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/test/digits.test
+-rw-r--r--   0 jab        (501) wheel        (0)      469 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/types/literals/test/nones.test
+-rw-r--r--   0 jab        (501) wheel        (0)      313 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/literals/test/numbers.test
+-rw-r--r--   0 jab        (501) wheel        (0)      591 2023-03-06 14:51:47.000000 pysyte-0.8.0/pysyte/types/literals/test/punctuation.test
+-rw-r--r--   0 jab        (501) wheel        (0)     3363 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/methods.py
+-rw-r--r--   0 jab        (501) wheel        (0)      620 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/numbers.py
+-rw-r--r--   0 jab        (501) wheel        (0)    33919 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/paths.py
+-rw-r--r--   0 jab        (501) wheel        (0)      936 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/strings.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.204604 pysyte-0.8.0/pysyte/types/test/
+-rw-r--r--   0 jab        (501) wheel        (0)     1954 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/test/dictionaries.test
+-rw-r--r--   0 jab        (501) wheel        (0)     1029 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/test/lines.test
+-rw-r--r--   0 jab        (501) wheel        (0)      658 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/test/lists.test
+-rw-r--r--   0 jab        (501) wheel        (0)     1102 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/test/numbers.test
+-rw-r--r--   0 jab        (501) wheel        (0)    10435 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/types/test/paths.test
+-rw-r--r--   0 jab        (501) wheel        (0)     1766 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/test/times.test
+-rw-r--r--   0 jab        (501) wheel        (0)      714 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/types/times.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.205854 pysyte-0.8.0/pysyte/unix/
+-rw-r--r--   0 jab        (501) wheel        (0)        0 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/unix/__init__.py
+-rw-r--r--   0 jab        (501) wheel        (0)      918 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/unix/root.py
+-rw-r--r--   0 jab        (501) wheel        (0)     1814 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/unix/root.yaml
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.206241 pysyte-0.8.0/pysyte/unix/test/
+-rw-r--r--   0 jab        (501) wheel        (0)      234 2023-03-01 23:03:27.000000 pysyte-0.8.0/pysyte/unix/test/root.test
+-rw-r--r--   0 jab        (501) wheel        (0)      603 2023-07-05 16:43:49.000000 pysyte-0.8.0/pysyte/words.py
+drwxr-xr-x   0 jab        (501) wheel        (0)        0 2023-07-05 16:44:41.169461 pysyte-0.8.0/pysyte.egg-info/
+-rw-r--r--   0 jab        (501) wheel        (0)      691 2023-07-05 16:44:40.000000 pysyte-0.8.0/pysyte.egg-info/PKG-INFO
+-rw-r--r--   0 jab        (501) wheel        (0)     2930 2023-07-05 16:44:41.000000 pysyte-0.8.0/pysyte.egg-info/SOURCES.txt
+-rw-r--r--   0 jab        (501) wheel        (0)        1 2023-07-05 16:44:40.000000 pysyte-0.8.0/pysyte.egg-info/dependency_links.txt
+-rw-r--r--   0 jab        (501) wheel        (0)       85 2023-07-05 16:44:40.000000 pysyte-0.8.0/pysyte.egg-info/requires.txt
+-rw-r--r--   0 jab        (501) wheel        (0)        7 2023-07-05 16:44:40.000000 pysyte-0.8.0/pysyte.egg-info/top_level.txt
+-rw-r--r--   0 jab        (501) wheel        (0)     1186 2023-07-05 16:44:41.207551 pysyte-0.8.0/setup.cfg
+-rw-r--r--   0 jab        (501) wheel        (0)      732 2023-07-03 12:36:32.000000 pysyte-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysyte-0.7.9/pysyte/bash/shell.py` & `pysyte-0.8.0/pysyte/bash/shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,54 @@
-"""Handle bash commands for the tools package"""
+"""Handle bash commands for pysyte"""
 
-import logging
 import os
 from contextlib import contextmanager
+from subprocess import getstatusoutput
+from typing import List
 
-from pysyte.bash.cmnds import getstatusoutput
-
-logger = logging.getLogger(__name__)
+from boltons.setutils import IndexedSet
 
 
 class BashError(ValueError):
     pass
 
 
-_working_dirs = ['']
-_displays = [False]
-_path = []
+_working_dirs: List[str] = [""]
+_paths: List[str] = []
 
 
-def cd(path):
+def cd(path: str):
     if _working_dirs[0] == path:
         return
-    logger.info('$ PWD=%s', path)
+    assert os.path.isdir(path)
     _working_dirs[0] = path
 
 
 @contextmanager
 def pushd(path):
+    assert os.path.isdir(path)
     _working_dirs.insert(0, path)
     yield
     del _working_dirs[0]
 
 
-def _get_path():
-    """Guarantee that /usr/local/bin and /usr/bin are in PATH"""
-    if _path:
-        return _path[0]
-    environ_paths = set(os.environ['PATH'].split(':'))
-    environ_paths.add('/usr/local/bin')
-    environ_paths.add('/usr/bin')
-    _path.append(':'.join(environ_paths))
-    logger.debug('PATH = %s', _path[-1])
-    return _path[0]
+def _get_path() -> str:
+    """Guarantee that /usr/local/bin, /usr/bin, /bin are in PATH"""
+    if _paths:
+        return _paths[0]
+    environ_paths = IndexedSet(os.environ["PATH"].split(":"))
+    minimal_paths = IndexedSet(["/usr/local/bin", "/usr/bin", "/bin"])
+    all_paths = environ_paths | minimal_paths
+    _paths.append(":".join(all_paths))
+    return _paths[0]
 
 
-def run(command):
-    path_command = 'PATH=%s %s' % (_get_path(), command)
+def run(command: str) -> str:
+    path_command = f"PATH={_get_path()} {command}"
     if _working_dirs[0]:
-        run_command = '(cd %s; %s)' % (_working_dirs[0], path_command)
-        logger.info('$ (cd %s; %s)', _working_dirs[0], command)
+        run_command = f"(cd {_working_dirs[0]}; {path_command})"
     else:
         run_command = path_command
-        logger.info('$ %s', command)
     status, output = getstatusoutput(run_command)
     if status:
-        logger.error('\n%s', output)
-        raise BashError(output)
-    elif output:
-        logger.info('\n%s', output)
+        raise BashError(f"{run_command}\n{output}")
     return output
-
-
-def set_verbosity(display):
-    _displays[0] = display
-
-
-def full_path(path):
-    """Get the real path, expanding links and bashisms"""
-    return os.path.realpath(os.path.expanduser(os.path.expandvars(path)))
```

### Comparing `pysyte-0.7.9/pysyte/colours/ansi_escapes.py` & `pysyte-0.8.0/pysyte/colours/ansi_escapes.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 
 All numbers used in this file are values usable in an ANSI escape sequence
     See http://en.wikipedia.org/wiki/ANSI_escape_code for values
 """
 
 
 def escape(string):
-    return '\033%s' % string
+    return f"\033{string}"
 
 
 def escape_sequence(string):
-    return escape('[%sm' % string)
+    return escape(f"[{string}m")
 
 
 def bold():
-    return escape_sequence('1')
+    return escape_sequence("1")
 
 
 def no_bold():
-    return escape_sequence('22')
+    return escape_sequence("22")
 
 
 def no_colour():
-    return escape_sequence('2') + escape_sequence('0')
+    return escape_sequence("2") + escape_sequence("0")
 
 
 def no_prompt():
     return prompt(no_colour())
 
 
 def _colour_16(ground, i):
     if i > 7:
         prefix = bold()
         i = i - 8
     else:
-        prefix = ''
-    return '%s%s' % (prefix, escape('[%d%dm' % (ground, i)))
+        prefix = ""
+    escaped = escape(f"[{ground}{i}m")
+    return f"{prefix}{escaped}"
 
 
 def _colour_256(ground, i):
-    return escape_sequence('%s;5;%d') % (ground, i)
+    return escape_sequence(f"{ground};5;{i}")
 
 
 def _background_16(i):
     return _colour_16(4, i)
 
 
 def _background_256(i):
@@ -59,37 +60,47 @@
 
 
 def _small_colour_number(i):
     return i < 16
 
 
 def foreground(i):
+    if not i:
+        return ""
     return _small_colour_number(i) and _foreground_16(i) or _foreground_256(i)
 
 
 def background(i):
+    if not i:
+        return ""
     return _small_colour_number(i) and _background_16(i) or _background_256(i)
 
 
 def prompt(string):
-    return '\001%s\002' % string
+    return f"\001{string}\002"
+
+
+def colour_string(colour, text):
+    stop = no_colour() if colour else ""
+    return f"{colour}{text}{stop}"
 
 
 def foreground_string(text, i):
-    return '%s%s%s' % (foreground(i), text, no_colour())
+    return colour_string(foreground(i), text)
 
 
 def background_string(text, i):
-    return '%s%s%s' % (background(i), text, no_colour())
+    return colour_string(background(i), text)
 
 
 def grounds_string(text, background_colour, foreground_colour):
-    return '%s%s%s%s' % (
+    return "%s%s%s%s" % (
         background(background_colour),
         foreground(foreground_colour),
         text,
-        no_colour())
+        no_colour(),
+    )
 
 
 def prompt_string(text, i):
     string = foreground(i)
-    return '%s%s%s' % (prompt(string), text, no_prompt())
+    return f"{prompt(string)}{text}{no_prompt()}"
```

### Comparing `pysyte-0.7.9/pysyte/colours/ansi_escapes.test` & `pysyte-0.8.0/pysyte/colours/test/ansi_escapes.test`

 * *Files identical despite different names*

### Comparing `pysyte-0.7.9/pysyte/colours/colour_names.py` & `pysyte-0.8.0/pysyte/colours/colour_names.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Methods to provide names for colours
 
 And numbers for those names"""
 
 
 def bw():
     """The simplest of all - no colour and full colour"""
-    return 'black white'.split()
+    return "black white".split()
 
 
 def rgb():
     """The basic cone sensitivities of your eyes"""
-    return 'red green blue'.split()
+    return "red green blue".split()
 
 
 primaries = rgb
 
 
 def cym():
     """The complements of the primaries"""
-    return 'cyan yellow magenta'.split()
+    return "cyan yellow magenta".split()
 
 
 secondaries = complementaries = cym
 
 
 def basic():
     """The basic colour names: Black, the primaries, their complements and white"""
     return bw() + rgb() + cym()
 
 
 def _cga_colour_names():
     """The basic CGA colours are in a slightly different order"""
-    return 'red green yellow blue magenta cyan'.split()
+    return "red green yellow blue magenta cyan".split()
 
 
 def dark_cga():
-    return ['black'] + _cga_colour_names() + ['silver']
+    return ["black"] + _cga_colour_names() + ["silver"]
 
 
 def light_cga():
-    return ['gray'] + [str('light %s' % name) for name in _cga_colour_names()]  + ['white']
+    return ["gray"] + [f"light {name}" for name in _cga_colour_names()] + ["white"]
 
 
 def cga():
     return dark_cga() + light_cga()
```

### Comparing `pysyte-0.7.9/pysyte/colours/colour_names.test` & `pysyte-0.8.0/pysyte/colours/test/colour_names.test`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 The colour_names module
 =======================
 
     >>> from pysyte.colours import colour_names
-    >>> assert 'provide names for colours' in  colour_names.__doc__
+    >>> assert 'provide names for colours' in colour_names.__doc__
 
 
 Basic colour names
 -----------------
 
 Start with the easy ones
     >>> assert colour_names.bw() == ['black', 'white']
     >>> assert colour_names.primaries() == ['red', 'green', 'blue']
     >>> assert colour_names.complementaries() == ['cyan', 'yellow', 'magenta']
 
 All of those are considered basic
-    >>> assert colour_names.basic() == colour_names.bw() + colour_names.primaries() + colour_names.complementaries()
+    >>> c_n = colour_names
+    >>> all_of_those = c_n.bw() + c_n.primaries() + c_n.complementaries()
+    >>> assert colour_names.basic() == all_of_those
 
 CGA colour names
 ----------------
 
 CGA has all the basic names
     >>> assert all([name in colour_names.cga() for name in colour_names.basic()])
```

### Comparing `pysyte-0.7.9/pysyte/colours/colour_numbers.py` & `pysyte-0.8.0/pysyte/colours/colour_numbers.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
     def grey_shade(red, green, blue):
         for i in red, green, blue:
             if (i - 8) % 10:
                 return False
         return 232 + ((red - 8) // 10)
 
-    red = (integer & 0xff0000) >> 16
-    green = (integer & 0x00ff00) >> 8
-    blue = integer & 0x0000ff
+    red = (integer & 0xFF0000) >> 16
+    green = (integer & 0x00FF00) >> 8
+    blue = integer & 0x0000FF
     result = grey_shade(red, green, blue)
     if result:
         return result
     red = rgb_to_decimal(red)
     green = rgb_to_decimal(green)
     blue = rgb_to_decimal(blue)
     return (red * 36) + (green * 6) + blue + 16
@@ -50,32 +50,33 @@
     assert 231 >= a >= 16
     red, green, blue = ((a - 16) / 36) % 6, ((a - 16) / 6) % 6, (a - 16) % 6
 
     def decimal_to_rgb(i):
         if not i:
             return 0
         return int((i * 40) + 55)
+
     return decimal_to_rgb(red), decimal_to_rgb(green), decimal_to_rgb(blue)
 
 
 def red_green_blue_to_int(red, green, blue):
     assert 0 <= red < 512
     assert 0 <= blue < 512
     assert 0 <= green < 512, green
     return (red << 16) + (green << 8) + blue
 
 
 def _hex_regexp():
-    return re.compile('(([0-9a-f]{6})|([0-9a-f]{3}))', re.IGNORECASE)
+    return re.compile("(([0-9a-f]{6})|([0-9a-f]{3}))", re.IGNORECASE)
 
 
 def _extract_html_hex(string):
     """Get the first 3 or 6 hex digits in the string"""
     try:
-        hex_string = string and _hex_regexp().search(string).group(0) or ''
+        hex_string = string and _hex_regexp().search(string).group(0) or ""
     except AttributeError:
         return None
     if len(hex_string) == 3:
         hex_string = hex_string[0] * 2 + hex_string[1] * 2 + hex_string[2] * 2
     return hex_string
 
 
@@ -86,33 +87,33 @@
         return None
     if not hex_string:
         return 0
     return int(hex_string, 16)
 
 
 def html_to_html(string):
-    digits = string.lstrip('#').upper()
+    digits = string.lstrip("#").upper()
     if len(digits) == 3:
-        return ''.join([d * 2 for d in digits])
+        return "".join([d * 2 for d in digits])
     return digits
 
 
 def hashed_html(string):
-    return '#%s' % html_to_html(string)
+    return f"#{html_to_html(string)}"
 
 
 def html_to_red_green_blue(string):
     string = _extract_html_hex(string)
-    if string is None:
+    if not string:
         return None, None, None
     return int(string[:2], 16), int(string[2:4], 16), int(string[4:], 16)
 
 
 def integer_to_html(integer):
-    return '#%06X' % integer
+    return "#%06X" % integer
 
 
 def html_to_ansi(string):
     i = html_to_small_ansi(string)
     if i is not None:
         return i
     i = html_to_int(string)
@@ -128,30 +129,30 @@
     else:
         r, g, b = ansi_to_red_green_blue(ansi)
     return red_green_blue_to_int(r, g, b)
 
 
 def small_values():
     return [
-        (0x00, '#000000'),
-        (0x01, '#800000'),
-        (0x02, '#008000'),
-        (0x03, '#808000'),
-        (0x04, '#000080'),
-        (0x05, '#800080'),
-        (0x06, '#008080'),
-        (0x07, '#C0C0C0'),
-        (0x08, '#808080'),
-        (0x09, '#FF0000'),
-        (0x0A, '#00FF00'),
-        (0x0B, '#FFFF00'),
-        (0x0C, '#0000FF'),
-        (0x0D, '#FF00FF'),
-        (0x0E, '#00FFFF'),
-        (0x0F, '#000000'),
+        (0x00, "#000000"),
+        (0x01, "#800000"),
+        (0x02, "#008000"),
+        (0x03, "#808000"),
+        (0x04, "#000080"),
+        (0x05, "#800080"),
+        (0x06, "#008080"),
+        (0x07, "#C0C0C0"),
+        (0x08, "#808080"),
+        (0x09, "#FF0000"),
+        (0x0A, "#00FF00"),
+        (0x0B, "#FFFF00"),
+        (0x0C, "#0000FF"),
+        (0x0D, "#FF00FF"),
+        (0x0E, "#00FFFF"),
+        (0x0F, "#000000"),
     ]
 
 
 def small_integers():
     return [integer for integer, _html in small_values()]
 
 
@@ -173,17 +174,31 @@
 def ansi_to_html(ansi):
     if ansi < 16:
         return small_ansi_to_html(ansi)
     i = ansi_to_int(ansi)
     return integer_to_html(i)
 
 
-def name_to_int(name):
+def name_to_id(name):
     """Get a number for that colour name
 
     if not a name, then not a number
+
+    >>> assert name_to_id('red') == 1
     """
     if not name:
-        return float('nan')
+        return None
     lower = name.lower()
     cga_names = {s: i for i, s in enumerate(colour_names.cga())}
     return cga_names.get(lower) or html_to_small_ansi(lower)
+
+
+def id_to_name(i):
+    """get the name of the colour with that id
+
+    >>> assert id_to_name(1) == 'red'
+    """
+    assert i >= 0
+    cgas = colour_names.cga()
+    if i < len(cgas):
+        return cgas[i].lower()
+    return ansi_to_html(i)
```

### Comparing `pysyte-0.7.9/pysyte/colours/colour_numbers.test` & `pysyte-0.8.0/pysyte/colours/test/colour_numbers.tests`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,121 @@
 The colour_numbers module
 =========================
 
     >>> from pysyte.colours import colour_numbers
-    >>> assert 'numbers known to represent colours' in  colour_numbers.__doc__
 
-Convert html strings to integers
---------------------------------
 
-A "web colour" is represented by a string with 3 hex values for R, G, B
-    For example
-    >>> html = '#00FF00'
+More modules for testing
+------------------------
 
-Converting that to an integer and back gives itself
-    >>> assert html == colour_numbers.integer_to_html(colour_numbers.html_to_int(html))
+    >>> import random
 
-Same result if we start with slight variations on the string
-    >>> assert html == colour_numbers.integer_to_html(colour_numbers.html_to_int(html.lower()))
-    >>> assert html == colour_numbers.integer_to_html(colour_numbers.html_to_int(html.replace('#','0x')))
+integers
+--------
 
-We can also use 3 single chars
-    >>> assert html == colour_numbers.integer_to_html(colour_numbers.html_to_int('0x0F0'))
+There are 16 small-numbered colours (CGA)
+    >>> assert all([bool(0 <= i <= 0x0F) for i in colour_numbers.small_integers()])
+
+integer to ansi
+---------------
+
+    >>> small_int = random.randint(0, 15)
+    >>> assert colour_numbers.integer_to_ansi(small_int) == small_int
+
+    >>> assert colour_numbers.integer_to_ansi(0x00005F) == 17
+    >>> assert colour_numbers.integer_to_ansi(0x000087) == 18
+    >>> assert colour_numbers.integer_to_ansi(0x0000AF) == 19
+    >>> assert colour_numbers.integer_to_ansi(0x0000D7) == 20
+    >>> assert colour_numbers.integer_to_ansi(0x0000FF) == 21
+
+    >>> assert colour_numbers.integer_to_ansi(0x005F00) == 22
+    >>> assert colour_numbers.integer_to_ansi(0x008700) == 28
+    >>> assert colour_numbers.integer_to_ansi(0x00AF00) == 34
+    >>> assert colour_numbers.integer_to_ansi(0x00D700) == 40
+    >>> assert colour_numbers.integer_to_ansi(0x00FF00) == 46
+
+    >>> assert colour_numbers.integer_to_ansi(0x5F0000) == 52
+    >>> assert colour_numbers.integer_to_ansi(0x870000) == 88
+    >>> assert colour_numbers.integer_to_ansi(0xAF0000) == 124
+    >>> assert colour_numbers.integer_to_ansi(0xD70000) == 160
+    >>> assert colour_numbers.integer_to_ansi(0xFF0000) == 196
+
+    >>> assert (
+    ...     colour_numbers.integer_to_html(colour_numbers.ansi_to_int(196)) == '#FF0000'
+    ... )
+
+    >>> assert colour_numbers.integer_to_ansi(0xFFFFFE) == 231
+    >>> assert colour_numbers.integer_to_ansi(0xFFFFFF) == 231
+
+    >>> assert colour_numbers.integer_to_ansi(0xAFD7FF) == 153
+    >>> assert colour_numbers.integer_to_ansi(0x5FAF87) == 72
+
+
+    >>> assert colour_numbers.integer_to_ansi(0x1C1C1C) == 234
+    >>> assert colour_numbers.integer_to_ansi(0xB2B2B2) == 249
+
+    >>> assert (
+    ...     colour_numbers.integer_to_html(colour_numbers.ansi_to_int(249)) == '#B2B2B2'
+    ... )
+
+Convert to ansi to integer and back
+------------------------------------
+
+    >>> # assert all([colour_numbers.integer_to_ansi(colour_numbers.ansi_to_int(i)) == i for i in range(1,255)])
+
+Convert to html to integer and back
+-----------------------------------
+
+The next iteration might take a while, so we'll skip a few points
+    >>> step = random.randint(0xCC, 0xFF)
+
+Can convert from integer to hex string (html) and back again for any number
+    >>> assert all(
+    ...     [
+    ...         colour_numbers.html_to_int(colour_numbers.integer_to_html(i)) == i
+    ...         for i in range(0x000000, 0xFFFFFF, step)
+    ...     ]
+    ... )
+
+    >>> assert colour_numbers.html_to_int('not a colour code') is None
+
+Can get the integer in 3 parts, for red, green, blue
+    >>> r, g, b = colour_numbers.html_to_red_green_blue('#A79')
+    >>> i = colour_numbers.html_to_int('#A79')
+    >>> assert r * 256 * 256 + g * 256 + b == i
+
+NINO
+    >>> assert colour_numbers.html_to_int('') == 0
+    >>> assert colour_numbers.html_to_red_green_blue('') == (None, None, None)
+
+convert ansi to html and back
+-----------------------------
+
+In converting ANSI codes into html codes and back again some do not pass through unchanged
+    because
+        the "pure colours" have entries for numbers < 16 and for other numbers
+        e.g. '#0000FF' is both 21 and 12
+        (or - "both 12 and 21 give '#0000FF')
+
+Test method to recognise pure colours
+    >>> def pure_colour(string):
+    ...     return string == '#808080' or all([bool(c in '0F') for c in string[1:]])
+    ...
+
+By "pure colour" I mean anything with only 0 and F, and Silver ('#808080')
+    >>> assert pure_colour('#808080')
+    >>> assert pure_colour('#FF0000')
+    >>> assert pure_colour('#FFFF00')
+    >>> assert not pure_colour('#005f87')
+
+So now we can test that (with the exception of such pure colours)
+    all colours pass through ANSI -> HTML -> ANSI
+    >>> for i in range(1, 255):
+    ...     html = colour_numbers.ansi_to_html(i)
+    ...     if pure_colour(html):
+    ...         continue
+    ...     if colour_numbers.html_to_ansi(html) != i:
+    ...         break
+    ...
 
-Any 3-char hex string is same as the 6-char version by just doubling the characters
-    (http://en.wikipedia.org/wiki/Web_colors#Shorthand_hexadecimal_form)
-    >>> assert colour_numbers.html_to_int('0x09C') == colour_numbers.html_to_int('#0099cc')
-
-Fixing HTML strings
--------------------
-
-    >>> assert colour_numbers.html_to_html('f00') == 'FF0000'
-    >>> assert colour_numbers.hashed_html('f00') == '#FF0000'
-
-Converting html colours to ANSI colours
----------------------------------------
-
-Convert an HTML colour string to an ANSI code (which is a number)
-    (Test values here come from https://github.com/twoerner/xterm-256colour/blob/master/xtermcolours.sh)
-
-    >>> html, ansi = '#875F5F', 95
-    >>> assert colour_numbers.html_to_ansi(html) == ansi
-
-And back again
-    >>> # assert colour_numbers.ansi_to_html(ansi) == html
-
-VGA colours
------------
-
-"Pure" colours have ANSI values less than 16 and come in "dark" and "light" shades
-    These colours were used on very old terminals, back when I was a lad
-    For example, blue:
-
-Dark blue
-    >>> assert colour_numbers.ansi_to_html(4) == '#000080'
-
-Lighter blue:
-    >>> assert colour_numbers.ansi_to_html(12) == '#0000FF'
-
-Names to numbers
-----------------
-
-Recognises colour names from English, case-insensitively
-    >>> assert colour_numbers.name_to_int('green') == 2 == colour_numbers.name_to_int('GREEN')
-
-And other languages
-    >>> assert colour_numbers.name_to_int('light red') == colour_numbers.name_to_int('f00')
-
-Colour names are case-insensitive
-    >>> assert colour_numbers.name_to_int('FF0000') == colour_numbers.name_to_int('f00')
+    >>> assert colour_numbers.small_ansi_to_html(0x0A) == '#00FF00'
+    >>> assert colour_numbers.small_ansi_to_html(0x10) is None
```

### Comparing `pysyte-0.7.9/pysyte/colours/texts.test` & `pysyte-0.8.0/pysyte/colours/test/texts.test`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 The texts module
 ================
 
     >>> from pysyte.colours import texts
     >>> assert 'colours in texts' in texts.__doc__
 
 Basic usage:
-    >>> hello = texts.colour_text('H', 'green').colour_text('ello ')
+    >>> hello = texts.colour_text('green', 'H').colour_text(None, 'ello ')
 
 Shorter way:
-    >>> world = texts.colour('W', 'red').text('orld')
+    >>> world = texts.red('W').none('orld')
 
 Both methods give a coloured tail
     >>> hello
     <ColouredTail '\x1b[32mH\x1b[2m\x1b[0m''ello '>
     >>> world
     <ColouredTail '\x1b[31mW\x1b[2m\x1b[0m''orld'>
 
 Adds in ANSI sequences (looks better on terminal than in a doctest)
     >>> assert str(hello) == '\x1b[32mH\x1b[2m\x1b[0mello '
     >>> assert str(world) == '\x1b[31mW\x1b[2m\x1b[0morld'
 
-Convenience method to highlight initials
+Convenience methods to highlight initials
 
-    >>> foo = texts.colour('H', 'red').colour('ello')
-    >>> assert foo == texts.colour_initial('Hello', 'red')
+    >>> foo = texts.colour('red', 'H').colour('ello')
+    >>> assert foo == texts.colour_initial('red', 'Hello')
 
+Can also take a list
+    >>> assert foo == texts.colour_initials('red', ['Hello'])
+
+For prompting users
+    >>> assert (
+    ...     texts.prompt_text('red', 'fred')
+    ...     == '\x01\x1b[31m\x02fred\x01\x1b[2m\x1b[0m\x02'
+    ... )
```

### Comparing `pysyte-0.7.9/pysyte/getch.py` & `pysyte-0.8.0/pysyte/oss/getch.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,35 +9,41 @@
         but keeping the implementatation
 
     And reducing down to just the tty version
         No need here for Windows/Carbon
 """
 
 import re
+import getpass
 import signal
 import sys
 import tty
 from curses import ascii
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Tuple
 
 import termios
 
 
 class NoKeys(StopIteration):
-    """Better name for StopIteration caused by running out of keys"""
+    """A StopIteration caused by running out of keys"""
+
     pass
 
 
 def get_ord():
     """The integer ordinal of the next byte read from sys.stdin"""
     return ord(sys.stdin.read(1))
 
 
 class TerminalContext(object):
     """Context wrapper to set up termios values"""
-    # pylint: disable=too-few-public-methods
+
     def __init__(self):
         self.fd = None
         self.old_settings = None
 
     def __enter__(self):
         self.fd = sys.stdin.fileno()
         self.old_settings = termios.tcgetattr(self.fd)
@@ -51,25 +57,26 @@
             pass  # exception
         if self.old_settings:
             termios.tcsetattr(self.fd, termios.TCSADRAIN, self.old_settings)
 
 
 class Timeout(Exception):
     """A timeout has occurred"""
+
     pass
 
 
 def timeout_raiser(_signum, _frame):
     """Raise a timeout exception"""
     raise Timeout()
 
 
 class TimerContext(object):
     """Context wrapper for a timeout"""
-    # pylint: disable=too-few-public-methods
+
     def __init__(self, seconds):
         self.seconds = seconds
         self.old_handler = None
         self.timed_out = False
 
     def __enter__(self):
         self.old_handler = signal.signal(signal.SIGALRM, timeout_raiser)
@@ -81,15 +88,15 @@
         if self.old_handler:
             signal.signal(signal.SIGALRM, self.old_handler)
         if isinstance(value, Timeout):
             self.timed_out = True
             return True
 
 
-_key_cache = []
+_key_cache: List[Tuple[int, ...]] = []
 
 
 def cache_keys(keys):
     """Allow debugging via PyCharm"""
     d = known_keys()
     known_names = dict(zip(d.values(), d.keys()))
     for k in keys:
@@ -105,15 +112,15 @@
     For example, pressing 'A' will give (65,)
     """
     try:
         return _key_cache.pop()
     except IndexError:
         pass
     result = []
-    terminators = 'ABCDFHPQRS~'
+    terminators = "ABCDFHPQRS~"
     with TerminalContext():
         code = get_ord()
         result.append(code)
         if code == 27:
             with TimerContext(0.1) as timer:
                 code = get_ord()
             if not timer.timed_out:
@@ -128,26 +135,27 @@
                         if chr(code) in terminators:
                             break
     return tuple(result)
 
 
 class ExtendedKey(Exception):
     """Raised for an unrecognised Extended key code"""
+
     def __init__(self, codes):
-        super(ExtendedKey, self).__init__(
-            'Too many key codes: %s' % repr(codes))
+        super(ExtendedKey, self).__init__(f"Too many key codes: {codes!r}")
         self.codes = codes
 
 
-def getch():
-    """Get a char or and ExtendedKey from a keyboard"""
-    codes = _get_keycodes()
-    if len(codes) == 1:
-        return chr(codes[0])
-    raise ExtendedKey(codes)
+def getch() -> int:
+    """Get a char or raise ExtendedKey from a keyboard"""
+    keycodes = _get_keycodes()
+    code, *codes = keycodes
+    if not codes:
+        return code
+    raise ExtendedKey(keycodes)
 
 
 def get_codes():
     """Get a tuple of stringified keycodes from the keyboard"""
     return tuple(str(_) for _ in _get_keycodes())
 
 
@@ -165,15 +173,15 @@
         return control_key_name(code)
     return get_extended_key_name(codes)
 
 
 def get_menu(**kwargs):
     key = get_key()
     for name, string in kwargs.items():
-        match = re.match('^%s$' % string, key)
+        match = re.match(f"^{string}$", key)
         if match:
             return name
         if key in name or key in string:
             return name
     return key
 
 
@@ -209,62 +217,94 @@
         return getch()
     except ExtendedKey as e:
         return e.codes
 
 
 def control_key_name(code):
     """Prefix the name of a control key with '^'"""
-    return '^%s' % (chr(code - 1 + ord('A')))
+    name = chr(code - 1 + ord("A"))
+    return f"^{name}"
 
 
 def get_extended_key_name(codes):
     """Get a name for the extended key with those codes
 
     Names are defined herein
     """
     return known_keys()[codes]
 
 
-def known_keys():
-    return {
-        (27, 79, 70): 'end',
-        (27, 79, 72): 'home',
-        (27, 79, 80): 'F1',
-        (27, 79, 81): 'F2',
-        (27, 79, 82): 'F3',
-        (27, 79, 83): 'F4',
-        (27, 91, 49, 53, 126): 'F5',
-        (27, 91, 49, 55, 126): 'F6',
-        (27, 91, 49, 56, 126): 'F7',
-        (27, 91, 49, 57, 126): 'F8',
-        (27, 91, 50): 'insert',
-        (27, 91, 50, 48, 126): 'F9',
-        (27, 91, 50, 49, 126): 'F10',
-        (27, 91, 50, 51, 126): 'F11',
-        (27, 91, 50, 52, 126): 'F12',
-        (27, 91, 49, 59, 50, 80): 'F13',
-        (27, 91, 49, 59, 50, 83): 'F16',
-        (27, 91, 49, 53, 59, 50, 126): 'F17',
-        (27, 91, 49, 55, 59, 50, 126): 'F18',
-        (27, 91, 49, 56, 59, 50, 126): 'F19',
-        (27, 91, 51, 126): 'Del',
-        (27, 91, 51): 'delete',
-        (27, 91, 53): 'page up',
-        (27, 91, 53, 126): 'page up',
-        (27, 91, 54): 'page down',
-        (27, 91, 54, 126): 'page down',
-        (27, 91, 65): 'up',
-        (27, 91, 66): 'down',
-        (27, 91, 67): 'right',
-        (27, 91, 68): 'left',
+def known_keys() -> Dict[Tuple[int, ...], str]:
+    result = {
+        (27, 79, 70): "end",
+        (27, 79, 72): "home",
+        (27, 79, 80): "F1",
+        (27, 79, 81): "F2",
+        (27, 79, 82): "F3",
+        (27, 79, 83): "F4",
+        (27, 91, 49, 53, 126): "F5",
+        (27, 91, 49, 53, 59, 50, 126): "F17",
+        (27, 91, 49, 55, 126): "F6",
+        (27, 91, 49, 55, 59, 50, 126): "F18",
+        (27, 91, 49, 56, 126): "F7",
+        (27, 91, 49, 56, 59, 50, 126): "F19",
+        (27, 91, 49, 57, 126): "F8",
+        (27, 91, 49, 59, 50, 65): "&up",
+        (27, 91, 49, 59, 50, 66): "&down",
+        (27, 91, 49, 59, 50, 67): "&right",
+        (27, 91, 49, 59, 50, 68): "&left",
+        (27, 91, 49, 59, 50, 80): "F13",
+        (27, 91, 49, 59, 50, 83): "F16",
+        (27, 91, 50): "insert",
+        (27, 91, 50, 48, 126): "F9",
+        (27, 91, 50, 49, 126): "F10",
+        (27, 91, 50, 51, 126): "F11",
+        # (27, 91, 50, 52, 126): "Cmd Backspace",
+        (27, 91, 50, 52, 126): "F12",
+        (27, 91, 51): "delete",
+        (27, 91, 51, 126): "Del",
+        # (27, 91, 51, 126): "FF12",
+        (27, 91, 53): "page up",
+        (27, 91, 53, 126): "page up",
+        (27, 91, 54): "page down",
+        (27, 91, 54, 126): "page down",
+        (27, 91, 65): "up",
+        (27, 91, 66): "down",
+        (27, 91, 67): "right",
+        (27, 91, 68): "left",
+        (27,): "esc",
+        (1,): "Ctrl A",
+        (32,): "space",
+        (48,): "0",
+        (65,): "A",
+        (97,): "a",
+        (127,): "backspace",
     }
+    return add_ascii_keys(result)
+
+
+def add_ascii_keys(data) -> Dict[Tuple[int, ...], str]:
+    """Update the data with ascii keys
+
+    >>> data = add_ascii_keys({})
+    >>> assert data[(48,)] == '0'
+    >>> assert data[(66,)] == 'B'
+    >>> assert data[(99,)] == 'c'
+    """
+    # See previous function for previous key, value pairs
+    for i in range(32):
+        data[(i + 1,)] = f"Ctrl {chr( ord('A') + i)}"
+    for i in range(32, 127):
+        data[(i,)] = f"{chr(i)}"
+    return data
 
 
 def _yielder(getter):
     """Keep yielding from that getter until KeyboardInteruptted"""
+
     def yield_till_stopped():
         """Yield from the getter until KeyboardInteruptted"""
         while True:
             try:
                 yield getter()
             except KeyboardInterrupt:
                 raise NoKeys
@@ -280,27 +320,31 @@
 
 def get_string():
     """A better str(_get_keycodes()) method"""
     keycodes = _get_keycodes()
     initial_code, codes = keycodes[0], keycodes[1:]
     initial_char = chr(initial_code)
     if initial_code == 27:
-        initial_char = '\\e'
+        initial_char = "\\e"
     elif not ascii.isgraph(initial_char):
-        initial_char = '\\x%x' % initial_code
-    chars = ''.join([chr(c) for c in codes])
-    return ''.join((initial_char, chars))
-
-
-def yield_asciis_old():
-    """This one is deprecated"""
-    k = get_ascii()
-    while True:
-        yield k
-
-
-def ask_user(prompt, default=None):
-    prompt_default = str('[%s]' % default) if default else ''
-    print('%s %s? ' % (prompt, prompt_default), end='')
-    result = getch().lower().strip()
+        initial_char = "\\x%x" % initial_code
+    chars = "".join([chr(c) for c in codes])
+    return "".join((initial_char, chars))
+
+
+user = getpass.getuser()
+
+
+def ask_user_simplified(
+    prompt: str = f"Hello {user}",
+    default_key: str = "y",
+    simplifier: Callable = lambda x: x.lower(),
+):
+    if prompt or default_key:
+        print(f"{prompt} [{default_key}] ", end="")
+    result = simplifier(getch())
+    if not result:
+        result = default_key
+    if not result:
+        raise KeyboardInterrupt
     print()
-    return result or default
+    return result
```

### Comparing `pysyte-0.7.9/pysyte/imports.py` & `pysyte-0.8.0/pysyte/importers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,160 +1,187 @@
+"""Import imports for pysyte"""
 import os
+import importlib
+import linecache
 import ast
-import imp
 from collections import defaultdict
-
-
-from pysyte import dictionaries
+from contextlib import contextmanager
+from dataclasses import dataclass
+from typing import Iterator
 
 
 class ImportVisitor(ast.NodeVisitor):
     def __init__(self):
-        dd = defaultdict
-        self.froms = dd(list)
-        self.imports = dd(list)
-        self.used = dd(list)
-        super(ImportVisitor, self).__init__()
+        super().__init__()
+        self.imports = defaultdict(list)
+        self.froms = defaultdict(list)
+
+    def imported(self, name, line):
+        raise NotImplementedError(f"imported({name}, {line}")
+
+    def collect_names(self, node):
+        names = [(_.name, getattr(_, "asname", None)) for _ in node.names]
+        for name, alias in names:
+            self.imports[alias if alias else name].append(node.lineno)
+        return names
 
     def find_value_id(self, node, attr=None):
         if not node:
             return None
-        value = getattr(node, 'value', None)
+        value = getattr(node, "value", None)
         if not value:
             if attr:
-                value = getattr(getattr(node, attr, None), 'value', None)
+                value = getattr(getattr(node, attr, None), "value", None)
                 if not value:
-                    name = getattr(getattr(node, attr, None), 'id', None)
+                    name = getattr(getattr(node, attr, None), "id", None)
                     if name:
                         return name
         if not value:
-            return None
-        result = getattr(value, 'id', None)
+            return getattr(node, "id", None)
+        result = getattr(value, "id", None)
         if result:
             return result
         return self.find_value_id(value, attr)
 
     def find_name(self, node, *args):
-        name = getattr(node, 'id', None)
+        name = getattr(node, "id", None)
         if name is not None:
             return name
         for attribute in args:
             attr = getattr(node, attribute, None)
             if attr:
                 name = self.find_name(attr, *args)
                 if name:
                     return name
         return None
 
-    def check_usage(self, name, line):
-        if not name:
-            return
-        found = name in self.imports
-        if found:
-            self.used[name].append(line)
-
-    def unused(self):
-        return {k: v for k, v in self.imports.items() if k not in self.used}
-
-    def multiples(self):
-        return {k: v for k, v in self.imports.items() if len(v) > 1}
-
-    def collect_names(self, node):
-        names = [(_.name, getattr(_, 'asname', None)) for _ in node.names]
-        for name, alias in names:
-            self.imports[alias if alias else name].append(node.lineno)
-        return names
-
     def visit_ImportFrom(self, node):
-        if node.module != '__future__':
+        if node.module != "__future__":
             names = self.collect_names(node)
             self.froms[node.module].extend(names)
         self.generic_visit(node)
 
     def visit_Import(self, node):
         self.collect_names(node)
         self.generic_visit(node)
 
     def visit_FunctionDef(self, node):
         for decorator in node.decorator_list:
-            name = self.find_name(decorator, 'func', 'value')
-            self.check_usage(name, decorator.lineno)
+            name = self.find_name(decorator, "func", "value")
+            self.imported(name, decorator)
         self.generic_visit(node)
 
     def visit_Subscript(self, node):
         name = self.find_value_id(node)
-        name2 = self.find_name(node, 'value')
+        name2 = self.find_name(node, "value")
         assert name == name2
-        self.check_usage(name, node.lineno)
-        subscript = self.find_value_id(node.slice)
-        name2 = self.find_name(node.slice, 'value')
-        assert subscript == name2
-        self.check_usage(subscript, node.lineno)
+        self.imported(name, node)
+        subname = self.find_value_id(node.slice)
+        assert subname == self.find_name(node.slice, "value")
+        self.imported(subname, node)
         self.generic_visit(node)
 
     def visit_Attribute(self, node):
         try:
-            self.check_usage(node.value.id, node.lineno)
+            self.imported(node.value.id, node.lineno)
+            full_name = f"{node.value.id}.{node.attr}"
+            self.imported(full_name, node.lineno)
         except AttributeError:
             pass
         self.generic_visit(node)
 
     def visit_ClassDef(self, node):
         for base in node.bases:
-            name = self.find_name(base, 'value')
-            self.check_usage(name, node.lineno)
+            name = self.find_name(base, "value")
+            self.imported(name, node)
         self.generic_visit(node)
 
     def visit_Call(self, node):
         func = node.func
         try:
             name = func.id
         except AttributeError:
-            name = self.find_value_id(func, 'func')
-            name2 = self.find_name(node, 'value', 'func')
+            name = self.find_value_id(func, "func")
+            name2 = self.find_name(node, "value", "func")
             assert name == name2
-        self.check_usage(name, node.lineno)
+        self.imported(name, node)
         self.generic_visit(node)
 
     def visit_Name(self, node):
         name = self.find_name(node)
-        self.check_usage(name, node.lineno)
+        self.imported(name, node)
         self.generic_visit(node)
 
 
-def find_imports(tree):
-    visitor = ImportVisitor()
-    visitor.visit(tree)
-    return visitor
+class ImportUser(ImportVisitor):
+    def __init__(self):
+        super().__init__()
+        self.used = defaultdict(list)
+
+    def imported(self, name, node):
+        if not name:
+            return
+        if name in self.imports:
+            self.used[name].append(node.lineno)
+
+    def unused(self):
+        return {k: v for k, v in self.imports.items() if k not in self.used}
+
+    def unused_lines(self):
+        result = defaultdict(set)
+        for name, lines in self.unused().items():
+            for line in lines:
+                result[line].add(name)
+        return result
 
+    def multiples(self):
+        return {k: v for k, v in self.imports.items() if len(v) > 1}
 
-def parse_python(path):
-    with open(path) as stream:
-        return ast.parse(stream.read(), path)
+    def line(self, line_number, with_number=True):
+        line = linecache.getline(self.path, line_number).rstrip()
+        if not with_number:
+            return line
+        return f"{line_number:4d}: {line}"
 
 
-def extract_imports(script):
-    """Extract all imports from a python script"""
-    if not os.path.isfile(script):
-        raise ValueError('Not a file: %s' % script)
-    parse_tree = parse_python(script)
-    result = find_imports(parse_tree)
-    result.path = script
-    return result
+@dataclass
+class AS3:
+    path: str
+    tree: ast.Module
 
 
-def load_module(package, module_name):
+def find_imports(as3: AS3) -> ImportUser:
+    import_user = ImportUser()
+    import_user.visit(as3.tree)
+    return import_user
 
-    def default_value(key):
 
-        def imp_load(a, b, c):
-            return imp.load_module(full_name, a, b, c)
+@contextmanager
+def parse_python(script) -> Iterator[AS3]:
+    with open(script) as stream:
+        as3 = ast.parse(stream.read(), script)
+        yield AS3(script, as3)
 
-        full_name = '%s.%s' % (package.__name__, module_name)
-        return imp_load(*imp.find_module(key, package.__path__))
 
-    # pylint: disable=protected-access
-    try:
-        _loaded = package._loaded
-    except AttributeError:
-        _loaded = package._loaded = dictionaries.LazyDefaultDict(default_value)
-    return _loaded[module_name]
+def parse(script) -> ImportUser:
+    """Extract all imports from a python script"""
+    if not os.path.isfile(script):
+        raise FileNotFoundError(f"Not a file: {script}")
+    with parse_python(script) as as3:
+        importer = find_imports(as3)
+        importer.path = script  # type: ignore [attr-defined]
+        return importer
+
+
+@contextmanager
+def importer(module):
+    """Provide a context with that module
+
+    >>> with importer(os) as os_, importer('pysyte.importers') as importers:
+    ...     assert os_.path is os.path
+    ...     assert importer.__code__ == importers.importer.__code__
+    ...
+    """
+    if isinstance(module, type(os)):
+        yield module
+    elif isinstance(module, str):
+        yield importlib.import_module(module)
```

### Comparing `pysyte-0.7.9/pysyte/iteration.py` & `pysyte-0.8.0/pysyte/iteration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-try:
-    from itertools import ifilter
-except ImportError:
-    ifilter = filter
+"""Handle iterators for pysyte"""
 
+from typing import Sequence
+from typing import TypeVar
 
-def first(sequence, message=None):
+T = TypeVar("T")  # Declare Type variable
+
+
+def first(sequence: Sequence[T], message=None) -> T:  # Generic function
     """The first item in that sequence
 
     If there aren't any, raise a ValueError with that message
+
+    >>> assert first([1, 2, 3]) == 1
     """
     try:
         return next(iter(sequence))
     except StopIteration:
-        raise ValueError(message or ('Sequence is empty: %s' % sequence))
+        raise ValueError(message or (f"Sequence is empty: {sequence}"))
 
 
-def last(sequence, message=None):
+def last(sequence: Sequence[T], message=None) -> T:
     """The last item in that sequence
 
     If there aren't any, raise a ValueError with that message
+
+    >>> assert last([1, 2, 3]) == 3
     """
-    try:
-        return sequence.pop()
-    except AttributeError:
-        return list(sequence).pop()
-    except IndexError:
-        raise ValueError(message or f'Sequence is empty: {sequence}')
+    return first(list(reversed(sequence)), message)
 
 
-def first_or(sequence, value):
+def first_or(sequence: Sequence[T], value) -> T:
+    """First item in that sequence, or that value
+
+    >>> assert first_or([1, 2, 3], 4) == 1
+    >>> assert first_or([], 4) == 4
+    """
     try:
         return first(sequence)
     except ValueError:
         return value
 
 
-def first_that(predicate, sequence, message=None):
+def first_that(predicate, sequence: Sequence[T], message=None) -> T:
     """The first item in that sequence that matches that predicate
 
     If none matches raise a KeyError with that message
+
+    >>> assert first_that(lambda x: x > 1, [1, 2, 3]) == 2
     """
     try:
-        return next(ifilter(predicate, sequence))
-    except StopIteration:
-        raise KeyError(message or 'Not Found')
+        return first([_ for _ in sequence if predicate(_)])
+    except (ValueError, StopIteration):
+        raise KeyError(message or "Not Found")
```

### Comparing `pysyte-0.7.9/pysyte/keyboard.py` & `pysyte-0.8.0/pysyte/oss/keyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Some keyboard handling code"""
 
 
 import sys
 
 
-from pysyte import getch
+from pysyte.oss import getch
 
 
 def _get_chosen_chars(chooser):
     while True:
         key = getch.get_as_key()
         try:
             if chooser(key):
@@ -25,12 +25,12 @@
 def get_letter():
     return _get_chosen_chars(lambda x: x.isupper() or x.islower())
 
 
 def quit_on_q():
     try:
         key = getch.get_as_key()
-        if key in 'qQ':
+        if key in "qQ":
             sys.exit()
         return key
     except KeyboardInterrupt:
         sys.exit()
```

### Comparing `pysyte-0.7.9/pysyte/paths.py` & `pysyte-0.8.0/pysyte/types/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,215 +1,454 @@
 """A collection of extended path classes and methods
 
 The classes all inherit from the original path.path
 """
 import os
+import re
+import stat
+import sys
+from dataclasses import dataclass
 from fnmatch import fnmatch
+from functools import singledispatch
+from importlib import import_module
+from typing import Iterable
+from typing import List
+from typing import Sequence
+from typing import Tuple
+from typing import Union
+
+from deprecated import deprecated
+
+from path import Path as path_Path
+from pysyte.types.lists import flatten
 
 
 class PathError(Exception):
     """Something went wrong with a path"""
-    prefix = 'Path Error'
 
-    def __init__(self, message):
-        Exception.__init__(self, message)
+    prefix = "Path Error"
+
+
+class MissingPath(PathError):
+    def __init__(self, path, desc=""):
+        self.path = path
+        description = desc or "path"
+        super().__init__(f"Missing {description}{path}")
+
+
+class MissingImport(MissingPath):
+    def __init__(self, module):
+        self.module = module
+        try:
+            path_ = module.__file__
+        except AttributeError:
+            path_ = module.__name__
+        super().__init__(path_, desc="module")
 
 
-class PathAssertions(object):
+class PathAssertions:
     """Assertions that can be made about paths"""
-    # pylint: disable=no-member
 
-    def assert_exists(self):
-        """Raise a PathError if this path does not exist on disk"""
+    def assertExists(self):
         if not self.exists():
-            raise PathError('%s does not exist' % self)
+            raise MissingPath(self)
         return self
 
     def assert_isdir(self):
         """Raise a PathError if this path is not a directory on disk"""
         if not self.isdir():
-            raise PathError('%s is not a directory' % self)
+            raise PathError(f"{self} is not a directory")
         return self
 
     def assert_isfile(self):
         """Raise a PathError if this path is not a file on disk"""
         if not self.isfile():
-            raise PathError('%s is not a file' % self)
+            raise PathError(f"{self} is not a file")
         return self
 
 
-from path import Path as PPath  # pylint: disable=wrong-import-position
+StrPath = Union["StringPath", str]  # many args can be either string or path
+
 
+class StringPath(path_Path):
+    """This class handles the path as if it were just a string
+
+    Sub-classes know about paths qua paths
+    """
 
-class DotPath(PPath):
-    """Some additions to the classic path class"""
     # pylint: disable=abstract-method
+    # pylint: disable=too-many-public-methods
 
-    def __repr__(self):
-        return '<%s %s>' % (
-            self.__class__.__name__,
-            repr(str(self)))
-
-    # The / operator joins paths.
-    def __div__(self, child):
-        """Join two path components, adding a separator character if needed.
+    def __hash__(self):
+        return hash(str(self))
 
-        If the result is a file return self.__file_class__(result)
+    def __repr__(self) -> str:
+        string = repr(f"{self}")
+        return f"<{self.__class__.__name__} {string}>"
 
-        >>> p = DotPath('/home/guido')
-        >>> p.__div__('fred') == p / 'fred' == p.joinpath('fred')
-        True
+    @deprecated(version="0.7.5", reason="Please use Python 3")
+    def __div__(self, other) -> "StringPath":
+        """Need to cover parent's use of older idiom"""
+        return self.__truediv__(other)
+
+    def __truediv__(self, substring: str) -> "StringPath":
+        """Handle the / operator
+
+        Add substring to self
+
+        >>> p = StringPath("/path/to")
+        >>> assert p.__truediv__("fred") == p / "fred"
+        >>> assert p / "fred" == "/path/to/fred"
+        >>> assert p / None is p
         """
-        if child:
-            result = os.path.join(self, child)
-        else:
-            result = str(self)  # pylint: disable=redefined-variable-type
-        return self.as_existing_file(result)
+        if not substring:
+            return self
+        full_string = os.path.join(str(self), substring)
+        return makepath(full_string)
+
+    def __floordiv__(self, substrings: Sequence[str]) -> "StringPath":
+        """Handle the // operator
+
+        Add substrings to self like a path in local os
+
+        >>> p = StringPath("/path/to")
+        >>> assert p.__floordiv__("fred") == p // "fred"
+        >>> assert p // ["module", "fred.py"] == "/path/to/module/fred.py"
+        >>> assert p // None is p
+        """
+        if not substrings:
+            return self
+        string = str(self)
+        strings = [string] + list(substrings)
+        return makepath(os.path.join(*strings))
+
+    def __eq__(self, other) -> bool:
+        return str(self) == str(other)
+
+    def __lt__(self, other) -> bool:
+        return str(self) < str(other)
+
+    # functools.total_ordering does not work properly cos we inherit from str
+    # Hence: we do need to define next 3
+    def __le__(self, other):
+        return self.__eq__(other) or self.__lt__(other)
+
+    def __gt__(self, other):
+        return not self.__le__(other)
 
-    __truediv__ = __div__
+    def __ge__(self, other):
+        return not self.__lt__(other)
 
-    def __cmp__(self, other):
-        return cmp(str(self), str(other))
+    def __contains__(self, other) -> bool:
+        """The other is in self if self.contains(other)
 
-    def _next_class(self, string):
-        return self.as_existing_file(string)
-
-    def as_existing_file(self, filepath):
-        """Return the file class for existing files only"""
-        if os.path.isfile(filepath) and hasattr(self, '__file_class__'):
-            return self.__file_class__(filepath)  # pylint: disable=no-member
-        return self.__class__(filepath)
+        this method should be specialised in sub-classes
+        """
+        return self.contains(other)
+
+    def contains(self, other: StrPath) -> bool:
+        """If other is also a path then this path should start with other
+
+        E.g. /path/to/file is "in" /path
+
+        Otherwise, just use the sub-string sense of "in"
+        """
+        if isinstance(other, StringPath):
+            return str(other).startswith(str(self))
+        return str(other) in str(self)
+
+    def basename(self) -> str:
+        return str(super().basename())
+
+    @property
+    def basename_(self) -> str:
+        return self.basename()
+
+    @property
+    def name(self) -> str:
+        return str(super().name)
+
+    @property
+    def stem(self) -> "StringPath":
+        stem, *_ = self.splitexts()
+        return stem
+
+    @property
+    def stem_name(self) -> str:
+        return self.stem.name
+
+    def splitexts(self) -> Tuple["StringPath", str]:
+        """Split all extensions from the path
+
+        >>> p = FilePath('here/fred.tar.gz')
+        >>> assert p.splitexts() == ('here/fred', '.tar.gz')
+        """
+        copy = self[:]
+        filename, ext = os.path.splitext(copy)
+        zippers = (
+            ".gz",
+            ".bz",
+            ".zip",
+            ".bzip",
+        )
+        for zipper in zippers:
+            if ext == zipper:
+                filename, ext_ = os.path.splitext(filename)
+                ext = f"{ext_}{zipper}"
+        return self.__class__(filename), ext
+
+    def add_ext(self, *args) -> "StringPath":
+        """Join all args as extensions
+
+        Strip any leading `.` from args
+
+        >>> source = makepath(__file__)
+        >>> new = source.add_ext('txt', '.new')
+        >>> assert new.name.endswith('.py.txt.new')
+        """
+        exts = [(a[1:] if a[0] == "." else a) for a in args]
+        string = ".".join([self] + list(exts))
+        return makepath(string)
+
+    def add_missing_ext(self, ext: str) -> "StringPath":
+        """Add that extension, if it is missing
+
+        >>> fred = makepath("fred.py")
+        >>> assert fred.add_missing_ext(".py") == fred
+        >>> assert fred.add_missing_ext(".txt").endswith(".py.txt")
+        """
+        copy = self[:]
+        _stem, old = os.path.splitext(copy)
+        extension = f'.{ext.lstrip(".")}'
+        if old == extension:
+            return makepath(self)
+        return self.add_ext(extension)
+
+    def extend_by(self, ext: str) -> "StringPath":
+        """The path to the file changed to use the given ext
+
+        >>> fred = "/path/to/fred.fred"
+        >>> assert makepath("/path/to/fred").extend_by("fred") == fred
+        >>> assert makepath("/path/to/fred.txt").extend_by(".fred") == fred
+        >>> assert makepath("/path/to/fred.txt").extend_by("..fred") == fred
+        """
+        copy = self[:]
+        filename, _ = os.path.splitext(copy)
+        return makepath(f'{filename}.{ext.lstrip(".")}')
+
+    def has_vcs_dir(self):
+        for vcs_dir in (".git", ".svn", ".hg"):
+            if self.fnmatch_part(vcs_dir):
+                return True
+        return False
+
+
+def ext_language(ext, exts=None, simple=True):
+    """Language of the extension in those extensions
+
+    If exts is supplied, then restrict recognition to those exts only
+    If exts is not supplied, then use all known extensions
+
+    >>> ext_language('.py') == 'python'
+    True
+    """
+    languages = {
+        ".py": "python",
+        ".py2": "python" if simple else "python2",
+        ".py3": "python" if simple else "python3",
+        ".sh": "bash",
+        ".bash": "bash",
+        ".pl": "perl",
+        ".txt": "english",
+    }
+    ext_languages = {_: languages[_] for _ in exts} if exts else languages
+    return ext_languages.get(ext)
+
+
+class NonePath(StringPath):
+    def __init__(self, string=None):
+        self.string = string if string else ""
+        self.proxy = FilePath(self.string) or DirectPath(self.string)
+
+    def __str__(self):
+        return self.string
+
+    def __repr__(self):
+        string = self.string
+        if self.proxy:
+            string = str(self.proxy)
+        return f'<{self.__class__.__name__} "{string}">'
+
+    def __bool__(self):
+        return False
+
+    def __eq__(self, other):
+        if self.string:
+            return str(self) == str(other)
+        return not other
+
+    def __lt__(self, other):
+        if self.string and other:
+            return str(self) < str(other)
+        return bool(other)
+
+    def contains(self, other: StrPath) -> bool:
+        """As this is not a real path, just use the substring sense"""
+        return str(other) in str(self)
+
+    def __truediv__(self, child):
+        result = os.path.join(self.string, child) if child else self.string
+        return makepath(result)
+
+    @property
+    def parent(self):
+        if "/" not in self.string:
+            return None
+        parent_string = "/".join(self.string.split("/")[:-1])
+        return makepath(parent_string)
+
+    def exists(self):
+        return False
+
+    isdir = isfile = isexec = isroot = exists
+
+    def __getattr__(self, name):
+        return getattr(self.proxy, name, None)
+
+    def makedirs(self):
+        os.makedirs(str(self))
+
+
+class DotPath(StringPath):
+    """This class add path-handling to a string"""
 
     def parent_directory(self):
-        if str(self) == '/':
+        if self.isroot():
             return None
         return self.parent
 
+    def parent_directories(self):
+        if self.isroot():
+            return []
+        parent = self.parent
+        return [parent] + parent.parent_directories()
+
     def directory(self):
         """Return a path to the path's directory"""
         return self.parent
 
     def dirnames(self):
         """Split the dirname into individual directory names
 
         An absolute path starts with an empty string, a relative path does not
 
-        >>> DotPath(u'/path/to/module.py').dirnames() == [u'', u'path', u'to']
+        >>> DotPath('/path/to/module.py').dirnames() == ['/', 'path', 'to']
         True
-        >>> DotPath(u'path/to/module.py').dirnames() == [u'path', u'to']
+        >>> DotPath('path/to/module.py').dirnames() == ['path', 'to']
         True
         """
-        return self.dirname().split(os.path.sep)
+        return [str(_) for _ in self.directory().split(os.path.sep)]
 
     def dirpaths(self):
         """Split the dirname into individual directory names
 
         An absolute path starts with an empty string, a relative path does not
 
-        >>> p = DotPath(u'/path/to/x.py')
-        >>> p.paths == p.dirpaths()
-        True
+        >>> p = DotPath('/path/to/x.py')
+        >>> assert p.paths == p.dirpaths()
         """
-        parts = self.parts()
-        result = [DotPath(parts[0] or '/')]
+        parts = self.split()
+        result = [DotPath(parts[0] or "/")]
         for name in parts[1:]:
             result.append(result[-1] / name)
         return result
 
-    def parts(self):
-        """Split the path into parts like Pathlib
-
-        >>> expected = ['/', 'path', 'to', 'there']
-        >>> assert DotPath('/path/to/there').parts() == expected
-        """
-        parts = self.split(os.path.sep)
-        parts[0] = parts[0] and parts[0] or '/'
-        return parts
-
     def directories(self):
         """Split the dirname into individual directory names
 
         No empty parts are included
 
-        >>> DotPath(u'path/to/module.py').directories() == [u'path', u'to']
+        >>> DotPath('path/to/module.py').directories() == ['path', 'to']
         True
-        >>> DotPath(u'/path/to/module.py').directories() == [u'path', u'to']
+        >>> DotPath('/path/to/module.py').directories() == ['/', 'path', 'to']
         True
         """
         return [d for d in self.dirnames() if d]
 
     parents = property(
-        dirnames, None, None,
+        dirnames,
+        None,
+        None,
         """ This path's parent directories, as a list of strings.
 
-        >>> DotPath(u'/path/to/module.py').parents == [u'', u'path', u'to']
+        >>> DotPath('/path/to/module.py').parents == ['/', 'path', 'to']
         True
-        """)
+        """,
+    )
 
     paths = property(
-        dirpaths, None, None,
+        dirpaths,
+        None,
+        None,
         """ This path's parent directories, as a sequence of paths.
 
         >>> paths = DotPath('/usr/bin/vim').paths
-        >>> paths[-1].isfile()  # vim might be a link
-        True
-        >>> paths[-2] == paths[-1].parent
-        True
-        >>> paths[-3] == paths[-2].parent
-        True
-        >>> paths[-4] == paths[-3].parent
-        True
-        >>> paths[-4] == paths[0]
-        True
-        """)
+        >>> assert paths[-1].exists()  # vim might be a link
+        >>> assert paths[-2] == paths[-1].parent
+        >>> assert paths[-3] == paths[-2].parent
+        >>> assert paths[-4] == paths[-3].parent
+        >>> assert paths[-4] == paths[0]
+        """,
+    )
+
+    def path_split(self, sep=None, maxsplit=-1):
+        separator = sep or os.path.sep
+        parts = super().split(separator, maxsplit)
+        parts[0] = makepath(parts[0] if parts[0] else "/")
+        return parts
+
+    split = path_split
+
+    def abspath(self):
+        return makepath(os.path.abspath(str(self)))
+
+    def slashpath(self):
+        return self + "/" if self.isdir() else self
 
     def short_relative_path_to(self, destination):
         """The shorter of either the absolute path of the destination,
             or the relative path to it
 
-        >>> print(DotPath('/home/guido/bin').short_relative_path_to(
-        ...     '/home/guido/build/python.tar'))
+        >>> print(
+        ...     DotPath('/home/guido/bin').short_relative_path_to(
+        ...         '/home/guido/build/python.tar'
+        ...     )
+        ... )
         ../build/python.tar
-        >>> print(DotPath('/home/guido/bin').short_relative_path_to(
-        ...     '/mnt/guido/build/python.tar'))
+        >>> print(
+        ...     DotPath('/home/guido/bin').short_relative_path_to(
+        ...         '/mnt/guido/build/python.tar'
+        ...     )
+        ... )
         /mnt/guido/build/python.tar
         """
         relative = self.relpathto(destination)
         absolute = self.__class__(destination).abspath()
-        if len(relative) < len(absolute):
+        if len(str(relative)) < len(str(absolute)):
             return relative
         return absolute
 
     def short_relative_path_to_here(self):
         """A short path relative to current working directory"""
         return self.short_relative_path_to(os.getcwd())
 
     def short_relative_path_from_here(self):
         """A short path relative to self to the current working directory"""
         return self.__class__(os.getcwd()).short_relative_path_to(self)
 
-    def walk_some_dirs(self, levels=-1, pattern=None):
-        """ D.walkdirs() -> iterator over subdirs, recursively.
-
-        With the optional 'pattern' argument, this yields only
-        directories whose names match the given pattern.  For
-        example, mydir.walkdirs('*test') yields only directories
-        with names ending in 'test'.
-        """
-        if not levels:
-            yield self
-            raise StopIteration
-        levels -= 1
-        for child in self.dirs():
-            if pattern is None or child.fnmatch(pattern):
-                yield child
-            if levels:
-                for subsubdir in child.walk_some_dirs(levels, pattern):
-                    yield subsubdir
-
     def fnmatch_basename(self, glob):
         if glob.startswith(os.path.sep):
             glob = glob.lstrip(os.path.sep)
         string = self.basename()
         if fnmatch(string, glob):
             return self
         return None
@@ -224,16 +463,14 @@
         if fnmatch(string, glob):
             return self
         return None
 
     def fnmatch_directories(self, glob):
         if glob.startswith(os.path.sep) or glob.endswith(os.path.sep):
             glob = glob.strip(os.path.sep)
-        else:
-            return
         strings = reversed(self.directory().splitall()[1:])
         for string in strings:
             if fnmatch(string, glob):
                 return self
         return None
 
     def fnmatch_part(self, glob):
@@ -243,282 +480,218 @@
             return self
         if self.fnmatch_directory(glob):
             return self
         if self.fnmatch_directories(glob):
             return self
         return None
 
-    def __get_owner_not_implemented(self):
-        pass
+    def expand(self):
+        """Expand the path completely
 
-    def expandall(self):
-        try:
-            return self.expand().realpath().abspath()
-        except AttributeError:
-            return self.__class__(
-                os.path.abspath(os.path.realpath(
-                    os.path.expanduser(os.path.expandvars(str(self)))
-                ))
-            )
+        This removes any "~" (for home dir) and any shell variables
+            eliminates any symbolic links
+            and converts from relative to absolute path
+        """
+        u = os.path.expanduser(str(self))
+        v = os.path.expandvars(u)
+        r = os.path.realpath(v)
+        return makepath(r)
 
     def same_path(self, other):
-        return self.expandall() == other.expandall()
+        """Whether this path points to same place as the other"""
+        return self.expand() == other.expand()
 
-    @property
-    def hidden(self):
+    def isroot(self):
+        raise NotImplementedError("Only a directory path can be a root")
+
+    def ishidden(self):
         """A 'hidden file' has a name starting with a '.'"""
         s = str(self.basename())
-        return s and s[0] == '.'
-
-
-def ext_language(ext, exts=None):
-    """Language of the extension in those extensions
-
-    If exts is supplied, then restrict recognition to those exts only
-    If exts is not supplied, then use all known extensions
-
-    >>> ext_language('.py') == 'python'
-    True
-    """
-    languages = {
-        '.py': 'python',
-        '.py2': 'python2',
-        '.py3': 'python3',
-        '.sh': 'bash',
-        '.bash': 'bash',
-        '.pl': 'perl',
-        '.js': 'javascript',
-        '.txt': 'english',
-    }
-    ext_languages = {_: languages[_] for _ in exts} if exts else languages
-    return ext_languages.get(ext)
-
-
-def find_language(script, exts=None):
-    """Determine the script's language  extension
-
-    >>> this_script = __file__.rstrip('c')
-    >>> find_language(makepath(this_script)) == 'python'
-    True
-
-    If exts are given they restrict which extensions are allowed
-    >>> find_language(makepath(this_script), ('.sh', '.txt')) is None
-    True
-
-    If there is no extension, but shebang is present, then use that
-    (Expecting to find "#!" in ~/.bashrc for this test,
-        but ~/.bashrc might not exist - then there's no language)
+        return s and s[0] == "."
 
-    >>> bashrc = home() / '.bashrc'
-    >>> find_language(bashrc) in ('bash', None)
-    True
-    """
-    if not script.isfile():
-        return None
-    if script.ext:
-        return ext_language(script.ext, exts)
-    shebang = script.shebang()
-    return shebang and str(shebang.name) or None
+    def is_executable(self):
+        """Whether the path is executable"""
+        # pylint: disable=no-self-use
+        return False
 
+    def isexec(self):
+        return self.is_executable()
 
-del PPath
+    def has_executable(self):
+        """Whether the path has any executable bits set"""
+        executable_bits = stat.S_IEXEC | stat.S_IXGRP | stat.S_IXOTH
+        try:
+            return bool(os.stat(self).st_mode & executable_bits)
+        except OSError:
+            return False
 
 
 class FilePath(DotPath, PathAssertions):
     """A path to a known file"""
 
-    def __div__(self, child):
-        raise PathError('%r has no children' % self)
-
-    __truediv__ = __div__
+    def __truediv__(self, child):
+        raise PathError("%r has no children" % self)
 
     def __iter__(self):
         for line in self.stripped_lines():
             yield line
 
-    def try_remove(self):
-        """Try to remove the file"""
-        self.remove()
+    def contains(self, other: StrPath) -> bool:
+        """Whether other is in this file's text"""
+        return str(other) in self.text()
 
     def stripped_lines(self):
         """A list of all lines without trailing whitespace
 
         If lines can not be read (e.g. no such file) then an empty list
         """
         try:
-            return [l.rstrip() for l in self.lines()]
-        except IOError:
+            return [_.rstrip() for _ in self.lines(retain=False)]
+        except (OSError, IOError, UnicodeDecodeError):
             return []
 
     def stripped_whole_lines(self):
         """A list of all lines without trailing whitespace or blank lines"""
-        return [l for l in self.stripped_lines() if l]
+        return [_ for _ in self.stripped_lines() if _]
 
     def non_comment_lines(self):
         """A list of all non-empty, non-comment lines"""
-        return [l
-                for l in self.stripped_whole_lines()
-                if not l.startswith('#')]
+        return [_ for _ in self.stripped_whole_lines() if not _.startswith("#")]
+
+    def isroot(self):
+        """A file cannot be root of a filesystem"""
+        return False
+
+    def is_executable(self):
+        """Whether the file has any executable bits set"""
+        return self.has_executable()
 
     def has_line(self, string):
         for line in self:
             if string == line:
                 return True
         return False
 
     def any_line_has(self, string):
         for line in self:
             if string in line:
                 return True
         return False
 
-    def split_all_ext(self):
-        copy = self[:]
-        filename, ext = os.path.splitext(copy)
-        if ext == '.gz':
-            filename, ext = os.path.splitext(filename)
-            ext = '%s.gz' % ext
-        return self.__class__(filename), ext
-
     def as_python(self):
         """The path to the file with a .py extension
 
-        >>> FilePath('/path/to/fred.txt').as_python()
-        <FilePath '/path/to/fred.py'>
+        >>> assert FilePath("/path/to/fred.txt").as_python() == "/path/to/fred.py"
         """
-        return self.extend_by('.py')
-
-    def extend_by(self, extension):
-        """The path to the file changed to use the given extension
-
-        >>> FilePath('/path/to/fred').extend_by('.txt')
-        <FilePath '/path/to/fred.txt'>
-        >>> FilePath('/path/to/fred.txt').extend_by('..tmp')
-        <FilePath '/path/to/fred.tmp'>
-        >>> FilePath('/path/to/fred.txt').extend_by('fred')
-        <FilePath '/path/to/fred.fred'>
-        """
-        copy = self[:]
-        filename, _ = os.path.splitext(copy)
-        return self.__class__('%s.%s' % (filename, extension.lstrip('.')))
+        return self.extend_by(".py")
 
     def make_read_only(self):
         """chmod the file permissions to -r--r--r--"""
         self.chmod(ChmodValues.readonly_file)
 
     def cd(self):  # pylint: disable=invalid-name
         """Change program's current directory to self"""
         return cd(self.parent)
 
     def dirname(self):
         return DirectPath(os.path.dirname(self))
+
     parent = property(dirname)
 
     def shebang(self):
         """The  #! entry from the first line of the file
 
         If no shebang is present, return an empty string
         """
         try:
-            try:
-                first_line = self.lines()[0]
-            except (OSError, UnicodeDecodeError):
-                return ''
-            if first_line.startswith('#!'):
-                rest_of_line = first_line[2:].strip()
-                parts = rest_of_line.split(' ')
-                interpreter = parts[0]
-                return makepath(interpreter)
+            first_line = self.stripped_lines()[0]
+            if first_line.startswith("#!"):
+                return first_line[2:].strip()
         except IndexError:
             pass
-        return ''
+        return ""
 
     def mv(self, destination):  # pylint: disable=invalid-name
         return self.move(destination)
 
-    def make_file_exist(self):
-        """Make sure the parent directory exists, then touch the file"""
-        self.parent.make_directory_exist()
-        self.parent.touch_file(self.name)
-        return self
-
     @property
     def language(self):
         """The language of this file"""
         try:
             return self._language
         except AttributeError:
-            self._language = find_language(self, getattr(self, 'exts', None))
+            self._language = ext_language(self.ext)
         return self._language
 
     @language.setter
     def language(self, value):
-        self._langauge = value
-
-    def choose_language(self, exts):
-        self._exts = exts
-        self._language = ext_language(self.ext, exts)
+        self._language = value
 
 
 class DirectPath(DotPath, PathAssertions):
     """A path which knows it might be a directory
 
     And that files are in directories
     """
 
     __file_class__ = FilePath
 
     def __iter__(self):
-        for a_path in DotPath.listdir(self):
+        for a_path in self.listdir():
             yield a_path
 
+    def contains(self, other: StrPath) -> bool:
+        """If other is a path then use that sense of "in"
+
+        So /path/to/here is "in" /path
+
+        Otherwise see if other is listed "in" this directory
+        """
+        if isinstance(other, DotPath):
+            return self in other.parent_directories()
+        return str(other) in [_.name for _ in self.listdir()] + [".", ".."]
+
     def directory(self):
         """Return a path to a directory.
 
         Either the path itself (if it is a directory), or its parent)
         """
         if self.isdir():
             return self
         return self.parent
 
-    def try_remove(self):
+    def remove_dir(self):
         """Try to remove the path
 
         If it is a directory, try recursive removal of contents too
         """
         if self.islink():
             self.unlink()
-        elif self.isfile():
-            self.remove()
         elif self.isdir():
             self.empty_directory()
             if self.isdir():
                 self.rmdir()
         else:
             return False
         return True
 
     def empty_directory(self):
         """Remove all contents of a directory
 
         Including any sub-directories and their contents"""
         for child in self.walkfiles():
             child.remove()
-        for child in reversed([d for d in self.walkdirs()]):
+        for child in reversed([self.walkdirs()]):
             if child == self or not child.isdir():
                 continue
             child.rmdir()
 
     def cd(self):  # pylint: disable=invalid-name
         """Change program's current directory to self"""
-        return cd(self)
-
-    def listdir(self, pattern=None):
-        return [self.as_existing_file(_)
-                for _ in DotPath.listdir(self, pattern)]
+        return cd(StringPath(self))
 
     def list_dirs(self, pattern=None):
         return self.list_dirs_files(pattern)[0]
 
     def list_files(self, pattern=None):
         return self.list_dirs_files(pattern)[1]
 
@@ -528,35 +701,14 @@
 
     def list_dirs_files(self, pattern=None):
         items = self.listdir(pattern)
         dirs = [_ for _ in items if _.isdir()]
         others = [_ for _ in items if not _.isdir()]
         return dirs, others
 
-    def make_directory_exist(self):
-        if self.isdir():
-            return False
-        if os.path.exists(self):
-            raise PathError('%s exists but is not a directory' % self)
-        self.makedirs()
-
-    def make_file_exist(self, filename=None):
-        """Make the directory exist, then touch the file
-
-        If the filename is None, then use self.name as filename
-        """
-        if filename is None:
-            path_to_file = FilePath(self)
-            path_to_file.make_file_exist()
-            return path_to_file
-        else:
-            self.make_directory_exist()
-            path_to_file = self.touch_file(filename)
-            return FilePath(path_to_file)
-
     def make_read_only(self):
         """chmod the directory permissions to -r-xr-xr-x"""
         self.chmod(ChmodValues.readonly_directory)
 
     def touch_file(self, filename):
         """Touch a file in the directory"""
         path_to_file = self.__file_class__(os.path.join(self, filename))
@@ -564,166 +716,306 @@
         return path_to_file
 
     def existing_sub_paths(self, sub_paths):
         """Those in the given list of sub_paths which do exist"""
         paths_to_subs = [self / _ for _ in sub_paths]
         return [_ for _ in paths_to_subs if _.exists()]
 
-    def clear_directory(self):
-        """Make sure the directory exists and is empty"""
-        self.make_directory_exist()
-        self.empty_directory()
+    # pylint: disable=arguments-differ
+    def walkdirs(self, pattern=None, errors="strict", ignores=None):
+        ignored = ignore_fnmatches(ignores)
+        for path_to_dir in super(DirectPath, self).walkdirs(pattern, errors):
+            if not ignored(path_to_dir.relpath(self)):
+                yield path_to_dir
 
     # pylint: disable=arguments-differ
-    def walkfiles(self, pattern=None, errors='strict', ignores=None):
-        ignored = ignore_globs(ignores)
+    def walkfiles(self, pattern=None, errors="strict", ignores=None):
+        ignored = ignore_fnmatches(ignores)
         for path_to_file in super(DirectPath, self).walkfiles(pattern, errors):
-            if not ignored(path_to_file):
+            if not ignored(path_to_file.relpath(self)):
                 yield path_to_file
 
     def listfiles(self, pattern=None, ignores=None):
-        ignored = ignore_globs(ignores)
+        ignored = ignore_fnmatches(ignores)
         return [_ for _ in self.listdir(pattern) if _.isfile() and not ignored(_)]
 
+    def isroot(self):
+        return str(self) == "/"
+
+
+@dataclass
+class FileTypeData:
+    type_: type
+    ext: str
+
+
+class FileType(FileTypeData):
+    def file(self, path_):
+        return path_.add_missing_ext(self.ext)
+
+    def typed(self, path_):
+        file = self.file(path_)
+        if file:
+            return self.type_(file)
+        return None
 
 
-def ignore_globs(ignores):
+@dataclass
+class FileTypesData:
+    file_types: List[FileType]
+
+
+class FileTypes(FileTypesData):
+    def types(self):
+        types_ = self.file_types
+        return [_ if isinstance(_, FileType) else FileType(*_) for _ in types_]
+
+    def files(self, path_):
+        for file_type in self.types():
+            file = file_type.file(path_)
+            if file:
+                yield file
+
+    def typed(self, path_):
+        for file_type in self.types():
+            typed = file_type.typed(path_)
+            if typed:
+                yield typed
 
+
+def ignore_fnmatches(ignores):
     def ignored(a_path):
         if not ignores:
             return False
         for ignore in ignores:
             if a_path.fnmatch_part(ignore):
                 return True
         return False
 
     return ignored
 
 
-class ChmodValues(object):
+class ChmodValues:
     # pylint: disable=too-few-public-methods
     readonly_file = 0o444
     readonly_directory = 0o555
 
 
-def makepath(s, as_file=False):
+def _make_module_path(arg):
+    """Make a path from a thing that has a module
+
+    classes and functions have modules, they'll be needing this
+    """
+    try:
+        return makepath(import_module(arg.__module__))
+    except (AttributeError, ModuleNotFoundError):
+        return None
+
+
+@singledispatch
+def makepath(arg) -> StringPath:
+    attribute = getattr(arg, "path", False)
+    return makepath(attribute) if attribute else makepath(str(arg))
+
+
+path = makepath
+
+
+@makepath.register(type(None))  # type: ignore[no-redef]
+def _(arg) -> StringPath:
+    """In the face of ambiguity, refuse the temptation to guess."""
+    return NonePath()
+
+
+@makepath.register(DotPath)  # type: ignore[no-redef]
+def _(arg) -> StringPath:
+    return arg
+
+
+@makepath.register(str)  # type: ignore[no-redef]
+def _(arg) -> StringPath:
     """Make a path from a string
 
     Expand out any variables, home squiggles, and normalise it
     See also http://stackoverflow.com/questions/26403972
-    """
-    if s is None:
-        return None
-    result = FilePath(s) if (os.path.isfile(s) or as_file) else DirectPath(s)
-    return result.expandall()
 
-path = makepath  # pylint: disable=invalid-name
+    See also Lynton Kwesi Johnson:
+        The Eagle and The Bear have people living in fear
+        Of impending nuclear warfare
+    """
+    if not arg:
+        return makepath(None)
+    if os.path.isfile(arg):
+        return FilePath(arg)
+    if os.path.isdir(arg):
+        string = arg if arg == "/" else arg.rstrip("/")
+        return DirectPath(string)
+    v = os.path.expandvars(arg)
+    u = os.path.expanduser(v)
+    if arg == u:
+        return NonePath(arg)
+    if os.path.exists(u):
+        return makepath(u)
+    return NonePath(arg)
+
+
+def imports():
+    return {sys, os, re, stat}
+
+
+@makepath.register(type(os))  # type: ignore[no-redef]
+def _(arg) -> StringPath:
+    """Make a path from a module"""
+    if arg.__name__ == "builtins":
+        return NonePath("builtins")
+    try:
+        return makepath(arg.__file__)
+    except AttributeError:
+        if arg not in imports() and arg not in sys.path:
+            raise MissingImport(arg)
+        python_ = makepath(sys.executable)
+        assert str(python_.parent.name) == "bin"
+        bin_ = python_.parent
+        root_ = bin_.parent
+        lib = root_ / "lib"
+        assert lib.isdir()
+        module = lib / f"{arg}.py"
+        if module.isfile():
+            return module
+        package = lib / arg
+        if package.isdir():
+            return package
+        raise ModuleNotFoundError(arg)
+
+
+@makepath.register(type(makepath))  # type: ignore[no-redef]
+def _(arg) -> StringPath:
+    """Make a path from a function's module"""
+    terminal_regexp = re.compile("<(stdin|.*python-input.*)>")
+    method = getattr(arg, "__wrapped__", arg)
+    filename = method.__code__.co_filename
+    if terminal_regexp.match(filename):
+        return NonePath(filename)
+    return _make_module_path(method)
+
+
+@makepath.register(type(DotPath))  # type: ignore[no-redef]
+def _(arg) -> StringPath:
+    """Make a path from a class's module"""
+    return _make_module_path(arg)
+
+
+@deprecated(reason="use pathstr()", version="0.7.57")
+def makestr(string: str) -> StringPath:
+    return pathstr(string)
+
+
+def pathstr(string: str) -> StringPath:
+    """Make a path from a string"""
+    if os.path.isfile(string) or os.path.isdir(string):
+        return makepath(string)
+    return NonePath(string)
 
 
-def cd(path_to):  # pylint: disable=invalid-name
+def cd(path_to: StringPath) -> bool:
     """cd to the given path
 
     If the path is a file, then cd to its parent directory
 
     Remember current directory before the cd
         so that we can cd back there with cd('-')
     """
-    if path_to == '-':
-        if not cd.previous:
-            raise PathError('No previous directory to return to')
-        return cd(cd.previous)
-    if not hasattr(path_to, 'cd'):
+    if path_to == "-":
+        previous = getattr(cd, "previous", "")
+        if not previous:
+            raise PathError("No previous directory to return to")
+        return cd(makepath(previous))
+    if not hasattr(path_to, "cd"):
         path_to = makepath(path_to)
     try:
         previous = os.getcwd()
     except OSError as e:
-        if 'No such file or directory' in str(e):
-            return False
-        raise
+        if "No such file or directory" not in str(e):
+            raise
+        previous = ""
     if path_to.isdir():
-        os.chdir(path_to)
+        cd_path = path_to
     elif path_to.isfile():
-        os.chdir(path_to.parent)
-    elif not os.path.exists(path_to):
+        cd_path = path_to.parent
+    elif not path_to.exists():
         return False
     else:
-        raise PathError('Cannot cd to %s' % path_to)
-    cd.previous = previous
+        raise PathError(f"Cannot cd to {path_to}")
+    cd.previous = previous  # type: ignore
+    os.chdir(cd_path)
     return True
 
 
 try:
-    cd.previous = makepath(os.getcwd())
+    setattr(cd, "previous", os.getcwd())
 except (OSError, AttributeError):
-    cd.previous = None
+    setattr(cd, "previous", "")
 
 
 def as_path(string_or_path):
     """Return the argument as a DirectPath
 
     If it is already one, return it unchanged
     If not, return the makepath()
     """
     if isinstance(string_or_path, DirectPath):
         return string_or_path
     return makepath(string_or_path)
 
 
-def string_to_paths(string):
-    for c in ':, ;':
+def string_to_paths(string) -> List[StringPath]:
+    for c in ":, ;":
         if c in string:
             return strings_to_paths(string.split(c))
     return [makepath(string)]
 
 
-def strings_to_paths(strings):
+def strings_to_paths(strings) -> List[StringPath]:
     return [makepath(s) for s in strings]
 
 
-def paths(strings):
-    return [p for p in strings_to_paths(strings) if p.exists()]
+def choose_paths(*strings, chooser) -> List[StringPath]:
+    return [_ for _ in strings_to_paths(strings) if chooser(_)]
 
 
-def split_directories(strings):
-    paths = strings_to_paths(strings)
-    return [_
-            for _ in paths
-            if _.isdir()], [_ for _ in paths if not _.isdir()]
+def paths(*strings: Iterable) -> List[StringPath]:
+    return choose_paths(*strings, chooser=lambda p: p.exists())
 
 
-def split_files(strings):
-    paths = strings_to_paths(strings)
-    return ([_ for _ in paths if _.isfile()],
-            [_ for _ in paths if not _.isfile()])
+def directories(*strings: Iterable) -> List[StringPath]:
+    return choose_paths(*strings, chooser=lambda p: p.isdir())
 
 
-def split_directories_files(strings):
-    paths = strings_to_paths(strings)
-    return ([_ for _ in paths if _.isdir()],
-            [_ for _ in paths if _.isfile()],
-            [_ for _ in paths if not (_.isfile() or _.isdir())])
+def files(*strings: Iterable) -> List[StringPath]:
+    return choose_paths(*strings, chooser=lambda p: p.isfile())
 
 
-def files(strings):
-    return split_files(strings)[0]
+def root():
+    return makepath("/")
 
 
-def directories(strings):
-    return split_directories(strings)[0]
+def tmp():
+    return makepath("/tmp")
 
 
-def home(sub_path = None):
-    return makepath('~') / sub_path
+def home():
+    _home = makepath(os.path.expanduser("~"))
+    assert _home
+    _ = _home.expand()
+    return _home
 
 
 def pwd():
     return makepath(os.getcwd())
 
-here = pwd  # pylint: disable=invalid-name
-
 
 def first_dir(path_string):
     """Get the first directory in that path
 
     >>> first_dir('usr/local/bin') == 'usr'
     True
     """
@@ -745,120 +1037,145 @@
 
     >>> unique_first_dirs(['usr/local/bin', 'bin']) == set(['usr', 'bin'])
     True
     """
     return set(first_dirs(path_strings))
 
 
-def _names_in_directory(path_to_directory):
+def paths_in_directory(path_: StringPath) -> List[DotPath]:
     """Get all items in the given directory
 
     Swallow errors to give an empty list
     """
     try:
-        return os.listdir(path_to_directory)
+        return [_ for _ in path_.listdir() if _]
     except OSError:
         return []
 
 
-def make_needed(pattern, path_to_directory, wanted):
-    """Make a method to check if an item matches the pattern, and is wanted
+def list_matcher(pattern, path_to_directory, wanted):
+    """Gives a method to check if an item matches the pattern, and is wanted
 
-    If wanted is None just check the pattern
+    If path_to_directory is given then items are checked there
+    By default, every item is wanted
     """
-    if wanted:
-        def needed(name):
-            return fnmatch(name, pattern) and wanted(
-                os.path.join(path_to_directory, name))
-        return needed
-    else:
-        return lambda name: fnmatch(name, pattern)
+    return lambda x: fnmatch(x, pattern) and wanted(os.path.join(path_to_directory, x))
+
 
+def list_items(path_to_directory, glob, wanted=lambda x: True) -> List[StringPath]:
+    """All items in the given path which match the given glob and are wanted
 
-def list_items(path_to_directory, pattern, wanted):
-    """All items in the given path which match the given glob and are wanted"""
-    if not path_to_directory:
-        return set()
-    needed = make_needed(pattern, path_to_directory, wanted)
-    return [os.path.join(path_to_directory, name)
-            for name in _names_in_directory(path_to_directory)
-            if needed(name)]
+    By default, every path is wanted
+    """
+    path_to_directory_ = makepath(path_to_directory)
+    if not path_to_directory_:
+        return []
+    result = []
+    for path_to_item in path_to_directory_.listdir():
+        if not fnmatch(path_to_item.name, glob):
+            continue
+        if wanted(path_to_item):
+            result.append(path_to_item)
+    return result
 
 
-def list_sub_directories(path_to_directory, pattern):
+def list_sub_directories(path_to_directory, glob):
     """All sub-directories of the given directory matching the given glob"""
-    return list_items(path_to_directory, pattern, os.path.isdir)
+    return list_items(path_to_directory, glob, os.path.isdir)
 
 
-def set_items(path_to_directory, pattern, wanted):
-    return set(list_items(path_to_directory, pattern, wanted))
+def set_items(path_to_directory, glob, wanted):
+    return set(list_items(path_to_directory, glob, wanted))
 
 
-def set_files(path_to_directory, pattern):
+def set_files(path_to_directory, glob):
     """A list of all files in the given directory matching the given glob"""
-    return set_items(path_to_directory, pattern, os.path.isfile)
+    return set_items(path_to_directory, glob, os.path.isfile)
 
 
-def contains_glob(path_to_directory, pattern, wanted=None):
+def contains_glob(path_to_directory, glob, wanted=lambda x: True):
     """Whether the given path contains an item matching the given glob"""
-    if not path_to_directory:
-        return False
-    needed = make_needed(pattern, path_to_directory, wanted)
-    for name in _names_in_directory(path_to_directory):
-        if needed(name):
-            return True
-    return False
+    return any(list_items(path_to_directory, glob, wanted))
 
 
-def contains_directory(path_to_directory, pattern):
+def contains_directory(path_to_directory, glob):
     """Whether the given path contains a directory matching the given glob"""
-    return contains_glob(path_to_directory, pattern, os.path.isdir)
+    return contains_glob(path_to_directory, glob, os.path.isdir)
 
 
-def contains_file(path_to_directory, pattern):
+def contains_file(path_to_directory, glob):
     """Whether the given directory contains a file matching the given glob"""
-    return contains_glob(path_to_directory, pattern, os.path.isfile)
+    return contains_glob(path_to_directory, glob, os.path.isfile)
 
 
-def environ_paths(key):
-    return [makepath(_) for _ in os.environ[key].split(':')]
+def environ_paths(key, default=None):
+    default_ = default or ""
+    return [makepath(_) for _ in os.environ.get(key, default_).split(":")]
 
 
-def environ_path(key):
-    return makepath(os.environ[key])
+def environ_path(key, default=None):
+    default_ = default or ""
+    return makepath(os.environ.get(key, default_))
 
 
 def default_environ_path(key, default):
     return makepath(os.environ.get(key, default))
 
 
-def tab_complete(string):
-    """Finish file names "left short" by tab-completion
+def add_star(string):
+    """Add '*' to string
 
-    For example, if an argument is "fred."
-        and no file called "fred." exists
-        but "fred.py" does exist
-        then return fred.py
-    """
-    if is_option(string):
-        return string
-    if not missing_extension(string):
-        return string
-    if os.path.isfile(string):
-        return string
-    extended_files = [f for f in extend(string) if os.path.isfile(f)]
-    try:
-        return extended_files[0]
-    except IndexError:
-        return string
+    >>> assert add_star('fred') == 'fred*'
+    """
+    return f"{string}*"
+
+
+def add_stars(strings):
+    """Add '.*' to each string
+
+    >>> assert add_stars(['fred', 'Fred.']) == ['fred*', 'Fred.*']
+    """
+    paths_ = [strings] if isinstance(strings, str) else strings
+    return [add_star(p) for p in paths_]
+
+
+def tab_complete(strings, globber=add_stars, select=os.path.exists):
+    """Finish path names "left short" by bash's tab-completion
+
+    strings is a string or strings
+        if any string exists as a path return those as paths
+
+    globber is a method which should return a list of globs
+        default: add_stars(['fred.']) == ['fred.*']
+            or, e.g: add_python(['fred', 'fred.']) == ['fred.py*']
+        if any expanded paths exist return those
+
+    select is a method to choose wanted paths
+        Defaults to selecting existing paths
+    """
+    strings_ = [strings] if isinstance(strings, str) else strings
+    globs = flatten([globber(s) for s in strings_])
+    here_ = pwd()
+    matches = []
+    for glob_ in globs:
+        if "/" in glob_:
+            directory, base = os.path.split(glob_)
+            dir_ = here_ / directory
+        else:
+            dir_ = here_
+            base = glob_
+        match = [p for p in dir_.listdir() if p.fnmatch_basename(base)]
+        matches.extend(match)
+    result = [p for p in set(matches) if select(p)]
+    return result if result[1:] else strings
 
 
 def pyc_to_py(path_to_file):
     """Change some file extensions to those which are more likely to be text
 
     >>> pyc_to_py('vim.pyc') == 'vim.py'
     True
     """
     stem, ext = os.path.splitext(path_to_file)
-    if ext == '.pyc':
-        return '%s.py' % stem
+    if ext == ".pyc":
+        return f"{stem}.py"
     return path_to_file
```

### Comparing `pysyte-0.7.9/pysyte/splits.py` & `pysyte-0.8.0/pysyte/splits.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,184 +1,195 @@
 """Generic methods for splitting strings"""
 
-
 import re
+from typing import Any
+from typing import List
+from typing import Optional
+from typing import Tuple
 
-from pysyte import literals
+from pysyte.types.literals import punctuation
+from pysyte.types.literals import nones
 
 
-def _default_separator():
+def _default_separator() -> str:
     """The default separator used by all methods is a comma
 
     Monkey-patching this method can change that default
     """
-    return literals.Punctuation.comma
+    return punctuation.comma
 
 
-def join(items, separator=None):
+def join(items: list, separator: Optional[str] = None) -> str:
     """Join the items into a string using the separator
 
     Converts items to strings if needed
 
     >>> join([1, 2, 3])
     '1,2,3'
     """
     if not items:
-        return ''
+        return ""
     if separator is None:
         separator = _default_separator()
     return separator.join([str(item) for item in items])
 
 
-def seamless_join(items):
+def seamless_join(items: list) -> str:
     """A seamless join does not show where the joins are
 
     >>> seamless_join(['fred', 'was', 'here'])
     'fredwashere'
     """
-    return join(items, literals.Empty.string)
+    return join(items, nones.string)
 
 
-def split(string, separator_regexp=None, maxsplit=0):
+def split(string: str, separator_regexp: Optional[str] = None, maxsplit=0) -> List[str]:
     """Split a string to a list
 
     >>> split('fred, was, here')
     ['fred', ' was', ' here']
     """
     if not string:
         return []
     if separator_regexp is None:
         separator_regexp = _default_separator()
     if not separator_regexp:
         return string.split()
     return re.split(separator_regexp, string, maxsplit)
 
 
-def split_and_strip(string, separator_regexp=None, maxsplit=0):
+def split_and_strip(
+    string: str, separator_regexp: Optional[str] = None, maxsplit=0
+) -> List[str]:
     """Split a string into items and trim any excess spaces from the items
 
     >>> split_and_strip('fred, was, here  ')
     ['fred', 'was', 'here']
     """
     if not string:
-        return ['']
+        return [""]
     if separator_regexp is None:
         separator_regexp = _default_separator()
     if not separator_regexp:
         return string.split()
-    return [item.strip()
-            for item in re.split(separator_regexp, string, maxsplit)]
+    return [item.strip() for item in re.split(separator_regexp, string, maxsplit)]
 
 
-def split_and_strip_without(string, exclude, separator_regexp=None):
+def split_and_strip_without(
+    string: str, exclude, separator_regexp: Optional[str] = None
+) -> List[str]:
     """Split a string into items, and trim any excess spaces
 
     Any items in exclude are not in the returned list
 
     >>> split_and_strip_without('fred, was, here  ', ['was'])
     ['fred', 'here']
     """
     result = split_and_strip(string, separator_regexp)
     if not exclude:
         return result
     return [x for x in result if x not in exclude]
 
 
-def split_and_strip_whole(string, separator_regexp=None):
+def split_and_strip_whole(
+    string: str, separator_regexp: Optional[str] = None
+) -> List[str]:
     """Split a string into items and trim any excess spaces from the items
 
     Exclude any empty items
 
     >>> split_and_strip_whole('fred, , was,here,')
     ['fred', 'was', 'here']
     """
-    return split_and_strip_without(string, [''], separator_regexp)
+    return split_and_strip_without(string, [""], separator_regexp)
 
 
-def split_by_count(items, count, filler=None):
+def split_by_count(items: list, count, filler: Optional[Any] = None) -> List[Tuple]:
     """Split the items into tuples of count items each
 
-    >>> split_by_count([0,1,2,3], 2)
+    >>> split_by_count([0, 1, 2, 3], 2)
     [(0, 1), (2, 3)]
 
     If there are a mutiple of count items then filler makes no difference
-    >>> split_by_count([0,1,2,7,8,9], 3, 0) == split_by_count([0,1,2,7,8,9], 3)
+    >>> split_by_count([0, 1, 2, 7, 8, 9], 3, 0) == split_by_count(
+    ...     [0, 1, 2, 7, 8, 9], 3
+    ... )
     True
 
     If there are not a multiple of count items, then any extras are discarded
-    >>> split_by_count([0,1,2,7,8,9,6], 3)
+    >>> split_by_count([0, 1, 2, 7, 8, 9, 6], 3)
     [(0, 1, 2), (7, 8, 9)]
 
     Specifying a filler expands the "lost" group
-    >>> split_by_count([0,1,2,7,8,9,6], 3, 0)
+    >>> split_by_count([0, 1, 2, 7, 8, 9, 6], 3, 0)
     [(0, 1, 2), (7, 8, 9), (6, 0, 0)]
     """
     if filler is not None:
         items = items[:]
         while len(items) % count:
             items.append(filler)
     iterator = iter(items)
     iterators = [iterator] * count
     return list(zip(*iterators))
 
 
-def pairs(items, filler=None):
+def pairs(items: list, filler: Optional[Any] = None) -> List[Tuple]:
     """Split the items into pairs
 
-    >>> pairs([0,1,2,7,8,9,10])
+    >>> pairs([0, 1, 2, 7, 8, 9, 10])
     [(0, 1), (2, 7), (8, 9)]
 
     If a filler is used any unpaired items are retained
-    >>> pairs([0,1,2,7,8,9,10], 99)
+    >>> pairs([0, 1, 2, 7, 8, 9, 10], 99)
     [(0, 1), (2, 7), (8, 9), (10, 99)]
     """
     return split_by_count(items, 2, filler)
 
 
-def threes(items, filler=None):
+def threes(items: list, filler: Optional[Any] = None) -> List[Tuple]:
     """Split the items into groups of 3
 
-    >>> threes([0,1,2,6,7,8,9])
+    >>> threes([0, 1, 2, 6, 7, 8, 9])
     [(0, 1, 2), (6, 7, 8)]
 
     If a filler is used any discarded items are retained
-    >>> threes([0,1,2,6,7,8,9], 5)
+    >>> threes([0, 1, 2, 6, 7, 8, 9], 5)
     [(0, 1, 2), (6, 7, 8), (9, 5, 5)]
     """
     return split_by_count(items, 3, filler)
 
 
-def despaced(string):
+def despaced(string: str) -> List[str]:
     """Split a string into spaceless items
 
     Split on spaces, trim excess space, exclude any empty strings
 
     >>> despaced('fred, , was,here today')
     ['fred,', ',', 'was,here', 'today']
     """
-    return split_and_strip_without(string, [''], ' ')
+    return split_and_strip_without(string, [""], " ")
 
 
-def words(string):
+def words(string: str) -> List[str]:
     """Split a string into words
 
     Split on (English) punctuaution, trim space, exclude any empty strings
 
     >>> words('fred, , was,here today')
     ['fred', 'was', 'here', 'today']
     """
-    return split_and_strip_without(string, [''], '[,;. ]')
+    return split_and_strip_without(string, [""], "[,;. ]")
 
 
-def rejoin(string, separator_regexp=None, spaced=False):
+def rejoin(string: str, separator_regexp: Optional[str] = None, spaced=False) -> str:
     """Split a string and then rejoin it
 
     Spaces are interspersed between items only if spaced is True
 
     >>> rejoin('fred, was, here  ')
     'fred,was,here'
     """
     strings = split_and_strip(string)
     if separator_regexp is None:
         separator_regexp = _default_separator()
-    joiner = spaced and '%s ' % separator_regexp or separator_regexp
+    joiner = spaced and f"{separator_regexp} " or separator_regexp
     return joiner.join(strings)
```

### Comparing `pysyte-0.7.9/pysyte/tracebacks.py` & `pysyte-0.8.0/pysyte/tracebacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-"""Facilities for tracebacks"""
+"""Handle tracebacks for pysyte"""
 
 import re
 
 
-def line_regexp():
+def _line_regexp():
     """Regular expression to match a traceback file line"""
-    return re.compile(r'''\s*
+    return re.compile(
+        r"""\s*
         File\s
         (
             (
                 ["']
                 (?P<path_to_python>[^"']+)
                 ["']
             ) | (
                 (?P<spaceless_path_to_python>[^ ]+)
             )
         )
         ,\sline\s
         (?P<line_number>[0-9]+)
         ,.in..*
-    ''', re.VERBOSE)
+    """,
+        re.VERBOSE,
+    )
 
 
 def parse_line(string):
     """Parse a single string as traceback line"""
-    match = line_regexp().match(string)
+    match = _line_regexp().match(string)
     if match:
         matches = match.groupdict()
-        line_number = matches['line_number']
-        path_to_python = matches['path_to_python']
-        spaceless_path_to_python = matches['spaceless_path_to_python']
+        line_number = int(matches["line_number"])
+        path_to_python = matches["path_to_python"]
+        spaceless_path_to_python = matches["spaceless_path_to_python"]
         if path_to_python:
             return path_to_python, line_number
         elif spaceless_path_to_python:
             return spaceless_path_to_python, line_number
```

### Comparing `pysyte-0.7.9/pysyte/words.py` & `pysyte-0.8.0/pysyte/words.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """This module provides methods to handle some features of English words"""
 
-
-import re
-
-
 import inflect
 
 _inlection = inflect.engine()
 
 
 def pluralize(string):
     """Returns the plural of string.
 
-    >>> pluralize('Index')  == 'Indices'
+    >>> pluralize('Cow') == 'Cows'
     True
     """
     return _inlection.plural_noun(string)
 
 
 def singularize(string):
     """Returns the singular of string.
```

### Comparing `pysyte-0.7.9/pysyte/words.test` & `pysyte-0.8.0/pysyte/test/words.test`

 * *Files 22% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 
 We can also get singular forms,
     >>> assert words.singularize('cows') == 'cow'
 
 Names for numbers
 -----------------
 
-    >>> assert words.number_name(-621.77) == 'minus six hundred and twenty-one point seven seven'
+    >>> expected = 'minus six hundred and twenty-one point seven seven'
+    >>> assert words.number_name(-621.77) == expected
```

### Comparing `pysyte-0.7.9/pysyte/words.tests` & `pysyte-0.8.0/pysyte/test/words.tests`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 ================
 
     >>> from pysyte import words
 
 This module handles some english words
 
     >>> expected = [
-    ...     ('punch', 'punches'),
-    ...     ('fish', 'fish'),
-    ...     ('lunch', 'lunches'),
+    ...     ('cat', 'cats'),
     ...     ('bass', 'basses'),
-    ...     ('fax', 'faxes'),
-    ...     ('coach', 'coaches'),
-    ...     ('rash', 'rashes'),
     ...     ('cheetah', 'cheetahs'),
-    ...     ('vacancy', 'vacancies'),
+    ...     ('coach', 'coaches'),
     ...     ('day', 'days'),
-    ...     ('man', 'men'),
-    ...     ('woman', 'women'),
-    ...     ('human', 'humans'),
-    ...     ('mouse', 'mice'),
-    ...     ('louse', 'lice'),
-    ...     ('house', 'houses'),
-    ...     ('knife', 'knives'),
-    ...     ('wife', 'wives'),
-    ...     ('sheep', 'sheep'),
     ...     ('deer', 'deer'),
+    ...     ('fax', 'faxes'),
+    ...     ('fish', 'fish'),
     ...     ('hero', 'heroes'),
+    ...     ('house', 'houses'),
+    ...     ('human', 'humans'),
+    ...     ('knife', 'knives'),
+    ...     ('louse', 'lice'),
+    ...     ('lunch', 'lunches'),
+    ...     ('man', 'men'),
+    ...     ('mouse', 'mice'),
     ...     ('piano', 'pianos'),
+    ...     ('punch', 'punches'),
+    ...     ('rash', 'rashes'),
+    ...     ('sheep', 'sheep'),
+    ...     ('vacancy', 'vacancies'),
+    ...     ('wife', 'wives'),
+    ...     ('woman', 'women'),
     ... ]
     >>> for singular, plural in expected:
-    ...     assert words.pluralize(singular) == plural, singular
+    ...     assert words.pluralize(singular) == plural, f'{singular} failed'
+    ...     assert words.singularize(plural) == singular, f'{plural} failed'
+    ...
 
     >>> words.pluralize('lowlife') == 'lowlifes'
     True
 
 
-    >>> assert words.singularize('cats') == 'cat'
-    >>> assert words.singularize('fish') == 'fish'
     >>> assert words.singularize('freds') == 'fred'
     >>> assert words.singularize('freddies') == 'freddy'
 
     >>> assert words.number_name('1') == 'one'
     >>> assert words.number_name(0) == 'zero'
     >>> assert words.number_name(-0) == 'zero'
     >>> assert words.number_name(1) == 'one'
@@ -51,27 +52,43 @@
     >>> assert words.number_name(20) == 'twenty'
     >>> assert words.number_name(26) == 'twenty-six'
     >>> assert words.number_name(400) == 'four hundred'
     >>> assert words.number_name(606) == 'six hundred and six'
     >>> assert words.number_name(876) == 'eight hundred and seventy-six'
     >>> assert words.number_name(3006) == 'three thousand and six'
     >>> assert words.number_name(3076) == 'three thousand and seventy-six'
-    >>> assert words.number_name(3870) == 'three thousand, eight hundred and seventy'
-    >>> assert words.number_name(23876) == 'twenty-three thousand, eight hundred and seventy-six'
+    >>> expected = 'three thousand, eight hundred and seventy'
+    >>> assert words.number_name(3870) == expected
+    >>> expected = 'twenty-three thousand, eight hundred and seventy-six'
+    >>> assert words.number_name(23876) == expected
     >>> assert words.number_name(500000) == 'five hundred thousand'
     >>> assert words.number_name(500002) == 'five hundred thousand and two'
-    >>> assert words.number_name(523876) == 'five hundred and twenty-three thousand, eight hundred and seventy-six'
-    >>> assert words.number_name(-523876) == 'minus five hundred and twenty-three thousand, eight hundred and seventy-six'
+    >>> expected = (
+    ...     'five hundred and twenty-three thousand, ' 'eight hundred and seventy-six'
+    ... )
+    >>> assert words.number_name(523876) == expected
+    >>> expected = 'minus five hundred and twenty-three thousand, eight hundred and seventy-six'
+    >>> assert words.number_name(-523876) == expected
     >>> assert words.number_name(1_000_000) == 'one million'
     >>> assert words.number_name(1_000_001) == 'one million and one'
     >>> assert words.number_name(1_000_100) == 'one million, one hundred'
     >>> assert words.number_name(1_001_000) == 'one million, one thousand'
-    >>> assert words.number_name(1_001_005) == 'one million, one thousand and five'
-    >>> assert words.number_name(1_001_050) == 'one million, one thousand and fifty'
-    >>> assert words.number_name(1_001_500) == 'one million, one thousand, five hundred'
-    >>> assert words.number_name(1_001_555) == 'one million, one thousand, five hundred and fifty-five'
-    >>> assert words.number_name(5_050_050) == 'five million, fifty thousand and fifty'
-    >>> assert words.number_name(235_000_150) == 'two hundred and thirty-five million, one hundred and fifty'
-    >>> assert words.number_name(19_004_300_900) == 'nineteen billion, four million, three hundred thousand, nine hundred'
+    >>> expected = 'one million, one thousand and five'
+    >>> assert words.number_name(1_001_005) == expected
+    >>> expected = 'one million, one thousand and fifty'
+    >>> assert words.number_name(1_001_050) == expected
+    >>> expected = 'one million, one thousand, five hundred'
+    >>> assert words.number_name(1_001_500) == expected
+    >>> expected = 'one million, one thousand, five hundred and fifty-five'
+    >>> assert words.number_name(1_001_555) == expected
+    >>> expected = 'five million, fifty thousand and fifty'
+    >>> assert words.number_name(5_050_050) == expected
+    >>> expected = 'two hundred and thirty-five million, one hundred and fifty'
+    >>> assert words.number_name(235_000_150) == expected
+    >>> expected = (
+    ...     'nineteen billion, four million, three hundred thousand, ' 'nine hundred'
+    ... )
+    >>> assert words.number_name(19_004_300_900) == expected
     >>> assert words.number_name(33_000_000_000_000) == 'thirty-three trillion'
     >>> import math
-    >>> assert words.number_name(-math.pi).startswith('minus three point one four one five nine')
+    >>> expected = 'minus three point one four one five nine'
+    >>> assert words.number_name(-math.pi).startswith(expected)
```

### Comparing `pysyte-0.7.9/pysyte.egg-info/SOURCES.txt` & `pysyte-0.8.0/pysyte.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,112 @@
+LICENSE
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
-bin/kat
-bin/short_dir
-bin/try
 pysyte/__init__.py
-pysyte/args.py
-pysyte/code.py
-pysyte/darwin.py
-pysyte/debuggers.py
-pysyte/decorators.py
-pysyte/dictionaries.py
-pysyte/dictionaries.test
-pysyte/getch.py
-pysyte/imports.py
+pysyte/importers.py
 pysyte/iteration.py
-pysyte/keyboard.py
-pysyte/linux.py
-pysyte/lists.py
-pysyte/literals.py
-pysyte/paths.py
-pysyte/paths.test
-pysyte/platforms.py
-pysyte/pp.py
+pysyte/pysyte.yaml
 pysyte/randoms.py
-pysyte/scripts.py
+pysyte/similarities.py
 pysyte/splits.py
-pysyte/splits.test
 pysyte/streams.py
-pysyte/streams.test
 pysyte/term.py
-pysyte/text_streams.py
 pysyte/tracebacks.py
 pysyte/words.py
-pysyte/words.test
-pysyte/words.tests
 pysyte.egg-info/PKG-INFO
 pysyte.egg-info/SOURCES.txt
 pysyte.egg-info/dependency_links.txt
 pysyte.egg-info/requires.txt
 pysyte.egg-info/top_level.txt
 pysyte/bash/__init__.py
-pysyte/bash/cmnds.py
-pysyte/bash/git.py
-pysyte/bash/git.test
+pysyte/bash/screen.py
 pysyte/bash/shell.py
+pysyte/bash/test/shell.test
+pysyte/cli/__init__.py
+pysyte/cli/app.py
+pysyte/cli/arguments.py
+pysyte/cli/config.py
+pysyte/cli/exceptions.py
+pysyte/cli/lines.py
+pysyte/cli/main.py
+pysyte/cli/paths.py
+pysyte/cli/streams.py
+pysyte/cli/test/arguments.test
+pysyte/cli/test/config.test
+pysyte/cli/test/main.test
 pysyte/colours/__init__.py
 pysyte/colours/ansi_escapes.py
-pysyte/colours/ansi_escapes.test
 pysyte/colours/colour_names.py
-pysyte/colours/colour_names.test
 pysyte/colours/colour_numbers.py
-pysyte/colours/colour_numbers.test
-pysyte/colours/colour_numbers.tests
-pysyte/colours/main.py
 pysyte/colours/texts.py
-pysyte/colours/texts.test
-pysyte/colours/texts.tests
 pysyte/colours/x11_colour_names.py
-pysyte/colours/x11_colour_names.test
-pysyte/testing/__init__.py
-pysyte/testing/files_for_test.py
-pysyte/testing/files_for_test.test
-pysyte/testing/files_for_test.tests
-pysyte/testing/see.py
-pysyte/testing/see.test
-pysyte/testing/see.tests
-pysyte/testing/try_plugins.py
-pysyte/testing/try_plugins.test
-pysyte/testing/trying.py
-pysyte/testing/trying.test
+pysyte/colours/test/ansi_escapes.test
+pysyte/colours/test/colour_names.test
+pysyte/colours/test/colour_numbers.test
+pysyte/colours/test/colour_numbers.tests
+pysyte/colours/test/texts.test
+pysyte/colours/test/x11_colour_names.test
+pysyte/colours/test/x11_colour_names.tests
+pysyte/config/__init__.py
+pysyte/config/types.py
+pysyte/config/urator.py
+pysyte/config/xdg.py
+pysyte/config/test/types.test
+pysyte/config/test/urator.test
+pysyte/config/test/xdg.test
+pysyte/imports/__init__.py
+pysyte/imports/__main__.py
+pysyte/kat/__init__.py
+pysyte/kat/__main__.py
+pysyte/keys/__init__.py
+pysyte/keys/__main__.py
+pysyte/net/test/hosts.test
+pysyte/oss/__init__.py
+pysyte/oss/darwin.py
+pysyte/oss/getch.py
+pysyte/oss/keyboard.py
+pysyte/oss/linux.py
+pysyte/oss/platforms.py
+pysyte/oss/test/linux.test
+pysyte/oss/test/platforms.test
+pysyte/test/importers.test
+pysyte/test/iteration.test
+pysyte/test/similarities.test
+pysyte/test/splits.test
+pysyte/test/streams.test
+pysyte/test/tracebacks.test
+pysyte/test/words.test
+pysyte/test/words.tests
+pysyte/types/__init__.py
+pysyte/types/colours.py
+pysyte/types/dictionaries.py
+pysyte/types/lines.py
+pysyte/types/lists.py
+pysyte/types/methods.py
+pysyte/types/numbers.py
+pysyte/types/paths.py
+pysyte/types/strings.py
+pysyte/types/times.py
+pysyte/types/literals/__init__.py
+pysyte/types/literals/ansi.py
+pysyte/types/literals/control.py
+pysyte/types/literals/digits.py
+pysyte/types/literals/nones.py
+pysyte/types/literals/numbers.py
+pysyte/types/literals/punctuation.py
+pysyte/types/literals/test/ansi.test
+pysyte/types/literals/test/digits.test
+pysyte/types/literals/test/nones.test
+pysyte/types/literals/test/numbers.test
+pysyte/types/literals/test/punctuation.test
+pysyte/types/test/dictionaries.test
+pysyte/types/test/lines.test
+pysyte/types/test/lists.test
+pysyte/types/test/numbers.test
+pysyte/types/test/paths.test
+pysyte/types/test/times.test
+pysyte/unix/__init__.py
+pysyte/unix/root.py
+pysyte/unix/root.yaml
+pysyte/unix/test/root.test
```

