# Comparing `tmp/nazca-2.0.2.tar.gz` & `tmp/nazca-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nazca-2.0.2.tar", last modified: Wed Aug  5 14:58:21 2020, max compression
+gzip compressed data, was "nazca-3.0.0.tar", last modified: Wed Jul  5 14:11:52 2023, max compression
```

## Comparing `nazca-2.0.2.tar` & `nazca-3.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20705 2020-06-22 15:21:09.000000 nazca-2.0.2/CHANGELOG.md
--rw-r--r--   0 schabot   (1000) schabot   (1000)      377 2020-06-22 15:26:56.000000 nazca-2.0.2/MANIFEST.in
--rw-r--r--   0 schabot   (1000) schabot   (1000)      568 2020-08-05 14:58:21.000000 nazca-2.0.2/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-2.0.2/README
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/doc/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    54838 2019-04-19 14:35:24.000000 nazca-2.0.2/doc/nazca-logo.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22785 2019-04-19 14:35:24.000000 nazca-2.0.2/doc.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/examples/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-2.0.2/examples/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6813 2020-05-07 07:41:53.000000 nazca-2.0.2/examples/demo.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2305 2019-04-19 14:35:24.000000 nazca-2.0.2/examples/goncourt.csv
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-2.0.2/nazca/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1906 2020-08-05 14:58:03.000000 nazca-2.0.2/nazca/__pkginfo__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      240 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/data/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32441 2020-05-07 07:41:53.000000 nazca-2.0.2/nazca/data/countries.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4882 2019-04-19 14:35:24.000000 nazca-2.0.2/nazca/data/countries_iso_3166.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)  4246181 2019-04-19 14:35:24.000000 nazca-2.0.2/nazca/data/french_lemmas.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32080 2020-05-07 07:41:53.000000 nazca-2.0.2/nazca/data/stopwords.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5401 2020-05-07 07:41:53.000000 nazca-2.0.2/nazca/data/us_states.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca/ner/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2763 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/ner/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3847 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/ner/filters.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2767 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/ner/preprocessors.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4427 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/ner/sources.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca/rl/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-2.0.2/nazca/rl/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15052 2020-06-22 15:16:55.000000 nazca-2.0.2/nazca/rl/aligner.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    27300 2020-06-17 10:55:56.000000 nazca-2.0.2/nazca/rl/blocking.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca/utils/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-06-03 13:28:47.000000 nazca-2.0.2/nazca/utils/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13998 2020-08-05 14:54:06.000000 nazca-2.0.2/nazca/utils/dataio.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22730 2020-06-22 15:16:55.000000 nazca-2.0.2/nazca/utils/distances.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8808 2020-06-22 15:29:53.000000 nazca-2.0.2/nazca/utils/minhashing.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16252 2020-05-07 07:41:53.000000 nazca-2.0.2/nazca/utils/normalize.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2746 2020-05-06 10:23:08.000000 nazca-2.0.2/nazca/utils/tokenizer.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      568 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1118 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/SOURCES.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/dependency_links.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2019-04-19 14:38:35.000000 nazca-2.0.2/nazca.egg-info/not-zip-safe
--rw-r--r--   0 schabot   (1000) schabot   (1000)       46 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/requires.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        6 2020-08-05 14:58:21.000000 nazca-2.0.2/nazca.egg-info/top_level.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2020-08-05 14:58:21.000000 nazca-2.0.2/setup.cfg
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2522 2020-05-06 10:23:08.000000 nazca-2.0.2/setup.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2020-08-05 14:58:21.000000 nazca-2.0.2/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2019-04-19 14:35:24.000000 nazca-2.0.2/test/data/alignfile.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)       86 2019-04-19 14:35:24.000000 nazca-2.0.2/test/data/file2parse
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20618 2019-04-19 14:35:24.000000 nazca-2.0.2/test/data/file2split
--rw-r--r--   0 schabot   (1000) schabot   (1000)       63 2019-04-19 14:35:24.000000 nazca-2.0.2/test/data/targetfile.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10290 2020-06-22 15:28:57.000000 nazca-2.0.2/test/test_alignment.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17179 2020-06-22 15:29:28.000000 nazca-2.0.2/test/test_blocking.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13602 2020-08-05 13:39:55.000000 nazca-2.0.2/test/test_dataio.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10203 2020-06-22 15:29:13.000000 nazca-2.0.2/test/test_distances.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7260 2020-05-07 07:41:53.000000 nazca-2.0.2/test/test_filters.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2671 2020-06-17 10:55:56.000000 nazca-2.0.2/test/test_minhashing.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15803 2020-05-07 07:41:53.000000 nazca-2.0.2/test/test_ner.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8212 2020-05-07 07:41:53.000000 nazca-2.0.2/test/test_normalize.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4479 2020-05-07 07:41:53.000000 nazca-2.0.2/test/test_preprocessors.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3948 2020-05-07 07:41:53.000000 nazca-2.0.2/test/test_tokenizer.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      715 2020-06-22 15:16:56.000000 nazca-2.0.2/tox.ini
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.366472 nazca-3.0.0/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20883 2023-07-05 13:54:58.000000 nazca-3.0.0/CHANGELOG.md
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      381 2023-07-05 13:18:11.000000 nazca-3.0.0/MANIFEST.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      668 2023-07-05 14:11:52.366472 nazca-3.0.0/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2023-07-05 13:28:03.000000 nazca-3.0.0/README.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/doc/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    54838 2019-04-19 14:35:24.000000 nazca-3.0.0/doc/nazca-logo.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22785 2019-04-19 14:35:24.000000 nazca-3.0.0/doc.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/examples/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/examples/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6653 2023-07-05 13:28:03.000000 nazca-3.0.0/examples/demo.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2305 2019-04-19 14:35:24.000000 nazca-3.0.0/examples/goncourt.csv
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/nazca/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1912 2023-07-05 13:54:13.000000 nazca-3.0.0/nazca/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      216 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    32441 2020-05-07 07:41:53.000000 nazca-3.0.0/nazca/data/countries.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4882 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/data/countries_iso_3166.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)  4246181 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/data/french_lemmas.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    24612 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/stopwords.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5376 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/data/us_states.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/ner/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2681 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3755 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/filters.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2699 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/ner/preprocessors.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3892 2023-07-05 13:31:15.000000 nazca-3.0.0/nazca/ner/sources.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/rl/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-04-19 14:35:24.000000 nazca-3.0.0/nazca/rl/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15110 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/rl/aligner.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26824 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/rl/blocking.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/nazca/utils/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2019-06-03 13:28:47.000000 nazca-3.0.0/nazca/utils/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12047 2023-07-05 13:31:49.000000 nazca-3.0.0/nazca/utils/dataio.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22287 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/distances.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8679 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/minhashing.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15394 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/normalize.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2655 2023-07-05 13:28:03.000000 nazca-3.0.0/nazca/utils/tokenizer.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.358472 nazca-3.0.0/nazca.egg-info/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      668 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1122 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/SOURCES.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/dependency_links.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2019-04-19 14:38:35.000000 nazca-3.0.0/nazca.egg-info/not-zip-safe
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       53 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/requires.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        6 2023-07-05 14:11:52.000000 nazca-3.0.0/nazca.egg-info/top_level.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2023-07-05 14:11:52.366472 nazca-3.0.0/setup.cfg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2461 2023-07-05 13:28:03.000000 nazca-3.0.0/setup.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.362472 nazca-3.0.0/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-07-05 14:11:52.366472 nazca-3.0.0/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       83 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/alignfile.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       86 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/file2parse
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20618 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/file2split
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       63 2019-04-19 14:35:24.000000 nazca-3.0.0/test/data/targetfile.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10516 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_alignment.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16831 2023-07-05 13:43:33.000000 nazca-3.0.0/test/test_blocking.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13276 2023-07-05 13:32:27.000000 nazca-3.0.0/test/test_dataio.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10180 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_distances.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7225 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_filters.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2667 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_minhashing.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15678 2023-07-05 13:30:48.000000 nazca-3.0.0/test/test_ner.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8590 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_normalize.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4454 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_preprocessors.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3923 2023-07-05 13:28:03.000000 nazca-3.0.0/test/test_tokenizer.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      871 2023-07-05 13:28:03.000000 nazca-3.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nazca-2.0.2/CHANGELOG.md` & `nazca-3.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+## Version 3.0.0 (2023-07-05)
+### 🎉 New features
 
-# CHANGELOG
+- *BREAKING CHANGE*: remove RQL related functions
+- correctly process OPTIONAL values in SPARQL
+- improve logging messages about statistics
 
 ## Version 2.0.0 (2020-06-22)
 ### New features
 
 - distance: add a function to convert distance of alignments to confidence
 - blocking: add a new parameter 'repeatable' to MinHashingBlocking
 
@@ -537,9 +541,7 @@
 - distance: Soudex : if there is a vowel between two identical numbered
 - test: Add some other tests to soudex, and some explanations too
 - test: The test for soundex was false, I corrected it (related #128982)
 - tests: Add tests for soundex and levenshtein (related #128982)
 - distances: Add soundex code (related #128982)
 - distance: add Levenshtein distance (related #128982)
 - Initial commit
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nazca-2.0.2/doc/nazca-logo.svg` & `nazca-3.0.0/doc/nazca-logo.svg`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/doc.rst` & `nazca-3.0.0/doc.rst`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/examples/demo.py` & `nazca-3.0.0/examples/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 #!/usr/bin/python
-# -*- coding:utf-8 -*-
 
-from __future__ import absolute_import
-from __future__ import print_function
 from os import path
 
 import six.moves.urllib.request, six.moves.urllib.parse, six.moves.urllib.error
 
 import nazca.distances as ald
 import nazca.normalize as aln
 from nazca.aligner import align, subalign, findneighbours, alignall
@@ -23,17 +20,15 @@
     try:
         return string[: string.lower().index(sub)].strip()
     except ValueError:
         return string
 
 
 def parserql(host, rql):
-    filehandle = six.moves.urllib.request.urlopen(
-        "%(host)sview?rql=%(rql)s&vid=csvexport" % {"rql": rql, "host": host}
-    )
+    filehandle = six.moves.urllib.request.urlopen(f"{host}view?rql={rql}&vid=csvexport")
     filehandle.readline()
     rset = [[e.decode("utf-8") for e in line.strip().split(";")] for line in filehandle]
     return rset
 
 
 def demo_0():
     # prixgoncourt is the list of Goncourt Prize, extracted
@@ -159,15 +154,15 @@
 def demo_3():
     print("Parsing files")
     alignset = parserql(
         host="http://demo.cubicweb.org/elections/",
         rql="Any E, N WHERE X is Commune, X eid E, X label N",
     )
     targetset = parsefile(dpath("FR.txt"), indexes=[0, 1])
-    print("%s×%s" % (len(alignset), len(targetset)))
+    print(f"{len(alignset)}×{len(targetset)}")
 
     tr_name = {"normalization": [aln.simplify], "metric": "levenshtein"}
 
     print("Alignment started")
     results = alignall(
         alignset,
         targetset,
@@ -175,15 +170,15 @@
         processings={1: tr_name},
         indexes=(1, 1),
         mode="minhashing",
         kwordsgram=1,
         siglen=200,
         uniq=True,
     )
-    dicresults = dict([(a, b) for (a, b) in results])
+    dicresults = {a: b for (a, b) in results}
 
     print("Done, writing output")
 
     with open(dpath("demo3_results"), "w") as fout:
         for line in alignset:
             sent = (
                 "http://demo.cubicweb.org/elections/commune/%s;"
```

### Comparing `nazca-2.0.2/examples/goncourt.csv` & `nazca-3.0.0/examples/goncourt.csv`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/nazca/__pkginfo__.py` & `nazca-3.0.0/nazca/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 __docformat__ = "restructuredtext en"
 from os.path import join
 import sys
 
 distname = "nazca"
 modname = "nazca"
 
-numversion = (2, 0, 2)
+numversion = (3, 0, 0)
 version = ".".join([str(num) for num in numversion])
 
 license = "LGPL"  # 2.1 or later
 description = "Python library for data alignment"
 web = "https://www.logilab.org/project/nazca"
 author = "Logilab"
 author_email = "contact@logilab.fr"
@@ -40,15 +40,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing",
 ]
 
 __depends__ = {
     "python-dateutil": None,
-    "lxml": None,
+    "lxml": "<= 4.9.2",
     "numpy": None,
     "scipy": None,
     "scikit-learn": None,
 }
 
 __recommends__ = {
     "sparqlwrapper": None,
```

### Comparing `nazca-2.0.2/nazca/data/countries.py` & `nazca-3.0.0/nazca/data/countries.py`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/nazca/data/countries_iso_3166.txt` & `nazca-3.0.0/nazca/data/countries_iso_3166.txt`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/nazca/data/french_lemmas.txt` & `nazca-3.0.0/nazca/data/french_lemmas.txt`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/nazca/data/stopwords.py` & `nazca-3.0.0/nazca/data/stopwords.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1873 +1,1864 @@
-# -*- coding: utf-8 -*-
 """
 Stopwords in different languages.
 """
 
-FRENCH_STOPWORDS = set(
-    [
-        "alors",
-        "au",
-        "aucuns",
-        "aussi",
-        "autre",
-        "aux",
-        "avant",
-        "avec",
-        "avoir",
-        "bon",
-        "car",
-        "ce",
-        "cela",
-        "ces",
-        "ceux",
-        "chaque",
-        "ci",
-        "comme",
-        "comment",
-        "dans",
-        "de",
-        "dedans",
-        "dehors",
-        "depuis",
-        "des",
-        "deux",
-        "devrait",
-        "doit",
-        "donc",
-        "dos",
-        "droite",
-        "du",
-        "début",
-        "elle",
-        "elles",
-        "en",
-        "encore",
-        "essai",
-        "est",
-        "et",
-        "eu",
-        "eux",
-        "fait",
-        "faites",
-        "fois",
-        "font",
-        "force",
-        "haut",
-        "hors",
-        "ici",
-        "il",
-        "ils",
-        "je",
-        "juste",
-        "la",
-        "le",
-        "les",
-        "leur",
-        "lui",
-        "là",
-        "ma",
-        "maintenant",
-        "mais",
-        "me",
-        "meme",
-        "mes",
-        "mine",
-        "moi",
-        "moins",
-        "mon",
-        "mot",
-        "ne",
-        "ni",
-        "nommés",
-        "nos",
-        "notre",
-        "nous",
-        "nouveaux",
-        "on",
-        "ou",
-        "où",
-        "par",
-        "parce",
-        "parole",
-        "pas",
-        "personnes",
-        "peu",
-        "peut",
-        "pièce",
-        "plupart",
-        "pour",
-        "pourquoi",
-        "qu",
-        "quand",
-        "que",
-        "quel",
-        "quelle",
-        "quelles",
-        "quels",
-        "qui",
-        "sa",
-        "sans",
-        "se",
-        "ses",
-        "seulement",
-        "si",
-        "sien",
-        "son",
-        "sont",
-        "sous",
-        "soyez",
-        "sujet",
-        "sur",
-        "ta",
-        "tandis",
-        "te",
-        "tellement",
-        "tels",
-        "tes",
-        "toi",
-        "ton",
-        "tous",
-        "tout",
-        "trop",
-        "très",
-        "tu",
-        "un",
-        "une",
-        "valeur",
-        "voie",
-        "voient",
-        "vont",
-        "vos",
-        "votre",
-        "vous",
-        "vu",
-        "ça",
-        "étaient",
-        "état",
-        "étions",
-        "été",
-        "être",
-    ]
-)
+FRENCH_STOPWORDS = {
+    "alors",
+    "au",
+    "aucuns",
+    "aussi",
+    "autre",
+    "aux",
+    "avant",
+    "avec",
+    "avoir",
+    "bon",
+    "car",
+    "ce",
+    "cela",
+    "ces",
+    "ceux",
+    "chaque",
+    "ci",
+    "comme",
+    "comment",
+    "dans",
+    "de",
+    "dedans",
+    "dehors",
+    "depuis",
+    "des",
+    "deux",
+    "devrait",
+    "doit",
+    "donc",
+    "dos",
+    "droite",
+    "du",
+    "début",
+    "elle",
+    "elles",
+    "en",
+    "encore",
+    "essai",
+    "est",
+    "et",
+    "eu",
+    "eux",
+    "fait",
+    "faites",
+    "fois",
+    "font",
+    "force",
+    "haut",
+    "hors",
+    "ici",
+    "il",
+    "ils",
+    "je",
+    "juste",
+    "la",
+    "le",
+    "les",
+    "leur",
+    "lui",
+    "là",
+    "ma",
+    "maintenant",
+    "mais",
+    "me",
+    "meme",
+    "mes",
+    "mine",
+    "moi",
+    "moins",
+    "mon",
+    "mot",
+    "ne",
+    "ni",
+    "nommés",
+    "nos",
+    "notre",
+    "nous",
+    "nouveaux",
+    "on",
+    "ou",
+    "où",
+    "par",
+    "parce",
+    "parole",
+    "pas",
+    "personnes",
+    "peu",
+    "peut",
+    "pièce",
+    "plupart",
+    "pour",
+    "pourquoi",
+    "qu",
+    "quand",
+    "que",
+    "quel",
+    "quelle",
+    "quelles",
+    "quels",
+    "qui",
+    "sa",
+    "sans",
+    "se",
+    "ses",
+    "seulement",
+    "si",
+    "sien",
+    "son",
+    "sont",
+    "sous",
+    "soyez",
+    "sujet",
+    "sur",
+    "ta",
+    "tandis",
+    "te",
+    "tellement",
+    "tels",
+    "tes",
+    "toi",
+    "ton",
+    "tous",
+    "tout",
+    "trop",
+    "très",
+    "tu",
+    "un",
+    "une",
+    "valeur",
+    "voie",
+    "voient",
+    "vont",
+    "vos",
+    "votre",
+    "vous",
+    "vu",
+    "ça",
+    "étaient",
+    "état",
+    "étions",
+    "été",
+    "être",
+}
 
 
-ENGLISH_STOPWORDS = set(
-    [
-        "a",
-        "able",
-        "about",
-        "above",
-        "according",
-        "accordingly",
-        "across",
-        "actually",
-        "after",
-        "afterwards",
-        "again",
-        "against",
-        "ain't",
-        "all",
-        "allow",
-        "allows",
-        "almost",
-        "alone",
-        "along",
-        "already",
-        "also",
-        "although",
-        "always",
-        "am",
-        "among",
-        "amongst",
-        "amoungst",
-        "amount",
-        "an",
-        "and",
-        "another",
-        "any",
-        "anybody",
-        "anyhow",
-        "anyone",
-        "anything",
-        "anyway",
-        "anyways",
-        "anywhere",
-        "apart",
-        "appear",
-        "appreciate",
-        "appropriate",
-        "are",
-        "aren't",
-        "around",
-        "as",
-        "aside",
-        "ask",
-        "asking",
-        "associated",
-        "at",
-        "available",
-        "away",
-        "awfully",
-        "back",
-        "be",
-        "became",
-        "because",
-        "become",
-        "becomes",
-        "becoming",
-        "been",
-        "before",
-        "beforehand",
-        "behind",
-        "being",
-        "believe",
-        "below",
-        "beside",
-        "besides",
-        "best",
-        "better",
-        "between",
-        "beyond",
-        "bill",
-        "both",
-        "bottom",
-        "brief",
-        "but",
-        "by",
-        "call",
-        "came",
-        "can",
-        "cannot",
-        "cant",
-        "can't",
-        "cause",
-        "causes",
-        "certain",
-        "certainly",
-        "changes",
-        "clearly",
-        "co",
-        "com",
-        "come",
-        "comes",
-        "computer",
-        "con",
-        "concerning",
-        "consequently",
-        "consider",
-        "considering",
-        "contain",
-        "containing",
-        "contains",
-        "corresponding",
-        "could",
-        "couldnt",
-        "couldn't",
-        "course",
-        "cry",
-        "currently",
-        "c'mon",
-        "c's",
-        "de",
-        "definitely",
-        "describe",
-        "described",
-        "despite",
-        "detail",
-        "did",
-        "didn't",
-        "different",
-        "do",
-        "does",
-        "doesn't",
-        "doing",
-        "done",
-        "don't",
-        "down",
-        "downwards",
-        "due",
-        "during",
-        "each",
-        "edu",
-        "eg",
-        "eight",
-        "either",
-        "eleven",
-        "else",
-        "elsewhere",
-        "empty",
-        "enough",
-        "entirely",
-        "especially",
-        "et",
-        "etc",
-        "even",
-        "ever",
-        "every",
-        "everybody",
-        "everyone",
-        "everything",
-        "everywhere",
-        "ex",
-        "exactly",
-        "example",
-        "except",
-        "far",
-        "few",
-        "fifteen",
-        "fifth",
-        "fify",
-        "fill",
-        "find",
-        "fire",
-        "first",
-        "five",
-        "followed",
-        "following",
-        "follows",
-        "for",
-        "former",
-        "formerly",
-        "forth",
-        "forty",
-        "found",
-        "four",
-        "from",
-        "front",
-        "full",
-        "further",
-        "furthermore",
-        "get",
-        "gets",
-        "getting",
-        "give",
-        "given",
-        "gives",
-        "go",
-        "goes",
-        "going",
-        "gone",
-        "got",
-        "gotten",
-        "greetings",
-        "had",
-        "hadn't",
-        "happens",
-        "hardly",
-        "has",
-        "hasnt",
-        "hasn't",
-        "have",
-        "haven't",
-        "having",
-        "he",
-        "hello",
-        "help",
-        "hence",
-        "her",
-        "here",
-        "hereafter",
-        "hereby",
-        "herein",
-        "hereupon",
-        "here's",
-        "hers",
-        "herself",
-        "he's",
-        "hi",
-        "him",
-        "himself",
-        "his",
-        "hither",
-        "hopefully",
-        "how",
-        "howbeit",
-        "however",
-        "hundred",
-        "i",
-        "i'd",
-        "i'll",
-        "i'm",
-        "i've",
-        "ie",
-        "if",
-        "ignored",
-        "immediate",
-        "in",
-        "inasmuch",
-        "inc",
-        "indeed",
-        "indicate",
-        "indicated",
-        "indicates",
-        "inner",
-        "insofar",
-        "instead",
-        "interest",
-        "into",
-        "inward",
-        "is",
-        "isn't",
-        "it",
-        "its",
-        "itself",
-        "it'd",
-        "it'll",
-        "it's'",
-        "i'd",
-        "i'll",
-        "i'm",
-        "i've",
-        "just",
-        "keep",
-        "keeps",
-        "kept",
-        "know",
-        "known",
-        "knows",
-        "last",
-        "lately",
-        "later",
-        "latter",
-        "latterly",
-        "least",
-        "less",
-        "lest",
-        "let",
-        "let's",
-        "like",
-        "liked",
-        "likely",
-        "little",
-        "look",
-        "looking",
-        "looks",
-        "ltd",
-        "made",
-        "mainly",
-        "many",
-        "may",
-        "maybe",
-        "me",
-        "mean",
-        "meanwhile",
-        "merely",
-        "might",
-        "mill",
-        "mine",
-        "more",
-        "moreover",
-        "most",
-        "mostly",
-        "move",
-        "much",
-        "must",
-        "my",
-        "myself",
-        "name",
-        "namely",
-        "nd",
-        "near",
-        "nearly",
-        "necessary",
-        "need",
-        "needs",
-        "neither",
-        "never",
-        "nevertheless",
-        "new",
-        "next",
-        "nine",
-        "no",
-        "nobody",
-        "non",
-        "none",
-        "noone",
-        "nor",
-        "normally",
-        "not",
-        "nothing",
-        "novel",
-        "now",
-        "nowhere",
-        "obviously",
-        "of",
-        "off",
-        "often",
-        "oh",
-        "ok",
-        "okay",
-        "old",
-        "on",
-        "once",
-        "one",
-        "ones",
-        "only",
-        "onto",
-        "or",
-        "other",
-        "others",
-        "otherwise",
-        "ought",
-        "our",
-        "ours",
-        "ourselves",
-        "out",
-        "outside",
-        "over",
-        "overall",
-        "own",
-        "part",
-        "particular",
-        "particularly",
-        "per",
-        "perhaps",
-        "placed",
-        "please",
-        "plus",
-        "possible",
-        "presumably",
-        "probably",
-        "provides",
-        "put",
-        "que",
-        "quite",
-        "qv",
-        "rather",
-        "rd",
-        "re",
-        "really",
-        "reasonably",
-        "regarding",
-        "regardless",
-        "regards",
-        "relatively",
-        "respectively",
-        "right",
-        "said",
-        "same",
-        "saw",
-        "say",
-        "saying",
-        "says",
-        "second",
-        "secondly",
-        "see",
-        "seeing",
-        "seem",
-        "seemed",
-        "seeming",
-        "seems",
-        "seen",
-        "self",
-        "selves",
-        "sensible",
-        "sent",
-        "serious",
-        "seriously",
-        "seven",
-        "several",
-        "shall",
-        "she",
-        "should",
-        "shouldn't",
-        "show",
-        "side",
-        "since",
-        "sincere",
-        "six",
-        "sixty",
-        "so",
-        "some",
-        "somebody",
-        "somehow",
-        "someone",
-        "something",
-        "sometime",
-        "sometimes",
-        "somewhat",
-        "somewhere",
-        "soon",
-        "sorry",
-        "specified",
-        "specify",
-        "specifying",
-        "still",
-        "sub",
-        "such",
-        "sup",
-        "sure",
-        "system",
-        "take",
-        "taken",
-        "tell",
-        "ten",
-        "tends",
-        "th",
-        "than",
-        "thank",
-        "thanks",
-        "thanx",
-        "that",
-        "that's",
-        "thats",
-        "that's",
-        "the",
-        "their",
-        "theirs",
-        "them",
-        "themselves",
-        "then",
-        "thence",
-        "there",
-        "thereafter",
-        "thereby",
-        "therefore",
-        "therein",
-        "theres",
-        "thereupon",
-        "there's",
-        "these",
-        "they",
-        "they'd",
-        "they'll",
-        "they're",
-        "they've",
-        "thick",
-        "thin",
-        "think",
-        "third",
-        "this",
-        "thorough",
-        "thoroughly",
-        "those",
-        "though",
-        "three",
-        "through",
-        "throughout",
-        "thru",
-        "thus",
-        "to",
-        "together",
-        "too",
-        "took",
-        "top",
-        "toward",
-        "towards",
-        "tried",
-        "tries",
-        "truly",
-        "try",
-        "trying",
-        "twelve",
-        "twenty",
-        "twice",
-        "two",
-        "t's",
-        "un",
-        "under",
-        "unfortunately",
-        "unless",
-        "unlikely",
-        "until",
-        "unto",
-        "up",
-        "upon",
-        "us",
-        "use",
-        "used",
-        "useful",
-        "uses",
-        "using",
-        "usually",
-        "value",
-        "various",
-        "very",
-        "via",
-        "viz",
-        "vs",
-        "want",
-        "wants",
-        "was",
-        "wasn't",
-        "way",
-        "we",
-        "welcome",
-        "well",
-        "went",
-        "were",
-        "weren't",
-        "we'd",
-        "we'll",
-        "we're",
-        "we've",
-        "what",
-        "whatever",
-        "what's",
-        "when",
-        "whence",
-        "whenever",
-        "where",
-        "whereafter",
-        "whereas",
-        "whereby",
-        "wherein",
-        "whereupon",
-        "wherever",
-        "where's",
-        "whether",
-        "which",
-        "while",
-        "whither",
-        "who",
-        "whoever",
-        "whole",
-        "whom",
-        "whose",
-        "who's",
-        "why",
-        "will",
-        "willing",
-        "wish",
-        "with",
-        "within",
-        "without",
-        "wonder",
-        "won't",
-        "would",
-        "wouldn't",
-        "yes",
-        "yet",
-        "you",
-        "your",
-        "yours",
-        "yourself",
-        "yourselves",
-        "you'd",
-        "you'll",
-        "you're",
-        "you've",
-        "zero",
-    ]
-)
+ENGLISH_STOPWORDS = {
+    "a",
+    "able",
+    "about",
+    "above",
+    "according",
+    "accordingly",
+    "across",
+    "actually",
+    "after",
+    "afterwards",
+    "again",
+    "against",
+    "ain't",
+    "all",
+    "allow",
+    "allows",
+    "almost",
+    "alone",
+    "along",
+    "already",
+    "also",
+    "although",
+    "always",
+    "am",
+    "among",
+    "amongst",
+    "amoungst",
+    "amount",
+    "an",
+    "and",
+    "another",
+    "any",
+    "anybody",
+    "anyhow",
+    "anyone",
+    "anything",
+    "anyway",
+    "anyways",
+    "anywhere",
+    "apart",
+    "appear",
+    "appreciate",
+    "appropriate",
+    "are",
+    "aren't",
+    "around",
+    "as",
+    "aside",
+    "ask",
+    "asking",
+    "associated",
+    "at",
+    "available",
+    "away",
+    "awfully",
+    "back",
+    "be",
+    "became",
+    "because",
+    "become",
+    "becomes",
+    "becoming",
+    "been",
+    "before",
+    "beforehand",
+    "behind",
+    "being",
+    "believe",
+    "below",
+    "beside",
+    "besides",
+    "best",
+    "better",
+    "between",
+    "beyond",
+    "bill",
+    "both",
+    "bottom",
+    "brief",
+    "but",
+    "by",
+    "call",
+    "came",
+    "can",
+    "cannot",
+    "cant",
+    "can't",
+    "cause",
+    "causes",
+    "certain",
+    "certainly",
+    "changes",
+    "clearly",
+    "co",
+    "com",
+    "come",
+    "comes",
+    "computer",
+    "con",
+    "concerning",
+    "consequently",
+    "consider",
+    "considering",
+    "contain",
+    "containing",
+    "contains",
+    "corresponding",
+    "could",
+    "couldnt",
+    "couldn't",
+    "course",
+    "cry",
+    "currently",
+    "c'mon",
+    "c's",
+    "de",
+    "definitely",
+    "describe",
+    "described",
+    "despite",
+    "detail",
+    "did",
+    "didn't",
+    "different",
+    "do",
+    "does",
+    "doesn't",
+    "doing",
+    "done",
+    "don't",
+    "down",
+    "downwards",
+    "due",
+    "during",
+    "each",
+    "edu",
+    "eg",
+    "eight",
+    "either",
+    "eleven",
+    "else",
+    "elsewhere",
+    "empty",
+    "enough",
+    "entirely",
+    "especially",
+    "et",
+    "etc",
+    "even",
+    "ever",
+    "every",
+    "everybody",
+    "everyone",
+    "everything",
+    "everywhere",
+    "ex",
+    "exactly",
+    "example",
+    "except",
+    "far",
+    "few",
+    "fifteen",
+    "fifth",
+    "fify",
+    "fill",
+    "find",
+    "fire",
+    "first",
+    "five",
+    "followed",
+    "following",
+    "follows",
+    "for",
+    "former",
+    "formerly",
+    "forth",
+    "forty",
+    "found",
+    "four",
+    "from",
+    "front",
+    "full",
+    "further",
+    "furthermore",
+    "get",
+    "gets",
+    "getting",
+    "give",
+    "given",
+    "gives",
+    "go",
+    "goes",
+    "going",
+    "gone",
+    "got",
+    "gotten",
+    "greetings",
+    "had",
+    "hadn't",
+    "happens",
+    "hardly",
+    "has",
+    "hasnt",
+    "hasn't",
+    "have",
+    "haven't",
+    "having",
+    "he",
+    "hello",
+    "help",
+    "hence",
+    "her",
+    "here",
+    "hereafter",
+    "hereby",
+    "herein",
+    "hereupon",
+    "here's",
+    "hers",
+    "herself",
+    "he's",
+    "hi",
+    "him",
+    "himself",
+    "his",
+    "hither",
+    "hopefully",
+    "how",
+    "howbeit",
+    "however",
+    "hundred",
+    "i",
+    "i'd",
+    "i'll",
+    "i'm",
+    "i've",
+    "ie",
+    "if",
+    "ignored",
+    "immediate",
+    "in",
+    "inasmuch",
+    "inc",
+    "indeed",
+    "indicate",
+    "indicated",
+    "indicates",
+    "inner",
+    "insofar",
+    "instead",
+    "interest",
+    "into",
+    "inward",
+    "is",
+    "isn't",
+    "it",
+    "its",
+    "itself",
+    "it'd",
+    "it'll",
+    "it's'",
+    "i'd",
+    "i'll",
+    "i'm",
+    "i've",
+    "just",
+    "keep",
+    "keeps",
+    "kept",
+    "know",
+    "known",
+    "knows",
+    "last",
+    "lately",
+    "later",
+    "latter",
+    "latterly",
+    "least",
+    "less",
+    "lest",
+    "let",
+    "let's",
+    "like",
+    "liked",
+    "likely",
+    "little",
+    "look",
+    "looking",
+    "looks",
+    "ltd",
+    "made",
+    "mainly",
+    "many",
+    "may",
+    "maybe",
+    "me",
+    "mean",
+    "meanwhile",
+    "merely",
+    "might",
+    "mill",
+    "mine",
+    "more",
+    "moreover",
+    "most",
+    "mostly",
+    "move",
+    "much",
+    "must",
+    "my",
+    "myself",
+    "name",
+    "namely",
+    "nd",
+    "near",
+    "nearly",
+    "necessary",
+    "need",
+    "needs",
+    "neither",
+    "never",
+    "nevertheless",
+    "new",
+    "next",
+    "nine",
+    "no",
+    "nobody",
+    "non",
+    "none",
+    "noone",
+    "nor",
+    "normally",
+    "not",
+    "nothing",
+    "novel",
+    "now",
+    "nowhere",
+    "obviously",
+    "of",
+    "off",
+    "often",
+    "oh",
+    "ok",
+    "okay",
+    "old",
+    "on",
+    "once",
+    "one",
+    "ones",
+    "only",
+    "onto",
+    "or",
+    "other",
+    "others",
+    "otherwise",
+    "ought",
+    "our",
+    "ours",
+    "ourselves",
+    "out",
+    "outside",
+    "over",
+    "overall",
+    "own",
+    "part",
+    "particular",
+    "particularly",
+    "per",
+    "perhaps",
+    "placed",
+    "please",
+    "plus",
+    "possible",
+    "presumably",
+    "probably",
+    "provides",
+    "put",
+    "que",
+    "quite",
+    "qv",
+    "rather",
+    "rd",
+    "re",
+    "really",
+    "reasonably",
+    "regarding",
+    "regardless",
+    "regards",
+    "relatively",
+    "respectively",
+    "right",
+    "said",
+    "same",
+    "saw",
+    "say",
+    "saying",
+    "says",
+    "second",
+    "secondly",
+    "see",
+    "seeing",
+    "seem",
+    "seemed",
+    "seeming",
+    "seems",
+    "seen",
+    "self",
+    "selves",
+    "sensible",
+    "sent",
+    "serious",
+    "seriously",
+    "seven",
+    "several",
+    "shall",
+    "she",
+    "should",
+    "shouldn't",
+    "show",
+    "side",
+    "since",
+    "sincere",
+    "six",
+    "sixty",
+    "so",
+    "some",
+    "somebody",
+    "somehow",
+    "someone",
+    "something",
+    "sometime",
+    "sometimes",
+    "somewhat",
+    "somewhere",
+    "soon",
+    "sorry",
+    "specified",
+    "specify",
+    "specifying",
+    "still",
+    "sub",
+    "such",
+    "sup",
+    "sure",
+    "system",
+    "take",
+    "taken",
+    "tell",
+    "ten",
+    "tends",
+    "th",
+    "than",
+    "thank",
+    "thanks",
+    "thanx",
+    "that",
+    "that's",
+    "thats",
+    "that's",
+    "the",
+    "their",
+    "theirs",
+    "them",
+    "themselves",
+    "then",
+    "thence",
+    "there",
+    "thereafter",
+    "thereby",
+    "therefore",
+    "therein",
+    "theres",
+    "thereupon",
+    "there's",
+    "these",
+    "they",
+    "they'd",
+    "they'll",
+    "they're",
+    "they've",
+    "thick",
+    "thin",
+    "think",
+    "third",
+    "this",
+    "thorough",
+    "thoroughly",
+    "those",
+    "though",
+    "three",
+    "through",
+    "throughout",
+    "thru",
+    "thus",
+    "to",
+    "together",
+    "too",
+    "took",
+    "top",
+    "toward",
+    "towards",
+    "tried",
+    "tries",
+    "truly",
+    "try",
+    "trying",
+    "twelve",
+    "twenty",
+    "twice",
+    "two",
+    "t's",
+    "un",
+    "under",
+    "unfortunately",
+    "unless",
+    "unlikely",
+    "until",
+    "unto",
+    "up",
+    "upon",
+    "us",
+    "use",
+    "used",
+    "useful",
+    "uses",
+    "using",
+    "usually",
+    "value",
+    "various",
+    "very",
+    "via",
+    "viz",
+    "vs",
+    "want",
+    "wants",
+    "was",
+    "wasn't",
+    "way",
+    "we",
+    "welcome",
+    "well",
+    "went",
+    "were",
+    "weren't",
+    "we'd",
+    "we'll",
+    "we're",
+    "we've",
+    "what",
+    "whatever",
+    "what's",
+    "when",
+    "whence",
+    "whenever",
+    "where",
+    "whereafter",
+    "whereas",
+    "whereby",
+    "wherein",
+    "whereupon",
+    "wherever",
+    "where's",
+    "whether",
+    "which",
+    "while",
+    "whither",
+    "who",
+    "whoever",
+    "whole",
+    "whom",
+    "whose",
+    "who's",
+    "why",
+    "will",
+    "willing",
+    "wish",
+    "with",
+    "within",
+    "without",
+    "wonder",
+    "won't",
+    "would",
+    "wouldn't",
+    "yes",
+    "yet",
+    "you",
+    "your",
+    "yours",
+    "yourself",
+    "yourselves",
+    "you'd",
+    "you'll",
+    "you're",
+    "you've",
+    "zero",
+}
 
 
-ENGLISH_REGULAR_VERBS = set(
-    [
-        "accept",
-        "add",
-        "admire",
-        "admit",
-        "advise",
-        "afford",
-        "agree",
-        "alert",
-        "allow",
-        "amuse",
-        "analyse",
-        "announce",
-        "annoy",
-        "answer",
-        "apologise",
-        "appear",
-        "applaud",
-        "appreciate",
-        "approve",
-        "argue",
-        "arrange",
-        "arrest",
-        "arrive",
-        "ask",
-        "attach",
-        "attack",
-        "attempt",
-        "attend",
-        "attract",
-        "avoid",
-        "back",
-        "bake",
-        "balance",
-        "ban",
-        "bang",
-        "bare",
-        "bat",
-        "bathe",
-        "battle",
-        "beam",
-        "beg",
-        "behave",
-        "belong",
-        "bleach",
-        "bless",
-        "blind",
-        "blink",
-        "blot",
-        "blush",
-        "boast",
-        "boil",
-        "bolt",
-        "bomb",
-        "book",
-        "bore",
-        "borrow",
-        "bounce",
-        "bow",
-        "box",
-        "brake",
-        "branch",
-        "breathe",
-        "bruise",
-        "brush",
-        "bubble",
-        "bump",
-        "burn",
-        "bury",
-        "buzz",
-        "calculate",
-        "call",
-        "camp",
-        "care",
-        "carry",
-        "carve",
-        "cause",
-        "challenge",
-        "change",
-        "charge",
-        "chase",
-        "cheat",
-        "check",
-        "cheer",
-        "chew",
-        "choke",
-        "chop",
-        "claim",
-        "clap",
-        "clean",
-        "clear",
-        "clip",
-        "close",
-        "coach",
-        "coil",
-        "collect",
-        "colour",
-        "comb",
-        "command",
-        "communicate",
-        "compare",
-        "compete",
-        "complain",
-        "complete",
-        "concentrate",
-        "concern",
-        "confess",
-        "confuse",
-        "connect",
-        "consider",
-        "consist",
-        "contain",
-        "continue",
-        "copy",
-        "correct",
-        "cough",
-        "count",
-        "cover",
-        "crack",
-        "crash",
-        "crawl",
-        "cross",
-        "crush",
-        "cry",
-        "cure",
-        "curl",
-        "curve",
-        "cycle",
-        "dam",
-        "damage",
-        "dance",
-        "dare",
-        "decay",
-        "deceive",
-        "decide",
-        "decorate",
-        "delay",
-        "delight",
-        "deliver",
-        "depend",
-        "describe",
-        "desert",
-        "deserve",
-        "destroy",
-        "detect",
-        "develop",
-        "disagree",
-        "disappear",
-        "disapprove",
-        "disarm",
-        "discover",
-        "dislike",
-        "divide",
-        "double",
-        "doubt",
-        "drag",
-        "drain",
-        "dream",
-        "dress",
-        "drip",
-        "drop",
-        "drown",
-        "drum",
-        "dry",
-        "dust",
-        "earn",
-        "educate",
-        "embarrass",
-        "employ",
-        "empty",
-        "encourage",
-        "end",
-        "enjoy",
-        "enter",
-        "entertain",
-        "escape",
-        "examine",
-        "excite",
-        "excuse",
-        "exercise",
-        "exist",
-        "expand",
-        "expect",
-        "explain",
-        "explode",
-        "extend",
-        "face",
-        "fade",
-        "fail",
-        "fancy",
-        "fasten",
-        "fax",
-        "fear",
-        "fence",
-        "fetch",
-        "file",
-        "fill",
-        "film",
-        "fire",
-        "fit",
-        "fix",
-        "flap",
-        "flash",
-        "float",
-        "flood",
-        "flow",
-        "flower",
-        "fold",
-        "follow",
-        "fool",
-        "force",
-        "form",
-        "found",
-        "frame",
-        "frighten",
-        "fry",
-        "gather",
-        "gaze",
-        "glow",
-        "glue",
-        "grab",
-        "grate",
-        "grease",
-        "greet",
-        "grin",
-        "grip",
-        "groan",
-        "guarantee",
-        "guard",
-        "guess",
-        "guide",
-        "hammer",
-        "hand",
-        "handle",
-        "hang",
-        "happen",
-        "harass",
-        "harm",
-        "hate",
-        "haunt",
-        "head",
-        "heal",
-        "heap",
-        "heat",
-        "help",
-        "hook",
-        "hop",
-        "hope",
-        "hover",
-        "hug",
-        "hum",
-        "hunt",
-        "hurry",
-        "identify",
-        "ignore",
-        "imagine",
-        "impress",
-        "improve",
-        "include",
-        "increase",
-        "influence",
-        "inform",
-        "inject",
-        "injure",
-        "instruct",
-        "intend",
-        "interest",
-        "interfere",
-        "interrupt",
-        "introduce",
-        "invent",
-        "invite",
-        "irritate",
-        "itch",
-        "jail",
-        "jam",
-        "jog",
-        "join",
-        "joke",
-        "judge",
-        "juggle",
-        "jump",
-        "kick",
-        "kill",
-        "kiss",
-        "kneel",
-        "knit",
-        "knock",
-        "knot",
-        "label",
-        "land",
-        "last",
-        "laugh",
-        "launch",
-        "learn",
-        "level",
-        "license",
-        "lick",
-        "lie",
-        "lighten",
-        "like",
-        "list",
-        "listen",
-        "live",
-        "load",
-        "lock",
-        "long",
-        "look",
-        "love",
-        "man",
-        "manage",
-        "march",
-        "mark",
-        "marry",
-        "match",
-        "mate",
-        "matter",
-        "measure",
-        "meddle",
-        "melt",
-        "memorise",
-        "mend",
-        "mess up",
-        "milk",
-        "mine",
-        "miss",
-        "mix",
-        "moan",
-        "moor",
-        "mourn",
-        "move",
-        "muddle",
-        "mug",
-        "multiply",
-        "murder",
-        "nail",
-        "name",
-        "need",
-        "nest",
-        "nod",
-        "note",
-        "notice",
-        "number",
-        "obey",
-        "object",
-        "observe",
-        "obtain",
-        "occur",
-        "offend",
-        "offer",
-        "open",
-        "order",
-        "overflow",
-        "owe",
-        "own",
-        "pack",
-        "paddle",
-        "paint",
-        "park",
-        "part",
-        "pass",
-        "paste",
-        "pat",
-        "pause",
-        "peck",
-        "pedal",
-        "peel",
-        "peep",
-        "perform",
-        "permit",
-        "phone",
-        "pick",
-        "pinch",
-        "pine",
-        "place",
-        "plan",
-        "plant",
-        "play",
-        "please",
-        "plug",
-        "point",
-        "poke",
-        "polish",
-        "pop",
-        "possess",
-        "post",
-        "pour",
-        "practise",
-        "pray",
-        "preach",
-        "precede",
-        "prefer",
-        "prepare",
-        "present",
-        "preserve",
-        "press",
-        "pretend",
-        "prevent",
-        "prick",
-        "print",
-        "produce",
-        "program",
-        "promise",
-        "protect",
-        "provide",
-        "pull",
-        "pump",
-        "punch",
-        "puncture",
-        "punish",
-        "push",
-        "question",
-        "queue",
-        "race",
-        "radiate",
-        "rain",
-        "raise",
-        "reach",
-        "realise",
-        "receive",
-        "recognise",
-        "record",
-        "reduce",
-        "reflect",
-        "refuse",
-        "regret",
-        "reign",
-        "reject",
-        "rejoice",
-        "relax",
-        "release",
-        "rely",
-        "remain",
-        "remember",
-        "remind",
-        "remove",
-        "repair",
-        "repeat",
-        "replace",
-        "reply",
-        "report",
-        "reproduce",
-        "request",
-        "rescue",
-        "retire",
-        "return",
-        "rhyme",
-        "rinse",
-        "risk",
-        "rob",
-        "rock",
-        "roll",
-        "rot",
-        "rub",
-        "ruin",
-        "rule",
-        "rush",
-        "sack",
-        "sail",
-        "satisfy",
-        "save",
-        "saw",
-        "scare",
-        "scatter",
-        "scold",
-        "scorch",
-        "scrape",
-        "scratch",
-        "scream",
-        "screw",
-        "scribble",
-        "scrub",
-        "seal",
-        "search",
-        "separate",
-        "serve",
-        "settle",
-        "shade",
-        "share",
-        "shave",
-        "shelter",
-        "shiver",
-        "shock",
-        "shop",
-        "shrug",
-        "sigh",
-        "sign",
-        "signal",
-        "sin",
-        "sip",
-        "ski",
-        "skip",
-        "slap",
-        "slip",
-        "slow",
-        "smash",
-        "smell",
-        "smile",
-        "smoke",
-        "snatch",
-        "sneeze",
-        "sniff",
-        "snore",
-        "snow",
-        "soak",
-        "soothe",
-        "sound",
-        "spare",
-        "spark",
-        "sparkle",
-        "spell",
-        "spill",
-        "spoil",
-        "spot",
-        "spray",
-        "sprout",
-        "squash",
-        "squeak",
-        "squeal",
-        "squeeze",
-        "stain",
-        "stamp",
-        "stare",
-        "start",
-        "stay",
-        "steer",
-        "step",
-        "stir",
-        "stitch",
-        "stop",
-        "store",
-        "strap",
-        "strengthen",
-        "stretch",
-        "strip",
-        "stroke",
-        "stuff",
-        "subtract",
-        "succeed",
-        "suck",
-        "suffer",
-        "suggest",
-        "suit",
-        "supply",
-        "support",
-        "suppose",
-        "surprise",
-        "surround",
-        "suspect",
-        "suspend",
-        "switch",
-        "talk",
-        "tame",
-        "tap",
-        "taste",
-        "tease",
-        "telephone",
-        "tempt",
-        "terrify",
-        "test",
-        "thank",
-        "thaw",
-        "tick",
-        "tickle",
-        "tie",
-        "time",
-        "tip",
-        "tire",
-        "touch",
-        "tour",
-        "tow",
-        "trace",
-        "trade",
-        "train",
-        "transport",
-        "trap",
-        "travel",
-        "treat",
-        "tremble",
-        "trick",
-        "trip",
-        "trot",
-        "trouble",
-        "trust",
-        "try",
-        "tug",
-        "tumble",
-        "turn",
-        "twist",
-        "type",
-        "undress",
-        "unfasten",
-        "unite",
-        "unlock",
-        "unpack",
-        "untidy",
-        "use",
-        "vanish",
-        "visit",
-        "wail",
-        "wait",
-        "walk",
-        "wander",
-        "want",
-        "warm",
-        "warn",
-        "wash",
-        "waste",
-        "watch",
-        "water",
-        "wave",
-        "weigh",
-        "welcome",
-        "whine",
-        "whip",
-        "whirl",
-        "whisper",
-        "whistle",
-        "wink",
-        "wipe",
-        "wish",
-        "wobble",
-        "wonder",
-        "work",
-        "worry",
-        "wrap",
-        "wreck",
-        "wrestle",
-        "wriggle",
-        "x-ray",
-        "yawn",
-        "yell",
-        "zip",
-        "zoom",
-    ]
-)
+ENGLISH_REGULAR_VERBS = {
+    "accept",
+    "add",
+    "admire",
+    "admit",
+    "advise",
+    "afford",
+    "agree",
+    "alert",
+    "allow",
+    "amuse",
+    "analyse",
+    "announce",
+    "annoy",
+    "answer",
+    "apologise",
+    "appear",
+    "applaud",
+    "appreciate",
+    "approve",
+    "argue",
+    "arrange",
+    "arrest",
+    "arrive",
+    "ask",
+    "attach",
+    "attack",
+    "attempt",
+    "attend",
+    "attract",
+    "avoid",
+    "back",
+    "bake",
+    "balance",
+    "ban",
+    "bang",
+    "bare",
+    "bat",
+    "bathe",
+    "battle",
+    "beam",
+    "beg",
+    "behave",
+    "belong",
+    "bleach",
+    "bless",
+    "blind",
+    "blink",
+    "blot",
+    "blush",
+    "boast",
+    "boil",
+    "bolt",
+    "bomb",
+    "book",
+    "bore",
+    "borrow",
+    "bounce",
+    "bow",
+    "box",
+    "brake",
+    "branch",
+    "breathe",
+    "bruise",
+    "brush",
+    "bubble",
+    "bump",
+    "burn",
+    "bury",
+    "buzz",
+    "calculate",
+    "call",
+    "camp",
+    "care",
+    "carry",
+    "carve",
+    "cause",
+    "challenge",
+    "change",
+    "charge",
+    "chase",
+    "cheat",
+    "check",
+    "cheer",
+    "chew",
+    "choke",
+    "chop",
+    "claim",
+    "clap",
+    "clean",
+    "clear",
+    "clip",
+    "close",
+    "coach",
+    "coil",
+    "collect",
+    "colour",
+    "comb",
+    "command",
+    "communicate",
+    "compare",
+    "compete",
+    "complain",
+    "complete",
+    "concentrate",
+    "concern",
+    "confess",
+    "confuse",
+    "connect",
+    "consider",
+    "consist",
+    "contain",
+    "continue",
+    "copy",
+    "correct",
+    "cough",
+    "count",
+    "cover",
+    "crack",
+    "crash",
+    "crawl",
+    "cross",
+    "crush",
+    "cry",
+    "cure",
+    "curl",
+    "curve",
+    "cycle",
+    "dam",
+    "damage",
+    "dance",
+    "dare",
+    "decay",
+    "deceive",
+    "decide",
+    "decorate",
+    "delay",
+    "delight",
+    "deliver",
+    "depend",
+    "describe",
+    "desert",
+    "deserve",
+    "destroy",
+    "detect",
+    "develop",
+    "disagree",
+    "disappear",
+    "disapprove",
+    "disarm",
+    "discover",
+    "dislike",
+    "divide",
+    "double",
+    "doubt",
+    "drag",
+    "drain",
+    "dream",
+    "dress",
+    "drip",
+    "drop",
+    "drown",
+    "drum",
+    "dry",
+    "dust",
+    "earn",
+    "educate",
+    "embarrass",
+    "employ",
+    "empty",
+    "encourage",
+    "end",
+    "enjoy",
+    "enter",
+    "entertain",
+    "escape",
+    "examine",
+    "excite",
+    "excuse",
+    "exercise",
+    "exist",
+    "expand",
+    "expect",
+    "explain",
+    "explode",
+    "extend",
+    "face",
+    "fade",
+    "fail",
+    "fancy",
+    "fasten",
+    "fax",
+    "fear",
+    "fence",
+    "fetch",
+    "file",
+    "fill",
+    "film",
+    "fire",
+    "fit",
+    "fix",
+    "flap",
+    "flash",
+    "float",
+    "flood",
+    "flow",
+    "flower",
+    "fold",
+    "follow",
+    "fool",
+    "force",
+    "form",
+    "found",
+    "frame",
+    "frighten",
+    "fry",
+    "gather",
+    "gaze",
+    "glow",
+    "glue",
+    "grab",
+    "grate",
+    "grease",
+    "greet",
+    "grin",
+    "grip",
+    "groan",
+    "guarantee",
+    "guard",
+    "guess",
+    "guide",
+    "hammer",
+    "hand",
+    "handle",
+    "hang",
+    "happen",
+    "harass",
+    "harm",
+    "hate",
+    "haunt",
+    "head",
+    "heal",
+    "heap",
+    "heat",
+    "help",
+    "hook",
+    "hop",
+    "hope",
+    "hover",
+    "hug",
+    "hum",
+    "hunt",
+    "hurry",
+    "identify",
+    "ignore",
+    "imagine",
+    "impress",
+    "improve",
+    "include",
+    "increase",
+    "influence",
+    "inform",
+    "inject",
+    "injure",
+    "instruct",
+    "intend",
+    "interest",
+    "interfere",
+    "interrupt",
+    "introduce",
+    "invent",
+    "invite",
+    "irritate",
+    "itch",
+    "jail",
+    "jam",
+    "jog",
+    "join",
+    "joke",
+    "judge",
+    "juggle",
+    "jump",
+    "kick",
+    "kill",
+    "kiss",
+    "kneel",
+    "knit",
+    "knock",
+    "knot",
+    "label",
+    "land",
+    "last",
+    "laugh",
+    "launch",
+    "learn",
+    "level",
+    "license",
+    "lick",
+    "lie",
+    "lighten",
+    "like",
+    "list",
+    "listen",
+    "live",
+    "load",
+    "lock",
+    "long",
+    "look",
+    "love",
+    "man",
+    "manage",
+    "march",
+    "mark",
+    "marry",
+    "match",
+    "mate",
+    "matter",
+    "measure",
+    "meddle",
+    "melt",
+    "memorise",
+    "mend",
+    "mess up",
+    "milk",
+    "mine",
+    "miss",
+    "mix",
+    "moan",
+    "moor",
+    "mourn",
+    "move",
+    "muddle",
+    "mug",
+    "multiply",
+    "murder",
+    "nail",
+    "name",
+    "need",
+    "nest",
+    "nod",
+    "note",
+    "notice",
+    "number",
+    "obey",
+    "object",
+    "observe",
+    "obtain",
+    "occur",
+    "offend",
+    "offer",
+    "open",
+    "order",
+    "overflow",
+    "owe",
+    "own",
+    "pack",
+    "paddle",
+    "paint",
+    "park",
+    "part",
+    "pass",
+    "paste",
+    "pat",
+    "pause",
+    "peck",
+    "pedal",
+    "peel",
+    "peep",
+    "perform",
+    "permit",
+    "phone",
+    "pick",
+    "pinch",
+    "pine",
+    "place",
+    "plan",
+    "plant",
+    "play",
+    "please",
+    "plug",
+    "point",
+    "poke",
+    "polish",
+    "pop",
+    "possess",
+    "post",
+    "pour",
+    "practise",
+    "pray",
+    "preach",
+    "precede",
+    "prefer",
+    "prepare",
+    "present",
+    "preserve",
+    "press",
+    "pretend",
+    "prevent",
+    "prick",
+    "print",
+    "produce",
+    "program",
+    "promise",
+    "protect",
+    "provide",
+    "pull",
+    "pump",
+    "punch",
+    "puncture",
+    "punish",
+    "push",
+    "question",
+    "queue",
+    "race",
+    "radiate",
+    "rain",
+    "raise",
+    "reach",
+    "realise",
+    "receive",
+    "recognise",
+    "record",
+    "reduce",
+    "reflect",
+    "refuse",
+    "regret",
+    "reign",
+    "reject",
+    "rejoice",
+    "relax",
+    "release",
+    "rely",
+    "remain",
+    "remember",
+    "remind",
+    "remove",
+    "repair",
+    "repeat",
+    "replace",
+    "reply",
+    "report",
+    "reproduce",
+    "request",
+    "rescue",
+    "retire",
+    "return",
+    "rhyme",
+    "rinse",
+    "risk",
+    "rob",
+    "rock",
+    "roll",
+    "rot",
+    "rub",
+    "ruin",
+    "rule",
+    "rush",
+    "sack",
+    "sail",
+    "satisfy",
+    "save",
+    "saw",
+    "scare",
+    "scatter",
+    "scold",
+    "scorch",
+    "scrape",
+    "scratch",
+    "scream",
+    "screw",
+    "scribble",
+    "scrub",
+    "seal",
+    "search",
+    "separate",
+    "serve",
+    "settle",
+    "shade",
+    "share",
+    "shave",
+    "shelter",
+    "shiver",
+    "shock",
+    "shop",
+    "shrug",
+    "sigh",
+    "sign",
+    "signal",
+    "sin",
+    "sip",
+    "ski",
+    "skip",
+    "slap",
+    "slip",
+    "slow",
+    "smash",
+    "smell",
+    "smile",
+    "smoke",
+    "snatch",
+    "sneeze",
+    "sniff",
+    "snore",
+    "snow",
+    "soak",
+    "soothe",
+    "sound",
+    "spare",
+    "spark",
+    "sparkle",
+    "spell",
+    "spill",
+    "spoil",
+    "spot",
+    "spray",
+    "sprout",
+    "squash",
+    "squeak",
+    "squeal",
+    "squeeze",
+    "stain",
+    "stamp",
+    "stare",
+    "start",
+    "stay",
+    "steer",
+    "step",
+    "stir",
+    "stitch",
+    "stop",
+    "store",
+    "strap",
+    "strengthen",
+    "stretch",
+    "strip",
+    "stroke",
+    "stuff",
+    "subtract",
+    "succeed",
+    "suck",
+    "suffer",
+    "suggest",
+    "suit",
+    "supply",
+    "support",
+    "suppose",
+    "surprise",
+    "surround",
+    "suspect",
+    "suspend",
+    "switch",
+    "talk",
+    "tame",
+    "tap",
+    "taste",
+    "tease",
+    "telephone",
+    "tempt",
+    "terrify",
+    "test",
+    "thank",
+    "thaw",
+    "tick",
+    "tickle",
+    "tie",
+    "time",
+    "tip",
+    "tire",
+    "touch",
+    "tour",
+    "tow",
+    "trace",
+    "trade",
+    "train",
+    "transport",
+    "trap",
+    "travel",
+    "treat",
+    "tremble",
+    "trick",
+    "trip",
+    "trot",
+    "trouble",
+    "trust",
+    "try",
+    "tug",
+    "tumble",
+    "turn",
+    "twist",
+    "type",
+    "undress",
+    "unfasten",
+    "unite",
+    "unlock",
+    "unpack",
+    "untidy",
+    "use",
+    "vanish",
+    "visit",
+    "wail",
+    "wait",
+    "walk",
+    "wander",
+    "want",
+    "warm",
+    "warn",
+    "wash",
+    "waste",
+    "watch",
+    "water",
+    "wave",
+    "weigh",
+    "welcome",
+    "whine",
+    "whip",
+    "whirl",
+    "whisper",
+    "whistle",
+    "wink",
+    "wipe",
+    "wish",
+    "wobble",
+    "wonder",
+    "work",
+    "worry",
+    "wrap",
+    "wreck",
+    "wrestle",
+    "wriggle",
+    "x-ray",
+    "yawn",
+    "yell",
+    "zip",
+    "zoom",
+}
 
 
-ENGLISH_IRREGULAR_VERBS = set(
-    [
-        "arise ",
-        "arisen",
-        "arose ",
-        "ate",
-        "awake",
-        "awakened",
-        "awoke",
-        "awoken",
-        "backslid",
-        "backslidden",
-        "backslide",
-        "bade",
-        "be",
-        "bear",
-        "beat",
-        "beaten",
-        "became",
-        "become",
-        "been",
-        "began",
-        "begin",
-        "begun",
-        "bend",
-        "bent",
-        "bet",
-        "betted",
-        "bid",
-        "bidden",
-        "bind",
-        "bit",
-        "bite",
-        "bitten",
-        "bled",
-        "bleed",
-        "blew",
-        "blow",
-        "blown",
-        "bore",
-        "born",
-        "borne",
-        "bought",
-        "bound",
-        "break",
-        "bred",
-        "breed",
-        "bring",
-        "broadcast",
-        "broadcasted",
-        "broke",
-        "broken",
-        "brought",
-        "build",
-        "built",
-        "burn",
-        "burned",
-        "burnt",
-        "burst",
-        "bust",
-        "busted",
-        "buy",
-        "came",
-        "cast",
-        "catch",
-        "caught",
-        "choose",
-        "chose",
-        "chosen",
-        "clad",
-        "cling",
-        "clothe",
-        "clothed",
-        "clung",
-        "come",
-        "cost",
-        "creep",
-        "crept",
-        "cut",
-        "daydream",
-        "daydreamed",
-        "daydreamt",
-        "deal",
-        "dealt",
-        "did",
-        "dig",
-        "disprove",
-        "disproved",
-        "disproven",
-        "dive",
-        "dived",
-        "do",
-        "done",
-        "dove",
-        "drank",
-        "draw",
-        "drawn",
-        "dream",
-        "dreamed",
-        "dreamt",
-        "drew",
-        "drink",
-        "drive",
-        "driven",
-        "drove",
-        "drunk",
-        "dug",
-        "dwell",
-        "dwelled",
-        "dwelt",
-        "eat",
-        "eaten",
-        "fall",
-        "fallen",
-        "fed",
-        "feed",
-        "feel",
-        "fell",
-        "felt",
-        "fight",
-        "find",
-        "fit",
-        "fitted",
-        "fled",
-        "flee",
-        "flew",
-        "fling",
-        "flown",
-        "flung",
-        "fly",
-        "forbade",
-        "forbid",
-        "forbidden",
-        "forecast",
-        "forego",
-        "foregone",
-        "foresaw",
-        "foresee",
-        "foreseen",
-        "foretell",
-        "foretold",
-        "forewent",
-        "forgave",
-        "forget",
-        "forgive",
-        "forgiven",
-        "forgot",
-        "forgotten",
-        "forsake",
-        "forsaken",
-        "forsook",
-        "fought",
-        "found",
-        "freeze",
-        "froze",
-        "frozen",
-        "gave",
-        "get",
-        "give",
-        "given",
-        "go",
-        "gone",
-        "got",
-        "gotten",
-        "grew",
-        "grind",
-        "ground",
-        "grow",
-        "grown",
-        "had",
-        "hang",
-        "have",
-        "hear",
-        "heard",
-        "held",
-        "hew",
-        "hewed",
-        "hewn",
-        "hid",
-        "hidden",
-        "hide",
-        "hit",
-        "hold",
-        "hung",
-        "hurt",
-        "keep",
-        "kept",
-        "kneel",
-        "kneeled",
-        "knelt",
-        "knew",
-        "knit",
-        "knitted",
-        "know",
-        "known",
-        "laid",
-        "lain",
-        "lay",
-        "lead",
-        "lean",
-        "leaned",
-        "leant",
-        "leap",
-        "leaped",
-        "leapt",
-        "learn",
-        "learned",
-        "learnt",
-        "leave",
-        "led",
-        "left",
-        "lend",
-        "lent",
-        "let",
-        "lie",
-        "lied",
-        "light",
-        "lighted",
-        "lit",
-        "lose",
-        "lost",
-        "made",
-        "make",
-        "mean",
-        "meant",
-        "meet",
-        "met",
-        "misunderstand",
-        "misunderstood",
-        "mow",
-        "mowed",
-        "mown",
-        "paid",
-        "partake",
-        "partaken",
-        "partook",
-        "pay",
-        "plead",
-        "pleaded",
-        "pled",
-        "proofread",
-        "prove",
-        "proved",
-        "proven",
-        "put",
-        "quick-freeze",
-        "quick-froze",
-        "quick-frozen",
-        "quit",
-        "quitted",
-        "ran",
-        "rang",
-        "read",
-        "rid",
-        "ridden",
-        "ride",
-        "ring",
-        "rise",
-        "risen",
-        "rode",
-        "rose",
-        "run",
-        "rung",
-        "said",
-        "sang",
-        "sank",
-        "sat",
-        "saw",
-        "sawed",
-        "sawn",
-        "say",
-        "see",
-        "seek",
-        "seen",
-        "sell",
-        "send",
-        "sent",
-        "set",
-        "sew",
-        "sewed",
-        "sewn",
-        "shake",
-        "shaken",
-        "shave",
-        "shaved",
-        "shaven",
-        "shear",
-        "sheared",
-        "shed",
-        "shine",
-        "shined",
-        "shone",
-        "shook",
-        "shoot",
-        "shorn",
-        "shot",
-        "show",
-        "showed",
-        "shown",
-        "shrank",
-        "shrink",
-        "shrunk",
-        "shut",
-        "sing",
-        "sink",
-        "sit",
-        "slain",
-        "slay",
-        "slayed",
-        "sleep",
-        "slept",
-        "slew",
-        "slid",
-        "slide",
-        "sling",
-        "slink",
-        "slinked",
-        "slit",
-        "slung",
-        "slunk",
-        "smell",
-        "smelled",
-        "smelt",
-        "sneak",
-        "sneaked",
-        "snuck",
-        "sold",
-        "sought",
-        "sow",
-        "sowed",
-        "sown",
-        "spat",
-        "speak",
-        "sped",
-        "speed",
-        "speeded",
-        "spell",
-        "spelled",
-        "spelt",
-        "spend",
-        "spent",
-        "spill",
-        "spilled",
-        "spilt",
-        "spin",
-        "spit",
-        "split",
-        "spoil",
-        "spoiled",
-        "spoilt",
-        "spoke",
-        "spoken",
-        "sprang",
-        "spread",
-        "spring",
-        "sprung",
-        "spun",
-        "stand ",
-        "stank",
-        "steal",
-        "stick",
-        "sting",
-        "stink",
-        "stole",
-        "stolen",
-        "stood",
-        "strew",
-        "strewed",
-        "strewn",
-        "stricken",
-        "stridden",
-        "stride",
-        "strike",
-        "string",
-        "strive",
-        "strived",
-        "striven",
-        "strode",
-        "strove",
-        "struck",
-        "strung",
-        "stuck",
-        "stung",
-        "stunk",
-        "sublet",
-        "sunburn",
-        "sunburned",
-        "sunburnt",
-        "sung",
-        "sunk",
-        "swam",
-        "swear",
-        "sweat",
-        "sweated",
-        "sweep",
-        "swell",
-        "swelled",
-        "swept",
-        "swim",
-        "swing",
-        "swollen",
-        "swore",
-        "sworn",
-        "swum",
-        "swung",
-        "take",
-        "taken",
-        "taught",
-        "teach",
-        "tear",
-        "telecast",
-        "tell",
-        "test-drive",
-        "test-driven",
-        "test-drove",
-        "test-flew",
-        "test-flown",
-        "test-fly",
-        "think",
-        "thought",
-        "threw",
-        "throw",
-        "thrown",
-        "thrust",
-        "told",
-        "took",
-        "tore",
-        "torn",
-        "tread",
-        "trod",
-        "trodden",
-        "understand",
-        "understood",
-        "undertake",
-        "undertaken",
-        "undertook",
-        "undid",
-        "undo",
-        "undone",
-        "wake",
-        "waked",
-        "was, were",
-        "waylaid",
-        "waylay",
-        "wear",
-        "weave",
-        "weaved",
-        "wed",
-        "wedded",
-        "weep",
-        "went",
-        "wept",
-        "wet",
-        "wetted",
-        "whet",
-        "whetted",
-        "win",
-        "wind",
-        "withdraw",
-        "withdrawn",
-        "withdrew",
-        "withheld",
-        "withhold",
-        "withstand",
-        "withstood",
-        "woke",
-        "woken",
-        "won",
-        "wore",
-        "worn",
-        "wound",
-        "wove",
-        "woven",
-        "wring",
-        "write",
-        "written",
-        "wrote",
-        "wrung",
-    ]
-)
+ENGLISH_IRREGULAR_VERBS = {
+    "arise ",
+    "arisen",
+    "arose ",
+    "ate",
+    "awake",
+    "awakened",
+    "awoke",
+    "awoken",
+    "backslid",
+    "backslidden",
+    "backslide",
+    "bade",
+    "be",
+    "bear",
+    "beat",
+    "beaten",
+    "became",
+    "become",
+    "been",
+    "began",
+    "begin",
+    "begun",
+    "bend",
+    "bent",
+    "bet",
+    "betted",
+    "bid",
+    "bidden",
+    "bind",
+    "bit",
+    "bite",
+    "bitten",
+    "bled",
+    "bleed",
+    "blew",
+    "blow",
+    "blown",
+    "bore",
+    "born",
+    "borne",
+    "bought",
+    "bound",
+    "break",
+    "bred",
+    "breed",
+    "bring",
+    "broadcast",
+    "broadcasted",
+    "broke",
+    "broken",
+    "brought",
+    "build",
+    "built",
+    "burn",
+    "burned",
+    "burnt",
+    "burst",
+    "bust",
+    "busted",
+    "buy",
+    "came",
+    "cast",
+    "catch",
+    "caught",
+    "choose",
+    "chose",
+    "chosen",
+    "clad",
+    "cling",
+    "clothe",
+    "clothed",
+    "clung",
+    "come",
+    "cost",
+    "creep",
+    "crept",
+    "cut",
+    "daydream",
+    "daydreamed",
+    "daydreamt",
+    "deal",
+    "dealt",
+    "did",
+    "dig",
+    "disprove",
+    "disproved",
+    "disproven",
+    "dive",
+    "dived",
+    "do",
+    "done",
+    "dove",
+    "drank",
+    "draw",
+    "drawn",
+    "dream",
+    "dreamed",
+    "dreamt",
+    "drew",
+    "drink",
+    "drive",
+    "driven",
+    "drove",
+    "drunk",
+    "dug",
+    "dwell",
+    "dwelled",
+    "dwelt",
+    "eat",
+    "eaten",
+    "fall",
+    "fallen",
+    "fed",
+    "feed",
+    "feel",
+    "fell",
+    "felt",
+    "fight",
+    "find",
+    "fit",
+    "fitted",
+    "fled",
+    "flee",
+    "flew",
+    "fling",
+    "flown",
+    "flung",
+    "fly",
+    "forbade",
+    "forbid",
+    "forbidden",
+    "forecast",
+    "forego",
+    "foregone",
+    "foresaw",
+    "foresee",
+    "foreseen",
+    "foretell",
+    "foretold",
+    "forewent",
+    "forgave",
+    "forget",
+    "forgive",
+    "forgiven",
+    "forgot",
+    "forgotten",
+    "forsake",
+    "forsaken",
+    "forsook",
+    "fought",
+    "found",
+    "freeze",
+    "froze",
+    "frozen",
+    "gave",
+    "get",
+    "give",
+    "given",
+    "go",
+    "gone",
+    "got",
+    "gotten",
+    "grew",
+    "grind",
+    "ground",
+    "grow",
+    "grown",
+    "had",
+    "hang",
+    "have",
+    "hear",
+    "heard",
+    "held",
+    "hew",
+    "hewed",
+    "hewn",
+    "hid",
+    "hidden",
+    "hide",
+    "hit",
+    "hold",
+    "hung",
+    "hurt",
+    "keep",
+    "kept",
+    "kneel",
+    "kneeled",
+    "knelt",
+    "knew",
+    "knit",
+    "knitted",
+    "know",
+    "known",
+    "laid",
+    "lain",
+    "lay",
+    "lead",
+    "lean",
+    "leaned",
+    "leant",
+    "leap",
+    "leaped",
+    "leapt",
+    "learn",
+    "learned",
+    "learnt",
+    "leave",
+    "led",
+    "left",
+    "lend",
+    "lent",
+    "let",
+    "lie",
+    "lied",
+    "light",
+    "lighted",
+    "lit",
+    "lose",
+    "lost",
+    "made",
+    "make",
+    "mean",
+    "meant",
+    "meet",
+    "met",
+    "misunderstand",
+    "misunderstood",
+    "mow",
+    "mowed",
+    "mown",
+    "paid",
+    "partake",
+    "partaken",
+    "partook",
+    "pay",
+    "plead",
+    "pleaded",
+    "pled",
+    "proofread",
+    "prove",
+    "proved",
+    "proven",
+    "put",
+    "quick-freeze",
+    "quick-froze",
+    "quick-frozen",
+    "quit",
+    "quitted",
+    "ran",
+    "rang",
+    "read",
+    "rid",
+    "ridden",
+    "ride",
+    "ring",
+    "rise",
+    "risen",
+    "rode",
+    "rose",
+    "run",
+    "rung",
+    "said",
+    "sang",
+    "sank",
+    "sat",
+    "saw",
+    "sawed",
+    "sawn",
+    "say",
+    "see",
+    "seek",
+    "seen",
+    "sell",
+    "send",
+    "sent",
+    "set",
+    "sew",
+    "sewed",
+    "sewn",
+    "shake",
+    "shaken",
+    "shave",
+    "shaved",
+    "shaven",
+    "shear",
+    "sheared",
+    "shed",
+    "shine",
+    "shined",
+    "shone",
+    "shook",
+    "shoot",
+    "shorn",
+    "shot",
+    "show",
+    "showed",
+    "shown",
+    "shrank",
+    "shrink",
+    "shrunk",
+    "shut",
+    "sing",
+    "sink",
+    "sit",
+    "slain",
+    "slay",
+    "slayed",
+    "sleep",
+    "slept",
+    "slew",
+    "slid",
+    "slide",
+    "sling",
+    "slink",
+    "slinked",
+    "slit",
+    "slung",
+    "slunk",
+    "smell",
+    "smelled",
+    "smelt",
+    "sneak",
+    "sneaked",
+    "snuck",
+    "sold",
+    "sought",
+    "sow",
+    "sowed",
+    "sown",
+    "spat",
+    "speak",
+    "sped",
+    "speed",
+    "speeded",
+    "spell",
+    "spelled",
+    "spelt",
+    "spend",
+    "spent",
+    "spill",
+    "spilled",
+    "spilt",
+    "spin",
+    "spit",
+    "split",
+    "spoil",
+    "spoiled",
+    "spoilt",
+    "spoke",
+    "spoken",
+    "sprang",
+    "spread",
+    "spring",
+    "sprung",
+    "spun",
+    "stand ",
+    "stank",
+    "steal",
+    "stick",
+    "sting",
+    "stink",
+    "stole",
+    "stolen",
+    "stood",
+    "strew",
+    "strewed",
+    "strewn",
+    "stricken",
+    "stridden",
+    "stride",
+    "strike",
+    "string",
+    "strive",
+    "strived",
+    "striven",
+    "strode",
+    "strove",
+    "struck",
+    "strung",
+    "stuck",
+    "stung",
+    "stunk",
+    "sublet",
+    "sunburn",
+    "sunburned",
+    "sunburnt",
+    "sung",
+    "sunk",
+    "swam",
+    "swear",
+    "sweat",
+    "sweated",
+    "sweep",
+    "swell",
+    "swelled",
+    "swept",
+    "swim",
+    "swing",
+    "swollen",
+    "swore",
+    "sworn",
+    "swum",
+    "swung",
+    "take",
+    "taken",
+    "taught",
+    "teach",
+    "tear",
+    "telecast",
+    "tell",
+    "test-drive",
+    "test-driven",
+    "test-drove",
+    "test-flew",
+    "test-flown",
+    "test-fly",
+    "think",
+    "thought",
+    "threw",
+    "throw",
+    "thrown",
+    "thrust",
+    "told",
+    "took",
+    "tore",
+    "torn",
+    "tread",
+    "trod",
+    "trodden",
+    "understand",
+    "understood",
+    "undertake",
+    "undertaken",
+    "undertook",
+    "undid",
+    "undo",
+    "undone",
+    "wake",
+    "waked",
+    "was, were",
+    "waylaid",
+    "waylay",
+    "wear",
+    "weave",
+    "weaved",
+    "wed",
+    "wedded",
+    "weep",
+    "went",
+    "wept",
+    "wet",
+    "wetted",
+    "whet",
+    "whetted",
+    "win",
+    "wind",
+    "withdraw",
+    "withdrawn",
+    "withdrew",
+    "withheld",
+    "withhold",
+    "withstand",
+    "withstood",
+    "woke",
+    "woken",
+    "won",
+    "wore",
+    "worn",
+    "wound",
+    "wove",
+    "woven",
+    "wring",
+    "write",
+    "written",
+    "wrote",
+    "wrung",
+}
```

### Comparing `nazca-2.0.2/nazca/data/us_states.py` & `nazca-3.0.0/nazca/data/us_states.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # See http://en.wikipedia.org/wiki/List_of_U.S._state_abbreviations
 # WARNING: The name of each state should be in French
 # (e.g. "Floride", not "Florida")
 US_STATES = {
     "AK": "Alaska",
     "AL": "Alabama",
     "AR": "Arkansas",
```

### Comparing `nazca-2.0.2/nazca/ner/__init__.py` & `nazca-3.0.0/nazca/ner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-# -*- coding: utf-8 -*-
 """ Process/Core functions for Named Entities Recognition.
 """
 from nazca.utils.tokenizer import RichStringTokenizer
 
 
 ###############################################################################
 # NER PROCESS #################################################################
 ###############################################################################
-class NerProcess(object):
-    """ High-level process for Named Entities Recognition
-    """
+class NerProcess:
+    """High-level process for Named Entities Recognition"""
 
     def __init__(self, ner_sources, preprocessors=None, filters=None, unique=False):
-        """ Initialise the class.
+        """Initialise the class.
 
         :tokenizer: an instance of tokenizer
         """
         self.ner_sources = list(ner_sources)
         self.preprocessors = preprocessors or []
         self.filters = filters or []
         self.unique = unique
 
     def add_ner_source(self, process):
-        """ Add a ner process
-        """
+        """Add a ner process"""
         self.ner_sources.append(process)
 
     def add_preprocessors(self, preprocessor):
-        """ Add a preprocessor
-        """
+        """Add a preprocessor"""
         self.preprocessors.append(preprocessor)
 
     def add_filters(self, filter):
-        """ Add a filter
-        """
+        """Add a filter"""
         self.filters.append(filter)
 
     def process_text(self, text):
-        """ High level function for analyzing a text
-        """
+        """High level function for analyzing a text"""
         tokenizer = RichStringTokenizer(text)
         return self.recognize_tokens(tokenizer)
 
     def recognize_tokens(self, tokens):
-        """ Recognize Named Entities from a tokenizer or
+        """Recognize Named Entities from a tokenizer or
         an iterator yielding tokens.
         """
         last_stop = 0
         named_entities = []
         for token in tokens:
             if token.start < last_stop:
                 continue  # this token overlaps with a previous match
@@ -69,11 +63,11 @@
                         break
                 if recognized and self.unique:
                     break
         # XXX Postprocess/filters may be sources dependant
         return self.postprocess(named_entities)
 
     def postprocess(self, named_entities):
-        """ Postprocess the results by applying filters """
+        """Postprocess the results by applying filters"""
         for filter in self.filters:
             named_entities = filter(named_entities)
         return named_entities
```

### Comparing `nazca-2.0.2/nazca/ner/filters.py` & `nazca-3.0.0/nazca/ner/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-# -*- coding: utf-8 -*-
 """ Filters for Named Entities Recognition.
 """
 from nazca.utils.dataio import sparqlquery
 
 
 ###############################################################################
 # NER FILTERS #################################################################
 ###############################################################################
-class AbstractNerFilter(object):
-    """ A filter used for cleaning named entities results
-    """
+class AbstractNerFilter:
+    """A filter used for cleaning named entities results"""
 
     def __call__(self, named_entities):
         raise NotImplementedError
 
 
-class NerOccurenceFilter(object):
-    """ A filter based on the number of occurence of
+class NerOccurenceFilter:
+    """A filter based on the number of occurence of
     named entities in the results.
     """
 
     def __init__(self, min_occ=None, max_occ=None):
         self.min_occ = min_occ
         self.max_occ = max_occ
 
     def __call__(self, named_entities):
         uris = [u for u, p, t in named_entities]
-        counts = dict([(u, uris.count(u)) for u in set(uris)])
+        counts = {u: uris.count(u) for u in set(uris)}
         return [
             n
             for n in named_entities
             if not (
                 (self.min_occ and counts[n[0]] < self.min_occ)
                 or (self.max_occ and counts[n[0]] > self.max_occ)
             )
         ]
 
 
-class NerRDFTypeFilter(object):
-    """ A filter based on the RDF type on entity
+class NerRDFTypeFilter:
+    """A filter based on the RDF type on entity
     E.g.
 
     filter = NerRDFTypeFilter('http://dbpedia.org/sparql',
                                 ('http://schema.org/Place',
                                 'http://dbpedia.org/ontology/Agent',
                                 'http://dbpedia.org/ontology/Place'))
 
@@ -58,25 +56,25 @@
         seen_uris = {}
         for uri, p, t in named_entities:
             if uri in seen_uris:
                 if seen_uris[uri]:
                     filtered_named_entities.append((uri, p, t))
             else:
                 results = sparqlquery(self.endpoint, self.query % {"uri": uri})
-                types = set([r[0] for r in results])
+                types = {r[0] for r in results}
                 if not len(types.intersection(self.accepted_types)):
                     seen_uris[uri] = False
                 else:
                     seen_uris[uri] = True
                     filtered_named_entities.append((uri, p, t))
         return filtered_named_entities
 
 
-class NerDisambiguationWordParts(object):
-    """ Disambiguate named entities based on the words parts.
+class NerDisambiguationWordParts:
+    """Disambiguate named entities based on the words parts.
     E.g.:
           'toto tutu': 'http://example.com/toto_tutu',
           'toto': 'http://example.com/toto'
 
           Then if 'toto' is found in the text, replace the URI 'http://example.com/toto'
           by 'http://example.com/toto_tutu'
     """
@@ -94,17 +92,16 @@
             if token.word.lower() in parts:
                 # Change URI
                 uri = parts[token.word.lower()]
             filtered_named_entities.append((uri, peid, token))
         return filtered_named_entities
 
 
-class NerReplacementRulesFilter(object):
-    """ Allow to define replacement rules for Named Entities
-    """
+class NerReplacementRulesFilter:
+    """Allow to define replacement rules for Named Entities"""
 
     def __init__(self, rules):
         self.rules = rules
 
     def __call__(self, named_entities):
         filtered_named_entities = []
         for uri, peid, token in named_entities:
```

### Comparing `nazca-2.0.2/nazca/ner/preprocessors.py` & `nazca-3.0.0/nazca/ner/preprocessors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-# -*- coding: utf-8 -*-
 """ Preprocessors for Named Entities Recognition.
 """
 from nazca.utils.tokenizer import Token
 from nazca.data.stopwords import FRENCH_STOPWORDS, ENGLISH_STOPWORDS
 
 STOPWORDS = {"fr": FRENCH_STOPWORDS, "en": ENGLISH_STOPWORDS}
 
 
 ###############################################################################
 # NER PREPROCESSORS ###########################################################
 ###############################################################################
-class AbstractNerPreprocessor(object):
-    """ Preprocessor
-    """
+class AbstractNerPreprocessor:
+    """Preprocessor"""
 
     def __call__(self, token):
         raise NotImplementedError
 
 
 class NerWordSizeFilterPreprocessor(AbstractNerPreprocessor):
-    """ Remove token based on the size of the word
-    """
+    """Remove token based on the size of the word"""
 
     def __init__(self, min_size=None, max_size=None):
         self.min_size = min_size
         self.max_size = max_size
 
     def __call__(self, token):
         if (self.min_size and len(token.word) < self.min_size) or (
             self.max_size and len(token.word) > self.max_size
         ):
             return None
         return token
 
 
 class NerLowerCaseFilterPreprocessor(AbstractNerPreprocessor):
-    """ Remove token with word in lower case
-    """
+    """Remove token with word in lower case"""
 
     def __call__(self, token):
         return None if token.word.islower() else token
 
 
 class NerLowerFirstWordPreprocessor(AbstractNerPreprocessor):
-    """ Lower the first word of each sentence if it is a stopword.
-    """
+    """Lower the first word of each sentence if it is a stopword."""
 
     def __init__(self, lang="en"):
         self.lang = lang
 
     def __call__(self, token):
         if token.start == token.sentence.start and token.word.split()[0].lower() in STOPWORDS.get(
             self.lang, ENGLISH_STOPWORDS
         ):
             word = token.word[0].lower() + token.word[1:]
             return Token(word, token.start, token.end, token.sentence)
         return token
 
 
 class NerStopwordsFilterPreprocessor(AbstractNerPreprocessor):
-    """ Remove stopwords
-    """
+    """Remove stopwords"""
 
     def __init__(self, split_words=False, lang="en"):
         self.split_words = split_words
         self.lang = lang
 
     def __call__(self, token):
         stopwords = STOPWORDS.get(self.lang, ENGLISH_STOPWORDS)
@@ -72,16 +66,15 @@
             return None
         if not self.split_words and token.word.lower() in stopwords:
             return None
         return token
 
 
 class NerHashTagPreprocessor(AbstractNerPreprocessor):
-    """ Cleanup hashtag
-    """
+    """Cleanup hashtag"""
 
     def __call__(self, token):
         if token.word.startswith("@"):
             # XXX Split capitalize letter ?
             # @BarackObama -> Barack Obama
             word = token.word[1:].replace("_", " ")
             return Token(word, token.start, token.end, token.sentence)
```

### Comparing `nazca-2.0.2/nazca/ner/sources.py` & `nazca-3.0.0/nazca/ner/sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,105 @@
-# -*- coding: utf-8 -*-
 """ Sources for Named Entities Recognition.
 """
-from nazca.utils.dataio import sparqlquery, rqlquery
+from nazca.utils.dataio import sparqlquery
 
 
 ###############################################################################
 # NER SOURCE ##################################################################
 ###############################################################################
-class AbstractNerSource(object):
-    """ High-level source for Named Entities Recognition
-    """
+class AbstractNerSource:
+    """High-level source for Named Entities Recognition"""
 
     def __init__(self, endpoint, query, name=None, use_cache=True, preprocessors=None):
-        """ Initialise the class.
-        """
+        """Initialise the class."""
         self.endpoint = endpoint
         self.query = query
         self.name = name
         self.preprocessors = preprocessors or []
         self.use_cache = use_cache
         self._recognized_cache = {}
 
     def add_preprocessors(self, preprocessor):
-        """ Add a preprocessor
-        """
+        """Add a preprocessor"""
         self.preprocessors.append(preprocessor)
 
     def recognize_token(self, token):
-        """ Recognize a token
-        """
+        """Recognize a token"""
         # Applies source specific preprocessors
         for preprocessor in self.preprocessors:
             token = preprocessor(token)
             if not token:
                 return []
         if self.use_cache and token.word in self._recognized_cache:
             return self._recognized_cache[token.word]
         uris = self.query_word(token.word) if token.word else []
         if self.use_cache:
             self._recognized_cache[token.word] = uris
         return uris
 
     def query_word(self, word):
-        """ Query a word for a Named Entities Recognition process
-        """
+        """Query a word for a Named Entities Recognition process"""
         raise NotImplementedError
 
 
 class NerSourceLexicon(AbstractNerSource):
-    """ Source based on a (pre-computed) dictionnary of words (token, uri)
-    """
+    """Source based on a (pre-computed) dictionnary of words (token, uri)"""
 
     def __init__(self, lexicon, name=None, use_cache=True, preprocessors=None):
         self.lexicon = lexicon
         self.name = name
         self.preprocessors = preprocessors or []
         self.use_cache = use_cache
         self._recognized_cache = {}
 
     def query_word(self, word):
         uri = self.lexicon.get(word)
-        return [uri,] if uri else []
+        return (
+            [
+                uri,
+            ]
+            if uri
+            else []
+        )
 
 
 class NerSourceLocalRql(AbstractNerSource):
-    """ High-level source for Named Entities Recognition
+    """High-level source for Named Entities Recognition
     Local RQL version
     """
 
     def __init__(self, session, query, name=None, use_cache=True, preprocessors=None):
-        """ Initialise the class.
-        """
+        """Initialise the class."""
         self.query = query
         self.session = session
         self.name = name
         self.preprocessors = preprocessors or []
         self.use_cache = use_cache
         self._recognized_cache = {}
 
     def query_word(self, word):
-        """ Query a word for a Named Entities Recognition process
-        """
+        """Query a word for a Named Entities Recognition process"""
         return [r[0] for r in self.session.execute(self.query, dict(word=word))]
 
 
-class NerSourceRql(AbstractNerSource):
-    """ High-level source for Named Entities Recognition
-    Url version (distant source)
-    """
-
-    def query_word(self, word):
-        """ Query a word for a Named Entities Recognition process
-        """
-        if self.endpoint.startswith("http://"):
-            # url
-            return [r[0] for r in rqlquery(self.endpoint, self.query % {"word": word})]
-        else:
-            return [r[0] for r in rqlquery(self.endpoint, self.query, word=word)]
-
-
 class NerSourceSparql(AbstractNerSource):
-    """ High-level source for Named Entities Recognition
-    SPARQL version
+    """High-level source for Named Entities Recognition
+     SPARQL version
 
-   >>> from ner.core import NerSourceSparql
-   >>> ner_source = NerSourceSparql('''SELECT ?uri
-                                         WHERE{
-                                         ?uri rdfs:label "%(word)s"@en}''',
-                                         'http://dbpedia.org/sparql')
-   >>> print ner_source.recognize_token('Victor Hugo')
-                ... ['http://dbpedia.org/resource/Category:Victor_Hugo',
-                     'http://dbpedia.org/resource/Victor_Hugo',
-                     'http://dbpedia.org/class/yago/VictorHugo',
-                     'http://dbpedia.org/class/yago/VictorHugo(ParisM%C3%A9tro)',
-                     'http://sw.opencyc.org/2008/06/10/concept/en/VictorHugo',
-                     'http://sw.opencyc.org/2008/06/10/concept/Mx4rve1ZXJwpEbGdrcN5Y29ycA']
+    >>> from ner.core import NerSourceSparql
+    >>> ner_source = NerSourceSparql('''SELECT ?uri
+                                          WHERE{
+                                          ?uri rdfs:label "%(word)s"@en}''',
+                                          'http://dbpedia.org/sparql')
+    >>> print ner_source.recognize_token('Victor Hugo')
+                 ... ['http://dbpedia.org/resource/Category:Victor_Hugo',
+                      'http://dbpedia.org/resource/Victor_Hugo',
+                      'http://dbpedia.org/class/yago/VictorHugo',
+                      'http://dbpedia.org/class/yago/VictorHugo(ParisM%C3%A9tro)',
+                      'http://sw.opencyc.org/2008/06/10/concept/en/VictorHugo',
+                      'http://sw.opencyc.org/2008/06/10/concept/Mx4rve1ZXJwpEbGdrcN5Y29ycA']
 
     """
 
     def query_word(self, word):
-        """ Query a word for a Named Entities Recognition process
-        """
+        """Query a word for a Named Entities Recognition process"""
         return [r[0] for r in sparqlquery(self.endpoint, self.query % {"word": word})]
```

### Comparing `nazca-2.0.2/nazca/rl/aligner.py` & `nazca-3.0.0/nazca/rl/aligner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -24,16 +23,15 @@
 from nazca.utils.dataio import parsefile
 
 
 ###############################################################################
 # UTILITY FUNCTIONS ###########################################################
 ###############################################################################
 def iter_aligned_pairs(refset, targetset, global_mat, global_matched, unique=True):
-    """ Return the aligned pairs
-    """
+    """Return the aligned pairs"""
     if unique:
         for refid in global_matched:
             bestid, _ = sorted(global_matched[refid], key=lambda x: x[1])[0]
             ref_record = refset[refid]
             target_record = targetset[bestid]
             distance = global_mat[refid, bestid] if global_mat is not None else None
             yield (ref_record[0], refid), (target_record[0], bestid), distance
@@ -45,15 +43,15 @@
                 distance = global_mat[refid, targetid] if global_mat is not None else None
                 yield (ref_record[0], refid), (target_record[0], targetid), distance
 
 
 ###############################################################################
 # BASE ALIGNER OBJECT #########################################################
 ###############################################################################
-class BaseAligner(object):
+class BaseAligner:
     def __init__(self, threshold, processings, normalize_matrix=False):
         self.threshold = threshold
         self.processings = processings
         self.normalize_matrix = normalize_matrix
         self.ref_normalizer = None
         self.target_normalizer = None
         self.target_normalizer = None
@@ -64,55 +62,55 @@
         self.nb_blocks = 0
         self.refset_size = None
         self.targetset_size = None
         self.time = None
         self.logger = logging.getLogger("nazca.aligner")
 
     def register_ref_normalizer(self, normalizer):
-        """ Register normalizers to be applied
-        before alignment """
+        """Register normalizers to be applied
+        before alignment"""
         self.ref_normalizer = normalizer
 
     def register_target_normalizer(self, normalizer):
-        """ Register normalizers to be applied
-        before alignment """
+        """Register normalizers to be applied
+        before alignment"""
         self.target_normalizer = normalizer
 
     def register_blocking(self, blocking):
         self.blocking = blocking
 
     def apply_normalization(self, dataset, normalizer):
         if normalizer:
             return normalizer.normalize_dataset(dataset)
         return dataset
 
     def compute_distance_matrix(self, refset, targetset, ref_indexes, target_indexes):
-        """ Compute and return the global alignment matrix.
+        """Compute and return the global alignment matrix.
         For each `processing` a `Distancematrix` is built, then all the
         matrices are summed with their own weighting and the result is the global
         alignment matrix, which is returned.
         """
         distmatrix = zeros((len(ref_indexes), len(target_indexes)), dtype="float32")
         for processing in self.processings:
             w = processing.weight
             distmatrix += w * processing.cdist(refset, targetset, ref_indexes, target_indexes)
         return distmatrix
 
     def threshold_matched(self, distmatrix):
-        """ Return the matched elements within a dictionnary,
+        """Return the matched elements within a dictionnary,
         each key being the indice from X, and the corresponding
         values being a list of couple (indice from Y, distance)
         """
         match = defaultdict(list)
         if self.normalize_matrix:
             distmatrix /= distmatrix.max()
         ind = (distmatrix <= self.threshold).nonzero()
         indrow = ind[0].tolist()
         indcol = ind[1].tolist()
-        for (i, j) in zip(indrow, indcol):
+        for i, j in zip(indrow, indcol):
             match[i].append((j, distmatrix[i, j]))
         return match
 
     def _get_match(self, refset, targetset, ref_indexes=None, target_indexes=None):
         # Build items
         ref_indexes = ref_indexes or range(len(refset))
         target_indexes = target_indexes or range(len(targetset))
@@ -124,15 +122,15 @@
         # Reapply matched to global indexes
         new_matched = {}
         for k, values in matched.items():
             new_matched[ref_indexes[k]] = [(target_indexes[i], d) for i, d in values]
         return mat, new_matched
 
     def align(self, refset, targetset, get_matrix=True):
-        """ Perform the alignment on the referenceset
+        """Perform the alignment on the referenceset
         and the targetset
         """
         start_time = time.time()
         refset = self.apply_normalization(refset, self.ref_normalizer)
         targetset = self.apply_normalization(targetset, self.target_normalizer)
         self.refset_size = len(refset)
         self.targetset_size = len(targetset)
@@ -157,16 +155,15 @@
                     if get_matrix:
                         # XXX avoid issue in sparse matrix
                         global_mat[k, v] = d or 10 ** (-10)
         self.time = time.time() - start_time
         return global_mat, global_matched
 
     def get_aligned_pairs(self, refset, targetset, unique=True, use_distance=True):
-        """ Get the pairs of aligned elements
-        """
+        """Get the pairs of aligned elements"""
         if not refset or not targetset:
             return
         global_mat, global_matched = self.align(refset, targetset, get_matrix=use_distance)
         for refitem, targetitem, distance in iter_aligned_pairs(
             refset, targetset, global_mat, global_matched, unique
         ):
             self.pairs_found += 1
@@ -181,15 +178,15 @@
         target_indexes=None,
         ref_encoding=None,
         target_encoding=None,
         ref_separator="\t",
         target_separator="\t",
         get_matrix=True,
     ):
-        """ Align data from files
+        """Align data from files
 
         Parameters
         ----------
 
         reffile: name of the reference file
 
         targetfile: name of the target file
@@ -220,67 +217,67 @@
         target_indexes=None,
         ref_encoding=None,
         target_encoding=None,
         ref_separator="\t",
         target_separator="\t",
         unique=True,
     ):
-        """ Get the pairs of aligned elements
-        """
+        """Get the pairs of aligned elements"""
         refset = parsefile(
             reffile, indexes=ref_indexes, encoding=ref_encoding, delimiter=ref_separator
         )
         targetset = parsefile(
             targetfile, indexes=target_indexes, encoding=target_encoding, delimiter=target_separator
         )
         if not refset or not targetset:
             return
         global_mat, global_matched = self.align(refset, targetset, get_matrix=False)
         yield from iter_aligned_pairs(refset, targetset, global_mat, global_matched, unique)
 
     def log_infos(self):
-        """ Display some info on the aligner process
-        """
+        """Display some info on the aligner process"""
         self.logger.info("Computation time : %s" % self.time)
         self.logger.info("Size reference set : %s" % self.refset_size)
         self.logger.info("Size target set : %s" % self.targetset_size)
+        self.logger.info("Comparisons maximum : %s" % (self.refset_size * self.targetset_size))
         self.logger.info("Comparisons done : %s" % self.nb_comparisons)
-        self.logger.info("Alignments done : %s" % self.alignments_done)
-        self.logger.info("Pairs found : %s" % self.pairs_found)
+        self.logger.info("Number of blocks : %s" % self.nb_blocks)
         self.logger.info(
-            "Ratio reference set/alignments done : %s"
-            % (self.alignments_done / float(self.refset_size))
+            "Blocking reduction : %i%%"
+            % (100 - (100 * self.nb_comparisons / float(self.refset_size * self.targetset_size)))
         )
+        if self.nb_blocks:
+            self.logger.info(
+                "Ratio comparisons/block : %.1f" % (float(self.nb_comparisons) / self.nb_blocks)
+            )
+        self.logger.info("Alignments done : %s" % self.alignments_done)
+        self.logger.info("Pairs found : %s" % self.pairs_found)
         self.logger.info(
-            "Ratio target set/alignments done : %s"
-            % (self.alignments_done / float(self.targetset_size))
+            "Ratio alignments done / reference set : %i%%"
+            % (100 * self.alignments_done / float(self.refset_size))
         )
         self.logger.info(
-            "Ratio reference set/pairs found : %s" % (self.pairs_found / float(self.refset_size))
+            "Ratio pairs found / reference set : %i%%"
+            % (100 * self.pairs_found / float(self.refset_size))
         )
         self.logger.info(
-            "Ratio target set/pairs found : %s" % (self.pairs_found / float(self.targetset_size))
+            "Ratio alignments done / target set : %i%%"
+            % (100 * self.alignments_done / float(self.targetset_size))
         )
-        self.logger.info("Maximum comparisons : %s" % (self.refset_size * self.targetset_size))
-        self.logger.info("Number of blocks : %s" % self.nb_blocks)
-        if self.nb_blocks:
-            self.logger.info(
-                "Ratio comparisons/block : %s" % (float(self.nb_comparisons) / self.nb_blocks)
-            )
         self.logger.info(
-            "Blocking reduction : %s"
-            % (self.nb_comparisons / float(self.refset_size * self.targetset_size))
+            "Ratio pairs found / target set : %i%%"
+            % (100 * self.pairs_found / float(self.targetset_size))
         )
 
 
 ###############################################################################
 # PIPELINE ALIGNER OBJECT ####################################################
 ###############################################################################
-class PipelineAligner(object):
-    """ This pipeline will perform iterative alignments, removing each time
+class PipelineAligner:
+    """This pipeline will perform iterative alignments, removing each time
     the aligned results from the previous aligner.
     """
 
     def __init__(self, aligners):
         self.aligners = aligners
         self.pairs = {}
         self.nb_comparisons = 0
@@ -289,16 +286,15 @@
         self.pairs_found = 0
         self.refset_size = None
         self.targetset_size = None
         self.time = None
         self.logger = logging.getLogger("nazca.aligner")
 
     def get_aligned_pairs(self, refset, targetset, unique=True):
-        """ Get the pairs of aligned elements
-        """
+        """Get the pairs of aligned elements"""
         if not refset or not targetset:
             return
         start_time = time.time()
         ref_index = range(len(refset))
         target_index = range(len(targetset))
         self.refset_size = len(refset)
         self.targetset_size = len(targetset)
@@ -324,39 +320,40 @@
             if ind_aligner < len(self.aligners) - 1:
                 # There are other aligners after this one
                 ref_index = [i for i in ref_index if i not in seen_refset]
         self.time = time.time() - start_time
         self.log_infos()
 
     def log_infos(self):
-        """ Display some info on the aligner process
-        """
+        """Display some info on the aligner process"""
         self.logger.info("Computation time : %s" % self.time)
         self.logger.info("Size reference set : %s" % self.refset_size)
         self.logger.info("Size target set : %s" % self.targetset_size)
+        self.logger.info("Maximum comparisons : %s" % (self.refset_size * self.targetset_size))
         self.logger.info("Comparisons done : %s" % self.nb_comparisons)
-        self.logger.info("Alignments done : %s" % self.alignments_done)
-        self.logger.info("Pairs found : %s" % self.pairs_found)
+        self.logger.info("Number of blocks : %s" % self.nb_blocks)
         self.logger.info(
-            "Ratio reference set/alignments done : %s"
-            % (self.alignments_done / float(self.refset_size))
+            "Blocking reduction : %i%%"
+            % (100 - (100 * self.nb_comparisons / float(self.refset_size * self.targetset_size)))
         )
+        if self.nb_blocks:
+            self.logger.info(
+                "Ratio comparisons/block : %.1f" % (float(self.nb_comparisons) / self.nb_blocks)
+            )
+        self.logger.info("Alignments done : %s" % self.alignments_done)
+        self.logger.info("Pairs found : %s" % self.pairs_found)
         self.logger.info(
-            "Ratio target set/alignments done : %s"
-            % (self.alignments_done / float(self.targetset_size))
+            "Ratio alignments done / reference set : %i%%"
+            % (100 * self.alignments_done / float(self.refset_size))
         )
         self.logger.info(
-            "Ratio reference set/pairs found : %s" % (self.pairs_found / float(self.refset_size))
+            "Ratio pairs found / reference set : %i%%"
+            % (100 * self.pairs_found / float(self.refset_size))
         )
         self.logger.info(
-            "Ratio target set/pairs found : %s" % (self.pairs_found / float(self.targetset_size))
+            "Ratio alignments done / target set : %i%%"
+            % (100 * self.alignments_done / float(self.targetset_size))
         )
-        self.logger.info("Maximum comparisons : %s" % (self.refset_size * self.targetset_size))
-        self.logger.info("Number of blocks : %s" % self.nb_blocks)
-        if self.nb_blocks:
-            self.logger.info(
-                "Ratio comparisons/block : %s" % (float(self.nb_comparisons) / self.nb_blocks)
-            )
         self.logger.info(
-            "Blocking reduction : %s"
-            % (self.nb_comparisons / float(self.refset_size * self.targetset_size))
+            "Ratio pairs found / target set : %i%%"
+            % (100 * self.pairs_found / float(self.targetset_size))
         )
```

### Comparing `nazca-2.0.2/nazca/rl/blocking.py` & `nazca-3.0.0/nazca/rl/blocking.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -34,21 +33,21 @@
 from nazca.utils.minhashing import Minlsh
 from nazca.utils.distances import soundexcode
 
 
 ###############################################################################
 # GENERAL BLOCKING ############################################################
 ###############################################################################
-class BaseBlocking(object):
-    """ An abstract general blocking object that exposes
+class BaseBlocking:
+    """An abstract general blocking object that exposes
     the API that should be common to all blockings object
     """
 
     def __init__(self, ref_attr_index, target_attr_index):
-        """ Build the blocking object
+        """Build the blocking object
 
         Parameters
         ----------
 
         ref_attr_index: index of the attribute of interest in a record
                         for the reference dataset
                         (i.e. attribute to be used for key computation)
@@ -63,81 +62,79 @@
         self.targetids = None
         self.is_fitted = False
 
     def _fit(self, refset, targetset):
         raise NotImplementedError
 
     def _iter_blocks(self):
-        """ Internal iteration function over blocks
-        """
+        """Internal iteration function over blocks"""
         raise NotImplementedError
 
     def _cleanup(self):
-        """ Internal cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Internal cleanup blocking for further use (e.g. in pipeline)"""
         raise NotImplementedError
 
     def fit(self, refset, targetset):
-        """ Fit the blocking technique on the reference and target datasets
+        """Fit the blocking technique on the reference and target datasets
 
         Parameters
         ----------
         refset: a dataset (list of records)
 
         targetset: a dataset (list of records)
         """
         self._fit(refset, targetset)
         # Keep ids for blocks building
         self.refids = [(i, r[0]) for i, r in enumerate(refset)]
         self.targetids = [(i, r[0]) for i, r in enumerate(targetset)]
         self.is_fitted = True
 
     def iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and contains the pair (index, id) of the record in the
                           corresponding dataset.
         """
         assert self.is_fitted
         return self._iter_blocks()
 
     def iter_indice_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and contains the indexes of the record in the
                           corresponding dataset.
         """
         assert self.is_fitted
         for block1, block2 in self._iter_blocks():
             yield [r[0] for r in block1], [r[0] for r in block2]
 
     def iter_id_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and contains the ids of the record in the
                           corresponding dataset.
         """
         assert self.is_fitted
         for block1, block2 in self._iter_blocks():
             yield [r[1] for r in block1], [r[1] for r in block2]
 
     def iter_pairs(self):
-        """ Iterator over the different possible pairs.
+        """Iterator over the different possible pairs.
 
         Returns
         -------
 
         (pair1, pari2): The pairs are always ((ind_reference, id_reference),
                                               (ind_target, id_target))
                         and are the ids of the record in the corresponding dataset.
@@ -145,213 +142,203 @@
         assert self.is_fitted
         for block1, block2 in self.iter_blocks():
             for val1 in block1:
                 for val2 in block2:
                     yield val1, val2
 
     def iter_indice_pairs(self):
-        """ Iterator over the different possible pairs.
+        """Iterator over the different possible pairs.
 
         Returns
         -------
 
         (pair1, pari2): The pairs are always (ind_reference, ind_target)
                         and are the ids of the record in the corresponding dataset.
         """
         assert self.is_fitted
         for block1, block2 in self.iter_indice_blocks():
             for val1 in block1:
                 for val2 in block2:
                     yield val1, val2
 
     def iter_id_pairs(self):
-        """ Iterator over the different possible pairs.
+        """Iterator over the different possible pairs.
 
         Returns
         -------
 
         (pair1, pari2): The pairs are always (id_reference, id_target)
                         and are the ids of the record in the corresponding dataset.
         """
         assert self.is_fitted
         for block1, block2 in self.iter_id_blocks():
             for val1 in block1:
                 for val2 in block2:
                     yield val1, val2
 
     def cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.is_fitted = True
         self._cleanup()
 
 
 ###############################################################################
 # KEY BLOCKING ################################################################
 ###############################################################################
 class KeyBlocking(BaseBlocking):
-    """ This blocking technique is based on a a blocking criteria
+    """This blocking technique is based on a a blocking criteria
     (or blocking key), that will be used to divide the datasets.
 
     The main idea here is:
 
     1 - to create an index of f(x) for each x in the reference set.
 
     2 - to create an index of f(y) for each y in the target set.
 
     3 - to iterate on each distinct value of f(x) and to return
         the identifiers of the records of the both sets for this value.
     """
 
     def __init__(self, ref_attr_index, target_attr_index, callback, ignore_none=False):
-        super(KeyBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.callback = callback
         self.ignore_none = ignore_none
         self.reference_index = {}
         self.target_index = {}
 
     def _fit(self, refset, targetset):
-        """ Fit a dataset in an index using the callback
-        """
+        """Fit a dataset in an index using the callback"""
         for ind, rec in enumerate(refset):
             key = self.callback(rec[self.ref_attr_index])
             if not key and self.ignore_none:
                 continue
             self.reference_index.setdefault(key, []).append((ind, rec[0]))
         for ind, rec in enumerate(targetset):
             key = self.callback(rec[self.target_attr_index])
             if not key and self.ignore_none:
                 continue
             self.target_index.setdefault(key, []).append((ind, rec[0]))
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and containts the indexes of the record in the
                           corresponding dataset.
         """
         for key, block1 in self.reference_index.items():
             block2 = self.target_index.get(key)
             if block1 and block2:
                 yield (block1, block2)
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.reference_index = {}
         self.target_index = {}
 
 
 class SoundexBlocking(KeyBlocking):
     def __init__(
-        self, ref_attr_index, target_attr_index, language="french",
+        self,
+        ref_attr_index,
+        target_attr_index,
+        language="french",
     ):
-        super(SoundexBlocking, self).__init__(
-            ref_attr_index, target_attr_index, partial(soundexcode, language=language)
-        )
+        super().__init__(ref_attr_index, target_attr_index, partial(soundexcode, language=language))
 
 
 ###############################################################################
 # BIGRAM BLOCKING #############################################################
 ###############################################################################
 class NGramBlocking(BaseBlocking):
-    """ This blocking technique is based on a a n-gram key.
-    """
+    """This blocking technique is based on a a n-gram key."""
 
     def __init__(self, ref_attr_index, target_attr_index, ngram_size=2, depth=2):
-        super(NGramBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.ngram_size = ngram_size
         self.depth = depth
         self.reference_index = {}
         self.target_index = {}
 
     def _fit_dataset(self, dataset, cur_index, attr_index):
-        """ Fit a dataset
-        """
+        """Fit a dataset"""
         for ind, r in enumerate(dataset):
             cur_dict = cur_index
             text = r[attr_index]
             for i in range(self.depth):
                 ngram = text[i * self.ngram_size : (i + 1) * self.ngram_size]
                 if i < self.depth - 1:
                     cur_dict = cur_dict.setdefault(ngram, {})
             cur_dict.setdefault(ngram, []).append((ind, r[0]))
 
     def _fit(self, refset, targetset):
-        """ Fit the two sets (reference set and target set)
-        """
+        """Fit the two sets (reference set and target set)"""
         self._fit_dataset(refset, self.reference_index, self.ref_attr_index)
         self._fit_dataset(targetset, self.target_index, self.target_attr_index)
 
     def _iter_dict(self, ref_cur_dict, target_cur_dict):
-        """ Iterative function used to create blocks from dicts
-        """
+        """Iterative function used to create blocks from dicts"""
         for key, sub_dict in ref_cur_dict.items():
             if key in target_cur_dict:
                 if isinstance(sub_dict, dict):
                     # There is another dict layer
-                    for block1, block2 in self._iter_dict(sub_dict, target_cur_dict[key]):
-                        yield block1, block2
+                    yield from self._iter_dict(sub_dict, target_cur_dict[key])
                 else:
                     # This is a list
                     yield sub_dict, target_cur_dict[key]
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and containts the indexes of the record in the
                           corresponding dataset.
         """
         for block1, block2 in self._iter_dict(self.reference_index, self.target_index):
             if block1 and block2:
                 yield block1, block2
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.reference_index = {}
         self.target_index = {}
 
 
 ###############################################################################
 # SORTKEY BLOCKING ############################################################
 ###############################################################################
 class SortedNeighborhoodBlocking(BaseBlocking):
-    """ This blocking technique is based on a a sorting blocking criteria
+    """This blocking technique is based on a a sorting blocking criteria
     (or blocking key), that will be used to divide the datasets.
     """
 
     def __init__(self, ref_attr_index, target_attr_index, key_func=lambda x: x, window_width=20):
-        super(SortedNeighborhoodBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.key_func = key_func
         self.window_width = window_width
         self.sorted_dataset = None
 
     def _fit(self, refset, targetset):
-        """ Fit a dataset in an index using the callback
-        """
+        """Fit a dataset in an index using the callback"""
         self.sorted_dataset = [
             ((ind, r[0]), r[self.ref_attr_index], 0) for ind, r in enumerate(refset)
         ]
         self.sorted_dataset.extend(
             [((ind, r[0]), r[self.target_attr_index], 1) for ind, r in enumerate(targetset)]
         )
         self.sorted_dataset.sort(key=lambda x: self.key_func(x[1]))
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
-        """
+        """Iterator over the different possible blocks."""
         for ind, (rid, record, dset) in enumerate(self.sorted_dataset):
             # Only keep reference set record
             if dset == 1:
                 continue
             block1 = [
                 rid,
             ]
@@ -359,24 +346,23 @@
             minind = minind if minind >= 0 else 0
             maxind = ind + self.window_width + 1
             block2 = [ri for ri, re, d in self.sorted_dataset[minind:maxind] if d == 1]
             if block1 and block2:
                 yield (block1, block2)
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.sorted_dataset = None
 
 
 ###############################################################################
 # MERGE BLOCKING ##############################################################
 ###############################################################################
 class MergeBlocking(BaseBlocking):
-    """ This blocking technique keep only one appearance of one given values,
+    """This blocking technique keep only one appearance of one given values,
     and removes all the other records having this value.
     The merge is based on a score function
 
     E.g.
       ('http://fr.wikipedia.org/wiki/Paris_%28Texas%29', 'Paris', 25898)
       ('http://fr.wikipedia.org/wiki/Paris', 'Paris', 12223100)
 
@@ -384,38 +370,36 @@
 
       ('http://fr.wikipedia.org/wiki/Paris', 'Paris', 12223100)
 
     !!! WARNING !!! This is only done on ONE set (the one with a non null attr index)
     """
 
     def __init__(self, ref_attr_index, target_attr_index, score_func):
-        super(MergeBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.score_func = score_func
         self.merged_dataset = None
         self.other_dataset = None
         if ref_attr_index is None and target_attr_index is None:
             raise ValueError(
                 "At least one of ref_attr_index or target_attr_index " "should not be None"
             )
 
     def _fit(self, refset, targetset):
-        """ Fit a dataset in an index using the callback
-        """
+        """Fit a dataset in an index using the callback"""
         if self.ref_attr_index is not None:
             # Merge refset
             self.merged_dataset = self._merge_dataset(refset, self.ref_attr_index)
             self.other_dataset = [(ind, r[0]) for ind, r in enumerate(targetset)]
         else:
             # Merge targetset
             self.merged_dataset = self._merge_dataset(targetset, self.target_attr_index)
             self.other_dataset = [(ind, r[0]) for ind, r in enumerate(refset)]
 
     def _merge_dataset(self, dataset, attr_index):
-        """ Merge a dataset
-        """
+        """Merge a dataset"""
         merged_dataset_dict = {}
         for ind, record in enumerate(dataset):
             score = self.score_func(record)
             if record[attr_index] not in merged_dataset_dict:
                 # Create new entry
                 merged_dataset_dict[record[attr_index]] = (ind, record, score)
             elif (
@@ -423,51 +407,52 @@
                 and merged_dataset_dict[record[attr_index]][2] < score
             ):
                 # Change current score
                 merged_dataset_dict[record[attr_index]] = (ind, record, score)
         return [(ind, r[0]) for ind, r, score in merged_dataset_dict.values()]
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
-        """
+        """Iterator over the different possible blocks."""
         if self.ref_attr_index is not None:
             yield self.merged_dataset, self.other_dataset
         else:
             # self.target_attr_index is not None
             yield self.other_dataset, self.merged_dataset
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.merged_dataset = None
         self.other_dataset = None
 
 
 ###############################################################################
 # CLUSTERING-BASED BLOCKINGS ##################################################
 ###############################################################################
 class KmeansBlocking(BaseBlocking):
-    """ A blocking technique based on Kmeans
-    """
+    """A blocking technique based on Kmeans"""
 
     def __init__(self, ref_attr_index, target_attr_index, n_clusters=None):
-        super(KmeansBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.n_clusters = n_clusters
         self.kmeans = None
         self.predicted = None
         from sklearn import cluster
 
         self.cluster_class = cluster.KMeans
 
     def _fit(self, refset, targetset):
-        """ Fit the reference dataset.
-        """
+        """Fit the reference dataset."""
         # If an element is None (missing), use instead the identity element.
         # The identity element is defined as the 0-vector
-        idelement = tuple([0,] * len(refset[0][self.ref_attr_index]))
+        idelement = tuple(
+            [
+                0,
+            ]
+            * len(refset[0][self.ref_attr_index])
+        )
         # We assume here that there are at least 2 elements in the refset
         n_clusters = self.n_clusters or (len(refset) // 10 or len(refset) // 2)
         try:
             kmeans = self.cluster_class(n_clusters=n_clusters)
         except TypeError:
             # Try older API version of sklearn
             kmeans = self.cluster_class(k=n_clusters)
@@ -475,15 +460,15 @@
         self.kmeans = kmeans
         # Predict on targetset
         self.predicted = self.kmeans.predict(
             [elt[self.target_attr_index] or idelement for elt in targetset]
         )
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and containts the indexes of the record in the
                           corresponding dataset.
@@ -495,37 +480,34 @@
         for ind, li in enumerate(self.kmeans.labels_):
             neighbours[li][0].append(self.refids[ind])
         for block1, block2 in neighbours:
             if len(block1) and len(block2):
                 yield block1, block2
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.kmeans = None
         self.predicted = None
 
 
 ###############################################################################
 # KDTREE BLOCKINGS ############################################################
 ###############################################################################
 class KdTreeBlocking(BaseBlocking):
-    """ A blocking technique based on KdTree
-    """
+    """A blocking technique based on KdTree"""
 
     def __init__(self, ref_attr_index, target_attr_index, threshold=0.1):
-        super(KdTreeBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.threshold = threshold
         self.reftree = None
         self.targettree = None
         self.nb_elements = None
 
     def _fit(self, refset, targetset):
-        """ Fit the blocking
-        """
+        """Fit the blocking"""
         firstelement = refset[0][self.ref_attr_index]
         self.nb_elements = len(refset)
         idsize = len(firstelement) if isinstance(firstelement, (tuple, list)) else 1
         idelement = (0,) * idsize
         # KDTree is expecting a two-dimensional array
         if idsize == 1:
             self.reftree = KDTree([(elt[self.ref_attr_index],) or idelement for elt in refset])
@@ -535,15 +517,15 @@
         else:
             self.reftree = KDTree([elt[self.ref_attr_index] or idelement for elt in refset])
             self.targettree = KDTree(
                 [elt[self.target_attr_index] or idelement for elt in targetset]
             )
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and containts the indexes of the record in the
                           corresponding dataset.
@@ -559,78 +541,75 @@
             _target = [self.targetids[v] for v in extraneighbours[ind]]
             neighbours.append((_ref, _target))
         for block1, block2 in neighbours:
             if len(block1) and len(block2):
                 yield block1, block2
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.reftree = None
         self.targettree = None
         self.nb_elements = None
 
 
 ###############################################################################
 # MINHASHING BLOCKINGS ########################################################
 ###############################################################################
 class MinHashingBlocking(BaseBlocking):
-    """ A blocking technique based on MinHashing
-    """
+    """A blocking technique based on MinHashing"""
 
     # This is the random seed to be used to computed the hash functions, when
     # the user wants repeatable results.
     FIXED_RANDOM_SEED = "4; chosen by fair dice roll. Guaranteed to be random."
 
     def __init__(
         self,
         ref_attr_index,
         target_attr_index,
         threshold=0.1,
         kwordsgram=1,
         siglen=200,
         repeatable=False,
     ):
-        """ Specific parameters of the MinHashingBlocking:
+        """Specific parameters of the MinHashingBlocking:
 
         :param kwordsgram: is the length of the k-wordgrams used
             (the lower k is, the faster is the training)
         :param siglen: the length of the sentences signature
         :param repeatable: whether a fixed random seed should be used or not.
             Using a fixed random seed allows to have repeatable results.
         """
 
-        super(MinHashingBlocking, self).__init__(ref_attr_index, target_attr_index)
+        super().__init__(ref_attr_index, target_attr_index)
         self.threshold = threshold
         self.kwordsgram = kwordsgram
         self.siglen = siglen
         self._repeatable = repeatable
         self.minhasher = self._get_new_minhasher()
         self.nb_elements = None
 
     def _get_new_minhasher(self):
         if self._repeatable:
             return Minlsh(random_seed=self.FIXED_RANDOM_SEED)
         return Minlsh()
 
     def _fit(self, refset, targetset):
-        """ Find the blocking using minhashing
-        """
+        """Find the blocking using minhashing"""
         # If an element is None (missing), use instead the identity element.
         idelement = ""
         self.minhasher.train(
             [elt[self.ref_attr_index] or idelement for elt in refset]
             + [elt[self.target_attr_index] or idelement for elt in targetset],
             self.kwordsgram,
             self.siglen,
         )
         self.nb_elements = len(refset)
 
     def _iter_blocks(self):
-        """ Iterator over the different possible blocks.
+        """Iterator over the different possible blocks.
 
         Returns
         -------
 
         (block1, block2): The blocks are always (reference_block, target_block)
                           and containts the indexes of the record in the
                           corresponding dataset.
@@ -647,46 +626,44 @@
             if len(neighbours[-1][0]) == 0 or len(neighbours[-1][1]) == 0:
                 neighbours.pop()
         for block1, block2 in neighbours:
             if len(block1) and len(block2):
                 yield block1, block2
 
     def _cleanup(self):
-        """ Cleanup blocking for further use (e.g. in pipeline)
-        """
+        """Cleanup blocking for further use (e.g. in pipeline)"""
         self.minhasher = self._get_new_minhasher()
         self.nb_elements = None
 
 
 ###############################################################################
 # BLOCKING PIPELINE ###########################################################
 ###############################################################################
 class PipelineBlocking(BaseBlocking):
-    """ Pipeline multiple blocking techniques
-    """
+    """Pipeline multiple blocking techniques"""
 
     def __init__(self, blockings, collect_stats=False):
-        """ Build the blocking object
+        """Build the blocking object
 
         Parameters
         ----------
 
         blockings: ordered list of blocking objects
         """
         self.blockings = blockings
         self.stored_blocks = []
         self.collect_stats = collect_stats
         self.stats = {}
 
     def _fit(self, refset, targetset):
-        """ Internal fit of the pipeline """
+        """Internal fit of the pipeline"""
         self._recursive_fit(refset, targetset, range(len(refset)), range(len(targetset)), 0)
 
     def _recursive_fit(self, refset, targetset, ref_index, target_index, ind):
-        """ Recursive fit of the blockings.
+        """Recursive fit of the blockings.
         Blocks are stored in the stored_blocks attribute.
         """
         if ind < len(self.blockings) - 1:
             # There are other blockings after this one
             blocking = self.blockings[ind]
             blocking.cleanup()
             blocking.fit([refset[i] for i in ref_index], [targetset[i] for i in target_index])
@@ -705,12 +682,11 @@
                 ind_block1 = [(ref_index[i], _id) for i, _id in block1]
                 ind_block2 = [(target_index[i], _id) for i, _id in block2]
                 if self.collect_stats:
                     self.stats.setdefault(ind, []).append((len(block1), len(block2)))
                 self.stored_blocks.append((ind_block1, ind_block2))
 
     def _iter_blocks(self):
-        """ Internal iteration function over blocks
-        """
+        """Internal iteration function over blocks"""
         for block1, block2 in self.stored_blocks:
             if block1 and block2:
                 yield block1, block2
```

### Comparing `nazca-2.0.2/nazca/utils/dataio.py` & `nazca-3.0.0/nazca/utils/dataio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -14,16 +13,14 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import codecs
 import json
 import csv
-import urllib
-from urllib.request import urlopen
 from os.path import exists as fileexists
 from os import path as osp
 
 from lxml import etree
 
 try:
     from SPARQLWrapper import SPARQLWrapper, JSON
@@ -33,15 +30,15 @@
     SPARQL_ENABLED = False
 
 
 ###############################################################################
 # UTILITY FUNCTIONS ###########################################################
 ###############################################################################
 def autocast(data, encoding=None):
-    """ Try to convert data into a specific type
+    """Try to convert data into a specific type
     in (int, float, str)
     """
     try:
         return int(data)
     except ValueError:
         try:
             return float(data.replace(",", "."))
@@ -49,71 +46,18 @@
             data = data.strip()
             if encoding and isinstance(data, bytes):
                 return data.decode(encoding)
             return data
 
 
 ###############################################################################
-# RQL FUNCTIONS ###############################################################
-###############################################################################
-def get_cw_cnx(endpoint):
-    """ Get a cnx on a CubicWeb database
-    """
-    from cubicweb import dbapi
-    from cubicweb.__pkginfo__ import numversion
-    from cubicweb.cwconfig import CubicWebConfiguration
-
-    CubicWebConfiguration.load_cwctl_plugins()
-    config = CubicWebConfiguration.config_for(endpoint)
-    if numversion < (3, 19):
-        sourceinfo = config.sources()["admin"]
-    else:
-        sourceinfo = config.default_admin_config
-    login = sourceinfo["login"]
-    password = sourceinfo["password"]
-    _, cnx = dbapi.in_memory_repo_cnx(config, login, password=password)
-    req = cnx.request()
-    return req
-
-
-def rqlquery(host, rql, indexes=None, formatopt=None, autocast_data=True, _cache_cnx={}, **kwargs):
-    """ Run the rql query on the given cubicweb host
-    Additional arguments can be passed to be properly substitued
-    in the execute() function for appid accces.
-    """
-    if host.startswith("http://"):
-        # By url
-        if host.endswith("/"):
-            host = host[:-1]
-        indexes = indexes or []
-        filehandle = urlopen(
-            "%(host)s/view?"
-            "rql=%(rql)s&vid=csvexport" % {"rql": urllib.parse.quote(rql), "host": host}
-        )
-        filehandle.readline()  # Skip the first line
-        lines = (line.decode("utf-8") for line in filehandle)
-        return parsefile(
-            lines, delimiter=";", indexes=indexes, formatopt=formatopt, autocast_data=autocast_data
-        )
-    else:
-        # By appid
-        if host in _cache_cnx:
-            cnx = _cache_cnx[host]
-        else:
-            cnx = get_cw_cnx(host)
-            _cache_cnx[host] = cnx
-        return cnx.execute(rql, kwargs)
-
-
-###############################################################################
 # SPARQL FUNCTIONS ############################################################
 ###############################################################################
 def _sparqlexecute(endpoint, query, raise_on_error=False, agent=None):
-    """ Execute a sparql query and return the raw results
-    """
+    """Execute a sparql query and return the raw results"""
     if not SPARQL_ENABLED:
         raise ImportError(
             "You have to install SPARQLWrapper and JSON modules to used this function"
         )
     if agent:
         sparql = SPARQLWrapper(endpoint, agent=agent)
     else:
@@ -134,45 +78,43 @@
         else:
             return []
 
 
 def sparqlquery(
     endpoint, query, indexes=None, autocast_data=True, raise_on_error=False, agent=None
 ):
-    """ Run the sparql query on the given endpoint, and wrap the items in the
+    """Run the sparql query on the given endpoint, and wrap the items in the
     indexes form. If indexes is empty, keep raw output"""
     results = []
     rawresults = _sparqlexecute(endpoint, query, raise_on_error, agent)
     if not rawresults:
         return results
     labels = rawresults["head"]["vars"]
     indexes = indexes or []
     if autocast_data:
         transform = autocast
     else:
-
-        def transform(x):
-            return x
+        transform = lambda x: x
 
     for raw in rawresults["results"]["bindings"]:
         data = []
         if not indexes:
-            data = [transform(raw[label]["value"]) for label in labels]
+            data = [(transform(raw[label]["value"]) if label in raw else None) for label in labels]
         else:
             for il, ind in enumerate(indexes):
                 if isinstance(ind, tuple):
                     data.append(tuple([transform(raw[labels[i]]["value"]) for i in ind]))
                 else:
                     data.append(transform(raw[labels[il]]["value"]))
         results.append(data)
     return results
 
 
 def sparqljson(endpoint, query, lang_order=("fr", "en"), raise_on_error=False, agent=None):
-    """ Execute and format the results of a sparql query.
+    """Execute and format the results of a sparql query.
     Sort the litterals using lang_order.
     """
     data = {}
     rawresults = _sparqlexecute(endpoint, query, raise_on_error, agent)
     if not rawresults:
         return data
     results = rawresults["results"]["bindings"]
@@ -188,15 +130,15 @@
             else:
                 # Literal - Use lang
                 data_lang.setdefault(k, []).append((v["value"], v.get("xml:lang")))
 
     def keyfunc(x):
         return lang_order.index(x[1]) if x[1] in lang_order else len(lang_order)
 
-    data.update(dict([(k, sorted(v, key=keyfunc)[0][0]) for k, v in data_lang.items()]))
+    data.update({k: sorted(v, key=keyfunc)[0][0] for k, v in data_lang.items()})
     return data
 
 
 ###############################################################################
 # FILE FUNCTIONS ##############################################################
 ###############################################################################
 def parsefile(
@@ -205,46 +147,46 @@
     nbmax=None,
     delimiter="\t",
     encoding="utf-8",
     field_size_limit=None,
     autocast_data=True,
     formatopt=None,
 ):
-    """ Parse the file (read ``nbmax`` line at maximum if given). Each
-        line is splitted according ``delimiter`` and only ``indexes`` are kept
+    """Parse the file (read ``nbmax`` line at maximum if given). Each
+    line is splitted according ``delimiter`` and only ``indexes`` are kept
 
-        eg : The file is :
-                1, house, 12, 19, apple
-                2, horse, 21.9, 19, stramberry
-                3, flower, 23, 2.17, cherry
-
-            >>> data = parsefile('myfile', [0, (2, 3), 4, 1], delimiter=',')
-            data = [[1, (12, 19), u'apple', u'house'],
-                    [2, (21.9, 19), u'stramberry', u'horse'],
-                    [3, (23, 2.17), u'cherry', u'flower']]
-
-            By default, all cells are "autocast" (thanks to the
-            ``autocast()`` function), but you can overpass it thanks to the
-            ``formatopt`` dictionnary. Each key is the index to work on, and the
-            value is the function to call. See the following example:
-
-            >>> data = parsefile('myfile', [0, (2, 3), 4, 1], delimiter=',',
-            >>>                  formatopt={2:lambda x:x.decode('utf-8')})
-            data = [[1, (u'12', 19), u'apple', u'house'],
-                    [2, (u'21.9', 19), u'stramberry', u'horse'],
-                    [3, (u'23', 2.17), u'cherry', u'flower']]
+    eg : The file is :
+            1, house, 12, 19, apple
+            2, horse, 21.9, 19, stramberry
+            3, flower, 23, 2.17, cherry
+
+        >>> data = parsefile('myfile', [0, (2, 3), 4, 1], delimiter=',')
+        data = [[1, (12, 19), u'apple', u'house'],
+                [2, (21.9, 19), u'stramberry', u'horse'],
+                [3, (23, 2.17), u'cherry', u'flower']]
+
+        By default, all cells are "autocast" (thanks to the
+        ``autocast()`` function), but you can overpass it thanks to the
+        ``formatopt`` dictionnary. Each key is the index to work on, and the
+        value is the function to call. See the following example:
+
+        >>> data = parsefile('myfile', [0, (2, 3), 4, 1], delimiter=',',
+        >>>                  formatopt={2:lambda x:x.decode('utf-8')})
+        data = [[1, (u'12', 19), u'apple', u'house'],
+                [2, (u'21.9', 19), u'stramberry', u'horse'],
+                [3, (u'23', 2.17), u'cherry', u'flower']]
 
     """
 
     def formatedoutput(filename):
         if field_size_limit:
             csv.field_size_limit(field_size_limit)
 
         if isinstance(filename, str):
-            csvfile = open(filename, "r")
+            csvfile = open(filename)
         else:
             csvfile = filename
         reader = csv.reader(csvfile, delimiter=delimiter)
         for row in reader:
             yield [cell.strip() for cell in row]
         csvfile.close()
 
@@ -281,38 +223,45 @@
                     data.append(None)
 
         result.append(data)
     return result
 
 
 def write_results(matched, alignset, targetset, resultfile):
-    """ Given a matched dictionnay, an alignset and a targetset to the
-        resultfile
+    """Given a matched dictionnay, an alignset and a targetset to the
+    resultfile
     """
     openmode = "a" if fileexists(resultfile) else "w"
     with open(resultfile, openmode) as fobj:
         if openmode == "w":
             fobj.write("aligned;targetted;distance\n")
         for aligned in matched:
             for target, dist in matched[aligned]:
                 alignid = alignset[aligned][0]
                 targetid = targetset[target][0]
-                fobj.write("%s;%s;%s\n" % (alignid, targetid, dist,))
+                fobj.write(
+                    "%s;%s;%s\n"
+                    % (
+                        alignid,
+                        targetid,
+                        dist,
+                    )
+                )
 
 
 def split_file(filename, outputdir, nblines=60000):
-    """ Split `filename` into smaller files of ``nblines`` lines. Files are
-        written into `outputdir`.
+    """Split `filename` into smaller files of ``nblines`` lines. Files are
+    written into `outputdir`.
 
-        Return the list of files
+    Return the list of files
     """
     NEW = object()
 
     def readlines(fobj, nblines):
-        """ yield all lines of the file, and
+        """yield all lines of the file, and
         at split-file boundaries, yield a NEW marker
         """
         for index, line in enumerate(fobj):
             if index and index % nblines == 0:
                 yield NEW
             yield line
 
@@ -330,22 +279,21 @@
         count += 1
     return list(map(str, range(count)))
 
 
 ###############################################################################
 # OUTPUT UTILITIES ############################################################
 ###############################################################################
-class AbstractPrettyPrint(object):
-    """ Pretty print the output of a named entities process
-    """
+class AbstractPrettyPrint:
+    """Pretty print the output of a named entities process"""
 
     def pprint_text(self, text, named_entities, **kwargs):
         newtext = ""
         indice = 0
-        tindices = dict([(t.start, (uri, t)) for uri, p, t in named_entities])
+        tindices = {t.start: (uri, t) for uri, p, t in named_entities}
         while indice < len(text):
             if indice in tindices:
                 uri, t = tindices[indice]
                 words = text[t.start : t.end]
                 fragment = self.pprint_entity(uri, words, **kwargs)
                 if not self.is_valid(newtext + fragment + text[t.end :]):
                     fragment = words
@@ -353,35 +301,34 @@
                 indice = t.end
             else:
                 newtext += text[indice]
                 indice += 1
         return newtext
 
     def pprint_entity(self, uri, word, **kwargs):
-        """ Pretty print an entity """
+        """Pretty print an entity"""
         raise NotImplementedError
 
     def is_valid(self, newtext):
         """Override to check the validity of the prettified content at each
         enrichement step"""
         return True
 
 
 class HTMLPrettyPrint(AbstractPrettyPrint):
-    """ Pretty print the output of a named entities process, in HTML
-    """
+    """Pretty print the output of a named entities process, in HTML"""
 
     def pprint_entity(self, uri, word, **kwargs):
-        """ Pretty print an entity """
+        """Pretty print an entity"""
         klass = ' class="%s"' % kwargs["html_class"] if "html_class" in kwargs else ""
-        return '<a href="%s"%s>%s</a>' % (uri, klass, word)
+        return '<a href="{}"{}>{}</a>'.format(uri, klass, word)
 
 
 class ValidXHTMLPrettyPrint(HTMLPrettyPrint):
-    """ Pretty print the output of a named entities process,
+    """Pretty print the output of a named entities process,
     in valid XHTML.
     """
 
     XHTML_DOC_TEMPLATE = b"""\
 <?xml version="1.0" encoding="UTF-8" ?>
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml">
@@ -393,12 +340,13 @@
 </html>"""  # noqa
 
     def is_valid(self, html):
         if isinstance(html, str):
             html = html.encode("utf-8")
         try:
             etree.fromstring(
-                self.XHTML_DOC_TEMPLATE % html, parser=etree.XMLParser(dtd_validation=True),
+                self.XHTML_DOC_TEMPLATE % html,
+                parser=etree.XMLParser(dtd_validation=True),
             )
         except etree.XMLSyntaxError:
             return False
         return True
```

### Comparing `nazca-2.0.2/nazca/utils/distances.py` & `nazca-3.0.0/nazca/utils/distances.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -32,17 +31,19 @@
 MAX_AUTOMATIC_CONFIDENCE = 0.9
 
 
 ###############################################################################
 # UTILITY FUNCTIONS ###########################################################
 ###############################################################################
 def distance_to_confidence(
-    distance, max_confidence=MAX_AUTOMATIC_CONFIDENCE, max_distance=1,
+    distance,
+    max_confidence=MAX_AUTOMATIC_CONFIDENCE,
+    max_distance=1,
 ):
-    """ Return a confidence between 0 and max_confidence based on the result of a Nazca
+    """Return a confidence between 0 and max_confidence based on the result of a Nazca
     processing
         :params distance: float (between 0 (exact match) and `max_distance`)
         :params max_confidence: the maximum confidence that can be returned.
         :params max_distance: the maximal distance that be used as input
             (usually 1, when a normalisation is used)
         :return: the confidence (float)
     """
@@ -53,15 +54,15 @@
     distance_callback,
     refset,
     targetset,
     matrix_normalized=False,
     ref_indexes=None,
     target_indexes=None,
 ):
-    """ Compute the metric matrix, given two datasets and a metric
+    """Compute the metric matrix, given two datasets and a metric
 
     Parameters
     ----------
     refset: a dataset (list of records)
 
     targetset: a dataset (list of records)
 
@@ -82,29 +83,29 @@
                 if matrix_normalized:
                     d = 1 - (1.0 / (1.0 + d))
             distmatrix[i, j] = d
     return distmatrix
 
 
 def _handlespaces(stra, strb, distance, tokenizer=None, **kwargs):
-    """ Compute the matrix of distances between all tokens of stra and strb
-        (with function ``distance``). Extra args are given to the distance
-        function
+    """Compute the matrix of distances between all tokens of stra and strb
+    (with function ``distance``). Extra args are given to the distance
+    function
 
-        The distance returned is defined as the max of the min of each rows of
-        each distance matrix, see the example above :
+    The distance returned is defined as the max of the min of each rows of
+    each distance matrix, see the example above :
 
-                 |  Victor |  Hugo                  Victor | Jean | Hugo
-         Victor  |     0   |    5           Victor |  0    |  6   |  5
-          Jean   |     6   |    4           Hugo   |  5    |  4   |  0
-          Hugo   |     5   |    0
+             |  Victor |  Hugo                  Victor | Jean | Hugo
+     Victor  |     0   |    5           Victor |  0    |  6   |  5
+      Jean   |     6   |    4           Hugo   |  5    |  4   |  0
+      Hugo   |     5   |    0
 
-                 --> 4                                --> 0
+             --> 4                                --> 0
 
-        Return 4
+    Return 4
     """
 
     if " " not in stra:
         stra += " "
     if " " not in strb:
         strb += " "
 
@@ -126,34 +127,32 @@
     return max(minlist)
 
 
 ###############################################################################
 # NUMERICAL DISTANCES #########################################################
 ###############################################################################
 def euclidean(a, b):
-    """ Simple euclidian distance
-    """
+    """Simple euclidian distance"""
     try:
         return abs(a - b)
     except TypeError:
         # a and b may be strings
         return abs(float(a) - float(b))
 
 
 ###############################################################################
 # STRING DISTANCES ############################################################
 ###############################################################################
 def exact_match(a, b):
-    """ The simplest distance, defined as 0 if both values are equal, 1 elsewise.
-    """
+    """The simplest distance, defined as 0 if both values are equal, 1 elsewise."""
     return 0 if a == b else 1
 
 
 def levenshtein(stra, strb, tokenizer=None):
-    """ Compute the Levenshtein distance between stra and strb.
+    """Compute the Levenshtein distance between stra and strb.
 
     The Levenshtein distance is defined as the minimal cost to transform stra
     into strb, where 3 operators are allowed :
         - Replace one character of stra into a character of strb
         - Add one character of strb into stra
         - Remove one character of strb
 
@@ -173,23 +172,23 @@
             addcost = thisrow[y - 1] + 1
             subcost = onerowago[y - 1] + (stra[x] != strb[y])
             thisrow[y] = min(delcost, addcost, subcost)
     return thisrow[lenb - 1]
 
 
 def soundexcode(word, language="french"):
-    """ Return the Soundex code of the word ``word``
-        For more information about soundex code see wiki_
+    """Return the Soundex code of the word ``word``
+    For more information about soundex code see wiki_
 
-        ``language`` can be 'french' or 'english'
+    ``language`` can be 'french' or 'english'
 
-        .:: wiki_ : https://en.wikipedia.org/wiki/Soundex
+    .:: wiki_ : https://en.wikipedia.org/wiki/Soundex
 
-        If spaces are found in stra or strb, this method returns
-            _handlespaces(stra, strb), soundex, language=language)
+    If spaces are found in stra or strb, this method returns
+        _handlespaces(stra, strb), soundex, language=language)
     """
 
     vowels = "AEHIOUWY"
     if language.lower() == "french":
         consonnantscode = {
             "B": "1",
             "P": "1",
@@ -264,51 +263,51 @@
     # Replace according to the codes
     code = code[0] + "".join([consonnantscode[c] for c in code[1:]])
     # First four letters, completed by zeros
     return code[:4] + "0" * (4 - len(code))
 
 
 def soundex(stra, strb, language="french", tokenizer=None):
-    """ Return the 1/0 distance between the soundex code of stra and strb.
-        0 means they have the same code, 1 they don't
+    """Return the 1/0 distance between the soundex code of stra and strb.
+    0 means they have the same code, 1 they don't
     """
     if " " in stra or " " in strb:
         return _handlespaces(stra, strb, soundex, tokenizer=tokenizer, language=language)
     return 0 if (soundexcode(stra, language) == soundexcode(strb, language)) else 1
 
 
 def jaccard(stra, strb, tokenizer=None):
-    r""" Return the jaccard distance between stra and strb, condering the tokens
-        set of stra and strb. If no tokenizer is given, it use if
-        alignement.normalize.tokenize's default one.
+    r"""Return the jaccard distance between stra and strb, condering the tokens
+    set of stra and strb. If no tokenizer is given, it use if
+    alignement.normalize.tokenize's default one.
 
-        J(A, B) = (A \cap B)/(A \cup B)
-        d(A, B) = 1 - J(A, B)
+    J(A, B) = (A \cap B)/(A \cup B)
+    d(A, B) = 1 - J(A, B)
     """
     seta = set(tokenize(stra, tokenizer))
     setb = set(tokenize(strb, tokenizer))
     return generic_jaccard(seta, setb)
 
 
 def generic_jaccard(seta, setb):
-    r""" Return the jaccard distance between two sets A and B.
+    r"""Return the jaccard distance between two sets A and B.
 
-        J(A, B) = (A \cap B)/(A \cup B)
-        d(A, B) = 1 - J(A, B)
+    J(A, B) = (A \cap B)/(A \cup B)
+    d(A, B) = 1 - J(A, B)
 
-        special case: if A and B are emtpy, return 1.
+    special case: if A and B are emtpy, return 1.
     """
     try:
         return 1.0 - 1.0 * len(seta.intersection(setb)) / len(seta.union(setb))
     except ZeroDivisionError:
         return 1.0
 
 
 def difflib_match(stra, strb):
-    """ Approximate matching.
+    """Approximate matching.
     Extract of SequenceMatched documentation
     '[...] The basic algorithm predates, and is a little fancier than, an algorithm
     published in the late 1980's by Ratcliff and Obershelp under the
     hyperbolic name "gestalt pattern matching"[...]'
 
     A value smaller than 0.4 means that sequences are close matches (we take
     1 - difflib.SequenceMatched)
@@ -318,16 +317,16 @@
 
 ###############################################################################
 # TEMPORAL DISTANCES ##########################################################
 ###############################################################################
 if DATEUTIL_ENABLED:
 
     class FrenchParserInfo(dateparser.parserinfo):
-        """ Inherit of the dateutil.parser.parserinfo and translate the english
-            dependant variables into french.
+        """Inherit of the dateutil.parser.parserinfo and translate the english
+        dependant variables into french.
         """
 
         HMS = [
             ("h", "heure", "heures"),
             ("m", "minute", "minutes"),
             ("s", "seconde", "seconde"),
         ]
@@ -356,24 +355,24 @@
             ("Sam", "Samedi"),
             ("Dim", "Dimanche"),
         ]
 
     def temporal(
         stra, strb, granularity="days", parserinfo=FrenchParserInfo, dayfirst=True, yearfirst=False
     ):
-        """ Return the distance between two strings (read as dates).
+        """Return the distance between two strings (read as dates).
 
-            ``granularity`` can be either ``days`` or ``months`` or ``years``
-            (be careful to the plural form !)
-            ``language`` can be either french or english
+        ``granularity`` can be either ``days`` or ``months`` or ``years``
+        (be careful to the plural form !)
+        ``language`` can be either french or english
 
-            ``dayfirst`` and ``yearfirst`` are used in case of ambiguity, for
-            instance 09/09/09, by default it assumes it's day/month/year
+        ``dayfirst`` and ``yearfirst`` are used in case of ambiguity, for
+        instance 09/09/09, by default it assumes it's day/month/year
 
-            Neither stra nor strb can have accent. Clean it before.
+        Neither stra nor strb can have accent. Clean it before.
         """
 
         datea = dateparser.parse(stra, parserinfo=parserinfo(dayfirst, yearfirst), fuzzy=True)
         dateb = dateparser.parse(strb, parserinfo=parserinfo(dayfirst, yearfirst), fuzzy=True)
         diff = datea - dateb
         if granularity.lower() == "years":
             return abs(diff.days / 365.25)
@@ -382,24 +381,24 @@
         return abs(diff.days)
 
 
 ###############################################################################
 # GEOGRAPHICAL DISTANCES ######################################################
 ###############################################################################
 def geographical(pointa, pointb, in_radians=False, planet_radius=6371009, units="m"):
-    """ Return the geographical distance between two points.
+    """Return the geographical distance between two points.
 
-        Both points must be tuples (latitude, longitude)
+    Both points must be tuples (latitude, longitude)
 
-        - in_radians is True, if latitude and longitude are in radians, false
-          otherwise
-        - planetRadius is the planet's radius in meters. By default, it's the
-          Earth'one.
+    - in_radians is True, if latitude and longitude are in radians, false
+      otherwise
+    - planetRadius is the planet's radius in meters. By default, it's the
+      Earth'one.
 
-        - `units` can be 'm' (meters) or 'km' (kilometers)
+    - `units` can be 'm' (meters) or 'km' (kilometers)
     """
     if units not in ("m", "km"):
         raise ValueError("unsupported units, should be in m or km")
     pointa = (float(pointa[0]), float(pointa[1]))
     pointb = (float(pointb[0]), float(pointb[1]))
 
     difflat = pointa[0] - pointb[0]
@@ -408,33 +407,33 @@
 
     if not in_radians:
         difflat *= pi / 180.0
         difflong *= pi / 180.0
         meanlat *= pi / 180.0
 
     coef = 1.0 if units == "m" else 0.001
-    return coef * planet_radius * sqrt(difflat ** 2 + (cos(meanlat) * difflong) ** 2)
+    return coef * planet_radius * sqrt(difflat**2 + (cos(meanlat) * difflong) ** 2)
 
 
 ###############################################################################
 # BASE PROCESSING ########################################################
 ###############################################################################
-class BaseProcessing(object):
-    """ A processing object used to provide an abstraction over the different
-    distance functions, and help building Nazca process. """
+class BaseProcessing:
+    """A processing object used to provide an abstraction over the different
+    distance functions, and help building Nazca process."""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         distance_callback=euclidean,
         weight=1,
         matrix_normalized=False,
     ):
-        """ Initiate the BaseProcessing
+        """Initiate the BaseProcessing
 
         Parameters
         ----------
 
         ref_attr_index: index of the attribute of interest in a record
                         for the reference dataset
                         (i.e. attribute to be used for key computation)
@@ -458,38 +457,38 @@
         self.ref_attr_index = ref_attr_index
         self.target_attr_index = target_attr_index
         self.distance_callback = distance_callback
         self.weight = weight
         self.matrix_normalized = matrix_normalized
 
     def build_record(self, record, index):
-        """ Allow to have ref_attr_index and target_attr_index to be couple
-        of index for (latitude, longitude) """
+        """Allow to have ref_attr_index and target_attr_index to be couple
+        of index for (latitude, longitude)"""
         if isinstance(index, tuple) and len(index) == 2:
             return (record[index[0]], record[index[1]])
         else:
             return record[index] if index is not None else record
 
     def distance(self, reference_record, target_record):
-        """ Compute the distance between two records
+        """Compute the distance between two records
 
         Parameters
         ----------
         reference_record: a record (tuple/list of values) of the reference dataset.
 
         target_record: a record (tuple/list of values) of the target dataset.
 
         """
         return self.distance_callback(
             self.build_record(reference_record, self.ref_attr_index),
             self.build_record(target_record, self.target_attr_index),
         )
 
     def cdist(self, refset, targetset, ref_indexes=None, target_indexes=None):
-        """ Compute the metric matrix, given two datasets and a metric
+        """Compute the metric matrix, given two datasets and a metric
 
         Parameters
         ----------
         refset: a dataset (list of records)
 
         targetset: a dataset (list of records)
 
@@ -505,15 +504,15 @@
             targetset,
             matrix_normalized=self.matrix_normalized,
             ref_indexes=ref_indexes,
             target_indexes=target_indexes,
         )
 
     def pdist(self, dataset):
-        """ Compute the upper triangular matrix in a way similar
+        """Compute the upper triangular matrix in a way similar
         to scipy.spatial.metric
 
         Parameters
         ----------
         dataset: a dataset (list of records)
 
         Returns
@@ -535,124 +534,115 @@
         return values
 
 
 ###############################################################################
 # CONCRETE PROCESSINGS ###################################################
 ###############################################################################
 class ExactMatchProcessing(BaseProcessing):
-    """ A processing based on the exact match (1 if a==b, 0 elsewise)
-    """
+    """A processing based on the exact match (1 if a==b, 0 elsewise)"""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         tokenizer=None,
         weight=1,
         matrix_normalized=False,
     ):
-        super(ExactMatchProcessing, self).__init__(
-            ref_attr_index, target_attr_index, exact_match, weight, matrix_normalized
-        )
+        super().__init__(ref_attr_index, target_attr_index, exact_match, weight, matrix_normalized)
 
 
 class LevenshteinProcessing(BaseProcessing):
-    """ A processing based on the levenshtein distance.
-    """
+    """A processing based on the levenshtein distance."""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         tokenizer=None,
         weight=1,
         matrix_normalized=False,
     ):
         distance_callback = partial(levenshtein, tokenizer=tokenizer)
-        super(LevenshteinProcessing, self).__init__(
+        super().__init__(
             ref_attr_index, target_attr_index, distance_callback, weight, matrix_normalized
         )
 
 
 class GeographicalProcessing(BaseProcessing):
-    """ A processing based on the geographical distance.
-    """
+    """A processing based on the geographical distance."""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         in_radians=False,
         planet_radius=6371009,
         units="m",
         weight=1,
         matrix_normalized=False,
     ):
         distance_callback = partial(
             geographical, in_radians=in_radians, planet_radius=planet_radius, units=units
         )
-        super(GeographicalProcessing, self).__init__(
+        super().__init__(
             ref_attr_index, target_attr_index, distance_callback, weight, matrix_normalized
         )
 
 
 class SoundexProcessing(BaseProcessing):
-    """ A processing based on the soundex distance.
-    """
+    """A processing based on the soundex distance."""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         tokenizer=None,
         weight=1,
         language="french",
         matrix_normalized=False,
     ):
         distance_callback = partial(soundex, language=language, tokenizer=tokenizer)
-        super(SoundexProcessing, self).__init__(
+        super().__init__(
             ref_attr_index, target_attr_index, distance_callback, weight, matrix_normalized
         )
 
 
 class JaccardProcessing(BaseProcessing):
-    """ A processing based on the jaccard distance.
-    """
+    """A processing based on the jaccard distance."""
 
     def __init__(
         self,
         ref_attr_index=None,
         target_attr_index=None,
         tokenizer=None,
         weight=1,
         matrix_normalized=False,
     ):
         distance_callback = partial(jaccard, tokenizer=tokenizer)
-        super(JaccardProcessing, self).__init__(
+        super().__init__(
             ref_attr_index, target_attr_index, distance_callback, weight, matrix_normalized
         )
 
 
 class DifflibProcessing(BaseProcessing):
-    """ A processing based on the difflib distance.
-    """
+    """A processing based on the difflib distance."""
 
     def __init__(
         self, ref_attr_index=None, target_attr_index=None, weight=1, matrix_normalized=False
     ):
-        super(DifflibProcessing, self).__init__(
+        super().__init__(
             ref_attr_index, target_attr_index, difflib_match, weight, matrix_normalized
         )
 
 
 if DATEUTIL_ENABLED:
 
     class TemporalProcessing(BaseProcessing):
-        """ A processing based on the temporal distance.
-        """
+        """A processing based on the temporal distance."""
 
         def __init__(
             self,
             ref_attr_index=None,
             target_attr_index=None,
             granularity="days",
             parserinfo=FrenchParserInfo,
@@ -664,10 +654,10 @@
             distance_callback = partial(
                 temporal,
                 granularity=granularity,
                 parserinfo=parserinfo,
                 dayfirst=dayfirst,
                 yearfirst=yearfirst,
             )
-            super(TemporalProcessing, self).__init__(
+            super().__init__(
                 ref_attr_index, target_attr_index, distance_callback, weight, matrix_normalized
             )
```

### Comparing `nazca-2.0.2/nazca/utils/minhashing.py` & `nazca-3.0.0/nazca/utils/minhashing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -22,34 +21,33 @@
 from scipy.optimize import bisect
 
 
 ###############################################################################
 # UTILITY FUNCTIONS ###########################################################
 ###############################################################################
 def randomhashfunction(zr, randint=random.randint):
-    """ Return a random hash function, mapping x in Z to ZR
-        h:x -> ax + b mod R
+    """Return a random hash function, mapping x in Z to ZR
+    h:x -> ax + b mod R
 
-        :param randint_function: a function that returns a random integer
-        in range [a, b], including both end points. If this function is not
-        given, the randint function from the standard random module is used.
+    :param randint_function: a function that returns a random integer
+    in range [a, b], including both end points. If this function is not
+    given, the randint function from the standard random module is used.
     """
     bound = max(zr - 1, 1)
     a = randint(1, bound)
     b = randint(1, bound)
 
     def hashfunc(x):
         return (a * x + b) % zr
 
     return hashfunc
 
 
 def count_vectorizer_func(sentences, min_n, max_n):
-    """ Perform a tokenization using scikit learn
-    """
+    """Perform a tokenization using scikit learn"""
     import sklearn
     import sklearn.feature_extraction.text as sklt
 
     skversion = tuple(int(x) for x in sklearn.__version__.split(".")[:2])
     if skversion < (0, 11):
         word_ngram = sklt.WordNGramAnalyzer(min_n=min_n, max_n=max)
         count_vec = sklt.CountVectorizer(analyzer=word_ngram)
@@ -61,20 +59,19 @@
     data = count_vec.fit_transform(sentences).tolil()
     return [list(row) for row in data.rows], data.shape
 
 
 ###############################################################################
 # MINHASHING ##################################################################
 ###############################################################################
-class Minlsh(object):
-    """ Operate minhashing + locally-sensitive-hashing to find similar sentences
-    """
+class Minlsh:
+    """Operate minhashing + locally-sensitive-hashing to find similar sentences"""
 
     def __init__(self, tokenizer_func=None, random_seed=None, verbose=False):
-        """ Initialize a minhashing/lsh object
+        """Initialize a minhashing/lsh object
 
         Parameters:
         ==========
 
            * tokenizer_func is a function that take the sentences
              as argument and return the rows of the sparse matrix
              of tokens, and its shape.
@@ -91,44 +88,43 @@
         self.sigmatrix = None
         if tokenizer_func:
             # Use given tokenizer_func
             self._buildmatrixdocument = lambda x, y: tokenizer_func(x)
         self._verbose = verbose
 
     def train(self, sentences, k=2, siglen=200):
-        """ Train the minlsh on the given sentences.
+        """Train the minlsh on the given sentences.
 
-            - `k` is the length of the k-wordgrams used
-              (the lower k is, the faster is the training)
-            - `siglen` the length of the sentences signature
+        - `k` is the length of the k-wordgrams used
+          (the lower k is, the faster is the training)
+        - `siglen` the length of the sentences signature
 
         """
         rows, shape = self._buildmatrixdocument(sentences, k)
         if self._verbose:
             print("Training is done. Wait while signaturing")
         self._computesignaturematrix(rows, shape, siglen)
         self._trained = True
 
     def _iter_wordgrams(self, sentence, k):
-        """ Generator of k-wordgrams on the given sentence
-        """
+        """Generator of k-wordgrams on the given sentence"""
         words = sentence.split(" ")
         for r in range(len(words)):
             for width in range(1, k + 1):
                 if r + width <= len(words):
                     yield " ".join(words[r : r + width])
 
     def _buildmatrixdocument(self, sentences, k):
-        """ Return a sparse matrix where :
+        """Return a sparse matrix where :
 
-            - Each sentence is a column
-            - Each row is a element of the universal set
+        - Each sentence is a column
+        - Each row is a element of the universal set
 
-            Each value (r, c) is set to 1 if the element at row r is in the
-            sentence c, 0 otherwise
+        Each value (r, c) is set to 1 if the element at row r is in the
+        sentence c, 0 otherwise
 
         """
         # Use default mode
         rows, universe, sizeofuniverse = [], {}, 0
         for nb, sent in enumerate(sentences):
             row = []
             for w in self._iter_wordgrams(sent, k):
@@ -138,18 +134,18 @@
             rows.append(row)
             if self._verbose and nb % 50000 == 0:
                 print(nb)
 
         return rows, (len(rows), sizeofuniverse)
 
     def _computesignaturematrix(self, rows, shape, siglen):
-        """ Return a matrix where each column is the signature the document
-            The signature is composed of `siglen` numbers
+        """Return a matrix where each column is the signature the document
+        The signature is composed of `siglen` numbers
 
-            The more the documents have rows in commun, the closer they are.
+        The more the documents have rows in commun, the closer they are.
         """
 
         nrows, ncols = shape
         sig = np.empty((siglen, nrows))
         # Generate the random hash functions
         minlsh_random = random.Random(self._random_seed)
         hashfunc = [randomhashfunction(ncols, randint=minlsh_random.randint) for _ in range(siglen)]
@@ -166,53 +162,52 @@
             sig[:, docind] = np.min(tmp[0], 1)
             docind += 1
             if self._verbose and docind % 50000 == 0:
                 print((docind * 100) / nrows)
         self.sigmatrix = sig
 
     def save(self, savefile):
-        """ Save the training into `savefile` for a future use """
+        """Save the training into `savefile` for a future use"""
 
         if not self._trained:
             print("Not trained, nothing to save")
             return
 
         with open(savefile, "wb") as fobj:
             pickler = pickle.Pickler(fobj)
             pickler.dump(self.sigmatrix)
 
     def load(self, savefile):
-        """ Load a trained minhashing """
+        """Load a trained minhashing"""
 
         with open(savefile, "rb") as fobj:
             pickler = pickle.Unpickler(fobj)
             self.sigmatrix = pickler.load()
 
         if self.sigmatrix is not None:
             self._trained = True
         else:
             self._trained = False
 
     def computebandsize(self, threshold, nbrows):
-        """ Compute the bandsize according to the threshold given """
+        """Compute the bandsize according to the threshold given"""
 
         # t ~ (1/b)^(1/r), where t is the threshold, b the number of
         # bands, and r the number of rows per band. And nbrows (the length
         # of the matrix is nbrows = b*r, so t ~ (r/L)^(1/r). So, let's
         # find the root of f(x) = (x/L)^(1/r) - t.
         def f(x):
             y = pow(x / nbrows, 1.0 / x) - threshold
             return y
 
         # Solve f(x) = 0, with x having values in [1, nbrows]
         return int(bisect(f, 1, nbrows))
 
     def predict(self, threshold, minclustersize=2):
-        """ Return a set of tuples of *possible* similar sentences
-        """
+        """Return a set of tuples of *possible* similar sentences"""
         if not self._trained:
             print("Train it before")
             return
 
         if not (0 < threshold <= 1):
             print("Threshold must be in ]0 ; 1]")
             return
@@ -225,9 +220,9 @@
 
         buckets = defaultdict(set)
         similars = set()
         for r in range(0, sig.shape[0], bandsize):
             buckets.clear()
             for i in range(sig.shape[1]):
                 buckets[tuple(sig[r : r + bandsize, i])].add(i)
-            similars.update(set(tuple(v) for v in buckets.values() if len(v) >= minclustersize))
+            similars.update({tuple(v) for v in buckets.values() if len(v) >= minclustersize})
         return similars
```

### Comparing `nazca-2.0.2/nazca/utils/normalize.py` & `nazca-3.0.0/nazca/utils/normalize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -16,158 +15,156 @@
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import re
 from string import punctuation
 from unicodedata import normalize as _uninormalize
 from functools import partial
 
-FRENCH_STOPWORDS = set(
-    [
-        "alors",
-        "au",
-        "aux",
-        "aucuns",
-        "aussi",
-        "autre",
-        "avant",
-        "avec",
-        "avoir",
-        "bon",
-        "car",
-        "ce",
-        "cela",
-        "ces",
-        "ceux",
-        "chaque",
-        "ci",
-        "comme",
-        "comment",
-        "dans",
-        "de",
-        "des",
-        "du",
-        "dedans",
-        "dehors",
-        "depuis",
-        "deux",
-        "devrait",
-        "doit",
-        "donc",
-        "dos",
-        "droite",
-        "début",
-        "elle",
-        "elles",
-        "en",
-        "encore",
-        "essai",
-        "est",
-        "et",
-        "eu",
-        "eux",
-        "fait",
-        "faites",
-        "fois",
-        "font",
-        "force",
-        "haut",
-        "hors",
-        "ici",
-        "il",
-        "ils",
-        "je",
-        "juste",
-        "la",
-        "le",
-        "les",
-        "leur",
-        "lui",
-        "là",
-        "ma",
-        "maintenant",
-        "mais",
-        "me",
-        "mes",
-        "moi",
-        "moins",
-        "mon",
-        "mot",
-        "même",
-        "ne",
-        "ni",
-        "nommés",
-        "nos",
-        "notre",
-        "nous",
-        "nouveaux",
-        "on",
-        "ou",
-        "où",
-        "par",
-        "parce",
-        "parole",
-        "pas",
-        "personnes",
-        "peut",
-        "peu",
-        "pièce",
-        "plupart",
-        "pour",
-        "pourquoi",
-        "quand",
-        "que",
-        "quel",
-        "quelle",
-        "quelles",
-        "quels",
-        "qui",
-        "sa",
-        "sans",
-        "se",
-        "ses",
-        "seulement",
-        "si",
-        "sien",
-        "son",
-        "sont",
-        "sous",
-        "soyez",
-        "sujet",
-        "sur",
-        "ta",
-        "tandis",
-        "tellement",
-        "te",
-        "tels",
-        "tes",
-        "toi",
-        "ton",
-        "tous",
-        "tout",
-        "trop",
-        "très",
-        "tu",
-        "un",
-        "une",
-        "valeur",
-        "voie",
-        "voient",
-        "vont",
-        "vos",
-        "votre",
-        "vous",
-        "vu",
-        "ça",
-        "étaient",
-        "état",
-        "étions",
-        "été",
-        "être",
-    ]
-)
+FRENCH_STOPWORDS = {
+    "alors",
+    "au",
+    "aux",
+    "aucuns",
+    "aussi",
+    "autre",
+    "avant",
+    "avec",
+    "avoir",
+    "bon",
+    "car",
+    "ce",
+    "cela",
+    "ces",
+    "ceux",
+    "chaque",
+    "ci",
+    "comme",
+    "comment",
+    "dans",
+    "de",
+    "des",
+    "du",
+    "dedans",
+    "dehors",
+    "depuis",
+    "deux",
+    "devrait",
+    "doit",
+    "donc",
+    "dos",
+    "droite",
+    "début",
+    "elle",
+    "elles",
+    "en",
+    "encore",
+    "essai",
+    "est",
+    "et",
+    "eu",
+    "eux",
+    "fait",
+    "faites",
+    "fois",
+    "font",
+    "force",
+    "haut",
+    "hors",
+    "ici",
+    "il",
+    "ils",
+    "je",
+    "juste",
+    "la",
+    "le",
+    "les",
+    "leur",
+    "lui",
+    "là",
+    "ma",
+    "maintenant",
+    "mais",
+    "me",
+    "mes",
+    "moi",
+    "moins",
+    "mon",
+    "mot",
+    "même",
+    "ne",
+    "ni",
+    "nommés",
+    "nos",
+    "notre",
+    "nous",
+    "nouveaux",
+    "on",
+    "ou",
+    "où",
+    "par",
+    "parce",
+    "parole",
+    "pas",
+    "personnes",
+    "peut",
+    "peu",
+    "pièce",
+    "plupart",
+    "pour",
+    "pourquoi",
+    "quand",
+    "que",
+    "quel",
+    "quelle",
+    "quelles",
+    "quels",
+    "qui",
+    "sa",
+    "sans",
+    "se",
+    "ses",
+    "seulement",
+    "si",
+    "sien",
+    "son",
+    "sont",
+    "sous",
+    "soyez",
+    "sujet",
+    "sur",
+    "ta",
+    "tandis",
+    "tellement",
+    "te",
+    "tels",
+    "tes",
+    "toi",
+    "ton",
+    "tous",
+    "tout",
+    "trop",
+    "très",
+    "tu",
+    "un",
+    "une",
+    "valeur",
+    "voie",
+    "voient",
+    "vont",
+    "vos",
+    "votre",
+    "vous",
+    "vu",
+    "ça",
+    "étaient",
+    "état",
+    "étions",
+    "été",
+    "être",
+}
 
 MANUAL_UNICODE_MAP = {
     "\xa1": "!",  # INVERTED EXCLAMATION MARK
     "\u0142": "l",  # LATIN SMALL LETTER L WITH STROKE
     "\u2044": "/",  # FRACTION SLASH
     "\xc6": "AE",  # LATIN CAPITAL LETTER AE
     "\xa9": "(c)",  # COPYRIGHT SIGN
@@ -206,33 +203,33 @@
         try:
             replacement = MANUAL_UNICODE_MAP[letter]
         except KeyError:
             if isinstance(letter, str):
                 replacement = _uninormalize("NFKD", letter)[0]
             else:
                 replacement = letter
-            if ord(replacement) >= 2 ** 7:
+            if ord(replacement) >= 2**7:
                 if substitute is None:
                     raise ValueError("can't deal with non-ascii based characters")
                 replacement = substitute
         res.append(replacement)
     return "".join(res)
 
 
 def lunormalize(sentence, substitute=None):
-    """ Normalize a sentence (ie remove accents, set to lower, etc) """
+    """Normalize a sentence (ie remove accents, set to lower, etc)"""
     return unormalize(sentence, substitute).lower()
 
 
 def simplify(sentence, lemmas=None, remove_stopwords=True, stopwords=FRENCH_STOPWORDS):
-    """ Simply the given sentence
-        0) If remove_stopwords, then remove the stop words
-        1) If lemmas are given, the sentence is lemmatized
-        2) Set the sentence to lower case
-        3) Remove punctuation
+    """Simply the given sentence
+    0) If remove_stopwords, then remove the stop words
+    1) If lemmas are given, the sentence is lemmatized
+    2) Set the sentence to lower case
+    3) Remove punctuation
     """
     if not isinstance(sentence, str):
         return sentence
 
     if lemmas:
         sentence = lemmatized(sentence, lemmas)
     sentence = sentence.lower()
@@ -243,19 +240,19 @@
     if not remove_stopwords:
         return cleansent
     else:
         return " ".join([w for w in cleansent.split(" ") if w not in stopwords])
 
 
 def tokenize(sentence, tokenizer=None, regexp=re.compile(r"[^\s]+")):
-    """ Tokenize a sentence.
-        Use ``tokenizer`` if given, else try to use the nltk WordPunctTokenizer,
-        in case of failure, it just split on spaces.
+    """Tokenize a sentence.
+    Use ``tokenizer`` if given, else try to use the nltk WordPunctTokenizer,
+    in case of failure, it just split on spaces.
 
-        Anyway, tokenizer must have a ``tokenize()`` method
+    Anyway, tokenizer must have a ``tokenize()`` method
     """
     if tokenizer:
         return tokenizer().tokenize(sentence)
     # XXX Unicode, could not use WorkTokenizer.
     # Instead split on whitespaces
     chunks = []
     for chunk in (t for t in regexp.findall(sentence) if t):
@@ -266,75 +263,73 @@
             chunks.append(schunks[-1])
         else:
             chunks.append(chunk)
     return chunks
 
 
 def lemmatized(sentence, lemmas, tokenizer=None):
-    """ Return the lemmatized sentence
-    """
+    """Return the lemmatized sentence"""
     tokenized_sent = tokenize(sentence, tokenizer)
     tokenized_sentformated = []
     for w in tokenized_sent:
         if w in ".,'" and len(tokenized_sentformated) > 0:
             tokenized_sentformated[-1] += w
         elif w not in punctuation:
             tokenized_sentformated.append(w)
     return " ".join([lemmatized_word(w, lemmas) for w in tokenized_sentformated])
 
 
 def lemmatized_word(word, lemmas):
-    """ Return the lemmatized word
-    """
+    """Return the lemmatized word"""
     lemma = lemmas.get(word.lower(), word)
     if "|" in lemma:
         _words = lemma.split("|")
         if word.lower() in _words:
             lemma = word.lower()
         else:
             lemma = _words[0]
     return lemma
 
 
 def roundstr(number, ndigits=0):
     """Return an unicode string of ``number`` rounded to a given precision
-        in decimal digits (default 0 digits)
+    in decimal digits (default 0 digits)
 
-        If ``number`` is not a float, this method casts it to a float. (An
-        exception may be raised if it's not possible)
+    If ``number`` is not a float, this method casts it to a float. (An
+    exception may be raised if it's not possible)
     """
     return format(round(float(number), ndigits), "0.%df" % ndigits)
 
 
 def rgxformat(string, regexp, output):
-    r""" Apply the regexp to the ``string`` and return a formatted string
+    r"""Apply the regexp to the ``string`` and return a formatted string
     according to ``output``
 
     eg :
         format(u'[Victor Hugo - 26 fev 1802 / 22 mai 1885]',
                r'\[(?P<firstname>\w+) (?p<lastname>\w+) - '
                r'(?P<birthdate>.*?) / (?<deathdate>.*?)\]',
                u'%(lastname)s, %(firstname)s (%(birthdate)s -'
                u'%(deathdate)s)')
 
      would return u'Hugo, Victor (26 fev 1802 - 22 mai 1885)'
-     """
+    """
     match = re.match(regexp, string)
     return output % match.groupdict()
 
 
 ###############################################################################
 # NORMALIZER OBJECTS ##########################################################
 ###############################################################################
-class BaseNormalizer(object):
-    """ A normalizer object used to provide an abstraction over the different
-    normalization functions, and help building Nazca process. """
+class BaseNormalizer:
+    """A normalizer object used to provide an abstraction over the different
+    normalization functions, and help building Nazca process."""
 
     def __init__(self, callback, attr_index=None):
-        """ Initiate the BaseNormalizer
+        """Initiate the BaseNormalizer
 
         Parameters
         ----------
         callback: normalization callback
 
         attr_index: index of the attribute of interest in a record
                     (i.e. attribute to be normalized).
@@ -347,15 +342,15 @@
         self.callback = callback
         if attr_index is not None:
             self.attr_index = attr_index if isinstance(attr_index, (tuple, list)) else (attr_index,)
         else:
             self.attr_index = attr_index
 
     def normalize(self, record):
-        """ Normalize a record
+        """Normalize a record
 
         Parameters
         ----------
         record: a record (tuple/list of values).
 
         Returns
         -------
@@ -368,15 +363,15 @@
             for attr_ind in self.attr_index:
                 record = list(
                     r if ind != attr_ind else self.callback(r) for ind, r in enumerate(record)
                 )
             return record
 
     def normalize_dataset(self, dataset, inplace=False):
-        """ Normalize a dataset
+        """Normalize a dataset
 
         Parameters
         ----------
         dataset: a list of record (tuple/list of values).
 
         inplace: Boolean. If True, normalize the dataset in place.
 
@@ -391,69 +386,68 @@
             # Change dataset in place
             for ind, record in enumerate(dataset):
                 dataset[ind] = self.normalize(record)
         return dataset
 
 
 class UnicodeNormalizer(BaseNormalizer):
-    """ Normalizer that unormalize the unicode
+    """Normalizer that unormalize the unicode
     (i.e. replace accentuating characters by ASCII ones)
     """
 
     def __init__(self, attr_index=None, substitute=None):
         callback = partial(lunormalize, substitute=substitute)
-        super(UnicodeNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 class SimplifyNormalizer(BaseNormalizer):
-    """ Normalizer that simplify a string
-        0) If remove_stopwords, then remove the stop words
-        1) If lemmas are given, the sentence is lemmatized
-        2) Set the sentence to lower case
-        3) Remove punctuation
+    """Normalizer that simplify a string
+    0) If remove_stopwords, then remove the stop words
+    1) If lemmas are given, the sentence is lemmatized
+    2) Set the sentence to lower case
+    3) Remove punctuation
     """
 
     def __init__(self, attr_index=None, lemmas=None, remove_stopwords=True):
         callback = partial(simplify, lemmas=lemmas, remove_stopwords=remove_stopwords)
-        super(SimplifyNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 class TokenizerNormalizer(BaseNormalizer):
-    """ Normalizer that tokenize a string
-        Use ``tokenizer`` if given, else try to use the nltk WordPunctTokenizer,
-        in case of failure, it just split on spaces.
-        Anyway, tokenizer must have a ``tokenize()`` method
+    """Normalizer that tokenize a string
+    Use ``tokenizer`` if given, else try to use the nltk WordPunctTokenizer,
+    in case of failure, it just split on spaces.
+    Anyway, tokenizer must have a ``tokenize()`` method
     """
 
     def __init__(self, attr_index=None, tokenizer=None, regexp=re.compile(r"[^\s]+")):
         callback = partial(tokenize, tokenizer=tokenizer, regexp=regexp)
-        super(TokenizerNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 class LemmatizerNormalizer(BaseNormalizer):
-    """ Normalizer that lemmatize a string
-    """
+    """Normalizer that lemmatize a string"""
 
     def __init__(self, lemmas, attr_index=None, tokenizer=None):
         callback = partial(lemmatized, lemmas=lemmas, tokenizer=tokenizer)
-        super(LemmatizerNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 class RoundNormalizer(BaseNormalizer):
     """Normalizer that round a string
     Return an unicode string of ``number`` rounded to a given precision
     in decimal digits (default 0 digits)
 
     If ``number`` is not a float, this method casts it to a float. (An
     exception may be raised if it's not possible)
     """
 
     def __init__(self, attr_index=None, ndigits=0):
         callback = partial(roundstr, ndigits=ndigits)
-        super(RoundNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 class RegexpNormalizer(BaseNormalizer):
     r"""Normalizer that normalize a string based on a regexp
 
      Apply the regexp to the ``string`` and return a formatted string
     according to ``output``
@@ -466,15 +460,15 @@
                u'%(deathdate)s)')
 
      would return u'Hugo, Victor (26 fev 1802 - 22 mai 1885)'
     """
 
     def __init__(self, regexp, output, attr_index=None):
         callback = partial(rgxformat, regexp=regexp, output=output)
-        super(RegexpNormalizer, self).__init__(callback, attr_index=attr_index)
+        super().__init__(callback, attr_index=attr_index)
 
 
 ###############################################################################
 # JOIN NORMALIZER #############################################################
 ###############################################################################
 class JoinNormalizer(BaseNormalizer):
     """Normalizer that join multiple fields in only one.
@@ -482,15 +476,15 @@
     """
 
     def __init__(self, attr_indexes, join_car=", "):
         self.attr_indexes = attr_indexes
         self.join_car = join_car
 
     def normalize(self, record):
-        """ Normalize a record
+        """Normalize a record
 
         Parameters
         ----------
         record: a record (tuple/list of values).
 
         Returns
         -------
@@ -504,28 +498,27 @@
         return _record
 
 
 ###############################################################################
 # NORMALIZER PIPELINE #########################################################
 ###############################################################################
 class NormalizerPipeline(BaseNormalizer):
-    """ Pipeline of Normalizers
-    """
+    """Pipeline of Normalizers"""
 
     def __init__(self, normalizers):
-        """ Initiate the NormalizerPipeline
+        """Initiate the NormalizerPipeline
 
         Parameters
         ----------
         normalizers: list (ordered) of Normalizer
         """
         self.normalizers = normalizers
 
     def normalize(self, record):
-        """ Normalize a record
+        """Normalize a record
 
         Parameters
         ----------
         record: a record (tuple/list of values).
 
         Returns
         -------
```

### Comparing `nazca-2.0.2/nazca/utils/tokenizer.py` & `nazca-3.0.0/nazca/utils/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """ Tokenizer for sentences/words segmentation.
 """
 import collections
 import re
 
 try:
     from nltk.tokenize.punkt import PunktSentenceTokenizer
@@ -11,15 +10,15 @@
 else:
     NLTK_AVAILABLE = True
 
 Token = collections.namedtuple("Token", ["word", "start", "end", "sentence"])
 Sentence = collections.namedtuple("Sentence", ["indice", "start", "end"])
 
 
-class RichStringTokenizer(object):
+class RichStringTokenizer:
     """Tokenizer for Yams' RichString content.
 
     The tokenizer uses a variable-length sliding window, i.e. a sliding
     window yielding tokens of N words.
     """
 
     def __init__(self, text, token_min_size=1, token_max_size=3):
@@ -30,16 +29,15 @@
         self.text = text
         self.token_min_size = token_min_size
         self.token_max_size = token_max_size
 
     words_re = r"[\w@-]+"
 
     def iter_tokens(self, text):
-        """ Iterate tokens over a text
-        """
+        """Iterate tokens over a text"""
         # Compute sentences
         sentences = self.find_sentences(text)
         # Compute words
         words = [m for m in re.finditer(self.words_re, text, re.UNICODE)]
         indice = 0
         while indice < len(words):
             # Choose the current sentence of the first word
@@ -53,24 +51,20 @@
                     continue
                 normalized_word = " ".join([w.group() for w in _words]).strip()
                 yield Token(normalized_word, _words[0].start(), _words[-1].end(), current_sentence)
             indice += 1
 
     @staticmethod
     def find_sentences(text):
-        """ Find the sentences
-        """
+        """Find the sentences"""
         if not NLTK_AVAILABLE:
             raise RuntimeError("find_sentences requires NLTK to be installed")
         sentences = PunktSentenceTokenizer().span_tokenize(text)
         return [Sentence(ind, start, end) for ind, (start, end) in enumerate(sentences)]
 
     def load_text(self, text):
-        """ Load the text to be tokenized
-        """
+        """Load the text to be tokenized"""
         self.text = text
 
     def __iter__(self):
-        """ Iterator over the text given in the object instantiation
-        """
-        for t in self.iter_tokens(self.text):
-            yield t
+        """Iterator over the text given in the object instantiation"""
+        yield from self.iter_tokens(self.text)
```

### Comparing `nazca-2.0.2/nazca.egg-info/SOURCES.txt` & `nazca-3.0.0/nazca.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 CHANGELOG.md
 MANIFEST.in
-README
+README.rst
 doc.rst
 setup.py
 tox.ini
 doc/nazca-logo.svg
 examples/__init__.py
 examples/demo.py
 examples/goncourt.csv
```

### Comparing `nazca-2.0.2/setup.py` & `nazca-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 # pylint: disable=W0404,W0622,W0704,W0613
 # copyright 2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -15,15 +14,14 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """Generic Setup script, takes package info from __pkginfo__.py file.
 """
-from __future__ import absolute_import
 
 __docformat__ = "restructuredtext en"
 
 from os.path import join, dirname
 
 from setuptools import find_packages, setup
 
@@ -41,25 +39,25 @@
 license = __pkginfo__["license"]
 description = __pkginfo__["description"]
 web = __pkginfo__["web"]
 author = __pkginfo__["author"]
 author_email = __pkginfo__["author_email"]
 classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, "README")) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()]
+install_requires = ["{} {}".format(d, v and v or "").strip() for d, v in requires.items()]
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
```

### Comparing `nazca-2.0.2/test/data/file2split` & `nazca-3.0.0/test/data/file2split`

 * *Files identical despite different names*

### Comparing `nazca-2.0.2/test/test_alignment.py` & `nazca-3.0.0/test/test_alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -69,44 +68,65 @@
             ["T3", "l4", (6.25, 48.91)],
         ]
 
         ref_indexes = range(len(refset))
         target_indexes = range(len(targetset))
 
         # Compute the distance matrix on the label only (weight=1)
-        aligner = alig.BaseAligner(threshold=0.2, processings=(LevenshteinProcessing(1, 1),),)
+        aligner = alig.BaseAligner(
+            threshold=0.2,
+            processings=(LevenshteinProcessing(1, 1),),
+        )
         mat_difflib = aligner.compute_distance_matrix(
-            refset, targetset, ref_indexes, target_indexes,
+            refset,
+            targetset,
+            ref_indexes,
+            target_indexes,
         )
 
         # Compute the distance matrix on the location only (weight=1)
         aligner = alig.BaseAligner(threshold=0.2, processings=(GeographicalProcessing(2, 2),))
-        mat_geo = aligner.compute_distance_matrix(refset, targetset, ref_indexes, target_indexes,)
+        mat_geo = aligner.compute_distance_matrix(
+            refset,
+            targetset,
+            ref_indexes,
+            target_indexes,
+        )
 
         # Compute the distance matrix with label and location (same weight)
         aligner = alig.BaseAligner(
-            threshold=0.2, processings=(LevenshteinProcessing(1, 1), GeographicalProcessing(2, 2),)
+            threshold=0.2,
+            processings=(
+                LevenshteinProcessing(1, 1),
+                GeographicalProcessing(2, 2),
+            ),
         )
         mat_difflib_geo = aligner.compute_distance_matrix(
-            refset, targetset, ref_indexes, target_indexes,
+            refset,
+            targetset,
+            ref_indexes,
+            target_indexes,
         )
 
         np.testing.assert_almost_equal(mat_difflib_geo, mat_geo + mat_difflib)
 
         # Same aligner, but the processings have ≠ weights, to show that the
         # weight is taken into account in the final result
         aligner = alig.BaseAligner(
             threshold=0.2,
             processings=(
                 LevenshteinProcessing(1, 1, weight=0.8),
                 GeographicalProcessing(2, 2, weight=0.2),
             ),
         )
         mat_difflib_geo = aligner.compute_distance_matrix(
-            refset, targetset, ref_indexes, target_indexes,
+            refset,
+            targetset,
+            ref_indexes,
+            target_indexes,
         )
 
         np.testing.assert_almost_equal(mat_difflib_geo, 0.2 * mat_geo + 0.8 * mat_difflib)
 
     def test_blocking_align(self):
         refset = [
             ["V1", "label1", (6.14194444444, 48.67)],
@@ -116,15 +136,15 @@
         ]
         targetset = [
             ["T1", "labelt1", (6.17, 48.7)],
             ["T2", "labelt2", (5.3, 48.2)],
             ["T3", "labelt3", (6.25, 48.91)],
         ]
         # Creation of the aligner object
-        true_matched = set([(0, 0), (0, 2), (1, 2), (3, 1)])
+        true_matched = {(0, 0), (0, 2), (1, 2), (3, 1)}
         processings = (GeographicalProcessing(2, 2, units="km"),)
         aligner = alig.BaseAligner(threshold=30, processings=processings)
         blocking = blo.KdTreeBlocking(ref_attr_index=2, target_attr_index=2, threshold=0.3)
         blocking.fit(refset, targetset)
         predict_matched = set()
         for alignind, targetind in blocking.iter_indice_blocks():
             mat, matched = aligner._get_match(refset, targetset, alignind, targetind)
@@ -142,15 +162,15 @@
         ]
         targetset = [
             ["T1", "labelt1", (6.17, 48.7)],
             ["T2", "labelt2", (5.3, 48.2)],
             ["T3", "labelt3", (6.25, 48.91)],
         ]
         # Creation of the aligner object
-        true_matched = set([(0, 0), (0, 2), (1, 2), (3, 1)])
+        true_matched = {(0, 0), (0, 2), (1, 2), (3, 1)}
         processings = (GeographicalProcessing(2, 2, units="km"),)
         aligner = alig.BaseAligner(threshold=30, processings=processings)
         aligner.register_blocking(
             blo.KdTreeBlocking(ref_attr_index=2, target_attr_index=2, threshold=0.3)
         )
         global_mat, global_matched = aligner.align(refset, targetset)
         predict_matched = set()
```

### Comparing `nazca-2.0.2/test/test_blocking.py` & `nazca-3.0.0/test/test_blocking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -108,16 +107,16 @@
 
     def test_baseblocking_pairs(self):
         blocking = KeyBlocking(
             ref_attr_index=1, target_attr_index=1, callback=partial(soundexcode, language="english")
         )
         blocking.fit(SOUNDEX_REFSET, SOUNDEX_TARGETSET)
         pairs = list(blocking.iter_pairs())
-        ref_ind = dict((r[0], ind) for ind, r in enumerate(SOUNDEX_REFSET))
-        target_ind = dict((r[0], ind) for ind, r in enumerate(SOUNDEX_TARGETSET))
+        ref_ind = {r[0]: ind for ind, r in enumerate(SOUNDEX_REFSET)}
+        target_ind = {r[0]: ind for ind, r in enumerate(SOUNDEX_TARGETSET)}
         true_pairs = [((ref_ind[r[0]], r[0]), (target_ind[r[1]], r[1])) for r in SOUNDEX_PAIRS]
         self.assertEqual(len(pairs), len(true_pairs))
         for pair in true_pairs:
             self.assertIn(pair, pairs)
 
     def test_baseblocking_id_pairs(self):
         blocking = KeyBlocking(
@@ -132,16 +131,16 @@
 
     def test_baseblocking_indice_pairs(self):
         blocking = KeyBlocking(
             ref_attr_index=1, target_attr_index=1, callback=partial(soundexcode, language="english")
         )
         blocking.fit(SOUNDEX_REFSET, SOUNDEX_TARGETSET)
         pairs = list(blocking.iter_indice_pairs())
-        ref_ind = dict((r[0], ind) for ind, r in enumerate(SOUNDEX_REFSET))
-        target_ind = dict((r[0], ind) for ind, r in enumerate(SOUNDEX_TARGETSET))
+        ref_ind = {r[0]: ind for ind, r in enumerate(SOUNDEX_REFSET)}
+        target_ind = {r[0]: ind for ind, r in enumerate(SOUNDEX_TARGETSET)}
         true_pairs = [(ref_ind[r[0]], target_ind[r[1]]) for r in SOUNDEX_PAIRS]
         self.assertEqual(len(pairs), len(true_pairs))
         for pair in true_pairs:
             self.assertIn(pair, pairs)
 
 
 class KeyBlockingTest(unittest.TestCase):
@@ -230,16 +229,15 @@
             (["a4"], ["b3"]),
         ]
         self.assertEqual(len(blocks), len(true_blocks))
         for block in true_blocks:
             self.assertIn(block, blocks)
 
     def test_sorted_neighborhood_keyfunc(self):
-        """ Test sort reversing values
-        """
+        """Test sort reversing values"""
         blocking = SortedNeighborhoodBlocking(
             ref_attr_index=1, target_attr_index=1, key_func=lambda x: x[::-1], window_width=1
         )
         blocking.fit(SOUNDEX_REFSET, SOUNDEX_TARGETSET)
         blocks = list(blocking.iter_id_blocks())
         true_blocks = [
             (["a1"], ["b3"]),
@@ -311,20 +309,14 @@
             ["V4", "label4", (5.2, 48.1)],
         ]
         targetset = [
             ["T1", "labelt1", (6.2, 48.9)],
             ["T2", "labelt2", (5.3, 48.2)],
             ["T3", "labelt3", (6.25, 48.91)],
         ]
-        try:
-            import sklearn as skl
-        except ImportError:
-            self.skipTest("Scikit learn does not seem to be installed")
-        if int(skl.__version__.split("-")[0].split(".")[1]) <= 11:
-            self.skipTest("Scikit learn version is too old - Skipping test")
         blocking = KmeansBlocking(ref_attr_index=2, target_attr_index=2)
         blocking.fit(refset, targetset)
         # Blocks
         blocks = list(blocking.iter_indice_blocks())
         self.assertEqual(len(blocks), 2)
         self.assertIn(([0, 1], [0, 2]), blocks)
         self.assertIn(([2, 3], [1]), blocks)
```

### Comparing `nazca-2.0.2/test/test_dataio.py` & `nazca-3.0.0/test/test_dataio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -24,15 +23,14 @@
 
 from nazca.utils.dataio import (
     HTMLPrettyPrint,
     ValidXHTMLPrettyPrint,
     sparqlquery,
     sparqljson,
     _sparqlexecute,
-    rqlquery,
     parsefile,
     autocast,
     split_file,
     SPARQL_ENABLED,
 )
 from nazca.utils.tokenizer import NLTK_AVAILABLE
 from nazca.ner import NerProcess
@@ -299,21 +297,19 @@
                  dbpedia-owl:designer ?designer .
             FILTER(regex(?label, "^Python"))
             }""",
         )
         self.assertEqual(
             results,
             {
-                "designer": set(["http://dbpedia.org/resource/Guido_van_Rossum"]),
-                "uri": set(
-                    [
-                        "http://dbpedia.org/resource/Python_(programming_language)",
-                        "http://dbpedia.org/resource/Python_for_S60",
-                    ]
-                ),
+                "designer": {"http://dbpedia.org/resource/Guido_van_Rossum"},
+                "uri": {
+                    "http://dbpedia.org/resource/Python_(programming_language)",
+                    "http://dbpedia.org/resource/Python_for_S60",
+                },
             },
         )
 
     @unittest.skipUnless(SPARQL_ENABLED, "python-sparqlwrapper is not installed")
     def test_sparql_autocast(self):
         alignset = sparqlquery(
             "http://dbpedia.inria.fr/sparql",
@@ -350,16 +346,10 @@
             "} LIMIT 100",
             indexes=[0, 1, (2, 3)],
             autocast_data=False,
         )
         self.assertEqual(len(alignset), 100)
         self.assertFalse(isinstance(alignset[0][2][0], float))
 
-    def test_rqlquery(self):
-        results = rqlquery(
-            "http://www.cubicweb.org", 'Any U LIMIT 1 WHERE X cwuri U, X name "apycot"'
-        )
-        self.assertEqual(results, [["http://www.cubicweb.org/1310453"]])
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nazca-2.0.2/test/test_distances.py` & `nazca-3.0.0/test/test_distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
```

### Comparing `nazca-2.0.2/test/test_filters.py` & `nazca-3.0.0/test/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -26,18 +25,18 @@
 )
 from nazca.ner.sources import NerSourceLexicon
 from nazca.utils.tokenizer import Token, Sentence, NLTK_AVAILABLE
 
 
 @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
 class FilterTest(unittest.TestCase):
-    """ Test of filters """
+    """Test of filters"""
 
     def test_occurence_filter_min_occ(self):
-        """ Test occurence filter """
+        """Test occurence filter"""
         text = "Hello everyone, this is   me speaking. And me."
         source1 = NerSourceLexicon(
             {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         )
         source2 = NerSourceLexicon({"me": "http://example2.com/me"})
         _filter = NerOccurenceFilter(min_occ=2)
         ner = NerProcess((source1, source2), filters=(_filter,))
@@ -73,15 +72,15 @@
                         word="me", start=43, end=45, sentence=Sentence(indice=1, start=39, end=46)
                     ),
                 ),
             ],
         )
 
     def test_occurence_filter_max_occ(self):
-        """ Test occurence filter """
+        """Test occurence filter"""
         text = "Hello everyone, this is   me speaking. And me."
         source1 = NerSourceLexicon(
             {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         )
         source2 = NerSourceLexicon({"me": "http://example2.com/me"})
         _filter = NerOccurenceFilter(max_occ=1)
         ner = NerProcess((source1, source2), filters=(_filter,))
@@ -99,15 +98,15 @@
                         sentence=Sentence(indice=0, start=0, end=38),
                     ),
                 ),
             ],
         )
 
     def test_disambiguation_word_length(self):
-        """ Test occurence filter """
+        """Test occurence filter"""
         text = "Hello toto tutu. And toto."
         source = NerSourceLexicon(
             {"toto tutu": "http://example.com/toto_tutu", "toto": "http://example.com/toto"}
         )
         _filter = NerDisambiguationWordParts()
         ner = NerProcess((source,), filters=(_filter,))
         named_entities = ner.process_text(text)
@@ -131,15 +130,15 @@
                         word="toto", start=21, end=25, sentence=Sentence(indice=1, start=17, end=26)
                     ),
                 ),
             ],
         )
 
     def test_disambiguation_word_case(self):
-        """ Test occurence filter """
+        """Test occurence filter"""
         text = "Hello Toto Tutu. And Toto."
         source = NerSourceLexicon(
             {"Toto Tutu": "http://example.com/toto_tutu", "Toto": "http://example.com/toto"}
         )
         _filter = NerDisambiguationWordParts()
         ner = NerProcess((source,), filters=(_filter,))
         named_entities = ner.process_text(text)
@@ -163,15 +162,15 @@
                         word="Toto", start=21, end=25, sentence=Sentence(indice=1, start=17, end=26)
                     ),
                 ),
             ],
         )
 
     def test_rules_filter(self):
-        """ Test rules filter """
+        """Test rules filter"""
         text = "Hello toto tutu. And toto."
         source = NerSourceLexicon(
             {"toto tutu": "http://example.com/toto_tutu", "toto": "http://example.com/toto"}
         )
         rules = {"http://example.com/toto": "http://example.com/tata"}
         _filter = NerReplacementRulesFilter(rules)
         ner = NerProcess((source,), filters=(_filter,))
```

### Comparing `nazca-2.0.2/test/test_minhashing.py` & `nazca-3.0.0/test/test_minhashing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -52,14 +51,16 @@
             "J'aime les bandes dessinées de genre comiques.",
             "Pour quelle occasion vous êtes-vous apprêtée ?",
             "Je les vis ensemble à plusieurs occasions.",
             "Je les ai vus ensemble à plusieurs occasions.",
         ]
         minlsh = Minlsh(random_seed="spam eggs bacon")
         minlsh.train(
-            (simplify(s, FRENCH_LEMMAS, remove_stopwords=True) for s in sentences), 1, 200,
+            (simplify(s, FRENCH_LEMMAS, remove_stopwords=True) for s in sentences),
+            1,
+            200,
         )
-        self.assertEqual(set([(0, 1), (2, 3), (5, 6)]), minlsh.predict(0.4))
+        self.assertEqual({(0, 1), (2, 3), (5, 6)}, minlsh.predict(0.4))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `nazca-2.0.2/test/test_ner.py` & `nazca-3.0.0/test/test_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -14,48 +13,56 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import unittest
 
-from nazca.ner.sources import NerSourceLexicon, NerSourceSparql, NerSourceRql
+from nazca.ner.sources import NerSourceLexicon, NerSourceSparql
 from nazca.ner import NerProcess
 from nazca.utils.tokenizer import Token, Sentence, NLTK_AVAILABLE
 from nazca.ner.preprocessors import NerStopwordsFilterPreprocessor
 from nazca.utils.dataio import SPARQL_ENABLED
 
 
 class NerTest(unittest.TestCase):
-    """ Test of Ner """
+    """Test of Ner"""
 
     def test_lexicon_source(self):
-        """ Test lexicon source """
+        """Test lexicon source"""
         lexicon = {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         source = NerSourceLexicon(lexicon)
-        self.assertEqual(source.query_word("me"), ["http://example.com/me",])
-        self.assertEqual(source.query_word("everyone"), ["http://example.com/everyone",])
+        self.assertEqual(
+            source.query_word("me"),
+            [
+                "http://example.com/me",
+            ],
+        )
+        self.assertEqual(
+            source.query_word("everyone"),
+            [
+                "http://example.com/everyone",
+            ],
+        )
         self.assertEqual(source.query_word("me everyone"), [])
         self.assertEqual(source.query_word("toto"), [])
         # Token
         token = Token("me", 0, 2, None)
-        self.assertEqual(source.recognize_token(token), ["http://example.com/me",])
+        self.assertEqual(
+            source.recognize_token(token),
+            [
+                "http://example.com/me",
+            ],
+        )
         token = Token("ma", 0, 2, None)
         self.assertEqual(source.recognize_token(token), [])
 
-    def test_rql_source(self):
-        """ Test rql source """
-        source = NerSourceRql(
-            "http://www.cubicweb.org", 'Any U LIMIT 1 WHERE X cwuri U, X name "%(word)s"'
-        )
-        self.assertEqual(source.query_word("apycot"), ["http://www.cubicweb.org/1310453",])
-
     @unittest.skipUnless(SPARQL_ENABLED, "python-sparqlwrapper is not installed")
     def test_sparql_source(self):
-        """ Test sparql source """
+        """Test sparql source"""
         source = NerSourceSparql(
             "http://dbpedia.org/sparql",
             """\
             PREFIX dbpedia-owl:<http://dbpedia.org/ontology/>
             SELECT DISTINCT ?uri
             WHERE {
             ?uri rdf:type <http://dbpedia.org/ontology/ProgrammingLanguage> ;
@@ -70,15 +77,15 @@
                 "http://dbpedia.org/resource/Python_(programming_language)",
                 "http://dbpedia.org/resource/Python_for_S60",
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello everyone, this is   me speaking. And me."
         source = NerSourceLexicon(
             {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         )
         ner = NerProcess((source,))
         named_entities = ner.process_text(text)
         self.assertEqual(
@@ -109,15 +116,15 @@
                     ),
                 ),
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process_multisources(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello everyone, this is   me speaking. And me."
         source1 = NerSourceLexicon(
             {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         )
         source2 = NerSourceLexicon({"me": "http://example2.com/me"})
         # Two sources, not unique
         ner = NerProcess((source1, source2))
@@ -228,15 +235,15 @@
                     ),
                 ),
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process_add_sources(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello everyone, this is   me speaking. And me."
         source1 = NerSourceLexicon(
             {"everyone": "http://example.com/everyone", "me": "http://example.com/me"}
         )
         source2 = NerSourceLexicon({"me": "http://example2.com/me"})
         ner = NerProcess((source1,))
         named_entities = ner.process_text(text)
@@ -314,15 +321,15 @@
                     ),
                 ),
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process_preprocess(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello Toto, this is   me speaking. And me."
         source = NerSourceLexicon(
             {"Toto": "http://example.com/toto", "me": "http://example.com/me"}
         )
         preprocessor = NerStopwordsFilterPreprocessor()
         ner = NerProcess((source,), preprocessors=(preprocessor,))
         named_entities = ner.process_text(text)
@@ -337,21 +344,23 @@
                     ),
                 )
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process_add_preprocess(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello Toto, this is   me speaking. And me."
         source = NerSourceLexicon(
             {"Toto": "http://example.com/toto", "me": "http://example.com/me"}
         )
         preprocessor = NerStopwordsFilterPreprocessor()
-        ner = NerProcess((source,),)
+        ner = NerProcess(
+            (source,),
+        )
         named_entities = ner.process_text(text)
         self.assertEqual(
             named_entities,
             [
                 (
                     "http://example.com/toto",
                     None,
@@ -388,15 +397,15 @@
                     ),
                 )
             ],
         )
 
     @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
     def test_ner_process_chained_word(self):
-        """ Test ner process """
+        """Test ner process"""
         text = "Hello everyone me, this is   me speaking. And me."
         source = NerSourceLexicon(
             {
                 "everyone": "http://example.com/everyone",
                 "everyone me": "http://example.com/everyone_me",
                 "me": "http://example.com/me",
             }
```

### Comparing `nazca-2.0.2/test/test_normalize.py` & `nazca-3.0.0/test/test_normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -49,15 +48,24 @@
     def test_simplify(self):
         self.assertEqual(
             simplify("J'aime les frites, les pommes et les" " scoubidous !", FRENCH_LEMMAS),
             "aimer frites pomme scoubidou",
         )
 
     def test_tokenize(self):
-        self.assertEqual(tokenize("J'aime les frites !"), ["J'", "aime", "les", "frites", "!",])
+        self.assertEqual(
+            tokenize("J'aime les frites !"),
+            [
+                "J'",
+                "aime",
+                "les",
+                "frites",
+                "!",
+            ],
+        )
 
     def test_lemmatizer(self):
         self.assertEqual(lemmatized("sacré rubert", FRENCH_LEMMAS), "sacré rubert")
         self.assertEqual(lemmatized("J'aime les frites !", FRENCH_LEMMAS), "je aimer le frite")
         self.assertEqual(lemmatized(", J'aime les frites", FRENCH_LEMMAS), "je aimer le frite")
 
     def test_round(self):
@@ -127,21 +135,37 @@
             ["a1", "aimer frites pomme scoubidou"],
             normalizer.normalize(["a1", "J'aime les frites, les pommes et les scoubidous !"]),
         )
 
     def test_tokenize(self):
         normalizer = TokenizerNormalizer()
         self.assertEqual(
-            ["J'", "aime", "les", "frites", "!",], normalizer.normalize("J'aime les frites !")
+            [
+                "J'",
+                "aime",
+                "les",
+                "frites",
+                "!",
+            ],
+            normalizer.normalize("J'aime les frites !"),
         )
 
     def test_tokenize_record(self):
         normalizer = TokenizerNormalizer(attr_index=1)
         self.assertEqual(
-            ["a1", ["J'", "aime", "les", "frites", "!",]],
+            [
+                "a1",
+                [
+                    "J'",
+                    "aime",
+                    "les",
+                    "frites",
+                    "!",
+                ],
+            ],
             normalizer.normalize(["a1", "J'aime les frites !"]),
         )
 
     def test_lemmatizer(self):
         normalizer = LemmatizerNormalizer(FRENCH_LEMMAS)
         self.assertEqual(normalizer.normalize("sacré rubert"), "sacré rubert")
         self.assertEqual(normalizer.normalize("J'aime les frites !"), "je aimer le frite")
```

### Comparing `nazca-2.0.2/test/test_preprocessors.py` & `nazca-3.0.0/test/test_preprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -19,15 +18,15 @@
 import unittest
 
 from nazca.utils import tokenizer
 from nazca.ner import preprocessors
 
 
 class PreprocessorTest(unittest.TestCase):
-    """ Test of preprocessors """
+    """Test of preprocessors"""
 
     def test_lowercasefilter(self):
         preprocessor = preprocessors.NerLowerCaseFilterPreprocessor()
         token = tokenizer.Token("toto", 0, 4, None)
         self.assertEqual(preprocessor(token), None)
         token = tokenizer.Token("toto Tata", 0, 4, None)
         self.assertEqual(preprocessor(token), token)
```

### Comparing `nazca-2.0.2/test/test_tokenizer.py` & `nazca-3.0.0/test/test_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding:utf-8 -*-
 #
 # copyright 2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -19,15 +18,15 @@
 import unittest
 
 from nazca.utils.tokenizer import RichStringTokenizer, Token, Sentence, NLTK_AVAILABLE
 
 
 @unittest.skipUnless(NLTK_AVAILABLE, "nltk is not available")
 class TokenizerTest(unittest.TestCase):
-    """ Test of tokenizer """
+    """Test of tokenizer"""
 
     def test_find_sentences(self):
         text = "Hello everyone, this is   me speaking. And me."
         sentences = RichStringTokenizer.find_sentences(text)
         self.assertEqual(sentences[0], Sentence(indice=0, start=0, end=38))
         self.assertEqual(sentences[1], Sentence(indice=1, start=39, end=46))
```

### Comparing `nazca-2.0.2/tox.ini` & `nazca-3.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [testenv]
 deps =
   pytest
   nltk
   SPARQLWrapper
   mock
+  git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs:test}
 
 [testenv:flake8]
 skip_install = true
 whitelist_externals =
   flake8
@@ -20,14 +21,20 @@
 
 [testenv:black]
 skip_install = true
 deps =
   black >= 19.10b0
 commands = black --check .
 
+[testenv:black-run]
+skip_install = true
+deps =
+  black >= 19.10b0
+commands = black .
+
 [flake8]
 exclude = examples/*,test/data/*,.tox/*
 max-line-length = 100
 # those error are incompatible with black. Let's ignore them.
 extend-ignore = E203, E731, E231
 
 [pytest]
```

