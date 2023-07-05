# Comparing `tmp/freerec-0.4.1.tar.gz` & `tmp/freerec-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.4.1.tar", last modified: Sun May 28 12:32:05 2023, max compression
+gzip compressed data, was "freerec-0.4.3.tar", last modified: Wed Jul  5 13:10:09 2023, max compression
```

## Comparing `freerec-0.4.1.tar` & `freerec-0.4.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.232179 freerec-0.4.1/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     3280 2023-05-28 12:32:05.231179 freerec-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2815 2023-05-25 01:23:33.000000 freerec-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.159134 freerec-0.4.1/freerec/
--rw-rw-rw-   0        0        0      505 2023-05-28 12:06:21.000000 freerec-0.4.1/freerec/__init__.py
--rw-rw-rw-   0        0        0     4528 2023-05-25 13:17:13.000000 freerec-0.4.1/freerec/__main__.py
--rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.4.1/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.196282 freerec-0.4.1/freerec/data/
--rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/__init__.py
--rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.4.1/freerec/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.198279 freerec-0.4.1/freerec/data/datasets/
--rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.4.1/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    19752 2023-05-28 05:44:01.000000 freerec-0.4.1/freerec/data/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.200279 freerec-0.4.1/freerec/data/datasets/context/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.4.1/freerec/data/datasets/context/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/context/base.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.207344 freerec-0.4.1/freerec/data/datasets/general/
--rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/general/__init__.py
--rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.4.1/freerec/data/datasets/general/amazon.py
--rw-rw-rw-   0        0        0     3876 2023-04-26 08:41:43.000000 freerec-0.4.1/freerec/data/datasets/general/base.py
--rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.4.1/freerec/data/datasets/general/gowalla.py
--rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.4.1/freerec/data/datasets/general/movielens.py
--rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.4.1/freerec/data/datasets/general/yelp.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.209348 freerec-0.4.1/freerec/data/datasets/knowledge/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.4.1/freerec/data/datasets/knowledge/__init__.py
--rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/datasets/knowledge/base.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.213926 freerec-0.4.1/freerec/data/datasets/sequential/
--rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.4.1/freerec/data/datasets/sequential/__init__.py
--rw-rw-rw-   0        0        0    10771 2023-04-26 07:43:46.000000 freerec-0.4.1/freerec/data/datasets/sequential/amazon.py
--rw-rw-rw-   0        0        0     3037 2023-05-26 07:30:24.000000 freerec-0.4.1/freerec/data/datasets/sequential/base.py
--rw-rw-rw-   0        0        0     1756 2023-04-26 07:33:17.000000 freerec-0.4.1/freerec/data/datasets/sequential/movielens.py
--rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.4.1/freerec/data/datasets/sequential/steam.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.216926 freerec-0.4.1/freerec/data/datasets/session/
--rw-rw-rw-   0        0        0       29 2023-05-26 06:43:44.000000 freerec-0.4.1/freerec/data/datasets/session/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-05-26 07:26:22.000000 freerec-0.4.1/freerec/data/datasets/session/base.py
--rw-rw-rw-   0        0        0     1427 2023-05-28 06:05:18.000000 freerec-0.4.1/freerec/data/datasets/session/diginetica.py
--rw-rw-rw-   0        0        0     3293 2023-05-28 06:04:35.000000 freerec-0.4.1/freerec/data/datasets/session/yoochoose.py
--rw-rw-rw-   0        0        0    29845 2023-04-25 10:57:51.000000 freerec-0.4.1/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.225664 freerec-0.4.1/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0     7097 2023-05-28 11:51:29.000000 freerec-0.4.1/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0    11138 2023-05-28 11:39:12.000000 freerec-0.4.1/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    19079 2023-05-26 07:00:49.000000 freerec-0.4.1/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     3228 2023-04-10 09:00:22.000000 freerec-0.4.1/freerec/data/postprocessing/source.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.228179 freerec-0.4.1/freerec/data/preprocessing/
--rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.4.1/freerec/data/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    22062 2023-05-28 05:33:20.000000 freerec-0.4.1/freerec/data/preprocessing/base.py
--rw-rw-rw-   0        0        0    12875 2023-05-28 05:48:08.000000 freerec-0.4.1/freerec/data/preprocessing/datasets.py
--rw-rw-rw-   0        0        0      864 2023-05-25 12:55:38.000000 freerec-0.4.1/freerec/data/tags.py
--rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.4.1/freerec/data/transformation.py
--rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.4.1/freerec/data/utils.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/dict2obj.py
--rw-rw-rw-   0        0        0    31054 2023-05-28 05:17:28.000000 freerec-0.4.1/freerec/launcher.py
--rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.4.1/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.230179 freerec-0.4.1/freerec/models/
--rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.4.1/freerec/models/base.py
--rw-rw-rw-   0        0        0    16699 2023-05-12 03:00:42.000000 freerec-0.4.1/freerec/parser.py
--rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.4.1/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:32:05.190472 freerec-0.4.1/freerec.egg-info/
--rw-rw-rw-   0        0        0     3280 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 12:32:05.000000 freerec-0.4.1/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 12:32:05.232686 freerec-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-05-25 05:39:48.000000 freerec-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.355662 freerec-0.4.3/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3280 2023-07-05 13:10:09.354663 freerec-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2815 2023-05-25 01:23:33.000000 freerec-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.098570 freerec-0.4.3/freerec/
+-rw-rw-rw-   0        0        0      511 2023-07-05 13:09:15.000000 freerec-0.4.3/freerec/__init__.py
+-rw-rw-rw-   0        0        0     5574 2023-06-21 07:18:51.000000 freerec-0.4.3/freerec/__main__.py
+-rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.4.3/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.169683 freerec-0.4.3/freerec/data/
+-rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/__init__.py
+-rw-rw-rw-   0        0        0    11067 2023-07-01 02:03:38.000000 freerec-0.4.3/freerec/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.178226 freerec-0.4.3/freerec/data/datasets/
+-rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.4.3/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    20784 2023-06-30 12:03:32.000000 freerec-0.4.3/freerec/data/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.186736 freerec-0.4.3/freerec/data/datasets/context/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.4.3/freerec/data/datasets/context/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/datasets/context/base.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.236372 freerec-0.4.3/freerec/data/datasets/general/
+-rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/datasets/general/__init__.py
+-rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.4.3/freerec/data/datasets/general/amazon.py
+-rw-rw-rw-   0        0        0     3876 2023-04-26 08:41:43.000000 freerec-0.4.3/freerec/data/datasets/general/base.py
+-rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.4.3/freerec/data/datasets/general/gowalla.py
+-rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.4.3/freerec/data/datasets/general/movielens.py
+-rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.4.3/freerec/data/datasets/general/yelp.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.247515 freerec-0.4.3/freerec/data/datasets/knowledge/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.4.3/freerec/data/datasets/knowledge/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/datasets/knowledge/base.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.266342 freerec-0.4.3/freerec/data/datasets/sequential/
+-rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.4.3/freerec/data/datasets/sequential/__init__.py
+-rw-rw-rw-   0        0        0    10771 2023-04-26 07:43:46.000000 freerec-0.4.3/freerec/data/datasets/sequential/amazon.py
+-rw-rw-rw-   0        0        0     2888 2023-06-19 02:47:40.000000 freerec-0.4.3/freerec/data/datasets/sequential/base.py
+-rw-rw-rw-   0        0        0     1756 2023-04-26 07:33:17.000000 freerec-0.4.3/freerec/data/datasets/sequential/movielens.py
+-rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.4.3/freerec/data/datasets/sequential/steam.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.269348 freerec-0.4.3/freerec/data/datasets/session/
+-rw-rw-rw-   0        0        0       55 2023-05-31 03:03:02.000000 freerec-0.4.3/freerec/data/datasets/session/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-06-30 05:23:38.000000 freerec-0.4.3/freerec/data/datasets/session/base.py
+-rw-rw-rw-   0        0        0     3175 2023-06-21 06:31:56.000000 freerec-0.4.3/freerec/data/datasets/session/diginetica.py
+-rw-rw-rw-   0        0        0     6539 2023-06-21 06:44:03.000000 freerec-0.4.3/freerec/data/datasets/session/yoochoose.py
+-rw-rw-rw-   0        0        0    29927 2023-06-25 06:55:12.000000 freerec-0.4.3/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.322753 freerec-0.4.3/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0     7097 2023-05-28 11:51:29.000000 freerec-0.4.3/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0    11286 2023-06-23 03:26:35.000000 freerec-0.4.3/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    24663 2023-07-01 03:28:35.000000 freerec-0.4.3/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     3362 2023-06-29 12:54:40.000000 freerec-0.4.3/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.351662 freerec-0.4.3/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.4.3/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    26379 2023-05-31 08:29:23.000000 freerec-0.4.3/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0    16366 2023-06-21 06:11:49.000000 freerec-0.4.3/freerec/data/preprocessing/datasets.py
+-rw-rw-rw-   0        0        0      864 2023-05-25 12:55:38.000000 freerec-0.4.3/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     5969 2023-06-18 13:30:46.000000 freerec-0.4.3/freerec/data/transformation.py
+-rw-rw-rw-   0        0        0     7453 2023-06-30 02:51:22.000000 freerec-0.4.3/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0    36769 2023-07-02 01:33:38.000000 freerec-0.4.3/freerec/launcher.py
+-rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.4.3/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.353664 freerec-0.4.3/freerec/models/
+-rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.4.3/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     5672 2023-06-30 13:43:04.000000 freerec-0.4.3/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16762 2023-06-30 04:10:23.000000 freerec-0.4.3/freerec/parser.py
+-rw-rw-rw-   0        0        0    14510 2023-05-30 13:17:10.000000 freerec-0.4.3/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:10:09.123097 freerec-0.4.3/freerec.egg-info/
+-rw-rw-rw-   0        0        0     3280 2023-07-05 13:10:08.000000 freerec-0.4.3/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2023-07-05 13:10:09.000000 freerec-0.4.3/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:10:08.000000 freerec-0.4.3/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-05 13:10:08.000000 freerec-0.4.3/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-07-05 13:10:08.000000 freerec-0.4.3/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 13:10:08.000000 freerec-0.4.3/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:10:09.355662 freerec-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-05-25 05:39:48.000000 freerec-0.4.3/setup.py
```

### Comparing `freerec-0.4.1/LICENSE` & `freerec-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/PKG-INFO` & `freerec-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.4.1
+Version: 0.4.3
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freerec-0.4.1/README.md` & `freerec-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/__main__.py` & `freerec-0.4.3/freerec/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,46 +31,64 @@
         filename=args.filename
     )
 
     star4pos = args.star4pos
     kcore4user = args.kcore4user
     kcore4item = args.kcore4item
     ratios = tuple(map(int, args.ratios.split(',')))
+    days = args.days
+    strict = not args.not_strict
     
     if args.datatype == 'gen' and args.by == 'ratio':
         fields = None if args.all else (USER.name, ITEM.name)
         converter.make_general_dataset(
             star4pos=star4pos,
             kcore4user=kcore4user,
             kcore4item=kcore4item,
+            strict=strict,
             ratios=ratios,
             fields=fields
         )
-    elif args.datatype == 'seq' and args.by == 'last-two':
+    elif args.datatype == 'seq' and args.by == 'leave-one-out':
         fields = None if args.all else (USER.name, ITEM.name, TIMESTAMP.name)
         converter.make_sequential_dataset(
             star4pos=star4pos,
             kcore4user=kcore4user,
             kcore4item=kcore4item,
+            strict=strict,
             fields=fields
         )
     elif args.datatype == 'seq' and args.by == 'ratio':
         fields = None if args.all else (USER.name, ITEM.name, TIMESTAMP.name)
         converter.make_sequential_dataset_by_ratio(
             star4pos=star4pos,
             kcore4user=kcore4user,
             kcore4item=kcore4item,
+            strict=strict,
+            ratios=ratios,
+            fields=fields
+        )
+    elif args.datatype == 'sess' and args.by == 'day':
+        fields = None if args.all else (SESSION.name, ITEM.name, TIMESTAMP.name)
+        converter.make_session_dataset_by_day(
+            star4pos=star4pos,
+            kcore4user=kcore4user,
+            kcore4item=kcore4item,
+            strict=strict,
+            days=days,
             fields=fields
         )
     elif args.datatype == 'sess' and args.by == 'ratio':
         fields = None if args.all else (SESSION.name, ITEM.name, TIMESTAMP.name)
-        converter.make_session_dataset(
+        converter.make_session_dataset_by_ratio(
             star4pos=star4pos,
             kcore4user=kcore4user,
             kcore4item=kcore4item,
+            strict=strict,
+            ratios=ratios,
             fields=fields
         )
     else:
         raise ValueError(f"`{args.datatype}' type dataset cannot be made by `{args.by}'")
 
 def main():
     parser = argparse.ArgumentParser("FreeRec")
@@ -97,21 +115,29 @@
     make_parser = subparsers.add_parser("make")
     make_parser.set_defaults(func=make)
 
     make_parser.add_argument("dataset", type=str, help="dataset name")
     make_parser.add_argument("--root", type=str, default=".", help="data")
     make_parser.add_argument("--filename", type=str, default=None, help="filename of Atomic files")
 
-    make_parser.add_argument("--datatype", type=str, choices=('gen', 'seq', 'sess'), default='gen')
-    make_parser.add_argument("--by", type=str, choices=('ratio', 'last-two'), default='ratio')
+    make_parser.add_argument(
+        "--datatype", type=str, choices=('gen', 'seq', 'sess'), default='gen', 
+        help="gen: general; seq: sequential; sess: session"
+    )
+    make_parser.add_argument(
+        "--by", type=str, choices=('ratio', 'leave-one-out', 'day'), default='ratio', 
+        help="gen: ratio; seq: leave-one-out; ratio; sess: ratio, day"
+    )
 
     make_parser.add_argument("--star4pos", type=int, default=0, help="select interactions with `Rating > star4pos'")
     make_parser.add_argument("--kcore4user", type=int, default=10, help="select kcore interactions according to User")
     make_parser.add_argument("--kcore4item", type=int, default=10, help="select kcore interactions according to Item")
+    make_parser.add_argument("--not-strict", action="store_true", default=False, help="filter by kcore once if True")
     make_parser.add_argument("--ratios", type=str, default="8,1,1", help="the ratios of training|validation|test set")
+    make_parser.add_argument("--days", type=int, default=7, help="the second last days for validation and last days for test")
 
     make_parser.add_argument("--all", action="store_true", default=False, help="reserve all fields if True")
 
     args = parser.parse_args()
     args.func(args)
 
 if __name__ == "__main__":
```

### Comparing `freerec-0.4.1/freerec/criterions.py` & `freerec-0.4.3/freerec/criterions.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/base.py` & `freerec-0.4.3/freerec/data/datasets/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from typing import Iterator, Optional, TypeVar, Tuple
+from typing import Iterator, Optional, TypeVar, Tuple, List
 
 import torch, os, abc
 import numpy as np
 import torchdata.datapipes as dp
 from freeplot.utils import import_pickle, export_pickle
 
 from ..tags import FieldTags, SPARSE, USER, SESSION, ITEM, ID
@@ -179,15 +179,15 @@
                 cols
             ))
 
     def summary(self):
         """Print a summary of the dataset."""
         infoLogger(str(self))
 
-    @timemeter("DataSet/to_graph")
+    @timemeter
     def to_heterograph(self, *edge_types: Tuple[Tuple[FieldTags], Optional[str], Tuple[FieldTags]]):
         r"""
         Convert datapipe to a heterograph.
 
         Parameters:
         -----------
         *edge_types: Tuple[Tuple[str, str], Optional[str], Tuple[str, str]]
@@ -477,15 +477,15 @@
                 self.mode
             ),
             non_deterministic=False # return sorted chunks
         )
         for file_ in datapipe:
             yield self.read_pickle(file_)
 
-    @timemeter("DataSet/compile")
+    @timemeter
     def compile(self):
         r"""
         Check current dataset and transformations.
 
         Flows:
         ------
         1. Check whether the transformation has been fitted:
@@ -542,15 +542,36 @@
         if self.mode == 'train':
             return self.trainsize
         elif self.mode == 'valid':
             return self.validsize
         else:
             return self.testsize
 
-    def to_seqs(self, master: Tuple = (USER, ID), keepid: bool = False):
+    def to_pairs(self, master: Tuple = (USER, ID)) -> List:
+        r"""
+        Return dataset in pairs.
+
+        Parameters:
+        -----------
+        master: Tuple
+            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
+        
+        Returns:
+        --------
+        List
+        """
+        Master = self.fields[master]
+        assert Master is not None, f"{Master} is not in fields ..."
+        pairs = []
+
+        for chunk in self:
+            pairs.extend(list(zip(chunk[master], chunk[ITEM, ID])))
+        return pairs
+
+    def to_seqs(self, master: Tuple = (USER, ID), keepid: bool = False) -> List:
         r"""
         Return dataset in sequence.
 
         Parameters:
         -----------
         master: Tuple
             Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
@@ -575,15 +596,15 @@
         if keepid:
             seqs = [(id_, tuple(items)) for id_, items in enumerate(seqs)]
         else:
             seqs = [tuple(items) for items in seqs]
 
         return seqs
 
-    def to_roll_seqs(self, master: Tuple = (USER, ID), minlen: int = 2):
+    def to_roll_seqs(self, master: Tuple = (USER, ID), minlen: int = 2) -> List:
         r"""
         Rolling dataset in sequence.
 
         Parameters:
         -----------
         master: Tuple
             Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
@@ -601,10 +622,26 @@
             for k in range(minlen, len(items) + 1):
                 roll_seqs.append(
                     (id_, items[:k])
                 )
 
         return roll_seqs
 
+    def seqlens(self, master: Tuple = (USER, ID)) -> List:
+        seqs = self.to_seqs(master, keepid=False)
+        return list(filter(lambda x: x > 0, [len(items) for items in seqs]))
+
+    @property
+    def maxlen(self) -> int:
+        return np.max(self.seqlens()).item()
+
+    @property
+    def minlen(self) -> int:
+        return np.min(self.seqlens()).item()
+
+    @property
+    def meanlen(self) -> int:
+        return np.mean(self.seqlens()).item()
+
     def __str__(self) -> str:
         cfg = '\n'.join(map(str, self.fields))
         return f"[{self.__class__.__name__}] >>> \n" + cfg
```

### Comparing `freerec-0.4.1/freerec/data/datasets/general/amazon.py` & `freerec-0.4.3/freerec/data/datasets/general/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/general/base.py` & `freerec-0.4.3/freerec/data/datasets/general/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/general/gowalla.py` & `freerec-0.4.3/freerec/data/datasets/general/gowalla.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/general/movielens.py` & `freerec-0.4.3/freerec/data/datasets/general/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/general/yelp.py` & `freerec-0.4.3/freerec/data/datasets/general/yelp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/sequential/amazon.py` & `freerec-0.4.3/freerec/data/datasets/sequential/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/sequential/base.py` & `freerec-0.4.3/freerec/data/datasets/sequential/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,19 +63,15 @@
 
     def summary(self):
         super().summary()
         from prettytable import PrettyTable
         User, Item = self.fields[USER, ID], self.fields[ITEM, ID]
 
         table = PrettyTable(['#Users', '#Items', 'Avg.Len', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
-        trainlens =  list(filter(lambda x: x > 0, [len(items) for items in self.train().to_seqs()]))
         table.add_row([
-            User.count, Item.count, 
-            np.mean(
-                trainlens
-            ).item() + 2,
+            User.count, Item.count, self.train().meanlen + 2,
             self.trainsize + self.validsize + self.testsize,
             self.trainsize, self.validsize, self.testsize,
             (self.trainsize + self.validsize + self.testsize) / (User.count * Item.count)
         ])
 
         infoLogger(table)
```

### Comparing `freerec-0.4.1/freerec/data/datasets/sequential/movielens.py` & `freerec-0.4.3/freerec/data/datasets/sequential/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/sequential/steam.py` & `freerec-0.4.3/freerec/data/datasets/sequential/steam.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/datasets/session/base.py` & `freerec-0.4.3/freerec/data/datasets/session/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from typing import Tuple
+from typing import Tuple, List
 
 import numpy as np
 import torchdata.datapipes as dp
 
 from ..base import RecDataSet
 from ...tags import TIMESTAMP, SESSION, ITEM, ID
 from ...fields import Field, SparseField, DenseField
@@ -17,20 +17,26 @@
 
 class SessionBasedRecSet(RecDataSet):
     DATATYPE =  "Session"
 
     def check(self):
         assert isinstance(self.fields[TIMESTAMP], Field), "SessionRecSet must have `TIMESTAMP' field."
 
-    def to_seqs(self, master: Tuple = (SESSION, ID), keepid: bool = False):
+    def to_pairs(self, master: Tuple = (SESSION, ID)) -> List:
+        return super().to_pairs(master)
+
+    def to_seqs(self, master: Tuple = (SESSION, ID), keepid: bool = False) -> List:
         return super().to_seqs(master, keepid)
 
-    def to_roll_seqs(self, master: Tuple = (SESSION, ID), minlen: int = 2):
+    def to_roll_seqs(self, master: Tuple = (SESSION, ID), minlen: int = 2) -> List:
         return super().to_roll_seqs(master, minlen)
 
+    def seqlens(self, master: Tuple = (SESSION, ID)) -> List:
+        return super().seqlens(master)
+
 
 class SessionItemTimeTriplet(SessionBasedRecSet):
 
     VALID_IS_TEST = False
 
     _cfg = Config(
         fields = [
@@ -55,17 +61,17 @@
 
     def summary(self):
         super().summary()
         from prettytable import PrettyTable
         Session, Item = self.fields[SESSION, ID], self.fields[ITEM, ID]
 
         table = PrettyTable(['#Sessions', '#Items', 'Avg.Len', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
-        trainlens =  list(filter(lambda x: x > 0, [len(items) for items in self.train().to_seqs()]))
-        validlens =  list(filter(lambda x: x > 0, [len(items) for items in self.valid().to_seqs()]))
-        testlens =  list(filter(lambda x: x > 0, [len(items) for items in self.test().to_seqs()]))
+        trainlens =  self.train().seqlens()
+        validlens =  self.valid().seqlens()
+        testlens =  self.test().seqlens()
         table.add_row([
             Session.count, Item.count,
             np.mean(
                 trainlens + validlens + testlens
             ).item(),
             self.trainsize + self.validsize + self.testsize,
             self.trainsize, self.validsize, self.testsize,
```

### Comparing `freerec-0.4.1/freerec/data/datasets/session/diginetica.py` & `freerec-0.4.3/freerec/data/datasets/session/diginetica.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .base import SessionItemTimeTriplet
 
 
 __all__ = [
     'Diginetica',
     'Diginetica_250811_Chron',
     'Diginetica_250712_Chron',
+    'Diginetica_2507_Chron',
 ]
 
 
 class Diginetica(SessionItemTimeTriplet):
     ...
 
 
@@ -25,20 +26,21 @@
     kcore4user: 2
     kcore4item: 5
     star4pos: 0
     ratios: (8, 1, 1)
 
     Statistics:
     -----------
-    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
-    | #Sessions | #Items |      Avg.Len       | #Interactions | #Train | #Valid | #Test |        Density         |
-    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
-    |   204061  | 42171  | 4.8475896913177925 |     989204    | 795142 | 96445  | 97617 | 0.00011495078825064125 |
-    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
+    | #Sessions | #Items |      Avg.Len       | #Interactions | #Train | #Valid | #Test  |        Density         |
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
+    |   204061  | 42171  | 4.8475896913177925 |     989204    | 777448 | 99310  | 112446 | 0.00011495078825064125 |
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
     """
+    URL = "https://zenodo.org/record/8062815/files/Diginetica_250811_Chron.zip"
 
 
 class Diginetica_250712_Chron(SessionItemTimeTriplet):
     r"""
     Chronologically-ordered Diginetica dataset.
 
     Config:
@@ -48,8 +50,38 @@
     kcore4user: 2
     kcore4item: 5
     star4pos: 0
     ratios: (7, 1, 2)
 
     Statistics:
     -----------
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
+    | #Sessions | #Items |      Avg.Len       | #Interactions | #Train | #Valid | #Test  |        Density         |
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
+    |   204061  | 42171  | 4.8475896913177925 |     989204    | 677308 | 100140 | 211756 | 0.00011495078825064125 |
+    +-----------+--------+--------------------+---------------+--------+--------+--------+------------------------+
+    """
+    URL = "https://zenodo.org/record/8062815/files/Diginetica_250712_Chron.zip"
+
+
+class Diginetica_2507_Chron(SessionItemTimeTriplet):
+    r"""
+    Chronologically-ordered Diginetica dataset.
+
+    Config:
+    -------
+    filename: diginetica
+    dataset: Diginetica
+    kcore4user: 2
+    kcore4item: 5
+    star4pos: 0
+    days: 7
+
+    Statistics:
+    -----------
+    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
+    | #Sessions | #Items |      Avg.Len       | #Interactions | #Train | #Valid | #Test |        Density         |
+    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
+    |   204061  | 42171  | 4.8475896913177925 |     989204    | 904408 | 57262  | 27534 | 0.00011495078825064125 |
+    +-----------+--------+--------------------+---------------+--------+--------+-------+------------------------+
     """
+    URL = "https://zenodo.org/record/8062815/files/Diginetica_2507_Chron.zip"
```

### Comparing `freerec-0.4.1/freerec/data/fields.py` & `freerec-0.4.3/freerec/data/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
         if root is None:
             pass
         elif root.match(SPARSE):
             self.count = root.count
             self.add_tag(*root.tags)
         elif root.match(DENSE):
             self.add_tag(*root.tags)
+        elif isinstance(root, Field):
+            self.add_tag(*root.tags)
         else:
             raise ValueError(
                 f"root should be `None|BufferField|FieldMoudle' but {type(root)} received ..."
             )
 
     def __getitem__(self, *args, **kwargs):
         return self.data.__getitem__(*args, **kwargs)
@@ -378,16 +380,16 @@
     """
 
     def __init__(
         self, name: str, na_value: Union[str, int, float], dtype: Callable, 
         tags: Union[FieldTags, Iterable[FieldTags]] = tuple(),
         transformer: Union[str, Callable] = 'label2index'
     ):
-        assert transformer == 'label2index', "SparseField supports 'label2index' only !"
         super().__init__(name, na_value, dtype, tags, transformer)
+        assert isinstance(self.transformer, Indexer), "SparseField supports 'Indexer' only !"
         self.add_tag(SPARSE)
 
     @property
     def count(self) -> Optional[int]:
         """Return the number of classes."""
         return self.transformer.count
```

### Comparing `freerec-0.4.1/freerec/data/postprocessing/base.py` & `freerec-0.4.3/freerec/data/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/postprocessing/column.py` & `freerec-0.4.3/freerec/data/postprocessing/column.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/postprocessing/row.py` & `freerec-0.4.3/freerec/data/postprocessing/row.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         assert isinstance(indices, Iterable), \
             f"{self.__class__.__name__} requires iterable indices but {type(indices)} recevied ..."
 
         self.source = source_dp
         self.fn = fn
         self.indices = sorted(set(indices))
 
-    def _apply_fn(self, row: Union[List, Tuple]):
+    def _apply_fn(self, row: Union[List, Tuple]) -> List:
         r"""
         Apply the specified function to the elements of the row at the specified indices.
 
         Parameters:
         -----------
         row : list or tuple
             The row of data to transform.
@@ -230,15 +230,15 @@
 
         super().__init__(
             source_dp=source_dp, 
             fn=self._rprune,
             indices=indices
         )
 
-    def _rprune(self, x):
+    def _rprune(self, x: Iterable) -> Iterable:
         return x[:self.maxlen]
 
 
 @dp.functional_datapipe("drop_duplicates_")
 class DropingDuplicates(RowMapper):
     r"""
     A functional datapipe that drop the duplicates.
@@ -263,18 +263,18 @@
 
         super().__init__(
             source_dp=source_dp, 
             fn=self._drop_in_order if self.ordered else self._drop,
             indices=indices
         )
 
-    def _drop(self, x):
+    def _drop(self, x: Iterable) -> List:
         return list(set(x))
 
-    def _drop_in_order(self, x):
+    def _drop_in_order(self, x: Iterable) -> List:
         return sorted(set(x), key=x.index)
 
 
 @dp.functional_datapipe("lshift_")
 class LeftShiftingRow(RowMapper):
     r"""
     Mapper that left shifts the input data by a specified offset.
@@ -299,18 +299,18 @@
             source_dp=source_dp, 
             fn=self._lshift,
             indices=indices,
         )
 
         self.offset = offset
 
-    def _reduce(self, item):
+    def _reduce(self, item: int):
         return item - self.offset
 
-    def _lshift(self, x):
+    def _lshift(self, x: Iterable) -> List:
         return list(map(self._reduce, x))
 
 
 @dp.functional_datapipe("rshift_")
 class RightShiftingRow(RowMapper):
     r"""
     Mapper that right shifts the input data by a specified offset.
@@ -335,18 +335,18 @@
 
         super().__init__(
             source_dp=source_dp, 
             fn=self._rshift,
             indices=indices
         )
 
-    def _add(self, item):
+    def _add(self, item: int):
         return item + self.offset
 
-    def _rshift(self, x):
+    def _rshift(self, x: Iterable) -> List:
         return list(map(self._add, x))
 
 
 @dp.functional_datapipe("lpad_")
 class LeftPaddingRow(RowMapper):
     r"""
     A functional data pipeline component that left pads sequences to a maximum length.
@@ -374,15 +374,15 @@
 
         super().__init__(
             source_dp=source_dp, 
             fn=self._lpad,
             indices=indices
         )
 
-    def _lpad(self, x):
+    def _lpad(self, x: Iterable) -> List:
         return list(chain(repeat(self.padding_value, self.maxlen - len(x)), x))
 
 
 @dp.functional_datapipe("rpad_")
 class RightPaddingRow(RowMapper):
     r"""
     A functional data pipeline component that right pads sequences to a maximum length.
@@ -410,9 +410,9 @@
 
         super().__init__(
             source_dp=source_dp, 
             fn=self._rpad,
             indices=indices
         )
 
-    def _rpad(self, x):
+    def _rpad(self, x: Iterable) -> List:
         return list(chain(x, repeat(self.padding_value, self.maxlen - len(x))))
```

### Comparing `freerec-0.4.1/freerec/data/postprocessing/sampler.py` & `freerec-0.4.3/freerec/data/postprocessing/sampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,166 @@
 
 
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Iterable
 
 import random
 import torchdata.datapipes as dp
+from collections import defaultdict
 
 from .base import Postprocessor
 from ..datasets.base import RecDataSet
 from ..fields import SparseField
 from ..tags import USER, SESSION, ITEM, ID
 from ...utils import timemeter
 
 
 __all__ = [
+    'GenTrainYielder', 'GenValidYielder', 'GenTestYielder',
     'GenTrainUniformSampler', 'GenValidYielder', 'GenTestYielder',
     'SeqTrainYielder', 'SeqValidYielder', 'SeqTestYielder', 
     'SeqTrainUniformSampler', 'SeqValidSampler', 'SeqTestSampler',
     'SessTrainYielder', 'SessValidYielder', 'SessTestYielder', 
+    'SessTrainUniformSampler', 'SessValidSampler', 'SessTestSampler',
 ]
 
 
 #===============================For General Recommendation===============================
 
+
+@dp.functional_datapipe("gen_train_yielding_")
+class GenTrainYielder(Postprocessor):
+    r"""A datapipe that yields (user, item) pairs."""
+
+    def __init__(
+        self, source_dp: dp.iter.IterDataPipe,
+        dataset: RecDataSet
+    ) -> None:
+        r"""
+        Initializes a new instance of the Tripleter postprocessor.
+        
+        Parameters:
+        -----------
+        source_dp: RecDatapipe or Postprocessor 
+            A RecDatapipe or another Postprocessor that yields dicts of NumPy arrays.
+        dataset: RecDataSet 
+            The dataset that provides the data source.
+        """
+        super().__init__(source_dp)
+
+        self.User: SparseField = dataset.fields[USER, ID]
+        self.Item: SparseField = dataset.fields[ITEM, ID]
+
+        self.prepare(dataset)
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        r"""
+        Prepares the dataset by building sets of seen items for each user.
+
+        Parameters:
+        -----------
+        dataset: RecDataSet 
+            The dataset that provides the data source.
+        """
+        self.posItems = [set() for _ in range(self.User.count)]
+
+        for chunk in dataset.train():
+            self.listmap(
+                lambda user, item: self.posItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+
+        self.posItems = [tuple(items) for items in self.posItems]
+
+    def _sample_pos(self, user: int) -> int:
+        r"""
+        Randomly sample a positive item for a user.
+
+        Parameters:
+        -----------
+        user: int 
+            A user index.
+
+        Returns:
+        --------
+        positive: int 
+            A positive item that the user has interacted with.
+        """
+        return random.choice(self.posItems[user])
+
+    def _check(self, user: int) -> bool:
+        return len(self.posItems[user]) > 0
+
+    def __iter__(self):
+        for user in self.source:
+            if self._check(user):
+                yield [user, self._sample_pos(user)]
+
+
+@dp.functional_datapipe("gen_valid_yielding_")
+class GenValidYielder(GenTrainYielder):
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        self.seenItems = [set() for _ in range(self.User.count)]
+        self.unseenItems = [set() for _ in range(self.User.count)]
+
+        for chunk in dataset.train():
+            self.listmap(
+                lambda user, item: self.seenItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+        for chunk in dataset.valid():
+            self.listmap(
+                lambda user, item: self.unseenItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+
+        self.seenItems = [tuple(items) for items in self.seenItems]
+        self.unseenItems = [tuple(items) for items in self.unseenItems]
+
+    def _check(self, user: int) -> bool:
+        return len(self.unseenItems[user]) > 0
+
+    def __iter__(self):
+        for user in self.source:
+            if self._check(user):
+                yield [user, self.unseenItems[user], self.seenItems[user]]
+
+
+@dp.functional_datapipe("gen_test_yielding_")
+class GenTestYielder(GenValidYielder):
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        self.seenItems = [set() for _ in range(self.User.count)]
+        self.unseenItems = [set() for _ in range(self.User.count)]
+
+        for chunk in dataset.train():
+            self.listmap(
+                lambda user, item: self.seenItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+        for chunk in dataset.valid():
+            self.listmap(
+                lambda user, item: self.seenItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+        for chunk in dataset.test():
+            self.listmap(
+                lambda user, item: self.unseenItems[user].add(item),
+                chunk[USER, ID], chunk[ITEM, ID]
+            )
+
+        self.seenItems = [tuple(items) for items in self.seenItems]
+        self.unseenItems = [tuple(items) for items in self.unseenItems]
+
+
 @dp.functional_datapipe("gen_train_uniform_sampling_")
-class GenTrainUniformSampler(Postprocessor):
+class GenTrainUniformSampler(GenTrainYielder):
     r"""
     A functional datapipe for uniformly sampling users and their negatives.
 
     Parameters:
     -----------
     source_dp: dp.iter.IterableWrapper 
         A datapipe that yields users.
@@ -38,42 +171,28 @@
     """
 
     def __init__(
         self, source_dp: dp.iter.IterableWrapper,
         dataset: RecDataSet,
         num_negatives: int = 1,
     ) -> None:
-        super().__init__(source_dp)
         self.num_negatives = num_negatives
-        self.User: SparseField = dataset.fields[USER, ID]
-        self.Item: SparseField = dataset.fields[ITEM, ID]
-        self.prepare(dataset)
+        super().__init__(source_dp, dataset)
 
-    @timemeter("GenUniformSampler/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before sampling.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset object that contains field objects.
-        """
         self.posItems = [set() for _ in range(self.User.count)]
-        self.negative_pool = self._sample_from_all(dataset.datasize * self.num_negatives)
+        self.negative_pool = self._sample_from_all(dataset.train().datasize * self.num_negatives)
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].add(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         self.posItems = [tuple(items) for items in self.posItems]
 
-    def _check(self, user) -> bool:
-        return len(self.posItems[user]) > 0
-
     def _sample_from_all(self, pool_size: int = 51200):
         r"""
         Randomly sample items from all items.
 
         Parameters:
         -----------
         pool_size: int 
@@ -103,30 +222,14 @@
             A negative item that has not been seen.
         """
         negative = next(self.negative_pool)
         while negative in seen:
             negative = next(self.negative_pool)
         return negative
 
-    def _sample_pos(self, user: int) -> int:
-        r"""
-        Randomly sample a positive item for a user.
-
-        Parameters:
-        -----------
-        user: int 
-            A user index.
-
-        Returns:
-        --------
-        positive: int 
-            A positive item that the user has interacted with.
-        """
-        return random.choice(self.posItems[user])
-
     def _sample_neg(self, user: int) -> List[int]:
         r"""Randomly sample negative items for a user.
 
         Parameters:
         ----------
         user: int 
             A user index.
@@ -141,127 +244,64 @@
 
     def __iter__(self):
         for user in self.source:
             if self._check(user):
                 yield [user, self._sample_pos(user), self._sample_neg(user)]
 
 
-@dp.functional_datapipe("gen_valid_yielding_")
-class GenValidYielder(Postprocessor):
-    r"""
-    A datapipe that yields (user, unseen, seen) triplets.
-    The ValidTripleter postprocessor takes a RecDataSet as input,
-    and yields (user, unseen, seen) triplets. The unseen and seen sets contain the IDs of
-    the items that the user has not seen and seen, respectively. Whether to use validation
-    or test set as the source of unseen items depends on the value of `dataset.VALID_IS_TEST`.
-    """
-
-    def __init__(
-        self, source_dp: dp.iter.IterDataPipe,
-        dataset: RecDataSet
-    ) -> None:
-        r"""
-        Initializes a new instance of the Tripleter postprocessor.
-        
-        Parameters:
-        -----------
-        source_dp: RecDatapipe or Postprocessor 
-            A RecDatapipe or another Postprocessor that yields dicts of NumPy arrays.
-        dataset: RecDataSet 
-            The dataset that provides the data source.
-        """
-        super().__init__(source_dp)
-
-        self.User: SparseField = dataset.fields[USER, ID]
-        self.Item: SparseField = dataset.fields[ITEM, ID]
+@dp.functional_datapipe("gen_valid_sampling_")
+class GenValidSampler(GenValidYielder):
 
-        self.prepare(dataset)
+    def _sample_negs(self, user: int, posItem: int):
+        idx = (user, posItem)
+        if self.negItems.get(idx, None) is None:
+            seen = self.seenItems[user]
+            unseen = list(set(self.Item.enums) - set(seen))
+            self.negItems[idx] = tuple(random.choices(unseen, k=100))
+        return self.negItems[idx]
 
-    @timemeter("GenValidYielder/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepares the dataset by building sets of seen items for each user.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset that provides the data source.
-        """
         self.seenItems = [set() for _ in range(self.User.count)]
-        self.unseenItems = [set() for _ in range(self.User.count)]
 
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.seenItems[user].add(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
-        for chunk in dataset.valid():
-            self.listmap(
-                lambda user, item: self.unseenItems[user].add(item),
-                chunk[USER, ID], chunk[ITEM, ID]
-            )
 
+        self.negItems = dict()
         self.seenItems = [tuple(items) for items in self.seenItems]
-        self.unseenItems = [tuple(items) for items in self.unseenItems]
-
-    def _check(self, user) -> bool:
-        return len(self.unseenItems[user]) > 0
 
     def __iter__(self):
-        r"""
-        Yields:
-        -------
-        user, unseen, seen: int, List[int], List[int]
-            Triplets for each user in the data source.
-        """
-        for user in self.source:
-            if self._check(user):
-                yield [user, self.unseenItems[user], self.seenItems[user]]
+        for user, posItem in self.source:
+            yield [user, (posItem,) + self._sample_negs(user, posItem)]
 
 
-@dp.functional_datapipe("gen_test_yielding_")
-class GenTestYielder(GenValidYielder):
-    r"""
-    A datapipe that yields (user, unseen, seen) triplets from the test set.
-    The TestTriplet postprocessor takes a RecDataSet as input,
-    and yields (user, unseen, seen) triplets from the test set. The unseen and seen sets contain the IDs of
-    the items that the user has not seen and seen, respectively.
-    """
+@dp.functional_datapipe("gen_test_sampling_")
+class GenTestSampler(GenValidSampler):
 
-    @timemeter("GenTestYielder/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepares the dataset by building sets of seen items for each user.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset that provides the data source.
-        """
         self.seenItems = [set() for _ in range(self.User.count)]
-        self.unseenItems = [set() for _ in range(self.User.count)]
 
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.seenItems[user].add(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
+
         for chunk in dataset.valid():
             self.listmap(
                 lambda user, item: self.seenItems[user].add(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
-        for chunk in dataset.test():
-            self.listmap(
-                lambda user, item: self.unseenItems[user].add(item),
-                chunk[USER, ID], chunk[ITEM, ID]
-            )
 
+        self.negItems = dict()
         self.seenItems = [tuple(items) for items in self.seenItems]
-        self.unseenItems = [tuple(items) for items in self.unseenItems]
 
 
 #===============================For Sequential Recommendation===============================
 
 
 @dp.functional_datapipe("seq_train_yielding_")
 class SeqTrainYielder(Postprocessor):
@@ -270,66 +310,60 @@
 
     Parameters:
     -----------
     source_dp: dp.iter.IterableWrapper 
         A datapipe that yields users.
     dataset: RecDataSet 
         The dataset object that contains field objects.
+    leave_one_out: bool, default to `True`
+        `True`: take the last one as a target
+        `False`: take `posItems[1:]` as targets
     """
 
     def __init__(
-        self, source_dp: dp.iter.IterableWrapper,
-        dataset: RecDataSet,
+        self, 
+        source_dp: dp.iter.IterableWrapper,
+        dataset: Optional[RecDataSet] = None,
+        leave_one_out: bool = True
     ) -> None:
         super().__init__(source_dp)
-        self.User: SparseField = dataset.fields[USER, ID]
-        self.Item: SparseField = dataset.fields[ITEM, ID]
+        self.User = dataset.fields[USER, ID]
+        self.Item = dataset.fields[ITEM, ID]
+        if leave_one_out:
+            self.marker = -1
+        else:
+            self.marker = 1
+
         self.prepare(dataset)
 
-    @timemeter("SeqTrainYielder/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before yielding.
+        pass
 
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset object that contains field objects.
-        """
-        self.posItems = [[] for _ in range(self.User.count)]
-        for chunk in dataset.train():
-            self.listmap(
-                lambda user, item: self.posItems[user].append(item),
-                chunk[USER, ID], chunk[ITEM, ID]
-            )
-        self.posItems = [tuple(items) for items in self.posItems]
-
-    def _check(self, user) -> bool:
-        return len(self.posItems[user]) > 1
+    def _check(self, seq: Tuple) -> bool:
+        return len(seq) > 1
 
     def __iter__(self):
-        for user in self.source:
-            if self._check(user):
-                posItems = self.posItems[user]
-                yield [user, posItems[:-1], posItems[1:]]
+        for user, seq in self.source:
+            if self._check(seq):
+                yield [user, seq[:-1], seq[self.marker:]]
 
 
 @dp.functional_datapipe("seq_valid_yielding_")
 class SeqValidYielder(SeqTrainYielder):
 
-    @timemeter("SeqValidYielder/prepare")
-    def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before yielding.
+    def __init__(
+        self, 
+        source_dp: dp.iter.IterableWrapper, 
+        dataset: RecDataSet
+    ) -> None:
+        super().__init__(source_dp, dataset, True)
 
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset object that contains field objects.
-        """
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
         self.posItems = [[] for _ in range(self.User.count)]
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         for chunk in dataset.valid():
@@ -337,33 +371,25 @@
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         self.posItems = [tuple(items) for items in self.posItems]
 
     def __iter__(self):
         for user in self.source:
-            if self._check(user):
-                posItems = self.posItems[user]
+            posItems = self.posItems[user]
+            if self._check(posItems):
                 # (user, seqs, unseen, seen)
                 yield [user, posItems[:-1], posItems[-1:], posItems[:-1]]
 
 
 @dp.functional_datapipe("seq_test_yielding_")
 class SeqTestYielder(SeqValidYielder):
 
-    @timemeter("SeqTestYielder/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before yielding.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet 
-            The dataset object that contains field objects.
-        """
         self.posItems = [[] for _ in range(self.User.count)]
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         for chunk in dataset.valid():
@@ -378,37 +404,25 @@
             )
         self.posItems = [tuple(items) for items in self.posItems]
 
 
 @dp.functional_datapipe("seq_train_uniform_sampling_")
 class SeqTrainUniformSampler(SeqTrainYielder):
 
-
-    @timemeter("SeqTrainUniformSampler/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before sampling.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet
-            The dataset object that contains field objects.
-        """
         self.posItems = [[] for _ in range(self.User.count)]
-        self.negative_pool = self._sample_from_all(dataset.datasize)
-
+        self.negative_pool = self._sample_from_all(dataset.train().datasize)
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
-
         self.posItems = [tuple(items) for items in self.posItems]
 
-
     def _sample_from_all(self, pool_size: int = 51200):
         r"""
         Randomly sample items from all items.
 
         Parameters:
         -----------
         pool_size: int 
@@ -438,55 +452,49 @@
             A negative item that has not been seen.
         """
         negative = next(self.negative_pool)
         while negative in seen:
             negative = next(self.negative_pool)
         return negative
 
-    def _sample_neg(self, user: int) -> List[int]:
+    def _sample_neg(self, user: int, positives: Tuple) -> List[int]:
         r"""Randomly sample negative items for a user.
 
         Parameters:
         ----------
-        user: int 
-            A user index.
+        user: int
+        positives: Tuple 
+            A tuple of positives.
 
         Returns:
         --------
         negatives: List[int] 
             A list of negative items that the user has not interacted with.
         """
         seen = self.posItems[user]
-        return self.listmap(self._sample_from_pool, [seen] * (len(seen) - 1))
+        return self.listmap(self._sample_from_pool, [seen] * (len(positives)))
 
     def __iter__(self):
-        for user in self.source:
-            if self._check(user):
-                posItems = self.posItems[user]
-                yield [user, posItems[:-1], posItems[1:], self._sample_neg(user)]
+        for user, seq in self.source:
+            if self._check(seq):
+                seen = seq[:-1]
+                positives = seq[self.marker:]
+                negatives = self._sample_neg(user, positives)
+                yield [user, seen, positives, self._sample_neg(user, negatives)]
 
 
 @dp.functional_datapipe("seq_valid_sampling_")
 class SeqValidSampler(SeqValidYielder):
 
-
     def _sample_negs(self, seen: List[int]):
         unseen = list(set(self.Item.enums) - set(seen))
         return tuple(random.choices(unseen, k=100))
 
-    @timemeter("SeqValidSampler/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before sampling.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet
-            The dataset object that contains field objects.
-        """
         self.posItems = [[] for _ in range(self.User.count)]
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
 
@@ -499,32 +507,24 @@
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         self.posItems = [tuple(items) for items in self.posItems]
 
     def __iter__(self):
         for user in self.source:
-            if self._check(user):
-                posItems = self.posItems[user]
+            posItems = self.posItems[user]
+            if self._check(posItems):
                 yield [user, posItems[:-1], posItems[-1:] + self.negItems[user]]
 
 
 @dp.functional_datapipe("seq_test_sampling_")
 class SeqTestSampler(SeqValidSampler):
 
-    @timemeter("SeqTestSampler/prepare")
+    @timemeter
     def prepare(self, dataset: RecDataSet):
-        r"""
-        Prepare the data before sampling.
-
-        Parameters:
-        -----------
-        dataset: RecDataSet
-            The dataset object that contains field objects.
-        """
         self.posItems = [[] for _ in range(self.User.count)]
         for chunk in dataset.train():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         for chunk in dataset.valid():
@@ -555,36 +555,222 @@
 
     Parameters:
     -----------
     source_dp: dp.iter.IterableWrapper 
         A datapipe that yields users.
     dataset: RecDataSet 
         The dataset object that contains field objects.
+    leave_one_out: bool, default to `True`
+        `True`: take the last one as a target
+        `False`: take `posItems[1:]` as targets
     """
 
     def __init__(
         self, source_dp: dp.iter.IterableWrapper,
         dataset: Optional[RecDataSet] = None,
+        leave_one_out: bool = True
     ) -> None:
         super().__init__(source_dp)
+        self.Item = dataset.fields[ITEM, ID]
+        if leave_one_out:
+            self.marker = -1
+        else:
+            self.marker = 1
+
+        self.prepare(dataset)
 
-    def _check(self, sequence) -> bool:
-        return len(sequence) > 1
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        pass
+
+    def _check(self, seq) -> bool:
+        return len(seq) > 1
 
     def __iter__(self):
-        for sess, sequence in self.source:
-            if self._check(sequence):
-                yield [sess, sequence[:-1], sequence[-1:]]
+        for sess, seq in self.source:
+            if self._check(seq):
+                yield [sess, seq[:-1], seq[self.marker:]]
 
 
 @dp.functional_datapipe("sess_valid_yielding_")
 class SessValidYielder(SessTrainYielder):
 
+    def __init__(
+        self, 
+        source_dp: dp.iter.IterableWrapper, 
+        dataset: RecDataSet
+    ) -> None:
+        super().__init__(source_dp, dataset, True)
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        self.seenItems = set()
+        for chunk in dataset.train():
+            self.listmap(
+                lambda item: self.seenItems.add(item),
+                chunk[ITEM, ID]
+            )
+
+    def _check(self, seq) -> bool:
+        # filter out the sequence with a target not appearing in training set
+        return len(seq) > 1 and seq[-1] in self.seenItems
+
     def __iter__(self):
-        for sess, sequence in self.source:
-            if self._check(sequence):
+        for sess, seq in self.source:
+            if self._check(seq):
                 # (user, seqs, unseen, seen)
-                yield [sess, sequence[:-1], sequence[-1:], sequence[:-1]]
+                yield [sess, seq[:-1], seq[-1:], seq[:-1]]
 
 
 @dp.functional_datapipe("sess_test_yielding_")
-class SessTestYielder(SessValidYielder): ...
+class SessTestYielder(SessValidYielder): ...
+
+
+@dp.functional_datapipe("sess_train_uniform_sampling_")
+class SessTrainUniformSampler(SessTrainYielder):
+    r"""
+    A functional datapipe for uniformly sampling negatives for each sequence.
+
+    Parameters:
+    -----------
+    source_dp: dp.iter.IterableWrapper 
+        A datapipe that yields users.
+    dataset: RecDataSet 
+        The dataset object that contains field objects.
+    num_negatives: int 
+        The number of negative samples for each piece of data.  
+    leave_one_out: bool, default to `True`
+        `True`: take the last one as a target
+        `False`: take `posItems[1:]` as targets
+    """
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        r"""
+        Prepare the data before sampling.
+
+        Parameters:
+        -----------
+        dataset: RecDataSet 
+            The dataset object that contains field objects.
+        """
+        self.negative_pool = self._sample_from_all(dataset.train().datasize)
+
+    def _sample_from_all(self, pool_size: int = 51200):
+        r"""
+        Randomly sample items from all items.
+
+        Parameters:
+        -----------
+        pool_size: int 
+            The number of items to be sampled.
+
+        Returns:
+        --------
+        Generator: A generator that yields sampled items.
+        """
+        allItems = self.Item.enums
+        while 1:
+            for item in random.choices(allItems, k=pool_size):
+                yield item
+
+    def _sample_from_pool(self, seen: Tuple):
+        r"""
+        Randomly sample a negative item from the pool of all items.
+
+        Parameters:
+        -----------
+        seen: set 
+            A set of seen items.
+
+        Returns:
+        --------
+        negative: int 
+            A negative item that has not been seen.
+        """
+        negative = next(self.negative_pool)
+        while negative in seen:
+            negative = next(self.negative_pool)
+        return negative
+
+    def _sample_neg(self, seen: Tuple, positives: Tuple) -> List[int]:
+        r"""Randomly sample negative items for a user.
+
+        Parameters:
+        ----------
+        seen: Tuple 
+            A sequence of seen items.
+        positives: Tuple
+            A sequence of positive items.
+
+        Returns:
+        --------
+        negatives: List[int] 
+            A list of negative items that the user has not interacted with.
+        """
+        return self.listmap(self._sample_from_pool, [seen] * len(positives))
+
+    def __iter__(self):
+        for sess, seq in self.source:
+            if self._check(seq):
+                seen = seq[:-1]
+                positives = seq[self.marker:]
+                negatives = self._sample_neg(seq, positives)
+                yield [sess, seen, positives, negatives]
+
+
+@dp.functional_datapipe("sess_valid_sampling_")
+class SessValidSampler(SessTrainYielder):
+
+    def __init__(
+        self, 
+        source_dp: dp.iter.IterableWrapper, 
+        dataset: Optional[RecDataSet] = None
+    ) -> None:
+        super().__init__(source_dp, dataset, True)
+
+    def _sample_negs(self, sess: int, seq: Tuple):
+        idx = (sess, tuple(seq))
+        if self.negItems.get(idx, None) is None:
+            seen = self.seenItems[sess]
+            unseen = list(set(self.Item.enums) - set(seen))
+            self.negItems[idx] = tuple(random.choices(unseen, k=100))
+        return self.negItems[idx]
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        self.seenItems = defaultdict(set)
+
+        for chunk in dataset.valid():
+            self.listmap(
+                lambda id_, item: self.seenItems[id_].add(item),
+                chunk[SESSION, ID], chunk[ITEM, ID]
+            )
+
+        self.negItems = dict()
+        for key in self.seenItems:
+            self.seenItems[key] = tuple(self.seenItems[key])
+
+    def __iter__(self):
+        for sess, seq in self.source:
+            if self._check(seq):
+                seen = seq[:-1]
+                posItem = seq[-1]
+                yield [sess, seen, (posItem,) + self._sample_negs(sess, seq)]
+
+
+@dp.functional_datapipe("sess_test_sampling_")
+class SessTestSampler(SessValidSampler):
+
+    @timemeter
+    def prepare(self, dataset: RecDataSet):
+        self.seenItems = defaultdict(set)
+
+        for chunk in dataset.test():
+            self.listmap(
+                lambda id_, item: self.seenItems[id_].add(item),
+                chunk[SESSION, ID], chunk[ITEM, ID]
+            )
+
+        self.negItems = dict()
+        for key in self.seenItems:
+            self.seenItems[key] = tuple(self.seenItems[key])
```

### Comparing `freerec-0.4.1/freerec/data/postprocessing/source.py` & `freerec-0.4.3/freerec/data/postprocessing/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from functools import partial
 
 from .base import BaseProcessor
 from ..fields import SparseField
 
 
 __all__ = [
-    'RandomSource', 'RandomShuffledSource', 'OrderedSource',
+    'RandomChoicedSource', 'RandomShuffledSource', 'OrderedSource',
     'RandomIDs', 'OrderedIDs', 'DummySource'
 ]
 
 
-class RandomSource(BaseProcessor):
+class RandomChoicedSource(BaseProcessor):
     r"""
     DataPipe that generates random items from given source.
+    Note that this sampling is with replacement.
 
     Parameters:
     -----------
     source: Iterable 
         The source data to start.
     datasize: int 
         Datasize.
@@ -42,14 +43,15 @@
         for _ in range(self.datasize):
             yield self._rng()
 
 
 class RandomShuffledSource(BaseProcessor):
     r"""
     DataPipe that generates shuffled source.
+    In this vein, every sample will be selected once per epoch.
 
     Parameters:
     -----------
     source: Iterable 
         The source data to start.
     """
 
@@ -84,15 +86,15 @@
         assert isinstance(source, Sequence), f"Sequence type is required but received {type(source)} type."
         self.source = tuple(source)
 
     def __iter__(self):
         yield from iter(self.source)
 
 
-class RandomIDs(RandomSource):
+class RandomIDs(RandomChoicedSource):
     r"""
     DataPipe that generates random IDs according to SparseField.
 
     Parameters:
     -----------
     field: SparseField 
         ID values to select from.
```

### Comparing `freerec-0.4.1/freerec/data/preprocessing/base.py` & `freerec-0.4.3/freerec/data/preprocessing/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -207,15 +207,16 @@
     
     def filter_by_core(
         self,
         low4user: Union[None, int, float] = None, 
         high4user: Union[None, int, float] = None,
         low4item: Union[None, int, float] = None, 
         high4item: Union[None, int, float] = None,
-        master: str = USER.name
+        master: str = USER.name,
+        strict: bool = True
     ):
         r"""
         Filter (user, item) by k-core settings.
 
         Parameters:
         -----------
         low4user: int, float, optional
@@ -226,14 +227,17 @@
             - `None`: float('inf')
         low4item: int, float, optional
             Minimum core for item.
             - `None`: float('-inf')
         max4item: int, float, optional
             Maximum core for item.
             - `None`: float('inf')
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
         """
         low4user = low4user if low4user else float('-inf')
         high4user = high4user if high4user else float('inf')
         low4item = low4item if low4item else float('-inf')
         high4item = high4item if high4item else float('inf')
         df = self.interactions
         dsz = -1
@@ -241,14 +245,15 @@
             f"[Converter] >>> Filter dataframe: "
             f"{master} in [{low4user}, {high4user}]; "
             f"Item in [{low4item}, {high4item}] ..."
         )
         infoLogger(f"[Converter] >>> Current datasize: {len(df)} ...")
         while dsz != len(df):
             dsz = len(df)
+
             # filter by user
             users = df[master]
             counts = users.value_counts()
             bool_indices = users.isin(
                 counts[(low4user <= counts) & (counts <= high4user)].index
             )
             df = df[bool_indices]
@@ -259,14 +264,17 @@
             bool_indices = items.isin(
                 counts[(low4item <= counts) & (counts <= high4item)].index
             )
             df = df[bool_indices]
 
             infoLogger(f"[Converter] >>> Current datasize: {len(df)}")
 
+            if not strict:
+                break
+
         self.interactions = df
 
     def user2token(self, master: str = USER.name):
         infoLogger(f"[Converter] >>> Map user ID to Token ...")
         user_ids = sorted(self.interactions[master].unique().tolist())
         self.userCount = len(user_ids)
 
@@ -372,28 +380,52 @@
         self.trainiter = pd.concat(traingroups).reset_index(drop=True)
         self.validiter = pd.concat(validgroups).reset_index(drop=True)
         self.testiter = pd.concat(testgroups).reset_index(drop=True)
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
+        # max(): choosing the last timestamp as the timestamp for the session
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
         validgroups = groups[l:r]
         testgroups = groups[r:]
 
         self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
         self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
         self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
 
+    def sess_split_by_day(self, days: int = 1):
+        infoLogger(f"[Converter] >>> Split by days: {days} ...")
+
+        seconds_per_day = 86400
+        seconds = seconds_per_day * days
+        last_date = self.interactions[TIMESTAMP.name].max().item()
+
+        # Group interactions by session and calculate session timestamps
+        session_timestamps = self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values()
+
+        # Split interactions into train, validation, and test sets based on session timestamps
+        traingroups = session_timestamps[session_timestamps < (last_date - 2 * seconds)].index
+        validgroups = session_timestamps[(session_timestamps >= (last_date - 2 * seconds)) & (session_timestamps < (last_date - seconds))].index
+        testgroups = session_timestamps[session_timestamps >= (last_date - seconds)].index
+
+        assert len(traingroups) >= 0, f"The given `days` of {days} leads to zero-size trainsets ..."
+        assert len(validgroups) >= 0, f"The given `days` of {days} leads to zero-size validsets ..."
+        assert len(testgroups) >= 0, f"The given `days` of {days} leads to zero-size testsets ..."
+
+        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
+        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
+        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
+
     def save(self, path: str):
         mkdirs(path)
 
         infoLogger(f"[Converter] >>> Save `train.txt' to {path} ...")
         df = pd.DataFrame(self.trainiter)
         df.to_csv(os.path.join(path, 'train.txt'), sep='\t', index=False)
 
@@ -422,37 +454,41 @@
         self.summary()
 
     def make_general_dataset(
         self,
         star4pos: int = 0,
         kcore4user: int = 10,
         kcore4item: int = 10,
+        strict: bool = True,
         ratios: Tuple[int, int, int] = (8, 1, 1),
         fields: Optional[Iterable[str]] = (USER.name, ITEM.name)
     ):
         r"""
         Make general dataset.
 
         Parameters:
         -----------
         star4pos: int, default to 0
             Select interactions with `Rating > star4pos'.
         kcore4user: int, default to 10
             Select kcore interactions according to User.
         kcore4item: int, default to 10
             Select kcore interactions according to Item.
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
         ratios: Tuple[int, int, int], default to (8, 1, 1)
             The ratios of training|validation|test set.
         fields: Iterable[str], default to (User, Item)
             The fields reserved.
         """
 
         self.load()
         self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item)
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
         self.user2token()
         self.item2token()
         self.sort_by_timestamp()
         if fields:
             self.reserve(fields)
         self.gen_split_by_ratio(ratios)
 
@@ -465,35 +501,38 @@
         self.save(path)
 
     def make_sequential_dataset(
         self,
         star4pos: int = 0,
         kcore4user: int = 5,
         kcore4item: int = 5,
+        strict: bool = True,
         fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name)
     ):
         r"""
         Make sequential dataset by leaving last two as validation|test samples.
 
         Parameters:
         -----------
         star4pos: int, default to 0
             Select interactions with `Rating > star4pos'.
         kcore4user: int, default to 10
             Select kcore interactions according to User.
         kcore4item: int, default to 10
             Select kcore interactions according to Item.
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
         fields: Iterable[str], default to (User, Item, TimeStamp)
             The fields reserved.
         """
 
-
         self.load()
         self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item)
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
         self.user2token()
         self.item2token()
         self.sort_by_timestamp()
         if fields:
             self.reserve(fields)
         self.seq_split_by_last_two()
 
@@ -506,14 +545,15 @@
         self.save(path)
 
     def make_sequential_dataset_by_ratio(
         self,
         star4pos: int = 0,
         kcore4user: int = 5,
         kcore4item: int = 5,
+        strict: bool = True,
         ratios: Tuple[int, int, int] = (8, 1, 1),
         fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name),
         seed: int = 0
     ):
         r"""
         Make sequential dataset by ratios.
 
@@ -521,22 +561,25 @@
         -----------
         star4pos: int, default to 0
             Select interactions with `Rating > star4pos'.
         kcore4user: int, default to 10
             Select kcore interactions according to User.
         kcore4item: int, default to 10
             Select kcore interactions according to Item.
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
         ratios: Tuple[int, int, int], default to (8, 1, 1)
             The ratios of training|validation|test set.
         fields: Iterable[str], default to (User, Item, Timestamp)
             The fields reserved.
         """
         self.load()
         self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item)
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
         self.user2token()
         self.item2token()
         self.sort_by_timestamp()
         if fields:
             self.reserve(fields)
         self.seq_split_by_ratio(ratios, seed=seed)
 
@@ -544,19 +587,71 @@
         path = os.path.join(
             self.root, 'Sequential', 
             '_'.join([self.dataset, code, 'Chron'])
         )
 
         self.save(path)
 
-    def make_session_dataset(
+    def make_session_dataset_by_day(
+        self,
+        star4pos: int = 0,
+        kcore4user: int = 2,
+        kcore4item: int = 5,
+        strict: bool = True,
+        days: int = 7,
+        fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
+    ):
+        r"""
+        Make session dataset by day.
+
+        Flows:
+        ------
+        1. filter out `inactive' items and short sessions;
+        2. training|validation|test set will be splited according to the start time of each session.
+
+        Parameters:
+        -----------
+        star4pos: int, default to 0
+            Select interactions with `Rating > star4pos'.
+        kcore4user: int, default to 10
+            Select kcore interactions according to User.
+        kcore4item: int, default to 10
+            Select kcore interactions according to Item.
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
+        days: int, default to 7
+            the number days used for validation and test
+        fields: Iterable[str], default to (User, Item, Timestamp)
+            The fields reserved.
+        """
+        self.load()
+        self.filter_by_rating(low=star4pos, high=None)
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name, strict=strict)
+        self.user2token(master=SESSION.name)
+        self.item2token()
+        self.sort_by_timestamp(master=SESSION.name)
+        if fields:
+            self.reserve(fields)
+        self.sess_split_by_day(days)
+
+        code = f"{kcore4user}{kcore4item}{star4pos}{days}"
+        path = os.path.join(
+            self.root, 'Session', 
+            '_'.join([self.dataset, code, 'Chron'])
+        )
+
+        self.save(path)
+
+    def make_session_dataset_by_ratio(
         self,
         star4pos: int = 0,
         kcore4user: int = 2,
         kcore4item: int = 5,
+        strict: bool = True,
         ratios: Tuple[int, int, int] = (8, 1, 1),
         fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
     ):
         r"""
         Make session dataset by ratios.
 
         Flows:
@@ -568,22 +663,25 @@
         -----------
         star4pos: int, default to 0
             Select interactions with `Rating > star4pos'.
         kcore4user: int, default to 10
             Select kcore interactions according to User.
         kcore4item: int, default to 10
             Select kcore interactions according to Item.
+        strict: bool, default to `True`
+            `True`: strictly filter by core
+            `False`: filter by core only once
         ratios: Tuple[int, int, int], default to (8, 1, 1)
             The ratios of training|validation|test set.
         fields: Iterable[str], default to (User, Item, Timestamp)
             The fields reserved.
         """
         self.load()
         self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name)
+        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name, strict=strict)
         self.user2token(master=SESSION.name)
         self.item2token()
         self.sort_by_timestamp(master=SESSION.name)
         if fields:
             self.reserve(fields)
         self.sess_split_by_ratio(ratios)
```

### Comparing `freerec-0.4.1/freerec/data/preprocessing/datasets.py` & `freerec-0.4.3/freerec/data/preprocessing/datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     filename = "yoochoose-buys"
 
 class YooChooseBuys14(YooChooseBuys):
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
         groups = groups[-ceil(len(groups) / 4):] # recent 1/4 sessions
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
@@ -287,15 +287,15 @@
 
 
 class YooChooseBuys164(YooChooseBuys):
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
         groups = groups[-ceil(len(groups) / 64):] # recent 1/64 sessions
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
@@ -316,42 +316,99 @@
 
 
 class YooChooseClicks14(YooChooseClicks):
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
         groups = groups[-ceil(len(groups) / 4):] # recent 1/4 sessions
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
         validgroups = groups[l:r]
         testgroups = groups[r:]
 
         self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
         self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
         self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
 
+    def sess_split_by_day(self, days: int = 1):
+        infoLogger(f"[Converter] >>> Split by days: {days} ...")
+
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
+        groups = groups[-ceil(len(groups) / 4):] # recent 1/4 sessions
+        self.interactions = self.interactions[self.interactions[SESSION.name].isin(groups)]
+
+        seconds_per_day = 86400
+        seconds = seconds_per_day * days
+
+        last_date = self.interactions[TIMESTAMP.name].max().item()
+
+        # Group interactions by session and calculate session timestamps
+        session_timestamps = self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values()
+
+        # Split interactions into train, validation, and test sets based on session timestamps
+        traingroups = session_timestamps[session_timestamps < (last_date - 2 * seconds)].index
+        validgroups = session_timestamps[(session_timestamps >= (last_date - 2 * seconds)) & (session_timestamps < (last_date - seconds))].index
+        testgroups = session_timestamps[session_timestamps >= (last_date - seconds)].index
+
+        assert len(traingroups) >= 0, f"The given `days` of {days} leads to zero-size trainsets ..."
+        assert len(validgroups) >= 0, f"The given `days` of {days} leads to zero-size validsets ..."
+        assert len(testgroups) >= 0, f"The given `days` of {days} leads to zero-size testsets ..."
+
+        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
+        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
+        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
+
 
 class YooChooseClicks164(YooChooseClicks):
 
     def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
         infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
 
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].min().sort_values().index)
-        groups = groups[-ceil(len(groups) / 64):] # recent 1/4 sessions
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
+        groups = groups[-ceil(len(groups) / 64):] # recent 1/64 sessions
 
         markers = np.cumsum(ratios)
         l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
         r = floor(markers[1] * len(groups) / markers[-1])
 
         traingroups = groups[:l]
         validgroups = groups[l:r]
         testgroups = groups[r:]
 
         self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
         self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
-        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
+        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
+
+    def sess_split_by_day(self, days: int = 1):
+        infoLogger(f"[Converter] >>> Split by days: {days} ...")
+
+        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
+        groups = groups[-ceil(len(groups) / 64):] # recent 1/64 sessions
+        self.interactions = self.interactions[self.interactions[SESSION.name].isin(groups)]
+
+        seconds_per_day = 86400
+        seconds = seconds_per_day * days
+
+        last_date = self.interactions[TIMESTAMP.name].max().item()
+
+        # Group interactions by session and calculate session timestamps
+        session_timestamps = self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values()
+
+        # Split interactions into train, validation, and test sets based on session timestamps
+        traingroups = session_timestamps[session_timestamps < (last_date - 2 * seconds)].index
+        validgroups = session_timestamps[(session_timestamps >= (last_date - 2 * seconds)) & (session_timestamps < (last_date - seconds))].index
+        testgroups = session_timestamps[session_timestamps >= (last_date - seconds)].index
+
+        assert len(traingroups) >= 0, f"The given `days` of {days} leads to zero-size trainsets ..."
+        assert len(validgroups) >= 0, f"The given `days` of {days} leads to zero-size validsets ..."
+        assert len(testgroups) >= 0, f"The given `days` of {days} leads to zero-size testsets ..."
+
+        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
+        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
+        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
+
```

### Comparing `freerec-0.4.1/freerec/data/tags.py` & `freerec-0.4.3/freerec/data/tags.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/data/transformation.py` & `freerec-0.4.3/freerec/data/transformation.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     Returns:
     --------
     Any
         The transformed data.
 
     Examples:
     ---------
-    >>> import torcharrow.dtypes as dt
     >>> col = [3, 2, 1]
     >>> transformer = Identifier()
     >>> transformer.transform(col)
     [3, 2, 1]
     """
 
     def __init__(self) -> None:
@@ -48,76 +47,142 @@
 
 class Indexer(Identifier):
     r"""
     Transform sparse items into indices.
 
     classes: set
         Set of unique classes seen during `fit`.
-    maper: dict
+    mapper: dict
         Mapping of input values to output indices.
 
     Examples:
     ---------
     >>> col = [3, 2, 1]
     >>> col2 = [4, 5, 6]
     >>> transformer = Indexer()
     >>> transformer.partial_fit(col)
     >>> transformer.classes
     {1, 2, 3}
-    >>> transformer.maper
+    >>> transformer.mapper
     {1: 0, 2: 1, 3: 2}
     >>> transformer.partial_fit(col2)
     >>> transformer.classes
     {1, 2, 3, 4, 5, 6}
-    >>> transformer.maper
+    >>> transformer.mapper
     {1: 0, 2: 1, 3: 2, 4: 3, 5: 4, 6: 5}
     >>> transformer.transform(col2)
     [3, 4, 5]
     """
 
     def reset(self):
         self.classes = set()
-        self.maper = None
+        self.mapper = None
         self.enums = None
 
     def partial_fit(self, col: List):
         self.classes |= set(col)
         ordered = sorted(self.classes)
         self.count = len(ordered)
         self.enums = tuple(range(self.count))
-        self.maper = dict(zip(ordered, self.enums))
+        self.mapper = dict(zip(ordered, self.enums))
 
     def _map(self, x):
-        return self.maper[x]
+        return self.mapper[x]
 
     def transform(self, col: List) -> List:
-        if self.maper:
+        if self.mapper:
             return list(map(self._map, col))
         else:
             raise TransformError("Indexer should be (partially) fitted before using ...")
 
 
+class UpIndexer(Indexer):
+    r"""
+    Transform sparse items into indices from zero to maximum.
+
+    Examples:
+    ---------
+    >>> col = [3, 2, 1]
+    >>> col2 = [4, 5, 6]
+    >>> transformer = UpIndexer()
+    >>> transformer.partial_fit(col)
+    >>> transformer.count
+    4
+    >>> transformer.enums
+    (0, 1, 2, 3)
+    >>> transformer.partial_fit(col2)
+    >>> transformer.count
+    7
+    >>> transformer.enums
+    (0, 1, 2, 3, 4, 5, 6)
+    >>> transformer.transform(col2)
+    [4, 5, 6]
+    """
+
+    def reset(self):
+        self.enums = None
+        self.count = float("-inf")
+
+    def partial_fit(self, col: List):
+        self.count = max(np.max(col).item() + 1, self.count)
+        self.enums = tuple(range(self.count))
+
+    def transform(self, col: List) -> List:
+        if self.enums:
+            return col
+        else:
+            raise TransformError("Indexer should be (partially) fitted before using ...")
+
+class NumIndexer(Indexer):
+    r"""
+    Transform sparse items into indices from zero to maximum.
+
+    Parameters:
+    -----------
+    nums: int
+        the maximum index.
+
+    Examples:
+    ---------
+    >>> transformer = NumIndexer(6)
+    >>> transformer.count
+    7
+    >>> transformer.enums
+    (0, 1, 2, 3, 4, 5, 6)
+    """
+
+    def __init__(self, nums: int) -> None:
+        self.nums = nums
+        super().__init__()
+
+    def reset(self):
+        self.count = self.nums + 1
+        self.enums = tuple(range(self.count))
+
+    def partial_fit(self, col: List): ...
+
+    def transform(self, col: List) -> List:
+        return col
+
+
 class StandardScaler(Identifier):
     r"""
     Normalize dense items using the standard scaler.
 
     Attributes:
     -----------
-    field: dt.Field or the Field defined in torcharrow.fields
-        The field type of the dense items.
-    n_samples: int
+    nums: int
         The number of fitted items.
-    sum_: float
+    sum: float
         The summation of the fitted items.
-    sum_of_squares: float 
+    ssum: float 
         The summation of the squared fitted items.
 
     Examples:
     ---------
-    >>> import torcharrow.dtypes as dt
     >>> col = [3., 2., 1.]
     >>> transformer = StandardScaler()
     >>> transformer.partial_fit(col)
     >>> transformer.transform(col)
     [1.2247448713915887, 0.0, -1.2247448713915887]
     """
```

### Comparing `freerec-0.4.1/freerec/data/utils.py` & `freerec-0.4.3/freerec/data/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,9 +203,8 @@
     with open(filename, 'rb') as f:
         while True:
             data = f.read(1048576)
             if not data:
                 break
             sha1.update(data)
 
-    return sha1.hexdigest() == sha1_hash
-
+    return sha1.hexdigest() == sha1_hash
```

### Comparing `freerec-0.4.1/freerec/dict2obj.py` & `freerec-0.4.3/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/launcher.py` & `freerec-0.4.3/freerec/launcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,1903 +39,2261 @@
 00000260: 696d 706f 7274 2041 7665 7261 6765 4d65  import AverageMe
 00000270: 7465 722c 204d 6f6e 6974 6f72 2c20 7469  ter, Monitor, ti
 00000280: 6d65 6d65 7465 722c 2069 6e66 6f4c 6f67  memeter, infoLog
 00000290: 6765 720d 0a66 726f 6d20 2e6d 6574 7269  ger..from .metri
 000002a0: 6373 2069 6d70 6f72 7420 2a0d 0a66 726f  cs import *..fro
 000002b0: 6d20 2e70 6172 7365 7220 696d 706f 7274  m .parser import
 000002c0: 2054 494d 450d 0a0d 0a0d 0a5f 5f61 6c6c   TIME......__all
-000002d0: 5f5f 203d 205b 2743 6869 6566 436f 6163  __ = ['ChiefCoac
-000002e0: 6827 2c20 2743 6f61 6368 272c 2027 4164  h', 'Coach', 'Ad
-000002f0: 6170 7465 7227 5d0d 0a0d 0a0d 0a44 4546  apter']......DEF
-00000300: 4155 4c54 5f4d 4554 5249 4353 203d 207b  AULT_METRICS = {
-00000310: 0d0a 2020 2020 274c 4f53 5327 3a20 6c61  ..    'LOSS': la
-00000320: 6d62 6461 2078 3a20 782c 0d0a 2020 2020  mbda x: x,..    
-00000330: 2323 2323 2323 2323 2323 2323 230d 0a20  #############.. 
-00000340: 2020 2027 4d53 4527 3a20 6d65 616e 5f73     'MSE': mean_s
-00000350: 7175 6172 6564 5f65 7272 6f72 2c0d 0a20  quared_error,.. 
-00000360: 2020 2027 4d41 4527 3a20 6d65 616e 5f61     'MAE': mean_a
-00000370: 6273 5f65 7272 6f72 2c0d 0a20 2020 2027  bs_error,..    '
-00000380: 524d 5345 273a 2072 6f6f 745f 6d73 652c  RMSE': root_mse,
-00000390: 0d0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
-000003a0: 2323 230d 0a20 2020 2027 5052 4543 4953  ###..    'PRECIS
-000003b0: 494f 4e27 3a20 7072 6563 6973 696f 6e2c  ION': precision,
-000003c0: 0d0a 2020 2020 2752 4543 414c 4c27 3a20  ..    'RECALL': 
-000003d0: 7265 6361 6c6c 2c0d 0a20 2020 2027 4631  recall,..    'F1
-000003e0: 273a 2066 315f 7363 6f72 652c 0d0a 2020  ': f1_score,..  
-000003f0: 2020 2741 5543 273a 2061 7572 6f63 2c0d    'AUC': auroc,.
-00000400: 0a20 2020 2027 4849 5452 4154 4527 3a20  .    'HITRATE': 
-00000410: 6869 745f 7261 7465 2c0d 0a20 2020 2023  hit_rate,..    #
-00000420: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-00000430: 2020 274e 4443 4727 3a20 6e6f 726d 616c    'NDCG': normal
-00000440: 697a 6564 5f64 6367 2c0d 0a20 2020 2027  ized_dcg,..    '
-00000450: 4d52 5227 3a20 6d65 616e 5f72 6563 6970  MRR': mean_recip
-00000460: 726f 6361 6c5f 7261 6e6b 2c0d 0a20 2020  rocal_rank,..   
-00000470: 2027 4d41 5027 3a20 6d65 616e 5f61 7665   'MAP': mean_ave
-00000480: 7261 6765 5f70 7265 6369 7369 6f6e 0d0a  rage_precision..
-00000490: 7d0d 0a0d 0a44 4546 4155 4c54 5f46 4d54  }....DEFAULT_FMT
-000004a0: 5320 3d20 7b0d 0a20 2020 2027 4c4f 5353  S = {..    'LOSS
-000004b0: 273a 2022 2e35 6622 2c0d 0a20 2020 2023  ': ".5f",..    #
-000004c0: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-000004d0: 2020 274d 5345 273a 2022 2e34 6622 2c0d    'MSE': ".4f",.
-000004e0: 0a20 2020 2027 4d41 4527 3a20 222e 3466  .    'MAE': ".4f
-000004f0: 222c 0d0a 2020 2020 2752 4d53 4527 3a20  ",..    'RMSE': 
-00000500: 222e 3466 222c 0d0a 2020 2020 2323 2323  ".4f",..    ####
-00000510: 2323 2323 2323 2323 230d 0a20 2020 2027  #########..    '
-00000520: 5052 4543 4953 494f 4e27 3a20 222e 3466  PRECISION': ".4f
-00000530: 222c 0d0a 2020 2020 2752 4543 414c 4c27  ",..    'RECALL'
-00000540: 3a20 222e 3466 222c 0d0a 2020 2020 2746  : ".4f",..    'F
-00000550: 3127 3a20 222e 3466 222c 0d0a 2020 2020  1': ".4f",..    
-00000560: 2741 5543 273a 2022 2e34 6622 2c0d 0a20  'AUC': ".4f",.. 
-00000570: 2020 2027 4849 5452 4154 4527 3a20 222e     'HITRATE': ".
-00000580: 3466 222c 0d0a 2020 2020 2323 2323 2323  4f",..    ######
-00000590: 2323 2323 2323 230d 0a20 2020 2027 4e44  #######..    'ND
-000005a0: 4347 273a 2022 2e34 6622 2c0d 0a20 2020  CG': ".4f",..   
-000005b0: 2027 4d52 5227 3a20 222e 3466 222c 0d0a   'MRR': ".4f",..
-000005c0: 2020 2020 274d 4150 273a 2022 2e34 6622      'MAP': ".4f"
-000005d0: 2c0d 0a7d 0d0a 0d0a 4445 4641 554c 545f  ,..}....DEFAULT_
-000005e0: 4245 5354 5f43 4153 5445 5220 3d20 7b0d  BEST_CASTER = {.
-000005f0: 0a20 2020 2027 4c4f 5353 273a 206d 696e  .    'LOSS': min
-00000600: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
-00000610: 2323 2323 0d0a 2020 2020 274d 5345 273a  ####..    'MSE':
-00000620: 206d 696e 2c0d 0a20 2020 2027 4d41 4527   min,..    'MAE'
-00000630: 3a20 6d69 6e2c 0d0a 2020 2020 2752 4d53  : min,..    'RMS
-00000640: 4527 3a20 6d69 6e2c 0d0a 2020 2020 2323  E': min,..    ##
-00000650: 2323 2323 2323 2323 2323 230d 0a20 2020  ###########..   
-00000660: 2027 5052 4543 4953 494f 4e27 3a20 6d61   'PRECISION': ma
-00000670: 782c 0d0a 2020 2020 2752 4543 414c 4c27  x,..    'RECALL'
-00000680: 3a20 6d61 782c 0d0a 2020 2020 2746 3127  : max,..    'F1'
-00000690: 3a20 6d61 782c 0d0a 2020 2020 2741 5543  : max,..    'AUC
-000006a0: 273a 206d 6178 2c0d 0a20 2020 2027 4849  ': max,..    'HI
-000006b0: 5452 4154 4527 3a20 6d61 782c 0d0a 2020  TRATE': max,..  
-000006c0: 2020 2323 2323 2323 2323 2323 2323 230d    #############.
-000006d0: 0a20 2020 2027 4e44 4347 273a 206d 6178  .    'NDCG': max
-000006e0: 2c0d 0a20 2020 2027 4d52 5227 3a20 6d61  ,..    'MRR': ma
-000006f0: 782c 0d0a 2020 2020 274d 4150 273a 206d  x,..    'MAP': m
-00000700: 6178 2c0d 0a7d 0d0a 0d0a 0d0a 636c 6173  ax,..}......clas
-00000710: 7320 5f44 756d 6d79 4d6f 6475 6c65 2874  s _DummyModule(t
-00000720: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 293a  orch.nn.Module):
-00000730: 0d0a 2020 2020 2222 2254 6869 7320 6973  ..    """This is
-00000740: 2061 2064 756d 6d79 206d 6f64 756c 6520   a dummy module 
-00000750: 7468 6174 2073 6572 7665 7320 6173 2061  that serves as a
-00000760: 2070 6c61 6365 686f 6c64 6572 2066 6f72   placeholder for
-00000770: 2061 2072 6561 6c20 6d6f 6465 6c2e 2222   a real model.""
-00000780: 220d 0a20 2020 2064 6566 2066 6f72 7761  "..    def forwa
-00000790: 7264 2873 656c 662c 202a 6172 6773 2c20  rd(self, *args, 
-000007a0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-000007b0: 2020 2020 2222 2244 756d 6d79 2066 6f72      """Dummy for
-000007c0: 7761 7264 206d 6574 686f 6420 7468 6174  ward method that
-000007d0: 2072 6169 7365 7320 6120 604e 6f74 496d   raises a `NotIm
-000007e0: 706c 656d 656e 7465 6445 7272 6f72 602e  plementedError`.
-000007f0: 2222 220d 0a20 2020 2020 2020 2072 6169  """..        rai
-00000800: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00000810: 6445 7272 6f72 2822 4e6f 206d 6f64 656c  dError("No model
-00000820: 2061 7661 696c 6162 6c65 2066 6f72 2043   available for C
-00000830: 6f61 6368 202e 2e2e 2229 0d0a 0d0a 2020  oach ...")....  
-00000840: 2020 6465 6620 7374 6570 2873 656c 662c    def step(self,
-00000850: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00000860: 293a 0d0a 2020 2020 2020 2020 2222 2244  ):..        """D
-00000870: 756d 6d79 2073 7465 7020 6d65 7468 6f64  ummy step method
-00000880: 2074 6861 7420 7261 6973 6573 2061 2060   that raises a `
-00000890: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-000008a0: 726f 7260 2e22 2222 0d0a 2020 2020 2020  ror`."""..      
-000008b0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-000008c0: 6d65 6e74 6564 4572 726f 7228 224e 6f20  mentedError("No 
-000008d0: 6f70 7469 6d69 7a65 7220 6f72 206c 7220  optimizer or lr 
-000008e0: 7363 6865 6475 6c65 7220 6176 6169 6c61  scheduler availa
-000008f0: 626c 6520 666f 7220 436f 6163 6820 2e2e  ble for Coach ..
-00000900: 2e22 290d 0a0d 0a20 2020 2064 6566 2062  .")....    def b
-00000910: 6163 6b77 6172 6428 7365 6c66 2c20 2a61  ackward(self, *a
-00000920: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00000930: 0a20 2020 2020 2020 2022 2222 4475 6d6d  .        """Dumm
-00000940: 7920 6261 636b 7761 7264 206d 6574 686f  y backward metho
-00000950: 6420 7468 6174 2072 6169 7365 7320 6120  d that raises a 
-00000960: 604e 6f74 496d 706c 656d 656e 7465 6445  `NotImplementedE
-00000970: 7272 6f72 602e 2222 220d 0a20 2020 2020  rror`."""..     
-00000980: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00000990: 656d 656e 7465 6445 7272 6f72 2822 4e6f  ementedError("No
-000009a0: 206f 7074 696d 697a 6572 2061 7661 696c   optimizer avail
-000009b0: 6162 6c65 2066 6f72 2043 6f61 6368 202e  able for Coach .
-000009c0: 2e2e 2229 0d0a 0d0a 0d0a 636c 6173 7320  ..")......class 
-000009d0: 4368 6965 6643 6f61 6368 286d 6574 6163  ChiefCoach(metac
-000009e0: 6c61 7373 3d61 6263 2e41 4243 4d65 7461  lass=abc.ABCMeta
-000009f0: 293a 0d0a 2020 2020 7222 2222 200d 0a20  ):..    r""" .. 
-00000a00: 2020 2054 6865 2060 4368 6965 6643 6f61     The `ChiefCoa
-00000a10: 6368 6020 636c 6173 7320 6973 2074 6865  ch` class is the
-00000a20: 2074 6f70 2d6c 6576 656c 2063 6c61 7373   top-level class
-00000a30: 2066 6f72 2072 756e 6e69 6e67 2074 6865   for running the
-00000a40: 2074 7261 696e 696e 6720 616e 6420 6576   training and ev
-00000a50: 616c 7561 7469 6f6e 206c 6f6f 7073 2e0d  aluation loops..
-00000a60: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000a70: 733a 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  s:..    --------
-00000a80: 2d2d 2d0d 0a20 2020 2074 7261 696e 7069  ---..    trainpi
-00000a90: 7065 203a 2049 7465 7244 6174 6150 6970  pe : IterDataPip
-00000aa0: 650d 0a20 2020 2020 2020 2049 7465 7261  e..        Itera
-00000ab0: 626c 6520 6461 7461 2070 6970 656c 696e  ble data pipelin
-00000ac0: 6520 666f 7220 7472 6169 6e69 6e67 2064  e for training d
-00000ad0: 6174 612e 0d0a 2020 2020 7661 6c69 6470  ata...    validp
-00000ae0: 6970 6520 3a20 4974 6572 4461 7461 5069  ipe : IterDataPi
-00000af0: 7065 2c20 6f70 7469 6f6e 616c 0d0a 2020  pe, optional..  
-00000b00: 2020 2020 2020 4974 6572 6162 6c65 2064        Iterable d
-00000b10: 6174 6120 7069 7065 6c69 6e65 2066 6f72  ata pipeline for
-00000b20: 2076 616c 6964 6174 696f 6e20 6461 7461   validation data
-00000b30: 2e0d 0a20 2020 2020 2020 2049 6620 604e  ...        If `N
-00000b40: 6f6e 6560 2c20 7573 6520 6074 7261 696e  one`, use `train
-00000b50: 7069 7065 6020 696e 7374 6561 642e 0d0a  pipe` instead...
-00000b60: 2020 2020 7465 7374 7069 7065 203a 2049      testpipe : I
-00000b70: 7465 7244 6174 6150 6970 652c 206f 7074  terDataPipe, opt
-00000b80: 696f 6e61 6c0d 0a20 2020 2020 2020 2049  ional..        I
-00000b90: 7465 7261 626c 6520 6461 7461 2070 6970  terable data pip
-00000ba0: 656c 696e 6520 666f 7220 7465 7374 696e  eline for testin
-00000bb0: 6720 6461 7461 2e0d 0a20 2020 2020 2020  g data...       
-00000bc0: 2049 6620 604e 6f6e 6560 2c20 7573 6520   If `None`, use 
-00000bd0: 6076 616c 6964 7069 7065 6020 696e 7374  `validpipe` inst
-00000be0: 6561 642e 0d0a 2020 2020 6669 656c 6473  ead...    fields
-00000bf0: 203a 2049 7465 7261 626c 655b 4669 656c   : Iterable[Fiel
-00000c00: 644d 6f64 756c 655d 0d0a 2020 2020 2020  dModule]..      
-00000c10: 2020 5475 706c 6520 6f66 2060 4669 656c    Tuple of `Fiel
-00000c20: 644d 6f64 756c 6560 7320 666f 7220 6461  dModule`s for da
-00000c30: 7461 7365 7420 6669 656c 6473 2e0d 0a20  taset fields... 
-00000c40: 2020 206d 6f64 656c 203a 2055 6e69 6f6e     model : Union
-00000c50: 5b52 6563 5379 7341 7263 682c 2074 6f72  [RecSysArch, tor
-00000c60: 6368 2e6e 6e2e 4d6f 6475 6c65 2c20 4e6f  ch.nn.Module, No
-00000c70: 6e65 5d0d 0a20 2020 2020 2020 204d 6f64  ne]..        Mod
-00000c80: 656c 2066 6f72 2074 7261 696e 696e 6720  el for training 
-00000c90: 616e 6420 6576 616c 7561 7469 6e67 2e20  and evaluating. 
-00000ca0: 0d0a 2020 2020 2020 2020 4966 2060 4e6f  ..        If `No
-00000cb0: 6e65 602c 2075 7365 205f 4475 6d6d 794d  ne`, use _DummyM
-00000cc0: 6f64 756c 6520 696e 7374 6561 642c 2077  odule instead, w
-00000cd0: 6869 6368 2073 686f 756c 6420 6e6f 7420  hich should not 
-00000ce0: 6361 6c6c 2060 666f 7277 6172 6460 2e0d  call `forward`..
-00000cf0: 0a20 2020 2063 7269 7465 7269 6f6e 203a  .    criterion :
-00000d00: 2055 6e69 6f6e 5b42 6173 6543 7269 7465   Union[BaseCrite
-00000d10: 7269 6f6e 2c20 4361 6c6c 6162 6c65 5d0d  rion, Callable].
-00000d20: 0a20 2020 2020 2020 2043 616c 6c61 626c  .        Callabl
-00000d30: 6520 666f 7220 636f 6d70 7574 696e 6720  e for computing 
-00000d40: 7468 6520 6c6f 7373 2066 756e 6374 696f  the loss functio
-00000d50: 6e2e 0d0a 2020 2020 6f70 7469 6d69 7a65  n...    optimize
-00000d60: 7220 3a20 746f 7263 682e 6f70 7469 6d2e  r : torch.optim.
-00000d70: 4f70 7469 6d69 7a65 722c 206f 7074 696f  Optimizer, optio
-00000d80: 6e61 6c0d 0a20 2020 2020 2020 204f 7074  nal..        Opt
-00000d90: 696d 697a 6572 2066 6f72 2075 7064 6174  imizer for updat
-00000da0: 696e 6720 6d6f 6465 6c20 7061 7261 6d65  ing model parame
-00000db0: 7465 7273 2e20 0d0a 2020 2020 2020 2020  ters. ..        
-00000dc0: 4966 2060 4e6f 6e65 602c 2075 7365 205f  If `None`, use _
-00000dd0: 4475 6d6d 794d 6f64 756c 6520 696e 7374  DummyModule inst
-00000de0: 6561 642c 2077 6869 6368 2073 686f 756c  ead, which shoul
-00000df0: 6420 6e6f 7420 6361 6c6c 2060 7374 6570  d not call `step
-00000e00: 6020 616e 6420 6062 6163 6b77 6172 6460  ` and `backward`
-00000e10: 2e0d 0a20 2020 206c 725f 7363 6865 6475  ...    lr_schedu
-00000e20: 6c65 7220 3a20 746f 7263 682e 6f70 7469  ler : torch.opti
-00000e30: 6d2e 6c72 5f73 6368 6564 756c 6572 2e5f  m.lr_scheduler._
-00000e40: 4c52 5363 6865 6475 6c65 722c 206f 7074  LRScheduler, opt
-00000e50: 696f 6e61 6c0d 0a20 2020 2020 2020 204c  ional..        L
-00000e60: 6561 726e 696e 6720 7261 7465 2073 6368  earning rate sch
-00000e70: 6564 756c 6572 2e20 4966 2060 4e6f 6e65  eduler. If `None
-00000e80: 602c 2075 7365 205f 4475 6d6d 794d 6f64  `, use _DummyMod
-00000e90: 756c 6520 696e 7374 6561 642c 200d 0a20  ule instead, .. 
-00000ea0: 2020 2020 2020 2077 6869 6368 2073 686f         which sho
-00000eb0: 756c 6420 6e6f 7420 6361 6c6c 2060 7374  uld not call `st
-00000ec0: 6570 602e 0d0a 2020 2020 6465 7669 6365  ep`...    device
-00000ed0: 203a 2055 6e69 6f6e 5b74 6f72 6368 2e64   : Union[torch.d
-00000ee0: 6576 6963 652c 2073 7472 2c20 696e 745d  evice, str, int]
-00000ef0: 0d0a 2020 2020 2020 2020 4465 7669 6365  ..        Device
-00000f00: 206f 6e20 7768 6963 6820 746f 2072 756e   on which to run
-00000f10: 2074 6865 2063 6f6d 7075 7461 7469 6f6e   the computation
-00000f20: 2e20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00000f30: 2d20 6074 6f72 6368 2e64 6576 6963 6560  - `torch.device`
-00000f40: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00000f50: 6073 7472 603a 204c 696b 6520 6063 7075  `str`: Like `cpu
-00000f60: 602c 2060 6375 6461 3a30 602e 0d0a 2020  `, `cuda:0`...  
-00000f70: 2020 2020 2020 2020 2020 2d20 6069 6e74            - `int
-00000f80: 603a 2055 7369 6e67 2063 7564 613a 6069  `: Using cuda:`i
-00000f90: 6e74 602e 0d0a 2020 2020 2222 220d 0a0d  nt`...    """...
-00000fa0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00000fb0: 745f 5f28 0d0a 2020 2020 2020 2020 7365  t__(..        se
-00000fc0: 6c66 2c20 2a2c 0d0a 2020 2020 2020 2020  lf, *,..        
-00000fd0: 7472 6169 6e70 6970 653a 2049 7465 7244  trainpipe: IterD
-00000fe0: 6174 6150 6970 652c 2076 616c 6964 7069  ataPipe, validpi
-00000ff0: 7065 3a20 4f70 7469 6f6e 616c 5b49 7465  pe: Optional[Ite
-00001000: 7244 6174 6150 6970 655d 2c20 7465 7374  rDataPipe], test
-00001010: 7069 7065 3a20 4f70 7469 6f6e 616c 5b49  pipe: Optional[I
-00001020: 7465 7244 6174 6150 6970 655d 2c20 6669  terDataPipe], fi
-00001030: 656c 6473 3a20 4974 6572 6162 6c65 5b46  elds: Iterable[F
-00001040: 6965 6c64 4d6f 6475 6c65 5d2c 0d0a 2020  ieldModule],..  
-00001050: 2020 2020 2020 6d6f 6465 6c3a 2055 6e69        model: Uni
-00001060: 6f6e 5b52 6563 5379 7341 7263 682c 2074  on[RecSysArch, t
-00001070: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 2c20  orch.nn.Module, 
-00001080: 4e6f 6e65 5d2c 2063 7269 7465 7269 6f6e  None], criterion
-00001090: 3a20 556e 696f 6e5b 4261 7365 4372 6974  : Union[BaseCrit
-000010a0: 6572 696f 6e2c 2043 616c 6c61 626c 655d  erion, Callable]
-000010b0: 2c20 0d0a 2020 2020 2020 2020 6f70 7469  , ..        opti
-000010c0: 6d69 7a65 723a 204f 7074 696f 6e61 6c5b  mizer: Optional[
-000010d0: 746f 7263 682e 6f70 7469 6d2e 4f70 7469  torch.optim.Opti
-000010e0: 6d69 7a65 725d 2c20 6c72 5f73 6368 6564  mizer], lr_sched
-000010f0: 756c 6572 3a20 4f70 7469 6f6e 616c 5b74  uler: Optional[t
-00001100: 6f72 6368 2e6f 7074 696d 2e6c 725f 7363  orch.optim.lr_sc
-00001110: 6865 6475 6c65 722e 5f4c 5253 6368 6564  heduler._LRSched
-00001120: 756c 6572 5d2c 0d0a 2020 2020 2020 2020  uler],..        
-00001130: 6465 7669 6365 3a20 556e 696f 6e5b 746f  device: Union[to
-00001140: 7263 682e 6465 7669 6365 2c20 7374 722c  rch.device, str,
-00001150: 2069 6e74 5d0d 0a20 2020 2029 3a0d 0a0d   int]..    ):...
-00001160: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-00001170: 656c 6473 3a20 4669 656c 6454 7570 6c65  elds: FieldTuple
-00001180: 5b46 6965 6c64 4d6f 6475 6c65 5d20 3d20  [FieldModule] = 
-00001190: 4669 656c 6454 7570 6c65 2866 6965 6c64  FieldTuple(field
-000011a0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-000011b0: 2e64 6576 6963 6520 3d20 746f 7263 682e  .device = torch.
-000011c0: 6465 7669 6365 2864 6576 6963 6529 0d0a  device(device)..
-000011d0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000011e0: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
-000011f0: 6375 6461 2e73 6574 5f64 6576 6963 6528  cuda.set_device(
-00001200: 7365 6c66 2e64 6576 6963 6529 0d0a 2020  self.device)..  
-00001210: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-00001220: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
-00001230: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-00001240: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
-00001250: 6275 7465 4572 726f 723a 0d0a 2020 2020  buteError:..    
-00001260: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
-00001270: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-00001280: 745f 6461 7461 7069 7065 2874 7261 696e  t_datapipe(train
-00001290: 7069 7065 2c20 7661 6c69 6470 6970 652c  pipe, validpipe,
-000012a0: 2074 6573 7470 6970 6529 0d0a 2020 2020   testpipe)..    
-000012b0: 2020 2020 7365 6c66 2e5f 7365 745f 6f74      self._set_ot
-000012c0: 6865 7228 6d6f 6465 6c2c 2063 7269 7465  her(model, crite
-000012d0: 7269 6f6e 2c20 6f70 7469 6d69 7a65 722c  rion, optimizer,
-000012e0: 206c 725f 7363 6865 6475 6c65 7229 0d0a   lr_scheduler)..
-000012f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00001300: 5f6d 6f64 6520 3d20 2774 7261 696e 270d  _mode = 'train'.
-00001310: 0a0d 0a20 2020 2020 2020 2064 6566 2063  ...        def c
-00001320: 6c65 616e 2829 3a0d 0a20 2020 2020 2020  lean():..       
-00001330: 2020 2020 2070 6172 656e 7420 3d20 7073       parent = ps
-00001340: 7574 696c 2e50 726f 6365 7373 286f 732e  util.Process(os.
-00001350: 6765 7470 6964 2829 290d 0a20 2020 2020  getpid())..     
-00001360: 2020 2020 2020 2063 6869 6c64 7265 6e20         children 
-00001370: 3d20 7061 7265 6e74 2e63 6869 6c64 7265  = parent.childre
-00001380: 6e28 7265 6375 7273 6976 653d 5472 7565  n(recursive=True
-00001390: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-000013a0: 6f72 2070 726f 6365 7373 2069 6e20 6368  or process in ch
-000013b0: 696c 6472 656e 3a0d 0a20 2020 2020 2020  ildren:..       
-000013c0: 2020 2020 2020 2020 2070 726f 6365 7373           process
-000013d0: 2e73 656e 645f 7369 676e 616c 2873 6967  .send_signal(sig
-000013e0: 6e61 6c2e 5349 4754 4552 4d29 0d0a 2020  nal.SIGTERM)..  
-000013f0: 2020 2020 2020 2020 2020 7073 7574 696c            psutil
-00001400: 2e77 6169 745f 7072 6f63 7328 6368 696c  .wait_procs(chil
-00001410: 6472 656e 2c20 7469 6d65 6f75 743d 3529  dren, timeout=5)
-00001420: 0d0a 0d0a 2020 2020 2020 2020 6174 6578  ....        atex
-00001430: 6974 2e72 6567 6973 7465 7228 636c 6561  it.register(clea
-00001440: 6e29 0d0a 0d0a 0d0a 2020 2020 6465 6620  n)......    def 
-00001450: 5f73 6574 5f64 6174 6170 6970 6528 0d0a  _set_datapipe(..
-00001460: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00001470: 2020 2020 2020 2074 7261 696e 7069 7065         trainpipe
-00001480: 2c0d 0a20 2020 2020 2020 2076 616c 6964  ,..        valid
-00001490: 7069 7065 3d4e 6f6e 652c 0d0a 2020 2020  pipe=None,..    
-000014a0: 2020 2020 7465 7374 7069 7065 3d4e 6f6e      testpipe=Non
-000014b0: 652c 0d0a 2020 2020 293a 0d0a 2020 2020  e,..    ):..    
-000014c0: 2020 2020 2222 2253 6574 2074 6865 2064      """Set the d
-000014d0: 6174 6120 7069 7065 2066 6f72 2074 7261  ata pipe for tra
-000014e0: 696e 696e 672c 2076 616c 6964 6174 696f  ining, validatio
-000014f0: 6e20 616e 6420 7465 7374 2e22 2222 0d0a  n and test."""..
-00001500: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00001510: 696e 7069 7065 203d 2074 7261 696e 7069  inpipe = trainpi
-00001520: 7065 0d0a 2020 2020 2020 2020 7365 6c66  pe..        self
-00001530: 2e76 616c 6964 7069 7065 203d 2073 656c  .validpipe = sel
-00001540: 662e 7472 6169 6e70 6970 6520 6966 2076  f.trainpipe if v
-00001550: 616c 6964 7069 7065 2069 7320 4e6f 6e65  alidpipe is None
-00001560: 2065 6c73 6520 7661 6c69 6470 6970 650d   else validpipe.
-00001570: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
-00001580: 7374 7069 7065 203d 2073 656c 662e 7661  stpipe = self.va
-00001590: 6c69 6470 6970 6520 6966 2074 6573 7470  lidpipe if testp
-000015a0: 6970 6520 6973 204e 6f6e 6520 656c 7365  ipe is None else
-000015b0: 2074 6573 7470 6970 650d 0a0d 0a20 2020   testpipe....   
-000015c0: 2064 6566 205f 7365 745f 6f74 6865 7228   def _set_other(
-000015d0: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
-000015e0: 0a20 2020 2020 2020 206d 6f64 656c 3d4e  .        model=N
-000015f0: 6f6e 652c 2063 7269 7465 7269 6f6e 3d4e  one, criterion=N
-00001600: 6f6e 652c 206f 7074 696d 697a 6572 3d4e  one, optimizer=N
-00001610: 6f6e 652c 206c 725f 7363 6865 6475 6c65  one, lr_schedule
-00001620: 723d 4e6f 6e65 2c0d 0a20 2020 2029 3a0d  r=None,..    ):.
-00001630: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
-00001640: 7468 6520 6f74 6865 7220 6e65 6365 7373  the other necess
-00001650: 6172 7920 636f 6d70 6f6e 656e 7473 2e22  ary components."
-00001660: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001670: 2e63 7269 7465 7269 6f6e 203d 2063 7269  .criterion = cri
-00001680: 7465 7269 6f6e 0d0a 2020 2020 2020 2020  terion..        
-00001690: 7365 6c66 2e6d 6f64 656c 203d 206d 6f64  self.model = mod
-000016a0: 656c 2e74 6f28 7365 6c66 2e64 6576 6963  el.to(self.devic
-000016b0: 6529 2069 6620 6d6f 6465 6c20 656c 7365  e) if model else
-000016c0: 205f 4475 6d6d 794d 6f64 756c 6528 290d   _DummyModule().
-000016d0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-000016e0: 7469 6d69 7a65 7220 3d20 6f70 7469 6d69  timizer = optimi
-000016f0: 7a65 7220 6966 206f 7074 696d 697a 6572  zer if optimizer
-00001700: 2065 6c73 6520 5f44 756d 6d79 4d6f 6475   else _DummyModu
-00001710: 6c65 2829 0d0a 2020 2020 2020 2020 7365  le()..        se
-00001720: 6c66 2e6c 725f 7363 6865 6475 6c65 7220  lf.lr_scheduler 
-00001730: 3d20 6c72 5f73 6368 6564 756c 6572 2069  = lr_scheduler i
-00001740: 6620 6c72 5f73 6368 6564 756c 6572 2065  f lr_scheduler e
-00001750: 6c73 6520 5f44 756d 6d79 4d6f 6475 6c65  lse _DummyModule
-00001760: 2829 0d0a 0d0a 2020 2020 4070 726f 7065  ()....    @prope
-00001770: 7274 790d 0a20 2020 2064 6566 206d 6f64  rty..    def mod
-00001780: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-00001790: 2020 2222 2247 6574 2074 6865 2063 7572    """Get the cur
-000017a0: 7265 6e74 206d 6f64 6520 6f66 2074 6865  rent mode of the
-000017b0: 2063 6869 6566 2063 6f61 6368 2e22 2222   chief coach."""
-000017c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000017d0: 2073 656c 662e 5f5f 6d6f 6465 0d0a 0d0a   self.__mode....
-000017e0: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
-000017f0: 436f 6163 682f 7472 6169 6e22 290d 0a20  Coach/train").. 
-00001800: 2020 2064 6566 2074 7261 696e 2873 656c     def train(sel
-00001810: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
-00001820: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
-00001830: 7420 7472 6169 6e69 6e67 2061 6e64 2072  t training and r
-00001840: 6574 7572 6e20 7468 6520 7472 6169 6e69  eturn the traini
-00001850: 6e67 206c 6f73 732e 2222 220d 0a20 2020  ng loss."""..   
-00001860: 2020 2020 2073 656c 662e 5f5f 6d6f 6465       self.__mode
-00001870: 203d 2027 7472 6169 6e27 0d0a 2020 2020   = 'train'..    
-00001880: 2020 2020 7365 6c66 2e6d 6f64 656c 2e74      self.model.t
-00001890: 7261 696e 2829 0d0a 2020 2020 2020 2020  rain()..        
-000018a0: 7265 7475 726e 2073 656c 662e 7472 6169  return self.trai
-000018b0: 6e5f 7065 725f 6570 6f63 6828 6570 6f63  n_per_epoch(epoc
-000018c0: 6829 0d0a 0d0a 2020 2020 4074 696d 656d  h)....    @timem
-000018d0: 6574 6572 2822 436f 6163 682f 7661 6c69  eter("Coach/vali
-000018e0: 6422 290d 0a20 2020 2040 746f 7263 682e  d")..    @torch.
-000018f0: 6e6f 5f67 7261 6428 290d 0a20 2020 2064  no_grad()..    d
-00001900: 6566 2076 616c 6964 2873 656c 662c 2065  ef valid(self, e
-00001910: 706f 6368 3a20 696e 7429 3a0d 0a20 2020  poch: int):..   
-00001920: 2020 2020 2022 2222 5374 6172 7420 7661       """Start va
-00001930: 6c69 6461 7469 6f6e 2061 6e64 2072 6574  lidation and ret
-00001940: 7572 6e20 7468 6520 7661 6c69 6461 7469  urn the validati
-00001950: 6f6e 206d 6574 7269 6373 2e22 2222 0d0a  on metrics."""..
-00001960: 2020 2020 2020 2020 7365 6c66 2e5f 5f6d          self.__m
-00001970: 6f64 6520 3d20 2776 616c 6964 270d 0a20  ode = 'valid'.. 
-00001980: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-00001990: 6c2e 6576 616c 2829 0d0a 2020 2020 2020  l.eval()..      
-000019a0: 2020 7265 7475 726e 2073 656c 662e 6576    return self.ev
-000019b0: 616c 7561 7465 2865 706f 6368 3d65 706f  aluate(epoch=epo
-000019c0: 6368 2c20 7072 6566 6978 3d27 7661 6c69  ch, prefix='vali
-000019d0: 6427 290d 0a0d 0a20 2020 2040 7469 6d65  d')....    @time
-000019e0: 6d65 7465 7228 2243 6f61 6368 2f74 6573  meter("Coach/tes
-000019f0: 7422 290d 0a20 2020 2040 746f 7263 682e  t")..    @torch.
-00001a00: 6e6f 5f67 7261 6428 290d 0a20 2020 2064  no_grad()..    d
-00001a10: 6566 2074 6573 7428 7365 6c66 2c20 6570  ef test(self, ep
-00001a20: 6f63 683a 2069 6e74 293a 0d0a 2020 2020  och: int):..    
-00001a30: 2020 2020 2222 2253 7461 7274 2074 6573      """Start tes
-00001a40: 7469 6e67 2061 6e64 2072 6574 7572 6e20  ting and return 
-00001a50: 7468 6520 7465 7374 206d 6574 7269 6373  the test metrics
-00001a60: 2e22 2222 0d0a 2020 2020 2020 2020 7365  ."""..        se
-00001a70: 6c66 2e5f 5f6d 6f64 6520 3d20 2774 6573  lf.__mode = 'tes
-00001a80: 7427 0d0a 2020 2020 2020 2020 7365 6c66  t'..        self
-00001a90: 2e6d 6f64 656c 2e65 7661 6c28 290d 0a20  .model.eval().. 
-00001aa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001ab0: 6c66 2e65 7661 6c75 6174 6528 6570 6f63  lf.evaluate(epoc
-00001ac0: 683d 6570 6f63 682c 2070 7265 6669 783d  h=epoch, prefix=
-00001ad0: 2774 6573 7427 290d 0a0d 0a20 2020 2040  'test')....    @
-00001ae0: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
-00001af0: 6f64 0d0a 2020 2020 6465 6620 7472 6169  od..    def trai
-00001b00: 6e5f 7065 725f 6570 6f63 6828 7365 6c66  n_per_epoch(self
-00001b10: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
-00001b20: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00001b30: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00001b40: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-00001b50: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
-00001b60: 5f2e 5f5f 6e61 6d65 5f5f 7d2e 7472 6169  _.__name__}.trai
-00001b70: 6e5f 7065 725f 6570 6f63 6828 2920 7368  n_per_epoch() sh
-00001b80: 6f75 6c64 2062 6520 696d 706c 656d 656e  ould be implemen
-00001b90: 7465 6420 2e2e 2e22 0d0a 2020 2020 2020  ted ..."..      
-00001ba0: 2020 290d 0a0d 0a20 2020 2040 6162 632e    )....    @abc.
-00001bb0: 6162 7374 7261 6374 6d65 7468 6f64 0d0a  abstractmethod..
-00001bc0: 2020 2020 6465 6620 6576 616c 7561 7465      def evaluate
-00001bd0: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
-00001be0: 742c 2070 7265 6669 783a 2073 7472 203d  t, prefix: str =
-00001bf0: 2027 7661 6c69 6427 293a 0d0a 2020 2020   'valid'):..    
-00001c00: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-00001c10: 6c65 6d65 6e74 6564 4572 726f 7228 0d0a  lementedError(..
-00001c20: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
-00001c30: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
-00001c40: 6e61 6d65 5f5f 7d2e 6576 616c 7561 7465  name__}.evaluate
-00001c50: 2829 2073 686f 756c 6420 6265 2069 6d70  () should be imp
-00001c60: 6c65 6d65 6e74 6564 202e 2e2e 220d 0a20  lemented ...".. 
-00001c70: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00001c80: 6465 6620 7265 6769 7374 6572 5f6d 6574  def register_met
-00001c90: 7269 6328 0d0a 2020 2020 2020 2020 7365  ric(..        se
-00001ca0: 6c66 2c20 6e61 6d65 3a20 7374 722c 2066  lf, name: str, f
-00001cb0: 756e 633a 2043 616c 6c61 626c 652c 200d  unc: Callable, .
-00001cc0: 0a20 2020 2020 2020 2066 6d74 3a20 7374  .        fmt: st
-00001cd0: 7220 3d20 272e 3466 272c 2062 6573 745f  r = '.4f', best_
-00001ce0: 6361 7374 6572 3a20 4361 6c6c 6162 6c65  caster: Callable
-00001cf0: 203d 206d 6178 0d0a 2020 2020 2920 2d3e   = max..    ) ->
-00001d00: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00001d10: 7222 2222 0d0a 2020 2020 2020 2020 5265  r"""..        Re
-00001d20: 6769 7374 6572 2061 206d 6574 7269 632e  gister a metric.
-00001d30: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-00001d40: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-00001d60: 2020 2020 6e61 6d65 203a 2073 7472 0d0a      name : str..
-00001d70: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001d80: 636f 6d70 6c65 7465 206e 616d 6520 6f66  complete name of
-00001d90: 2074 6865 206d 6574 7269 632c 2073 7563   the metric, suc
-00001da0: 6820 6173 2060 4c4f 5353 3260 2e0d 0a20  h as `LOSS2`... 
-00001db0: 2020 2020 2020 2020 2020 2054 6865 206e             The n
-00001dc0: 6f74 6174 696f 6e20 6040 6020 7368 6f75  otation `@` shou
-00001dd0: 6c64 206e 6f74 2062 6520 696e 636c 7564  ld not be includ
-00001de0: 6564 2c20 692e 652e 2c20 274c 4f53 5340  ed, i.e., 'LOSS@
-00001df0: 3227 2069 7320 696e 7661 6c69 642e 0d0a  2' is invalid...
-00001e00: 2020 2020 2020 2020 6675 6e63 203a 2043          func : C
-00001e10: 616c 6c61 626c 650d 0a20 2020 2020 2020  allable..       
-00001e20: 2020 2020 2054 6865 2066 756e 6374 696f       The functio
-00001e30: 6e20 746f 2070 726f 6365 7373 2074 6865  n to process the
-00001e40: 2064 6174 6120 666f 7220 7468 6520 6d65   data for the me
-00001e50: 7472 6963 2e0d 0a20 2020 2020 2020 2066  tric...        f
-00001e60: 6d74 203a 2073 7472 2c20 6f70 7469 6f6e  mt : str, option
-00001e70: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-00001e80: 5468 6520 666f 726d 6174 2074 6f20 7573  The format to us
-00001e90: 6520 7768 656e 2070 7269 6e74 696e 6720  e when printing 
-00001ea0: 7468 6520 6d65 7472 6963 2c20 6465 6661  the metric, defa
-00001eb0: 756c 7473 2074 6f20 6027 2e34 6627 602e  ults to `'.4f'`.
-00001ec0: 0d0a 2020 2020 2020 2020 6265 7374 5f63  ..        best_c
-00001ed0: 6173 7465 7220 3a20 4361 6c6c 6162 6c65  aster : Callable
-00001ee0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00001ef0: 2020 2020 2020 2020 4120 6675 6e63 7469          A functi
-00001f00: 6f6e 2075 7365 6420 746f 2063 6173 7420  on used to cast 
-00001f10: 7468 6520 6265 7374 2076 616c 7565 206f  the best value o
-00001f20: 6620 7468 6520 6d65 7472 6963 2c20 6465  f the metric, de
-00001f30: 6661 756c 7473 2074 6f20 606d 6178 602e  faults to `max`.
-00001f40: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00001f50: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
-00001f60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00001f70: 0d0a 2020 2020 2020 2020 4e6f 6e65 0d0a  ..        None..
-00001f80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001f90: 2020 5261 6973 6573 0d0a 2020 2020 2020    Raises..      
-00001fa0: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
-00001fb0: 2020 4173 7365 7274 696f 6e45 7272 6f72    AssertionError
-00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00001fd0: 656e 2060 6e61 6d65 6020 6861 7320 616c  en `name` has al
-00001fe0: 7265 6164 7920 6265 656e 2072 6567 6973  ready been regis
-00001ff0: 7465 7265 6420 6f72 2063 6f6e 7461 696e  tered or contain
-00002000: 7320 7468 6520 6e6f 7461 7469 6f6e 2060  s the notation `
-00002010: 4060 2e0d 0a20 2020 2020 2020 2022 2222  @`...        """
-00002020: 0d0a 0d0a 2020 2020 2020 2020 6e61 6d65  ....        name
-00002030: 203d 206e 616d 652e 7570 7065 7228 290d   = name.upper().
-00002040: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002050: 4445 4641 554c 545f 4d45 5452 4943 532e  DEFAULT_METRICS.
-00002060: 6765 7428 6e61 6d65 2c20 4e6f 6e65 2920  get(name, None) 
-00002070: 6973 204e 6f6e 652c 2066 2254 6865 206d  is None, f"The m
-00002080: 6574 7269 6320 7b6e 616d 657d 2061 6c72  etric {name} alr
-00002090: 6561 6479 2065 7869 7374 7320 2e2e 2e22  eady exists ..."
-000020a0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000020b0: 2027 4027 206e 6f74 2069 6e20 6e61 6d65   '@' not in name
-000020c0: 2c20 6622 5468 6520 6d65 7472 6963 206e  , f"The metric n
-000020d0: 616d 6520 6861 7320 696e 7661 6c69 6420  ame has invalid 
-000020e0: 6e6f 7461 7469 6f6e 206f 6620 6040 2720  notation of `@' 
-000020f0: 2e2e 2e22 0d0a 2020 2020 2020 2020 4445  ..."..        DE
-00002100: 4641 554c 545f 4d45 5452 4943 535b 6e61  FAULT_METRICS[na
-00002110: 6d65 5d20 3d20 6675 6e63 0d0a 2020 2020  me] = func..    
-00002120: 2020 2020 4445 4641 554c 545f 464d 5453      DEFAULT_FMTS
-00002130: 5b6e 616d 655d 203d 2066 6d74 0d0a 2020  [name] = fmt..  
-00002140: 2020 2020 2020 4445 4641 554c 545f 4245        DEFAULT_BE
-00002150: 5354 5f43 4153 5445 525b 6e61 6d65 5d20  ST_CASTER[name] 
-00002160: 3d20 6265 7374 5f63 6173 7465 720d 0a0d  = best_caster...
-00002170: 0a0d 0a63 6c61 7373 2043 6f61 6368 2843  ...class Coach(C
-00002180: 6869 6566 436f 6163 6829 3a0d 0a20 2020  hiefCoach):..   
-00002190: 2022 2222 5468 6520 6672 616d 6577 6f72   """The framewor
-000021a0: 6b20 666f 7220 7472 6169 6e69 6e67 2e22  k for training."
-000021b0: 2222 0d0a 0d0a 2020 2020 6465 6620 7072  ""....    def pr
-000021c0: 6570 6172 655f 6461 7461 6c6f 6164 6572  epare_dataloader
-000021d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
-000021e0: 0a20 2020 2020 2020 2022 2222 5072 6570  .        """Prep
-000021f0: 6172 6520 6461 7461 206c 6f61 6465 7273  are data loaders
-00002200: 2066 6f72 2074 7261 696e 696e 672c 2076   for training, v
-00002210: 616c 6964 6174 696f 6e2c 2061 6e64 2074  alidation, and t
-00002220: 6573 7469 6e67 2064 6174 612e 2222 220d  esting data.""".
-00002230: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
-00002240: 6169 6e6c 6f61 6465 7220 3d20 4461 7461  ainloader = Data
-00002250: 4c6f 6164 6572 280d 0a20 2020 2020 2020  Loader(..       
-00002260: 2020 2020 2064 6174 6170 6970 653d 7365       datapipe=se
-00002270: 6c66 2e74 7261 696e 7069 7065 2c20 0d0a  lf.trainpipe, ..
-00002280: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00002290: 776f 726b 6572 733d 7365 6c66 2e63 6667  workers=self.cfg
-000022a0: 2e6e 756d 5f77 6f72 6b65 7273 2c0d 0a20  .num_workers,.. 
-000022b0: 2020 2020 2020 2020 2020 2070 696e 5f6d             pin_m
-000022c0: 656d 6f72 793d 7365 6c66 2e63 6667 2e70  emory=self.cfg.p
-000022d0: 696e 5f6d 656d 6f72 790d 0a20 2020 2020  in_memory..     
-000022e0: 2020 2029 0d0a 2020 2020 2020 2020 7365     )..        se
-000022f0: 6c66 2e76 616c 6964 6c6f 6164 6572 203d  lf.validloader =
-00002300: 2044 6174 614c 6f61 6465 7228 0d0a 2020   DataLoader(..  
-00002310: 2020 2020 2020 2020 2020 6461 7461 7069            datapi
-00002320: 7065 3d73 656c 662e 7661 6c69 6470 6970  pe=self.validpip
-00002330: 652c 200d 0a20 2020 2020 2020 2020 2020  e, ..           
-00002340: 206e 756d 5f77 6f72 6b65 7273 3d73 656c   num_workers=sel
-00002350: 662e 6366 672e 6e75 6d5f 776f 726b 6572  f.cfg.num_worker
-00002360: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00002370: 7069 6e5f 6d65 6d6f 7279 3d73 656c 662e  pin_memory=self.
-00002380: 6366 672e 7069 6e5f 6d65 6d6f 7279 0d0a  cfg.pin_memory..
-00002390: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000023a0: 2020 2073 656c 662e 7465 7374 6c6f 6164     self.testload
-000023b0: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
-000023c0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000023d0: 7461 7069 7065 3d73 656c 662e 7465 7374  tapipe=self.test
-000023e0: 7069 7065 2c20 0d0a 2020 2020 2020 2020  pipe, ..        
-000023f0: 2020 2020 6e75 6d5f 776f 726b 6572 733d      num_workers=
-00002400: 7365 6c66 2e63 6667 2e6e 756d 5f77 6f72  self.cfg.num_wor
-00002410: 6b65 7273 2c0d 0a20 2020 2020 2020 2020  kers,..         
-00002420: 2020 2070 696e 5f6d 656d 6f72 793d 7365     pin_memory=se
-00002430: 6c66 2e63 6667 2e70 696e 5f6d 656d 6f72  lf.cfg.pin_memor
-00002440: 790d 0a20 2020 2020 2020 2029 0d0a 2020  y..        )..  
-00002450: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-00002460: 790d 0a20 2020 2064 6566 2064 6174 616c  y..    def datal
-00002470: 6f61 6465 7228 7365 6c66 293a 0d0a 2020  oader(self):..  
-00002480: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00002490: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-000024a0: 6720 6461 7461 206c 6f61 6465 7220 6465  g data loader de
-000024b0: 7065 6e64 696e 6720 6f6e 2074 6865 2063  pending on the c
-000024c0: 7572 7265 6e74 206d 6f64 652e 2222 220d  urrent mode.""".
-000024d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000024e0: 2e6d 6f64 6520 3d3d 2027 7472 6169 6e27  .mode == 'train'
-000024f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00002500: 6574 7572 6e20 7365 6c66 2e74 7261 696e  eturn self.train
-00002510: 6c6f 6164 6572 0d0a 2020 2020 2020 2020  loader..        
-00002520: 656c 6966 2073 656c 662e 6d6f 6465 203d  elif self.mode =
-00002530: 3d20 2776 616c 6964 273a 0d0a 2020 2020  = 'valid':..    
-00002540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002550: 656c 662e 7661 6c69 646c 6f61 6465 720d  elf.validloader.
-00002560: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002570: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002580: 726e 2073 656c 662e 7465 7374 6c6f 6164  rn self.testload
-00002590: 6572 0d0a 0d0a 2020 2020 4070 726f 7065  er....    @prope
-000025a0: 7274 790d 0a20 2020 2064 6566 206d 6f6e  rty..    def mon
-000025b0: 6974 6f72 7328 7365 6c66 2920 2d3e 204d  itors(self) -> M
-000025c0: 6f6e 6974 6f72 3a0d 0a20 2020 2020 2020  onitor:..       
-000025d0: 2022 2222 5265 7475 726e 2074 6865 206d   """Return the m
-000025e0: 6f6e 6974 6f72 2064 6963 7469 6f6e 6172  onitor dictionar
-000025f0: 7920 666f 7220 7468 6520 6469 6666 6572  y for the differ
-00002600: 656e 7420 6d6f 6465 7320 2827 7472 6169  ent modes ('trai
-00002610: 6e27 2c20 2776 616c 6964 272c 2027 7465  n', 'valid', 'te
-00002620: 7374 2729 2e22 2222 0d0a 2020 2020 2020  st')."""..      
-00002630: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00002640: 6d6f 6e69 746f 7273 0d0a 0d0a 2020 2020  monitors....    
-00002650: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-00002660: 6566 206d 6574 6572 3462 6573 7428 7365  ef meter4best(se
-00002670: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00002680: 7475 726e 2073 656c 662e 5f5f 6265 7374  turn self.__best
-00002690: 5f6d 6574 6572 0d0a 0d0a 2020 2020 406d  _meter....    @m
-000026a0: 6574 6572 3462 6573 742e 7365 7474 6572  eter4best.setter
-000026b0: 0d0a 2020 2020 6465 6620 6d65 7465 7234  ..    def meter4
-000026c0: 6265 7374 2873 656c 662c 206d 6574 6572  best(self, meter
-000026d0: 3a20 4176 6572 6167 654d 6574 6572 293a  : AverageMeter):
-000026e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000026f0: 5f62 6573 745f 6d65 7465 7220 3d20 6d65  _best_meter = me
-00002700: 7465 720d 0a20 2020 2020 2020 2069 6e66  ter..        inf
-00002710: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
-00002720: 5d20 3e3e 3e20 5365 7420 6265 7374 206d  ] >>> Set best m
-00002730: 6574 6572 3a20 7b6d 6574 6572 2e6e 616d  eter: {meter.nam
-00002740: 657d 2022 290d 0a0d 0a20 2020 2040 7469  e} ")....    @ti
-00002750: 6d65 6d65 7465 7228 2243 6f61 6368 2f63  memeter("Coach/c
-00002760: 6f6d 7069 6c65 2229 0d0a 2020 2020 6465  ompile")..    de
-00002770: 6620 636f 6d70 696c 6528 0d0a 2020 2020  f compile(..    
-00002780: 2020 2020 7365 6c66 2c20 6366 673a 2043      self, cfg: C
-00002790: 6f6e 6669 672c 206d 6f6e 6974 6f72 733a  onfig, monitors:
-000027a0: 204c 6973 745b 7374 725d 2c20 0d0a 2020   List[str], ..  
-000027b0: 2020 2020 2020 7768 6963 6834 6265 7374        which4best
-000027c0: 3a20 7374 7220 3d20 274c 4f53 5327 0d0a  : str = 'LOSS'..
-000027d0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-000027e0: 7222 2222 0d0a 2020 2020 2020 2020 4c6f  r"""..        Lo
-000027f0: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
-00002800: 7469 6f6e 2061 6e64 2073 6574 2075 7020  tion and set up 
-00002810: 6d6f 6e69 746f 7273 2066 6f72 2074 7261  monitors for tra
-00002820: 696e 696e 672e 0d0a 0d0a 2020 2020 2020  ining.....      
-00002830: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00002840: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00002850: 0d0a 2020 2020 2020 2020 6366 6720 3a20  ..        cfg : 
-00002860: 436f 6e66 6967 0d0a 2020 2020 2020 2020  Config..        
-00002870: 2020 2020 4120 636f 6e66 6967 7572 6174      A configurat
-00002880: 696f 6e20 6f62 6a65 6374 2077 6974 6820  ion object with 
-00002890: 7468 6520 7472 6169 6e69 6e67 2064 6574  the training det
-000028a0: 6169 6c73 2e0d 0a20 2020 2020 2020 206d  ails...        m
-000028b0: 6f6e 6974 6f72 7320 3a20 4c69 7374 5b73  onitors : List[s
-000028c0: 7472 5d0d 0a20 2020 2020 2020 2020 2020  tr]..           
-000028d0: 2041 206c 6973 7420 6f66 206d 6574 7269   A list of metri
-000028e0: 6320 6e61 6d65 7320 746f 2062 6520 6d6f  c names to be mo
-000028f0: 6e69 746f 7265 6420 6475 7269 6e67 2074  nitored during t
-00002900: 7261 696e 696e 672e 0d0a 2020 2020 2020  raining...      
-00002910: 2020 7768 6963 6834 6265 7374 203a 2073    which4best : s
-00002920: 7472 2c20 6465 6661 756c 7473 2060 4c4f  tr, defaults `LO
-00002930: 5353 270d 0a20 2020 2020 2020 2020 2020  SS'..           
-00002940: 2054 6865 206d 6574 7269 6320 7573 6564   The metric used
-00002950: 2066 6f72 2073 656c 6563 7469 6e67 2074   for selecting t
-00002960: 6865 2062 6573 7420 6368 6563 6b70 6f69  he best checkpoi
-00002970: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2045  nt.....        E
-00002980: 7861 6d70 6c65 730d 0a20 2020 2020 2020  xamples..       
-00002990: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
-000029a0: 2020 203e 3e3e 2063 6f61 6368 3a20 436f     >>> coach: Co
-000029b0: 6163 680d 0a20 2020 2020 2020 203e 3e3e  ach..        >>>
-000029c0: 2063 6f61 6368 2e63 6f6d 7069 6c65 2863   coach.compile(c
-000029d0: 6667 2c20 6d6f 6e69 746f 7273 3d5b 276c  fg, monitors=['l
-000029e0: 6f73 7327 2c20 2772 6563 616c 6c40 3130  oss', 'recall@10
-000029f0: 272c 2027 7265 6361 6c6c 4032 3027 2c20  ', 'recall@20', 
-00002a00: 276e 6463 6740 3130 272c 2027 6e64 6367  'ndcg@10', 'ndcg
-00002a10: 4032 3027 5d29 0d0a 2020 2020 2020 2020  @20'])..        
-00002a20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00002a30: 662e 6366 6720 3d20 6366 670d 0a20 2020  f.cfg = cfg..   
-00002a40: 2020 2020 2023 206d 6574 6572 7320 666f       # meters fo
-00002a50: 7220 7472 6169 6e7c 7661 6c69 647c 7465  r train|valid|te
-00002a60: 7374 0d0a 2020 2020 2020 2020 7365 6c66  st..        self
-00002a70: 2e5f 5f6d 6f6e 6974 6f72 7320 3d20 4d6f  .__monitors = Mo
-00002a80: 6e69 746f 7228 290d 0a20 2020 2020 2020  nitor()..       
-00002a90: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
-00002aa0: 5b27 7472 6169 6e27 5d20 3d20 6465 6661  ['train'] = defa
-00002ab0: 756c 7464 6963 7428 6c69 7374 290d 0a20  ultdict(list).. 
-00002ac0: 2020 2020 2020 2073 656c 662e 5f5f 6d6f         self.__mo
-00002ad0: 6e69 746f 7273 5b27 7661 6c69 6427 5d20  nitors['valid'] 
-00002ae0: 3d20 6465 6661 756c 7464 6963 7428 6c69  = defaultdict(li
-00002af0: 7374 290d 0a20 2020 2020 2020 2073 656c  st)..        sel
-00002b00: 662e 5f5f 6d6f 6e69 746f 7273 5b27 7465  f.__monitors['te
-00002b10: 7374 275d 203d 2064 6566 6175 6c74 6469  st'] = defaultdi
-00002b20: 6374 286c 6973 7429 0d0a 0d0a 2020 2020  ct(list)....    
-00002b30: 2020 2020 6465 6620 7365 745f 6d6f 6e69      def set_moni
-00002b40: 746f 7228 0d0a 2020 2020 2020 2020 2020  tor(..          
-00002b50: 2020 6e61 6d65 3a20 7374 722c 206c 6173    name: str, las
-00002b60: 746e 616d 653a 2073 7472 2c20 7072 6566  tname: str, pref
-00002b70: 6978 3a20 7374 7220 3d20 2774 7261 696e  ix: str = 'train
-00002b80: 272c 202a 2a6b 7761 7267 730d 0a20 2020  ', **kwargs..   
-00002b90: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00002ba0: 2020 2020 2022 2222 4164 6420 6120 6d6f       """Add a mo
-00002bb0: 6e69 746f 7220 666f 7220 7468 6520 7370  nitor for the sp
-00002bc0: 6563 6966 6965 6420 6d65 7472 6963 2e22  ecified metric."
-00002bd0: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
-00002be0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00002bf0: 2020 2020 2020 6d65 7465 7220 3d20 4176        meter = Av
-00002c00: 6572 6167 654d 6574 6572 280d 0a20 2020  erageMeter(..   
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 2020 206e 616d 653d 6e61 6d65 2c0d       name=name,.
-00002c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c40: 2020 2020 2020 2020 206d 6574 7269 633d           metric=
-00002c50: 7061 7274 6961 6c28 4445 4641 554c 545f  partial(DEFAULT_
-00002c60: 4d45 5452 4943 535b 6c61 7374 6e61 6d65  METRICS[lastname
-00002c70: 5d2c 202a 2a6b 7761 7267 7329 2c0d 0a20  ], **kwargs),.. 
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2020 2020 2066 6d74 3d44 4546 4155         fmt=DEFAU
-00002ca0: 4c54 5f46 4d54 535b 6c61 7374 6e61 6d65  LT_FMTS[lastname
-00002cb0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00002cc0: 2020 2020 2020 2020 2020 2020 6265 7374              best
-00002cd0: 5f63 6173 7465 723d 4445 4641 554c 545f  _caster=DEFAULT_
-00002ce0: 4245 5354 5f43 4153 5445 525b 6c61 7374  BEST_CASTER[last
-00002cf0: 6e61 6d65 5d0d 0a20 2020 2020 2020 2020  name]..         
-00002d00: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00002d10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002d20: 6c66 2e5f 5f6d 6f6e 6974 6f72 735b 7072  lf.__monitors[pr
-00002d30: 6566 6978 5d5b 6c61 7374 6e61 6d65 5d2e  efix][lastname].
-00002d40: 6170 7065 6e64 286d 6574 6572 290d 0a20  append(meter).. 
-00002d50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00002d60: 7420 4b65 7945 7272 6f72 3a0d 0a20 2020  t KeyError:..   
-00002d70: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00002d80: 7365 204b 6579 4572 726f 7228 0d0a 2020  se KeyError(..  
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 6622 5468 6520 6d65 7472 6963 206f    f"The metric o
-00002db0: 6620 7b6c 6173 746e 616d 657d 2069 7320  f {lastname} is 
-00002dc0: 6e6f 7420 696e 636c 7564 6564 2e20 220d  not included. ".
-00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002de0: 2020 2020 2066 2259 6f75 2063 616e 2072       f"You can r
-00002df0: 6567 6973 7465 7220 6279 2063 616c 6c69  egister by calli
-00002e00: 6e67 2060 7265 6769 7374 6572 5f6d 6574  ng `register_met
-00002e10: 7269 6328 2e2e 2e29 2720 2e2e 2e22 0d0a  ric(...)' ..."..
-00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00002e40: 6574 7572 6e20 6d65 7465 720d 0a0d 0a20  eturn meter.... 
-00002e50: 2020 2020 2020 2023 2055 5050 4552 0d0a         # UPPER..
-00002e60: 2020 2020 2020 2020 7768 6963 6834 6265          which4be
-00002e70: 7374 203d 2077 6869 6368 3462 6573 742e  st = which4best.
-00002e80: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
-00002e90: 206d 6f6e 6974 6f72 7320 3d20 5b27 4c4f   monitors = ['LO
-00002ea0: 5353 275d 202b 205b 6e61 6d65 2e75 7070  SS'] + [name.upp
-00002eb0: 6572 2829 2066 6f72 206e 616d 6520 696e  er() for name in
-00002ec0: 206d 6f6e 6974 6f72 735d 202b 205b 7768   monitors] + [wh
-00002ed0: 6963 6834 6265 7374 5d0d 0a20 2020 2020  ich4best]..     
-00002ee0: 2020 206d 6f6e 6974 6f72 7320 3d20 736f     monitors = so
-00002ef0: 7274 6564 2873 6574 286d 6f6e 6974 6f72  rted(set(monitor
-00002f00: 7329 2c20 6b65 793d 6d6f 6e69 746f 7273  s), key=monitors
-00002f10: 2e69 6e64 6578 290d 0a0d 0a20 2020 2020  .index)....     
-00002f20: 2020 2066 6f72 206e 616d 6520 696e 206d     for name in m
-00002f30: 6f6e 6974 6f72 733a 0d0a 2020 2020 2020  onitors:..      
-00002f40: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
-00002f50: 2069 6e20 2827 7472 6169 6e27 2c20 2776   in ('train', 'v
-00002f60: 616c 6964 272c 2027 7465 7374 2729 3a0d  alid', 'test'):.
-00002f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f80: 2069 6620 2740 2720 696e 206e 616d 653a   if '@' in name:
-00002f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002fa0: 2020 2020 2020 6c61 7374 6e61 6d65 2c20        lastname, 
-00002fb0: 4b20 3d20 6e61 6d65 2e73 706c 6974 2827  K = name.split('
-00002fc0: 4027 290d 0a20 2020 2020 2020 2020 2020  @')..           
-00002fd0: 2020 2020 2020 2020 206d 6574 6572 203d           meter =
-00002fe0: 2073 6574 5f6d 6f6e 6974 6f72 280d 0a20   set_monitor(.. 
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003000: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-00003010: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003020: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
-00003030: 616d 653d 6c61 7374 6e61 6d65 2c0d 0a20  ame=lastname,.. 
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 2070 7265 6669 783d 7072         prefix=pr
-00003060: 6566 6978 2c0d 0a20 2020 2020 2020 2020  efix,..         
-00003070: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00003080: 3d69 6e74 284b 290d 0a20 2020 2020 2020  =int(K)..       
-00003090: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000030c0: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
-000030d0: 616d 6520 3d20 6e61 6d65 0d0a 2020 2020  ame = name..    
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 6d65 7465 7220 3d20 7365 745f 6d6f 6e69  meter = set_moni
-00003100: 746f 7228 0d0a 2020 2020 2020 2020 2020  tor(..          
-00003110: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00003120: 6d65 3d6e 616d 652c 0d0a 2020 2020 2020  me=name,..      
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 6c61 7374 6e61 6d65 3d6c 6173 746e    lastname=lastn
-00003150: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
-00003160: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00003170: 6566 6978 3d70 7265 6669 780d 0a20 2020  efix=prefix..   
-00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003190: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000031a0: 2020 2020 6966 2070 7265 6669 7820 3d3d      if prefix ==
-000031b0: 2027 7661 6c69 6427 2061 6e64 206e 616d   'valid' and nam
-000031c0: 6520 3d3d 2077 6869 6368 3462 6573 743a  e == which4best:
-000031d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000031e0: 2020 2020 2020 7365 6c66 2e6d 6574 6572        self.meter
-000031f0: 3462 6573 7420 3d20 6d65 7465 720d 0a20  4best = meter.. 
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 2073 656c 662e 5f62 6573 7420 3d20     self._best = 
-00003220: 2d66 6c6f 6174 2827 696e 6627 2920 6966  -float('inf') if
-00003230: 206d 6574 6572 2e63 6173 7465 7220 6973   meter.caster is
-00003240: 206d 6178 2065 6c73 6520 666c 6f61 7428   max else float(
-00003250: 2769 6e66 2729 0d0a 2020 2020 2020 2020  'inf')..        
-00003260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003270: 2e5f 6265 7374 5f65 706f 6368 203d 2030  ._best_epoch = 0
-00003280: 0d0a 0d0a 2020 2020 2020 2020 2320 5072  ....        # Pr
-00003290: 6570 6172 6520 6461 7461 206c 6f61 6465  epare data loade
-000032a0: 7273 0d0a 2020 2020 2020 2020 7365 6c66  rs..        self
-000032b0: 2e70 7265 7061 7265 5f64 6174 616c 6f61  .prepare_dataloa
-000032c0: 6465 7228 290d 0a0d 0a20 2020 2064 6566  der()....    def
-000032d0: 2073 6176 6528 7365 6c66 2920 2d3e 204e   save(self) -> N
-000032e0: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-000032f0: 2253 6176 6520 7468 6520 6d6f 6465 6c22  "Save the model"
-00003300: 2222 0d0a 2020 2020 2020 2020 746f 7263  ""..        torc
-00003310: 682e 7361 7665 2873 656c 662e 6d6f 6465  h.save(self.mode
-00003320: 6c2e 7374 6174 655f 6469 6374 2829 2c20  l.state_dict(), 
-00003330: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00003340: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00003350: 7365 6c66 2e63 6667 2e53 4156 4544 5f46  self.cfg.SAVED_F
-00003360: 494c 454e 414d 4529 290d 0a0d 0a20 2020  ILENAME))....   
-00003370: 2064 6566 206c 6f61 6428 7365 6c66 2c20   def load(self, 
-00003380: 7061 7468 3a20 7374 722c 2066 696c 656e  path: str, filen
-00003390: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-000033a0: 725d 203d 204e 6f6e 652c 202a 2a6b 7761  r] = None, **kwa
-000033b0: 7267 7329 202d 3e20 4e6f 6e65 3a0d 0a20  rgs) -> None:.. 
-000033c0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-000033d0: 3d20 7365 6c66 2e63 6667 2e53 4156 4544  = self.cfg.SAVED
-000033e0: 5f46 494c 454e 414d 4520 6966 2066 696c  _FILENAME if fil
-000033f0: 656e 616d 6520 6973 204e 6f6e 6520 656c  ename is None el
-00003400: 7365 2066 696c 656e 616d 650d 0a20 2020  se filename..   
-00003410: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
-00003420: 6c6f 6164 5f73 7461 7465 5f64 6963 7428  load_state_dict(
-00003430: 746f 7263 682e 6c6f 6164 286f 732e 7061  torch.load(os.pa
-00003440: 7468 2e6a 6f69 6e28 7061 7468 2c20 6669  th.join(path, fi
-00003450: 6c65 6e61 6d65 292c 202a 2a6b 7761 7267  lename), **kwarg
-00003460: 7329 290d 0a0d 0a20 2020 2064 6566 2073  s))....    def s
-00003470: 6176 655f 6368 6563 6b70 6f69 6e74 2873  ave_checkpoint(s
-00003480: 656c 662c 2065 706f 6368 3a20 696e 7429  elf, epoch: int)
-00003490: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-000034a0: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
-000034b0: 2053 6176 6520 6375 7272 656e 7420 6368   Save current ch
-000034c0: 6563 6b70 6f69 6e74 2061 7420 6570 6f63  eckpoint at epoc
-000034d0: 682e 0d0a 0d0a 2020 2020 2020 2020 5061  h.....        Pa
-000034e0: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
-000034f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a     -----------..
-00003500: 2020 2020 2020 2020 2020 2020 6570 6f63              epoc
-00003510: 6820 3a69 6e74 2043 7572 7265 6e74 2065  h :int Current e
-00003520: 706f 6368 206e 756d 6265 722e 0d0a 0d0a  poch number.....
-00003530: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00003540: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00003550: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
-00003560: 4e6f 6e65 0d0a 2020 2020 2020 2020 2222  None..        ""
-00003570: 220d 0a20 2020 2020 2020 2070 6174 6820  "..        path 
-00003580: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-00003590: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
-000035a0: 4e54 5f50 4154 482c 2073 656c 662e 6366  NT_PATH, self.cf
-000035b0: 672e 4348 4543 4b50 4f49 4e54 5f46 494c  g.CHECKPOINT_FIL
-000035c0: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
-000035d0: 6368 6563 6b70 6f69 6e74 203d 2064 6963  checkpoint = dic
-000035e0: 7428 290d 0a20 2020 2020 2020 2063 6865  t()..        che
-000035f0: 636b 706f 696e 745b 2765 706f 6368 275d  ckpoint['epoch']
-00003600: 203d 2065 706f 6368 0d0a 2020 2020 2020   = epoch..      
-00003610: 2020 666f 7220 6d6f 6475 6c65 2069 6e20    for module in 
-00003620: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
-00003630: 494e 545f 4d4f 4455 4c45 533a 0d0a 2020  INT_MODULES:..  
-00003640: 2020 2020 2020 2020 2020 6368 6563 6b70            checkp
-00003650: 6f69 6e74 5b6d 6f64 756c 655d 203d 2067  oint[module] = g
-00003660: 6574 6174 7472 2873 656c 662c 206d 6f64  etattr(self, mod
-00003670: 756c 6529 2e73 7461 7465 5f64 6963 7428  ule).state_dict(
-00003680: 290d 0a20 2020 2020 2020 2063 6865 636b  )..        check
-00003690: 706f 696e 745b 276d 6f6e 6974 6f72 7327  point['monitors'
-000036a0: 5d20 3d20 7365 6c66 2e6d 6f6e 6974 6f72  ] = self.monitor
-000036b0: 732e 7374 6174 655f 6469 6374 2829 0d0a  s.state_dict()..
-000036c0: 2020 2020 2020 2020 746f 7263 682e 7361          torch.sa
-000036d0: 7665 2863 6865 636b 706f 696e 742c 2070  ve(checkpoint, p
-000036e0: 6174 6829 0d0a 0d0a 2020 2020 6465 6620  ath)....    def 
-000036f0: 6c6f 6164 5f63 6865 636b 706f 696e 7428  load_checkpoint(
-00003700: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
-00003710: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
-00003720: 2020 2020 204c 6f61 6420 6c61 7374 2073       Load last s
-00003730: 6176 6564 2063 6865 636b 706f 696e 742e  aved checkpoint.
-00003740: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00003750: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
-00003760: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00003770: 6570 6f63 683a 2069 6e74 200d 0a20 2020  epoch: int ..   
-00003780: 2020 2020 2020 2020 2054 6865 2065 706f           The epo
-00003790: 6368 206e 756d 6265 7220 6c6f 6164 6564  ch number loaded
-000037a0: 2066 726f 6d20 7468 6520 6368 6563 6b70   from the checkp
-000037b0: 6f69 6e74 2e0d 0a20 2020 2020 2020 2022  oint...        "
-000037c0: 2222 0d0a 2020 2020 2020 2020 7061 7468  ""..        path
-000037d0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000037e0: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
-000037f0: 494e 545f 5041 5448 2c20 7365 6c66 2e63  INT_PATH, self.c
-00003800: 6667 2e43 4845 434b 504f 494e 545f 4649  fg.CHECKPOINT_FI
-00003810: 4c45 4e41 4d45 290d 0a20 2020 2020 2020  LENAME)..       
-00003820: 2063 6865 636b 706f 696e 7420 3d20 746f   checkpoint = to
-00003830: 7263 682e 6c6f 6164 2870 6174 6829 0d0a  rch.load(path)..
-00003840: 2020 2020 2020 2020 666f 7220 6d6f 6475          for modu
-00003850: 6c65 2069 6e20 7365 6c66 2e63 6667 2e43  le in self.cfg.C
-00003860: 4845 434b 504f 494e 545f 4d4f 4455 4c45  HECKPOINT_MODULE
-00003870: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
-00003880: 6765 7461 7474 7228 7365 6c66 2c20 6d6f  getattr(self, mo
-00003890: 6475 6c65 292e 6c6f 6164 5f73 7461 7465  dule).load_state
-000038a0: 5f64 6963 7428 6368 6563 6b70 6f69 6e74  _dict(checkpoint
-000038b0: 5b6d 6f64 756c 655d 290d 0a20 2020 2020  [module])..     
-000038c0: 2020 2073 656c 662e 6d6f 6e69 746f 7273     self.monitors
-000038d0: 2e6c 6f61 645f 7374 6174 655f 6469 6374  .load_state_dict
-000038e0: 2863 6865 636b 706f 696e 745b 276d 6f6e  (checkpoint['mon
-000038f0: 6974 6f72 7327 5d29 0d0a 2020 2020 2020  itors'])..      
-00003900: 2020 7265 7475 726e 2063 6865 636b 706f    return checkpo
-00003910: 696e 745b 2765 706f 6368 275d 0d0a 0d0a  int['epoch']....
-00003920: 2020 2020 6465 6620 7361 7665 5f62 6573      def save_bes
-00003930: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-00003940: 0d0a 2020 2020 2020 2020 746f 7263 682e  ..        torch.
-00003950: 7361 7665 2873 656c 662e 6d6f 6465 6c2e  save(self.model.
-00003960: 7374 6174 655f 6469 6374 2829 2c20 6f73  state_dict(), os
-00003970: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00003980: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
-00003990: 6c66 2e63 6667 2e42 4553 545f 4649 4c45  lf.cfg.BEST_FILE
-000039a0: 4e41 4d45 2929 0d0a 0d0a 2020 2020 6465  NAME))....    de
-000039b0: 6620 6c6f 6164 5f62 6573 7428 7365 6c66  f load_best(self
-000039c0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-000039d0: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
-000039e0: 225b 436f 6163 685d 203e 3e3e 204c 6f61  "[Coach] >>> Loa
-000039f0: 6420 6265 7374 206d 6f64 656c 2040 4570  d best model @Ep
-00003a00: 6f63 6820 7b73 656c 662e 5f62 6573 745f  och {self._best_
-00003a10: 6570 6f63 683a 3c34 647d 2022 290d 0a20  epoch:<4d} ").. 
-00003a20: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-00003a30: 6c2e 6c6f 6164 5f73 7461 7465 5f64 6963  l.load_state_dic
-00003a40: 7428 746f 7263 682e 6c6f 6164 286f 732e  t(torch.load(os.
-00003a50: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00003a60: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
-00003a70: 662e 6366 672e 4245 5354 5f46 494c 454e  f.cfg.BEST_FILEN
-00003a80: 414d 4529 2929 0d0a 0d0a 2020 2020 6465  AME)))....    de
-00003a90: 6620 6368 6563 6b5f 6265 7374 2873 656c  f check_best(sel
-00003aa0: 662c 2065 706f 6368 3a20 696e 7429 202d  f, epoch: int) -
-00003ab0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00003ac0: 2022 2222 5570 6461 7465 2062 6573 7420   """Update best 
-00003ad0: 7661 6c75 652e 2222 220d 0a20 2020 2020  value."""..     
-00003ae0: 2020 2069 6620 7365 6c66 2e6d 6574 6572     if self.meter
-00003af0: 3462 6573 742e 6163 7469 7665 3a0d 0a20  4best.active:.. 
-00003b00: 2020 2020 2020 2020 2020 2062 6573 745f             best_
-00003b10: 203d 2073 656c 662e 6d65 7465 7234 6265   = self.meter4be
-00003b20: 7374 2e77 6869 6368 5f69 735f 6265 7474  st.which_is_bett
-00003b30: 6572 2873 656c 662e 5f62 6573 7429 0d0a  er(self._best)..
-00003b40: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-00003b50: 6573 745f 2021 3d20 7365 6c66 2e5f 6265  est_ != self._be
-00003b60: 7374 3a0d 0a20 2020 2020 2020 2020 2020  st:..           
-00003b70: 2020 2020 2073 656c 662e 5f62 6573 7420       self._best 
-00003b80: 3d20 6265 7374 5f0d 0a20 2020 2020 2020  = best_..       
-00003b90: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00003ba0: 6573 745f 6570 6f63 6820 3d20 6570 6f63  est_epoch = epoc
-00003bb0: 680d 0a20 2020 2020 2020 2020 2020 2020  h..             
-00003bc0: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
-00003bd0: 5b43 6f61 6368 5d20 3e3e 3e20 4265 7474  [Coach] >>> Bett
-00003be0: 6572 202a 2a2a 7b73 656c 662e 6d65 7465  er ***{self.mete
-00003bf0: 7234 6265 7374 2e6e 616d 657d 2a2a 2a20  r4best.name}*** 
-00003c00: 6f66 202a 2a2a 7b73 656c 662e 5f62 6573  of ***{self._bes
-00003c10: 743a 2e34 667d 2a2a 2a20 2229 0d0a 2020  t:.4f}*** ")..  
-00003c20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003c30: 6c66 2e73 6176 655f 6265 7374 2829 0d0a  lf.save_best()..
-00003c40: 0d0a 2020 2020 6465 6620 6576 616c 5f61  ..    def eval_a
-00003c50: 745f 6265 7374 2873 656c 6629 3a0d 0a20  t_best(self):.. 
-00003c60: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00003c70: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00003c80: 6164 5f62 6573 7428 290d 0a20 2020 2020  ad_best()..     
-00003c90: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00003ca0: 6428 7365 6c66 2e5f 6265 7374 5f65 706f  d(self._best_epo
-00003cb0: 6368 290d 0a20 2020 2020 2020 2020 2020  ch)..           
-00003cc0: 2073 656c 662e 7465 7374 2873 656c 662e   self.test(self.
-00003cd0: 5f62 6573 745f 6570 6f63 6829 0d0a 2020  _best_epoch)..  
-00003ce0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00003cf0: 7465 7028 7365 6c66 2e5f 6265 7374 5f65  tep(self._best_e
-00003d00: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
-00003d10: 2020 2073 656c 662e 6c6f 6164 2873 656c     self.load(sel
-00003d20: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00003d30: 7365 6c66 2e63 6667 2e53 4156 4544 5f46  self.cfg.SAVED_F
-00003d40: 494c 454e 414d 4529 0d0a 2020 2020 2020  ILENAME)..      
-00003d50: 2020 6578 6365 7074 2046 696c 654e 6f74    except FileNot
-00003d60: 466f 756e 6445 7272 6f72 3a0d 0a20 2020  FoundError:..   
-00003d70: 2020 2020 2020 2020 2069 6e66 6f4c 6f67           infoLog
-00003d80: 6765 7228 6622 5b43 6f61 6368 5d20 3e3e  ger(f"[Coach] >>
-00003d90: 3e20 4e6f 2062 6573 7420 6d6f 6465 6c20  > No best model 
-00003da0: 7761 7320 7265 636f 7264 6564 2e20 536b  was recorded. Sk
-00003db0: 6970 2069 7420 2e2e 2e22 290d 0a0d 0a20  ip it ...").... 
-00003dc0: 2020 2064 6566 2072 6573 756d 6528 7365     def resume(se
-00003dd0: 6c66 2920 2d3e 2069 6e74 3a0d 0a20 2020  lf) -> int:..   
-00003de0: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
-00003df0: 2020 2052 6573 756d 6520 7472 6169 6e69     Resume traini
-00003e00: 6e67 2066 726f 6d20 7468 6520 6c61 7374  ng from the last
-00003e10: 2063 6865 636b 706f 696e 742e 0d0a 0d0a   checkpoint.....
-00003e20: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00003e30: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00003e40: 2d2d 0d0a 2020 2020 2020 2020 7374 6172  --..        star
-00003e50: 745f 6570 6f63 683a 2069 6e74 0d0a 2020  t_epoch: int..  
-00003e60: 2020 2020 2020 2020 2020 5468 6520 6570            The ep
-00003e70: 6f63 6820 6e75 6d62 6572 2074 6f20 7265  och number to re
-00003e80: 7375 6d65 2074 7261 696e 696e 6720 6672  sume training fr
-00003e90: 6f6d 2e0d 0a20 2020 2020 2020 2022 2222  om...        """
-00003ea0: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
-00003eb0: 6570 6f63 683a 2069 6e74 203d 2030 0d0a  epoch: int = 0..
-00003ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003ed0: 6366 672e 7265 7375 6d65 3a0d 0a20 2020  cfg.resume:..   
-00003ee0: 2020 2020 2020 2020 2073 7461 7274 5f65           start_e
-00003ef0: 706f 6368 203d 2073 656c 662e 6c6f 6164  poch = self.load
-00003f00: 5f63 6865 636b 706f 696e 7428 290d 0a20  _checkpoint().. 
-00003f10: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
-00003f20: 6f67 6765 7228 6622 5b43 6f61 6368 5d20  ogger(f"[Coach] 
-00003f30: 3e3e 3e20 4c6f 6164 206c 6173 7420 6368  >>> Load last ch
-00003f40: 6563 6b70 6f69 6e74 2061 6e64 2074 7261  eckpoint and tra
-00003f50: 696e 2066 726f 6d20 6570 6f63 683a 207b  in from epoch: {
-00003f60: 7374 6172 745f 6570 6f63 687d 2229 0d0a  start_epoch}")..
-00003f70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003f80: 7461 7274 5f65 706f 6368 0d0a 0d0a 2020  tart_epoch....  
-00003f90: 2020 4074 6f72 6368 2e6e 6f5f 6772 6164    @torch.no_grad
-00003fa0: 2829 0d0a 2020 2020 6465 6620 6d6f 6e69  ()..    def moni
-00003fb0: 746f 7228 0d0a 2020 2020 2020 2020 7365  tor(..        se
-00003fc0: 6c66 2c20 2a76 616c 7565 732c 0d0a 2020  lf, *values,..  
-00003fd0: 2020 2020 2020 6e3a 2069 6e74 203d 2031        n: int = 1
-00003fe0: 2c20 6d6f 6465 3a20 7374 7220 3d20 276d  , mode: str = 'm
-00003ff0: 6561 6e27 2c20 0d0a 2020 2020 2020 2020  ean', ..        
-00004000: 7072 6566 6978 3a20 7374 7220 3d20 2774  prefix: str = 't
-00004010: 7261 696e 272c 2070 6f6f 6c3a 204f 7074  rain', pool: Opt
-00004020: 696f 6e61 6c5b 4974 6572 6162 6c65 5d20  ional[Iterable] 
-00004030: 3d20 4e6f 6e65 0d0a 2020 2020 293a 0d0a  = None..    ):..
-00004040: 0d0a 2020 2020 2020 2020 7222 2222 0d0a  ..        r"""..
-00004050: 2020 2020 2020 2020 4c6f 6720 6461 7461          Log data
-00004060: 2076 616c 7565 7320 746f 2073 7065 6369   values to speci
-00004070: 6669 6320 6d6f 6e69 746f 7273 2e0d 0a0d  fic monitors....
-00004080: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00004090: 6572 733a 0d0a 2020 2020 2020 2020 2d2d  ers:..        --
-000040a0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-000040b0: 2020 202a 7661 6c75 6573 203a 2064 6174     *values : dat
-000040c0: 610d 0a20 2020 2020 2020 2020 2020 2054  a..            T
-000040d0: 6865 2064 6174 6120 7661 6c75 6573 2074  he data values t
-000040e0: 6f20 6265 206c 6f67 6765 642e 0d0a 2020  o be logged...  
-000040f0: 2020 2020 2020 6e20 3a20 696e 740d 0a20        n : int.. 
-00004100: 2020 2020 2020 2020 2020 2054 6865 2062             The b
-00004110: 6174 6368 2073 697a 6520 696e 2067 656e  atch size in gen
-00004120: 6572 616c 2e0d 0a20 2020 2020 2020 206d  eral...        m
-00004130: 6f64 6520 3a20 7374 722c 206f 7074 696f  ode : str, optio
-00004140: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
-00004150: 2054 6865 206d 6f64 6520 746f 2063 6f6d   The mode to com
-00004160: 7075 7465 2074 6865 206d 6574 7269 632e  pute the metric.
-00004170: 2043 616e 2062 6520 2773 756d 2720 6f72   Can be 'sum' or
-00004180: 2027 6d65 616e 2720 2864 6566 6175 6c74   'mean' (default
-00004190: 292e 0d0a 2020 2020 2020 2020 7072 6566  )...        pref
-000041a0: 6978 203a 2073 7472 2c20 6f70 7469 6f6e  ix : str, option
-000041b0: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-000041c0: 5468 6520 7072 6566 6978 2073 7472 696e  The prefix strin
-000041d0: 6720 696e 6469 6361 7469 6e67 2077 6869  g indicating whi
-000041e0: 6368 206d 6f64 6520 7468 6520 7661 6c75  ch mode the valu
-000041f0: 6573 2062 656c 6f6e 6720 746f 2e20 4361  es belong to. Ca
-00004200: 6e20 6265 2027 7472 6169 6e27 2c20 2774  n be 'train', 't
-00004210: 6573 7427 206f 7220 2776 616c 6964 272e  est' or 'valid'.
-00004220: 0d0a 2020 2020 2020 2020 706f 6f6c 203a  ..        pool :
-00004230: 204c 6973 745b 7374 725d 2c20 6f70 7469   List[str], opti
-00004240: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-00004250: 2020 4120 6c69 7374 206f 6620 6d65 7472    A list of metr
-00004260: 6963 206e 616d 6573 2074 6f20 6c6f 672e  ic names to log.
-00004270: 2049 6620 4e6f 6e65 2c20 616c 6c20 6d65   If None, all me
-00004280: 7472 6963 7320 696e 2074 6865 2070 6f6f  trics in the poo
-00004290: 6c20 6f66 2060 7072 6566 6978 6020 7769  l of `prefix` wi
-000042a0: 6c6c 2062 6520 6c6f 6767 6564 2e0d 0a20  ll be logged... 
-000042b0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-000042c0: 2020 2020 2020 6d65 7472 6963 733a 2044        metrics: D
-000042d0: 6963 745b 4c69 7374 5d20 3d20 7365 6c66  ict[List] = self
-000042e0: 2e6d 6f6e 6974 6f72 735b 7072 6566 6978  .monitors[prefix
-000042f0: 5d0d 0a20 2020 2020 2020 2070 6f6f 6c20  ]..        pool 
-00004300: 3d20 6d65 7472 6963 7320 6966 2070 6f6f  = metrics if poo
-00004310: 6c20 6973 204e 6f6e 6520 656c 7365 2070  l is None else p
-00004320: 6f6f 6c0d 0a20 2020 2020 2020 2066 6f72  ool..        for
-00004330: 206c 6173 746e 616d 6520 696e 2070 6f6f   lastname in poo
-00004340: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
-00004350: 666f 7220 6d65 7465 7220 696e 206d 6574  for meter in met
-00004360: 7269 6373 2e67 6574 286c 6173 746e 616d  rics.get(lastnam
-00004370: 652e 7570 7065 7228 292c 205b 5d29 3a0d  e.upper(), []):.
-00004380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004390: 206d 6574 6572 282a 7661 6c75 6573 2c20   meter(*values, 
-000043a0: 6e3d 6e2c 206d 6f64 653d 6d6f 6465 290d  n=n, mode=mode).
-000043b0: 0a0d 0a20 2020 2064 6566 2073 7465 7028  ...    def step(
-000043c0: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
-000043d0: 293a 0d0a 2020 2020 2020 2020 7222 2222  ):..        r"""
-000043e0: 0d0a 2020 2020 2020 2020 5072 696e 7473  ..        Prints
-000043f0: 2074 7261 696e 696e 6720 7374 6174 7573   training status
-00004400: 2061 6e64 2065 7661 6c75 6174 696f 6e20   and evaluation 
-00004410: 7265 7375 6c74 7320 666f 7220 6561 6368  results for each
-00004420: 2065 706f 6368 2c20 0d0a 2020 2020 2020   epoch, ..      
-00004430: 2020 616e 6420 7265 7365 7473 2074 6865    and resets the
-00004440: 2063 6f72 7265 7370 6f6e 6469 6e67 2060   corresponding `
-00004450: 4176 6572 6167 654d 6574 6572 6020 696e  AverageMeter` in
-00004460: 7374 616e 6365 732e 0d0a 0d0a 2020 2020  stances.....    
-00004470: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-00004480: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00004490: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6570  ----..        ep
-000044a0: 6f63 6820 3a20 696e 740d 0a20 2020 2020  och : int..     
-000044b0: 2020 2020 2020 2054 6865 2065 706f 6368         The epoch
-000044c0: 206e 756d 6265 722e 0d0a 0d0a 2020 2020   number.....    
-000044d0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-000044e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
-000044f0: 2020 2020 2020 2020 4e6f 6e65 0d0a 2020          None..  
-00004500: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004510: 2020 206d 6574 7269 6373 3a20 4469 6374     metrics: Dict
-00004520: 5b73 7472 2c20 4c69 7374 5b41 7665 7261  [str, List[Avera
-00004530: 6765 4d65 7465 725d 5d0d 0a20 2020 2020  geMeter]]..     
-00004540: 2020 2066 6f72 2070 7265 6669 782c 206d     for prefix, m
-00004550: 6574 7269 6373 2069 6e20 7365 6c66 2e6d  etrics in self.m
-00004560: 6f6e 6974 6f72 732e 6974 656d 7328 293a  onitors.items():
-00004570: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00004580: 666f 7320 3d20 5b66 225b 436f 6163 685d  fos = [f"[Coach]
-00004590: 203e 3e3e 207b 7072 6566 6978 2e75 7070   >>> {prefix.upp
-000045a0: 6572 2829 3a35 7d20 4045 706f 6368 3a20  er():5} @Epoch: 
-000045b0: 7b65 706f 6368 3a3c 3464 7d20 3e3e 3e20  {epoch:<4d} >>> 
-000045c0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-000045d0: 666f 7220 6d65 7465 7273 2069 6e20 6d65  for meters in me
-000045e0: 7472 6963 732e 7661 6c75 6573 2829 3a0d  trics.values():.
-000045f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004600: 2069 6e66 6f73 202b 3d20 5b6d 6574 6572   infos += [meter
-00004610: 2e73 7465 7028 2920 666f 7220 6d65 7465  .step() for mete
-00004620: 7220 696e 206d 6574 6572 7320 6966 206d  r in meters if m
-00004630: 6574 6572 2e61 6374 6976 655d 0d0a 2020  eter.active]..  
-00004640: 2020 2020 2020 2020 2020 696e 666f 4c6f            infoLo
-00004650: 6767 6572 2827 207c 7c20 272e 6a6f 696e  gger(' || '.join
-00004660: 2869 6e66 6f73 2929 0d0a 0d0a 2020 2020  (infos))....    
-00004670: 4074 696d 656d 6574 6572 2822 436f 6163  @timemeter("Coac
-00004680: 682f 7375 6d6d 6172 7922 290d 0a20 2020  h/summary")..   
-00004690: 2064 6566 2073 756d 6d61 7279 2873 656c   def summary(sel
-000046a0: 6629 3a0d 0a20 2020 2020 2020 2072 2222  f):..        r""
-000046b0: 220d 0a20 2020 2020 2020 2053 756d 6d61  "..        Summa
-000046c0: 7279 2074 6865 2077 686f 6c65 2074 7261  ry the whole tra
-000046d0: 696e 696e 6720 7072 6f63 6573 732e 0d0a  ining process...
-000046e0: 0d0a 2020 2020 2020 2020 4765 6e65 7261  ..        Genera
-000046f0: 7465 2061 2073 756d 6d61 7279 206f 6620  te a summary of 
-00004700: 7468 6520 656e 7469 7265 2074 7261 696e  the entire train
-00004710: 696e 6720 7072 6f63 6573 732c 2069 6e63  ing process, inc
-00004720: 6c75 6469 6e67 2074 6865 2068 6973 746f  luding the histo
-00004730: 7269 6361 6c20 6576 616c 7561 7469 6f6e  rical evaluation
-00004740: 2072 6573 756c 7473 2c20 7468 6520 6265   results, the be
-00004750: 7374 0d0a 2020 2020 2020 2020 6869 7374  st..        hist
-00004760: 6f72 6963 616c 2072 6573 756c 7473 2c20  orical results, 
-00004770: 616e 6420 7468 6520 6375 7276 6573 206f  and the curves o
-00004780: 6620 6869 7374 6f72 6963 616c 2072 6573  f historical res
-00004790: 756c 7473 2e20 5468 6520 7265 7375 6c74  ults. The result
-000047a0: 696e 6720 7375 6d6d 6172 7920 6973 2073  ing summary is s
-000047b0: 6176 6564 2074 6f20 6120 4d61 726b 646f  aved to a Markdo
-000047c0: 776e 2066 696c 6520 6e61 6d65 640d 0a20  wn file named.. 
-000047d0: 2020 2020 2020 2022 5375 6d6d 6172 792e         "Summary.
-000047e0: 6d64 2220 696e 2074 6865 2060 7365 6c66  md" in the `self
-000047f0: 2e63 6667 2e4c 4f47 5f50 4154 4860 2064  .cfg.LOG_PATH` d
-00004800: 6972 6563 746f 7279 2e0d 0a0d 0a20 2020  irectory.....   
-00004810: 2020 2020 2041 6464 6974 696f 6e61 6c6c       Additionall
-00004820: 792c 2074 6865 2062 6573 7420 6869 7374  y, the best hist
-00004830: 6f72 6963 616c 2072 6573 756c 7473 2061  orical results a
-00004840: 7265 2073 6176 6564 2074 6f20 6120 6269  re saved to a bi
-00004850: 6e61 7279 2066 696c 6520 6e61 6d65 6420  nary file named 
-00004860: 6073 656c 662e 6366 672e 4d4f 4e49 544f  `self.cfg.MONITO
-00004870: 525f 4245 5354 5f46 494c 454e 414d 4560  R_BEST_FILENAME`
-00004880: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00004890: 2020 2020 2020 2020 696d 706f 7274 2070          import p
-000048a0: 616e 6461 7320 6173 2070 640d 0a0d 0a20  andas as pd.... 
-000048b0: 2020 2020 2020 2073 203d 2022 7c20 207b         s = "|  {
-000048c0: 7072 6566 6978 7d20 207c 2020 207b 6e61  prefix}  |   {na
-000048d0: 6d65 7d20 2020 7c20 2020 7b76 616c 7d20  me}   |   {val} 
-000048e0: 2020 7c20 2020 7b65 706f 6368 7d20 2020    |   {epoch}   
-000048f0: 7c20 2020 7b69 6d67 7d20 2020 7c5c 6e22  |   {img}   |\n"
-00004900: 0d0a 2020 2020 2020 2020 696e 666f 203d  ..        info =
-00004910: 2022 220d 0a20 2020 2020 2020 2069 6e66   ""..        inf
-00004920: 6f20 2b3d 2022 7c20 2050 7265 6669 7820  o += "|  Prefix 
-00004930: 207c 2020 204d 6574 7269 6320 2020 7c20   |   Metric   | 
-00004940: 2020 4265 7374 2020 207c 2020 2040 4570    Best   |   @Ep
-00004950: 6f63 6820 2020 7c20 2020 496d 6720 2020  och   |   Img   
-00004960: 7c5c 6e22 0d0a 2020 2020 2020 2020 696e  |\n"..        in
-00004970: 666f 202b 3d20 227c 203a 2d2d 2d2d 2d2d  fo += "| :------
-00004980: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
-00004990: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
-000049a0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
-000049b0: 2d3a 207c 5c6e 220d 0a20 2020 2020 2020  -: |\n"..       
-000049c0: 2064 6174 6120 3d20 5b5d 0d0a 2020 2020   data = []..    
-000049d0: 2020 2020 6265 7374 203d 2064 6566 6175      best = defau
-000049e0: 6c74 6469 6374 2864 6963 7429 0d0a 0d0a  ltdict(dict)....
-000049f0: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
-00004a00: 6978 2c20 6d65 7472 6963 7320 696e 2073  ix, metrics in s
-00004a10: 656c 662e 6d6f 6e69 746f 7273 2e69 7465  elf.monitors.ite
-00004a20: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00004a30: 2020 206d 6574 7269 6373 3a20 6465 6661     metrics: defa
-00004a40: 756c 7464 6963 745b 7374 722c 204c 6973  ultdict[str, Lis
-00004a50: 745b 4176 6572 6167 654d 6574 6572 5d5d  t[AverageMeter]]
-00004a60: 0d0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
-00004a70: 6571 203d 2031 2069 6620 7072 6566 6978  eq = 1 if prefix
-00004a80: 203d 3d20 2774 7261 696e 2720 656c 7365   == 'train' else
-00004a90: 2073 656c 662e 6366 672e 4556 414c 5f46   self.cfg.EVAL_F
-00004aa0: 5245 510d 0a20 2020 2020 2020 2020 2020  REQ..           
-00004ab0: 2066 6f72 206c 6173 746e 616d 652c 206d   for lastname, m
-00004ac0: 6574 6572 7320 696e 206d 6574 7269 6373  eters in metrics
-00004ad0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00004ae0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
-00004af0: 6574 6572 2069 6e20 6d65 7465 7273 3a0d  eter in meters:.
-00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b10: 2020 2020 2023 2053 6b69 7020 7468 6f73       # Skip thos
-00004b20: 6520 6d65 7465 7273 206e 6576 6572 2061  e meters never a
-00004b30: 6374 6976 6174 6564 2e0d 0a20 2020 2020  ctivated...     
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004b50: 6620 6c65 6e28 6d65 7465 722e 6869 7374  f len(meter.hist
-00004b60: 6f72 7929 203d 3d20 303a 0d0a 2020 2020  ory) == 0:..    
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2020 6d65 7465 722e 706c 6f74 2866 7265    meter.plot(fre
-00004bb0: 713d 6672 6571 290d 0a20 2020 2020 2020  q=freq)..       
-00004bc0: 2020 2020 2020 2020 2020 2020 2069 6d67               img
-00004bd0: 6e61 6d65 203d 206d 6574 6572 2e73 6176  name = meter.sav
-00004be0: 6528 7061 7468 3d6f 732e 7061 7468 2e6a  e(path=os.path.j
-00004bf0: 6f69 6e28 7365 6c66 2e63 6667 2e4c 4f47  oin(self.cfg.LOG
-00004c00: 5f50 4154 482c 2073 656c 662e 6366 672e  _PATH, self.cfg.
-00004c10: 5355 4d4d 4152 595f 4449 5229 2c20 7072  SUMMARY_DIR), pr
-00004c20: 6566 6978 3d70 7265 6669 7829 0d0a 2020  efix=prefix)..  
-00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c40: 2020 6570 6f63 682c 2076 616c 203d 206d    epoch, val = m
-00004c50: 6574 6572 2e61 7267 6265 7374 2866 7265  eter.argbest(fre
-00004c60: 7129 0d0a 2020 2020 2020 2020 2020 2020  q)..            
-00004c70: 2020 2020 2020 2020 696e 666f 202b 3d20          info += 
-00004c80: 732e 666f 726d 6174 280d 0a20 2020 2020  s.format(..     
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ca0: 2020 2070 7265 6669 783d 7072 6566 6978     prefix=prefix
-00004cb0: 2c20 6e61 6d65 3d6d 6574 6572 2e6e 616d  , name=meter.nam
-00004cc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00004cd0: 2020 2020 2020 2020 2020 2020 7661 6c3d              val=
-00004ce0: 7661 6c2c 2065 706f 6368 3d65 706f 6368  val, epoch=epoch
-00004cf0: 2c20 696d 673d 6622 215b 5d28 7b69 6d67  , img=f"![]({img
-00004d00: 6e61 6d65 7d29 220d 0a20 2020 2020 2020  name})"..       
-00004d10: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d30: 2020 2020 6461 7461 2e61 7070 656e 6428      data.append(
-00004d40: 5b70 7265 6669 782c 206d 6574 6572 2e6e  [prefix, meter.n
-00004d50: 616d 652c 2076 616c 2c20 6570 6f63 685d  ame, val, epoch]
-00004d60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004d70: 2020 2020 2020 2069 6620 7661 6c20 213d         if val !=
-00004d80: 202d 313a 2023 204f 6e6c 7920 7361 7665   -1: # Only save
-00004d90: 2061 7661 696c 6162 6c65 2064 6174 612e   available data.
-00004da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004db0: 2020 2020 2020 2020 2020 6265 7374 5b70            best[p
-00004dc0: 7265 6669 785d 5b6d 6574 6572 2e6e 616d  refix][meter.nam
-00004dd0: 655d 203d 2076 616c 0d0a 0d0a 2020 2020  e] = val....    
-00004de0: 2020 2020 6669 6c65 5f20 3d20 6f73 2e70      file_ = os.p
-00004df0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
-00004e00: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
-00004e10: 2e63 6667 2e53 554d 4d41 5259 5f44 4952  .cfg.SUMMARY_DIR
-00004e20: 2c20 7365 6c66 2e63 6667 2e53 554d 4d41  , self.cfg.SUMMA
-00004e30: 5259 5f46 494c 454e 414d 4529 0d0a 2020  RY_FILENAME)..  
-00004e40: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00004e50: 6669 6c65 5f2c 2022 7722 2c20 656e 636f  file_, "w", enco
-00004e60: 6469 6e67 3d22 7574 6638 2229 2061 7320  ding="utf8") as 
-00004e70: 6668 3a0d 0a20 2020 2020 2020 2020 2020  fh:..           
-00004e80: 2066 682e 7772 6974 6528 696e 666f 290d   fh.write(info).
-00004e90: 0a0d 0a20 2020 2020 2020 2064 6620 3d20  ...        df = 
-00004ea0: 7064 2e44 6174 6146 7261 6d65 2864 6174  pd.DataFrame(dat
-00004eb0: 612c 2063 6f6c 756d 6e73 3d5b 2750 7265  a, columns=['Pre
-00004ec0: 6669 7827 2c20 274d 6574 7269 6327 2c20  fix', 'Metric', 
-00004ed0: 2742 6573 7427 2c20 2740 4570 6f63 6827  'Best', '@Epoch'
-00004ee0: 5d29 0d0a 2020 2020 2020 2020 696e 666f  ])..        info
-00004ef0: 4c6f 6767 6572 2873 7472 2864 6629 290d  Logger(str(df)).
-00004f00: 0a20 2020 2020 2020 2069 6e66 6f4c 6f67  .        infoLog
-00004f10: 6765 7228 6622 5b4c 6f47 5f50 6154 485d  ger(f"[LoG_PaTH]
-00004f20: 203e 3e3e 207b 7365 6c66 2e63 6667 2e4c   >>> {self.cfg.L
-00004f30: 4f47 5f50 4154 487d 2229 0d0a 0d0a 2020  OG_PATH}")....  
-00004f40: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
-00004f50: 6f72 732e 7772 6974 6528 6f73 2e70 6174  ors.write(os.pat
-00004f60: 682e 6a6f 696e 2873 656c 662e 6366 672e  h.join(self.cfg.
-00004f70: 4c4f 475f 5041 5448 2c20 7365 6c66 2e63  LOG_PATH, self.c
-00004f80: 6667 2e53 554d 4d41 5259 5f44 4952 2929  fg.SUMMARY_DIR))
-00004f90: 2023 2074 656e 736f 7262 6f61 7264 0d0a   # tensorboard..
-00004fa0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00004fb0: 6f6e 6974 6f72 732e 7361 7665 286f 732e  onitors.save(os.
-00004fc0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00004fd0: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
-00004fe0: 662e 6366 672e 4441 5441 5f44 4952 292c  f.cfg.DATA_DIR),
-00004ff0: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
-00005000: 525f 4649 4c45 4e41 4d45 290d 0a20 2020  R_FILENAME)..   
-00005010: 2020 2020 2065 7870 6f72 745f 7069 636b       export_pick
-00005020: 6c65 2862 6573 742c 206f 732e 7061 7468  le(best, os.path
-00005030: 2e6a 6f69 6e28 7365 6c66 2e63 6667 2e4c  .join(self.cfg.L
-00005040: 4f47 5f50 4154 482c 2073 656c 662e 6366  OG_PATH, self.cf
-00005050: 672e 4441 5441 5f44 4952 2c20 7365 6c66  g.DATA_DIR, self
-00005060: 2e63 6667 2e4d 4f4e 4954 4f52 5f42 4553  .cfg.MONITOR_BES
-00005070: 545f 4649 4c45 4e41 4d45 2929 0d0a 0d0a  T_FILENAME))....
-00005080: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00005090: 2020 4074 696d 656d 6574 6572 2822 436f    @timemeter("Co
-000050a0: 6163 682f 6669 7422 290d 0a20 2020 2064  ach/fit")..    d
-000050b0: 6566 2066 6974 2873 656c 6629 3a0d 0a0d  ef fit(self):...
-000050c0: 0a20 2020 2020 2020 2064 6566 2073 6967  .        def sig
-000050d0: 6e61 6c5f 6861 6e64 6c65 7228 7369 672c  nal_handler(sig,
-000050e0: 2066 7261 6d65 293a 0d0a 2020 2020 2020   frame):..      
-000050f0: 2020 2020 2020 696e 666f 4c6f 6767 6572        infoLogger
-00005100: 2866 225c 3033 335b 303b 3331 3b34 376d  (f"\033[0;31;47m
-00005110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d54  ===============T
-00005130: 4552 4d49 4e41 5445 2043 5552 5245 4e54  ERMINATE CURRENT
-00005140: 2050 524f 4345 5353 3d3d 3d3d 3d3d 3d3d   PROCESS========
-00005150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005160: 3d3d 3d3d 3d3d 3d5c 3033 335b 306d 2229  =======\033[0m")
-00005170: 0d0a 2020 2020 2020 2020 2020 2020 7379  ..            sy
-00005180: 732e 6578 6974 2829 0d0a 2020 2020 2020  s.exit()..      
-00005190: 2020 7369 676e 616c 2e73 6967 6e61 6c28    signal.signal(
-000051a0: 7369 676e 616c 2e53 4947 494e 542c 2073  signal.SIGINT, s
-000051b0: 6967 6e61 6c5f 6861 6e64 6c65 7229 0d0a  ignal_handler)..
-000051c0: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
-000051d0: 6570 6f63 6820 3d20 7365 6c66 2e72 6573  epoch = self.res
-000051e0: 756d 6528 290d 0a20 2020 2020 2020 2066  ume()..        f
-000051f0: 6f72 2065 706f 6368 2069 6e20 7261 6e67  or epoch in rang
-00005200: 6528 7374 6172 745f 6570 6f63 682c 2073  e(start_epoch, s
-00005210: 656c 662e 6366 672e 6570 6f63 6873 293a  elf.cfg.epochs):
-00005220: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00005230: 2065 706f 6368 2025 2073 656c 662e 6366   epoch % self.cf
-00005240: 672e 4348 4543 4b50 4f49 4e54 5f46 5245  g.CHECKPOINT_FRE
-00005250: 5120 3d3d 2030 3a0d 0a20 2020 2020 2020  Q == 0:..       
-00005260: 2020 2020 2020 2020 2073 656c 662e 7361           self.sa
-00005270: 7665 5f63 6865 636b 706f 696e 7428 6570  ve_checkpoint(ep
-00005280: 6f63 6829 0d0a 2020 2020 2020 2020 2020  och)..          
-00005290: 2020 6966 2065 706f 6368 2025 2073 656c    if epoch % sel
-000052a0: 662e 6366 672e 4556 414c 5f46 5245 5120  f.cfg.EVAL_FREQ 
-000052b0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-000052c0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000052d0: 6667 2e45 5641 4c5f 5641 4c49 443a 0d0a  fg.EVAL_VALID:..
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2020 7365 6c66 2e76 616c 6964 2865      self.valid(e
-00005300: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
-00005310: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00005320: 6667 2e45 5641 4c5f 5445 5354 3a0d 0a20  fg.EVAL_TEST:.. 
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2073 656c 662e 7465 7374 2865 706f     self.test(epo
-00005350: 6368 290d 0a20 2020 2020 2020 2020 2020  ch)..           
-00005360: 2073 656c 662e 6368 6563 6b5f 6265 7374   self.check_best
-00005370: 2865 706f 6368 290d 0a20 2020 2020 2020  (epoch)..       
-00005380: 2020 2020 2073 656c 662e 7374 6570 2865       self.step(e
-00005390: 706f 6368 290d 0a20 2020 2020 2020 2020  poch)..         
-000053a0: 2020 2073 656c 662e 7472 6169 6e28 6570     self.train(ep
-000053b0: 6f63 6829 0d0a 0d0a 2020 2020 2020 2020  och)....        
-000053c0: 7365 6c66 2e73 6176 6528 290d 0a0d 0a20  self.save().... 
-000053d0: 2020 2020 2020 2023 206c 6173 7420 6570         # last ep
-000053e0: 6f63 680d 0a20 2020 2020 2020 2073 656c  och..        sel
-000053f0: 662e 7661 6c69 6428 7365 6c66 2e63 6667  f.valid(self.cfg
-00005400: 2e65 706f 6368 7329 0d0a 2020 2020 2020  .epochs)..      
-00005410: 2020 7365 6c66 2e74 6573 7428 7365 6c66    self.test(self
-00005420: 2e63 6667 2e65 706f 6368 7329 0d0a 2020  .cfg.epochs)..  
-00005430: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-00005440: 5f62 6573 7428 7365 6c66 2e63 6667 2e65  _best(self.cfg.e
-00005450: 706f 6368 7329 0d0a 2020 2020 2020 2020  pochs)..        
-00005460: 7365 6c66 2e73 7465 7028 7365 6c66 2e63  self.step(self.c
-00005470: 6667 2e65 706f 6368 7329 0d0a 0d0a 2020  fg.epochs)....  
-00005480: 2020 2020 2020 7365 6c66 2e73 756d 6d61        self.summa
-00005490: 7279 2829 0d0a 0d0a 2020 2020 2020 2020  ry()....        
-000054a0: 7365 6c66 2e65 7661 6c5f 6174 5f62 6573  self.eval_at_bes
-000054b0: 7428 290d 0a0d 0a0d 0a63 6c61 7373 2041  t()......class A
-000054c0: 6461 7074 6572 3a0d 0a20 2020 2072 2222  dapter:..    r""
-000054d0: 220d 0a20 2020 2050 6172 616d 7320 7475  "..    Params tu
-000054e0: 6e65 722e 0d0a 0d0a 2020 2020 466c 6f77  ner.....    Flow
-000054f0: 733a 0d0a 2020 2020 2d2d 2d2d 2d2d 0d0a  s:..    ------..
-00005500: 2020 2020 312e 2063 6f6d 7069 6c65 3a20      1. compile: 
-00005510: 636f 6e66 6967 7572 6520 7468 6520 636f  configure the co
-00005520: 6d6d 616e 642c 2065 6e76 6972 6f6e 6d65  mmand, environme
-00005530: 6e74 732c 2061 6e64 2070 6172 616d 6574  nts, and paramet
-00005540: 6572 7320 666f 7220 7472 6169 6e69 6e67  ers for training
-00005550: 2e0d 0a20 2020 2032 2e20 616c 6c6f 6361  ...    2. alloca
-00005560: 7465 2064 6576 6963 6573 2066 6f72 2076  te devices for v
-00005570: 6172 696f 7573 2070 6172 616d 6574 6572  arious parameter
-00005580: 733a 0d0a 2020 2020 2020 2020 2d20 7265  s:..        - re
-00005590: 6769 7374 6572 2074 6865 2049 442c 206c  gister the ID, l
-000055a0: 6f67 2070 6174 682c 2061 6e64 2064 6576  og path, and dev
-000055b0: 6963 6520 6669 7273 740d 0a20 2020 2020  ice first..     
-000055c0: 2020 202d 2065 7865 6375 7465 2074 6865     - execute the
-000055d0: 2063 6f6d 6d61 6e64 0d0a 2020 2020 2020   command..      
-000055e0: 2020 2d20 636f 6c6c 6563 7420 696e 666f    - collect info
-000055f0: 726d 6174 696f 6e20 6672 6f6d 2074 6865  rmation from the
-00005600: 206c 6f67 2070 6174 6820 616e 6420 6f75   log path and ou
-00005610: 7470 7574 2074 6f20 5465 6e73 6f72 426f  tput to TensorBo
-00005620: 6172 640d 0a20 2020 2020 2020 202d 2073  ard..        - s
-00005630: 6176 6520 7468 6520 6368 6563 6b70 6f69  ave the checkpoi
-00005640: 6e74 0d0a 2020 2020 2020 2020 2d20 7265  nt..        - re
-00005650: 6c65 6173 6520 7468 6520 636f 7272 6573  lease the corres
-00005660: 706f 6e64 696e 6720 6465 7669 6365 0d0a  ponding device..
-00005670: 0d0a 2020 2020 4578 616d 706c 6573 3a0d  ..    Examples:.
-00005680: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a  .    ---------..
-00005690: 2020 2020 3e3e 3e20 6366 6720 3d20 7b27      >>> cfg = {'
-000056a0: 636f 6d6d 616e 6427 3a20 2770 7974 686f  command': 'pytho
-000056b0: 6e20 7878 782e 7079 272c 2027 7061 7261  n xxx.py', 'para
-000056c0: 6d73 273a 207b 276f 7074 696d 697a 6572  ms': {'optimizer
-000056d0: 273a 205b 2773 6764 272c 2027 6164 616d  ': ['sgd', 'adam
-000056e0: 275d 7d7d 0d0a 2020 2020 3e3e 3e20 7475  ']}}..    >>> tu
-000056f0: 6e65 7220 3d20 4164 6170 7465 7228 290d  ner = Adapter().
-00005700: 0a20 2020 203e 3e3e 2074 756e 6572 2e63  .    >>> tuner.c
-00005710: 6f6d 7069 6c65 2863 6667 290d 0a20 2020  ompile(cfg)..   
-00005720: 203e 3e3e 2074 756e 6572 2e66 6974 2829   >>> tuner.fit()
-00005730: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
-00005740: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00005750: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
-00005760: 2020 2020 2020 7365 6c66 2e70 6172 616d        self.param
-00005770: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00005780: 7365 6c66 2e76 616c 7565 7320 3d20 5b5d  self.values = []
-00005790: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-000057a0: 6576 6963 6573 203d 2074 7570 6c65 2829  evices = tuple()
-000057b0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-000057c0: 790d 0a20 2020 2064 6566 2043 4f4d 4d41  y..    def COMMA
-000057d0: 4e44 2873 656c 6629 3a0d 0a20 2020 2020  ND(self):..     
-000057e0: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
-000057f0: 6667 2e43 4f4d 4d41 4e44 0d0a 0d0a 2020  fg.COMMAND....  
-00005800: 2020 6465 6620 7265 6769 7374 6572 2873    def register(s
-00005810: 656c 662c 2064 6576 6963 653a 2073 7472  elf, device: str
-00005820: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
-00005830: 7374 725d 3a0d 0a20 2020 2020 2020 2073  str]:..        s
-00005840: 656c 662e 6366 672e 454e 5653 5b27 6964  elf.cfg.ENVS['id
-00005850: 275d 203d 2074 696d 652e 7374 7266 7469  '] = time.strfti
-00005860: 6d65 2854 494d 4529 0d0a 2020 2020 2020  me(TIME)..      
-00005870: 2020 7365 6c66 2e63 6667 2e45 4e56 535b    self.cfg.ENVS[
-00005880: 2764 6576 6963 6527 5d20 3d20 6465 7669  'device'] = devi
-00005890: 6365 0d0a 2020 2020 2020 2020 636f 6d6d  ce..        comm
-000058a0: 616e 6420 3d20 7365 6c66 2e43 4f4d 4d41  and = self.COMMA
-000058b0: 4e44 202b 2073 656c 662e 6765 745f 6f70  ND + self.get_op
-000058c0: 7469 6f6e 2827 6964 272c 2073 656c 662e  tion('id', self.
-000058d0: 6366 672e 454e 5653 2e69 6429 0d0a 2020  cfg.ENVS.id)..  
-000058e0: 2020 2020 2020 636f 6d6d 616e 6420 2b3d        command +=
-000058f0: 2073 656c 662e 6765 745f 6f70 7469 6f6e   self.get_option
-00005900: 2827 6465 7669 6365 272c 2073 656c 662e  ('device', self.
-00005910: 6366 672e 454e 5653 2e64 6576 6963 6529  cfg.ENVS.device)
-00005920: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00005930: 2063 6f6d 6d61 6e64 2c20 7365 6c66 2e63   command, self.c
-00005940: 6667 2e45 4e56 532e 6964 2c20 7365 6c66  fg.ENVS.id, self
-00005950: 2e63 6667 2e4c 4f47 5f50 4154 482e 666f  .cfg.LOG_PATH.fo
-00005960: 726d 6174 282a 2a73 656c 662e 6366 672e  rmat(**self.cfg.
-00005970: 454e 5653 290d 0a0d 0a20 2020 2040 7469  ENVS)....    @ti
-00005980: 6d65 6d65 7465 7228 2241 6461 7074 6572  memeter("Adapter
-00005990: 2f63 6f6d 7069 6c65 2229 0d0a 2020 2020  /compile")..    
-000059a0: 6465 6620 636f 6d70 696c 6528 7365 6c66  def compile(self
-000059b0: 2c20 6366 673a 2043 6f6e 6669 6729 202d  , cfg: Config) -
-000059c0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-000059d0: 2072 2222 220d 0a20 2020 2020 2020 2043   r"""..        C
-000059e0: 6f6e 6669 6775 7265 2074 6865 2063 6f6d  onfigure the com
-000059f0: 6d61 6e64 2c20 656e 7669 726f 6e6d 656e  mand, environmen
-00005a00: 7473 2c20 616e 6420 7061 7261 6d65 7465  ts, and paramete
-00005a10: 7273 2066 6f72 2074 7261 696e 696e 672e  rs for training.
-00005a20: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-00005a30: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
-00005a40: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020   -----------..  
-00005a50: 2020 2020 2020 6366 6720 3a20 436f 6e66        cfg : Conf
-00005a60: 6967 0d0a 2020 2020 2020 2020 2020 2020  ig..            
-00005a70: 416e 206f 626a 6563 7420 7468 6174 2063  An object that c
-00005a80: 6f6e 7461 696e 7320 7468 6520 636f 6d6d  ontains the comm
-00005a90: 616e 642c 2065 6e76 6972 6f6e 6d65 6e74  and, environment
-00005aa0: 732c 2070 6172 616d 6574 6572 732c 2061  s, parameters, a
-00005ab0: 6e64 2064 6566 6175 6c74 732e 0d0a 0d0a  nd defaults.....
-00005ac0: 2020 2020 2020 2020 466c 6f77 733a 0d0a          Flows:..
-00005ad0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
-00005ae0: 2020 2020 2020 2020 312e 2041 6464 2065          1. Add e
-00005af0: 6e76 6972 6f6e 6d65 6e74 616c 2070 6172  nvironmental par
-00005b00: 616d 6574 6572 7320 746f 2074 6865 2062  ameters to the b
-00005b10: 6173 6963 2060 636f 6d6d 616e 6460 2e0d  asic `command`..
-00005b20: 0a20 2020 2020 2020 2032 2e20 5265 6769  .        2. Regi
-00005b30: 7374 6572 2061 6c6c 2061 7661 696c 6162  ster all availab
-00005b40: 6c65 2064 6576 6963 6573 2e0d 0a20 2020  le devices...   
-00005b50: 2020 2020 2033 2e20 436f 6e76 6572 7420       3. Convert 
-00005b60: 616c 6c20 7061 7261 6d65 7465 7273 2066  all parameters f
-00005b70: 726f 6d20 6063 6667 2e50 4152 414d 5360  rom `cfg.PARAMS`
-00005b80: 2e0d 0a20 2020 2020 2020 2034 2e20 436f  ...        4. Co
-00005b90: 6e76 6572 7420 616c 6c20 6465 6661 756c  nvert all defaul
-00005ba0: 7473 2066 726f 6d20 6063 6667 2e44 4546  ts from `cfg.DEF
-00005bb0: 4155 4c54 5360 2e0d 0a0d 0a20 2020 2020  AULTS`.....     
-00005bc0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00005bd0: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-00005be0: 2020 2020 2020 204e 6f6e 650d 0a20 2020         None..   
-00005bf0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005c00: 2020 7365 6c66 2e63 6667 203d 2063 6667    self.cfg = cfg
-00005c10: 0d0a 2020 2020 2020 2020 7069 6563 6520  ..        piece 
-00005c20: 3d20 225c 747b 6b65 797d 3a20 7b76 616c  = "\t{key}: {val
-00005c30: 737d 205c 6e22 0d0a 2020 2020 2020 2020  s} \n"..        
-00005c40: 656e 7673 2c20 7061 7261 6d73 2c20 6465  envs, params, de
-00005c50: 6661 756c 7473 203d 2022 222c 2022 222c  faults = "", "",
-00005c60: 2022 220d 0a20 2020 2020 2020 2066 6f72   ""..        for
-00005c70: 206b 6579 2c20 7661 6c20 696e 2073 656c   key, val in sel
-00005c80: 662e 6366 672e 454e 5653 2e69 7465 6d73  f.cfg.ENVS.items
-00005c90: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00005ca0: 2069 6620 6b65 7920 3d3d 2027 6465 7669   if key == 'devi
-00005cb0: 6365 273a 0d0a 2020 2020 2020 2020 2020  ce':..          
-00005cc0: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
-00005cd0: 6573 203d 2074 7570 6c65 2876 616c 2e73  es = tuple(val.s
-00005ce0: 706c 6974 2827 2c27 2929 0d0a 2020 2020  plit(','))..    
-00005cf0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005d10: 656c 662e 6366 672e 434f 4d4d 414e 4420  elf.cfg.COMMAND 
-00005d20: 2b3d 2073 656c 662e 6765 745f 6f70 7469  += self.get_opti
-00005d30: 6f6e 286b 6579 2c20 7661 6c29 0d0a 2020  on(key, val)..  
-00005d40: 2020 2020 2020 2020 2020 656e 7673 202b            envs +
-00005d50: 3d20 7069 6563 652e 666f 726d 6174 286b  = piece.format(k
-00005d60: 6579 3d6b 6579 2c20 7661 6c73 3d76 616c  ey=key, vals=val
-00005d70: 290d 0a20 2020 2020 2020 2066 6f72 206b  )..        for k
-00005d80: 6579 2c20 7661 6c73 2069 6e20 7365 6c66  ey, vals in self
-00005d90: 2e63 6667 2e50 4152 414d 532e 6974 656d  .cfg.PARAMS.item
-00005da0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00005db0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00005dc0: 7661 6c73 2c20 2873 7472 2c20 696e 742c  vals, (str, int,
-00005dd0: 2066 6c6f 6174 2929 3a0d 0a20 2020 2020   float)):..     
-00005de0: 2020 2020 2020 2020 2020 2076 616c 7320             vals 
-00005df0: 3d20 5b76 616c 735d 0d0a 2020 2020 2020  = [vals]..      
-00005e00: 2020 2020 2020 7365 6c66 2e64 6570 6c6f        self.deplo
-00005e10: 795f 7061 7261 6d73 286b 6579 2c20 7661  y_params(key, va
-00005e20: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
-00005e30: 2070 6172 616d 7320 2b3d 2070 6965 6365   params += piece
-00005e40: 2e66 6f72 6d61 7428 6b65 793d 6b65 792c  .format(key=key,
-00005e50: 2076 616c 733d 7661 6c73 290d 0a20 2020   vals=vals)..   
-00005e60: 2020 2020 2066 6f72 206b 6579 2c20 7661       for key, va
-00005e70: 6c20 696e 2073 656c 662e 6366 672e 4445  l in self.cfg.DE
-00005e80: 4641 554c 5453 2e69 7465 6d73 2829 3a0d  FAULTS.items():.
-00005e90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005ea0: 662e 6366 672e 4445 4641 554c 5453 5b6b  f.cfg.DEFAULTS[k
-00005eb0: 6579 5d20 3d20 7661 6c0d 0a20 2020 2020  ey] = val..     
-00005ec0: 2020 2020 2020 2064 6566 6175 6c74 7320         defaults 
-00005ed0: 2b3d 2070 6965 6365 2e66 6f72 6d61 7428  += piece.format(
-00005ee0: 6b65 793d 6b65 792c 2076 616c 733d 7661  key=key, vals=va
-00005ef0: 6c29 0d0a 0d0a 2020 2020 2020 2020 6366  l)....        cf
-00005f00: 675f 696e 666f 7320 3d20 6622 636f 6d6d  g_infos = f"comm
-00005f10: 616e 643a 207b 7365 6c66 2e63 6667 2e43  and: {self.cfg.C
-00005f20: 4f4d 4d41 4e44 7d20 5c6e 656e 7673 3a20  OMMAND} \nenvs: 
-00005f30: 5c6e 7b65 6e76 737d 7061 7261 6d73 3a20  \n{envs}params: 
-00005f40: 5c6e 7b70 6172 616d 737d 6465 6661 756c  \n{params}defaul
-00005f50: 7473 3a20 5c6e 7b64 6566 6175 6c74 737d  ts: \n{defaults}
-00005f60: 220d 0a20 2020 2020 2020 2069 6e66 6f4c  "..        infoL
-00005f70: 6f67 6765 7228 6622 5c30 3333 5b30 3b33  ogger(f"\033[0;3
-00005f80: 313b 3437 6d7b 6366 675f 696e 666f 737d  1;47m{cfg_infos}
-00005f90: 5c30 3333 5b30 6d22 290d 0a20 2020 2020  \033[0m")..     
-00005fa0: 2020 200d 0a0d 0a20 2020 2064 6566 2064     ....    def d
-00005fb0: 6570 6c6f 795f 7061 7261 6d73 2873 656c  eploy_params(sel
-00005fc0: 662c 206b 6579 3a20 7374 722c 2076 616c  f, key: str, val
-00005fd0: 733a 2049 7465 7261 626c 6529 3a0d 0a20  s: Iterable):.. 
-00005fe0: 2020 2020 2020 2073 656c 662e 7061 7261         self.para
-00005ff0: 6d73 2e61 7070 656e 6428 6b65 7929 0d0a  ms.append(key)..
-00006000: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00006010: 7565 732e 6170 7065 6e64 2876 616c 7329  ues.append(vals)
-00006020: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-00006030: 6574 686f 640d 0a20 2020 2064 6566 2067  ethod..    def g
-00006040: 6574 5f6f 7074 696f 6e28 6b65 793a 2073  et_option(key: s
-00006050: 7472 2c20 7661 6c3a 2041 6e79 293a 0d0a  tr, val: Any):..
-00006060: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
-00006070: 2020 2020 2020 436f 6e76 6572 7420 286b        Convert (k
-00006080: 6579 2c20 7661 6c29 2074 6f20 272d 2d6b  ey, val) to '--k
-00006090: 6579 3d76 616c 272e 0d0a 0d0a 2020 2020  ey=val'.....    
-000060a0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-000060b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000060c0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6b65  ----..        ke
-000060d0: 7920 3a20 7374 720d 0a20 2020 2020 2020  y : str..       
-000060e0: 2020 2020 2054 6865 206b 6579 206f 6620       The key of 
-000060f0: 7468 6520 7061 7261 6d65 7465 722e 0d0a  the parameter...
-00006100: 2020 2020 2020 2020 7661 6c20 3a20 416e          val : An
-00006110: 790d 0a20 2020 2020 2020 2020 2020 2054  y..            T
-00006120: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00006130: 7061 7261 6d65 7465 722e 0d0a 0d0a 2020  parameter.....  
-00006140: 2020 2020 2020 4e6f 7465 733a 0d0a 2020        Notes:..  
-00006150: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
-00006160: 2020 2020 2020 416c 6c20 275f 2720 696e        All '_' in
-00006170: 2060 6b65 7960 2077 696c 6c20 6265 2072   `key` will be r
-00006180: 6570 6c61 6365 6420 6279 2027 2d27 2e0d  eplaced by '-'..
-00006190: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000061a0: 6e73 3a0d 0a20 2020 2020 2020 202d 2d2d  ns:..        ---
-000061b0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-000061c0: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
-000061d0: 5468 6520 7061 7261 6d65 7465 7220 7769  The parameter wi
-000061e0: 7468 2066 6f72 6d61 7420 272d 2d6b 6579  th format '--key
-000061f0: 3d76 616c 272e 0d0a 0d0a 2020 2020 2020  =val'.....      
-00006200: 2020 4578 616d 706c 6573 3a0d 0a20 2020    Examples:..   
-00006210: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a       ---------..
-00006220: 2020 2020 2020 2020 3e3e 3e20 4164 6170          >>> Adap
-00006230: 7465 722e 6765 745f 6f70 7469 6f6e 2827  ter.get_option('
-00006240: 6c72 272c 2027 3165 2d33 2729 0d0a 2020  lr', '1e-3')..  
-00006250: 2020 2020 2020 272d 2d6c 723d 3165 2d33        '--lr=1e-3
-00006260: 270d 0a20 2020 2020 2020 203e 3e3e 2041  '..        >>> A
-00006270: 6461 7074 6572 2e67 6574 5f6f 7074 696f  dapter.get_optio
-00006280: 6e28 276c 6561 726e 696e 675f 7261 7465  n('learning_rate
-00006290: 272c 2027 3165 2d33 2729 0d0a 2020 2020  ', '1e-3')..    
-000062a0: 2020 2020 272d 2d6c 6561 726e 696e 672d      '--learning-
-000062b0: 7261 7465 3d31 652d 3327 0d0a 2020 2020  rate=1e-3'..    
-000062c0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000062d0: 2072 6574 7572 6e20 6622 202d 2d7b 6b65   return f" --{ke
-000062e0: 792e 7265 706c 6163 6528 275f 272c 2027  y.replace('_', '
-000062f0: 2d27 297d 3d7b 7661 6c7d 220d 0a0d 0a20  -')}={val}".... 
-00006300: 2020 2064 6566 206c 6f61 645f 6265 7374     def load_best
-00006310: 2873 656c 662c 206c 6f67 5061 7468 3a20  (self, logPath: 
-00006320: 7374 7229 3a0d 0a20 2020 2020 2020 2022  str):..        "
-00006330: 2222 4c6f 6164 2062 6573 742e 7069 636b  ""Load best.pick
-00006340: 6c65 2066 726f 6d20 6c6f 6750 6174 6820  le from logPath 
-00006350: 6f66 2063 6f72 7265 7370 6f6e 6469 6e67  of corresponding
-00006360: 2e22 2222 0d0a 2020 2020 2020 2020 6669  ."""..        fi
-00006370: 6c65 5f20 3d20 6f73 2e70 6174 682e 6a6f  le_ = os.path.jo
-00006380: 696e 286c 6f67 5061 7468 2c20 7365 6c66  in(logPath, self
-00006390: 2e63 6667 2e44 4154 415f 4449 522c 2073  .cfg.DATA_DIR, s
-000063a0: 656c 662e 6366 672e 4d4f 4e49 544f 525f  elf.cfg.MONITOR_
-000063b0: 4245 5354 5f46 494c 454e 414d 4529 0d0a  BEST_FILENAME)..
-000063c0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-000063d0: 6d70 6f72 745f 7069 636b 6c65 2866 696c  mport_pickle(fil
-000063e0: 655f 290d 0a0d 0a20 2020 2064 6566 2077  e_)....    def w
-000063f0: 7269 7465 2873 656c 662c 2069 645f 3a20  rite(self, id_: 
-00006400: 7374 722c 206c 6f67 5061 7468 3a20 7374  str, logPath: st
-00006410: 722c 2070 6172 616d 733a 2044 6963 7429  r, params: Dict)
-00006420: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
-00006430: 0a20 2020 2020 2020 2057 7269 7465 2065  .        Write e
-00006440: 7870 6572 696d 656e 7420 7265 7375 6c74  xperiment result
-00006450: 7320 746f 2074 656e 736f 7262 6f61 7264  s to tensorboard
-00006460: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00006470: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
-00006480: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
-00006490: 2020 2020 2020 2069 645f 3a20 7374 720d         id_: str.
-000064a0: 0a20 2020 2020 2020 2020 2020 2045 7870  .            Exp
-000064b0: 6572 696d 656e 7420 4944 2e0d 0a20 2020  eriment ID...   
-000064c0: 2020 2020 206c 6f67 5061 7468 3a20 7374       logPath: st
-000064d0: 720d 0a20 2020 2020 2020 2020 2020 2050  r..            P
-000064e0: 6174 6820 746f 2074 6865 2065 7870 6572  ath to the exper
-000064f0: 696d 656e 7420 6c6f 6773 2e0d 0a20 2020  iment logs...   
-00006500: 2020 2020 2070 6172 616d 733a 2044 6963       params: Dic
-00006510: 740d 0a20 2020 2020 2020 2020 2020 2043  t..            C
-00006520: 6f6e 6669 6775 7261 7469 6f6e 2070 6172  onfiguration par
-00006530: 616d 6574 6572 7320 6f66 2074 6865 2065  ameters of the e
-00006540: 7870 6572 696d 656e 742e 0d0a 0d0a 2020  xperiment.....  
-00006550: 2020 2020 2020 466c 6f77 733a 0d0a 2020        Flows:..  
-00006560: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
-00006570: 2020 2020 2020 312e 204c 6f61 6420 7468        1. Load th
-00006580: 6520 6265 7374 2064 6174 6120 6672 6f6d  e best data from
-00006590: 2060 6c6f 6750 6174 6860 2e0d 0a20 2020   `logPath`...   
-000065a0: 2020 2020 2032 2e20 5772 6974 6520 7468       2. Write th
-000065b0: 6520 6265 7374 2064 6174 6120 746f 2074  e best data to t
-000065c0: 656e 736f 7262 6f61 7264 2077 6974 6820  ensorboard with 
-000065d0: 6070 6172 616d 7360 2e0d 0a0d 0a20 2020  `params`.....   
-000065e0: 2020 2020 204e 6f74 6573 3a0d 0a20 2020       Notes:..   
-000065f0: 2020 2020 202d 2d2d 2d2d 2d0d 0a20 2020       ------..   
-00006600: 2020 2020 2049 6620 796f 7520 6669 6e64       If you find
-00006610: 2060 2d31 6020 6170 7065 6172 696e 6720   `-1` appearing 
-00006620: 696e 2074 6865 2074 656e 736f 7262 6f61  in the tensorboa
-00006630: 7264 2c0d 0a20 2020 2020 2020 2069 7420  rd,..        it 
-00006640: 636f 756c 6420 6d65 616e 2074 6861 7420  could mean that 
-00006650: 7468 6520 6461 7461 2069 7320 6f66 2060  the data is of `
-00006660: 7374 7260 2074 7970 652c 0d0a 2020 2020  str` type,..    
-00006670: 2020 2020 7768 6963 6820 7769 6c6c 2063      which will c
-00006680: 6175 7365 2061 6e20 6572 726f 7220 6966  ause an error if
-00006690: 2069 7420 6973 2073 656e 7420 746f 2074   it is sent to t
-000066a0: 656e 736f 7262 6f61 7264 2064 6972 6563  ensorboard direc
-000066b0: 746c 7921 0d0a 2020 2020 2020 2020 2222  tly!..        ""
-000066c0: 220d 0a20 2020 2020 2020 2074 7279 3a0d  "..        try:.
-000066d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000066e0: 6120 3d20 7365 6c66 2e6c 6f61 645f 6265  a = self.load_be
-000066f0: 7374 286c 6f67 5061 7468 290d 0a20 2020  st(logPath)..   
-00006700: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-00006710: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00006720: 662e 6366 672e 434f 5245 5f4c 4f47 5f50  f.cfg.CORE_LOG_P
-00006730: 4154 482c 2069 645f 290d 0a20 2020 2020  ATH, id_)..     
-00006740: 2020 2020 2020 2077 6974 6820 5375 6d6d         with Summ
-00006750: 6172 7957 7269 7465 7228 6c6f 675f 6469  aryWriter(log_di
-00006760: 723d 7061 7468 2920 6173 2077 7269 7465  r=path) as write
-00006770: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00006780: 2020 2020 6d65 7472 6963 7320 3d20 6469      metrics = di
-00006790: 6374 2829 0d0a 2020 2020 2020 2020 2020  ct()..          
-000067a0: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
-000067b0: 2c20 6265 7374 2069 6e20 6461 7461 2e69  , best in data.i
-000067c0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-000067d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000067e0: 206d 6574 7269 632c 2076 616c 2069 6e20   metric, val in 
-000067f0: 6265 7374 2e69 7465 6d73 2829 3a0d 0a20  best.items():.. 
-00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
-00006820: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
-00006830: 616c 2c20 2869 6e74 2c20 666c 6f61 7429  al, (int, float)
-00006840: 2920 656c 7365 202d 310d 0a20 2020 2020  ) else -1..     
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 206d 6574 7269 6373 5b27 2f27 2e6a     metrics['/'.j
-00006870: 6f69 6e28 5b70 7265 6669 782c 206d 6574  oin([prefix, met
-00006880: 7269 635d 295d 203d 2076 616c 0d0a 2020  ric])] = val..  
-00006890: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-000068a0: 6974 6572 2e61 6464 5f68 7061 7261 6d73  iter.add_hparams
-000068b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000068c0: 2020 2020 2020 2070 6172 616d 732c 206d         params, m
-000068d0: 6574 7269 6373 2c0d 0a20 2020 2020 2020  etrics,..       
-000068e0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-000068f0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00006900: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
-00006910: 2020 2069 6e66 6f4c 6f67 6765 7228 0d0a     infoLogger(..
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 6622 5c30 3333 5b30 3b33 313b 3437 6d5b  f"\033[0;31;47m[
-00006940: 4164 6170 7465 725d 203e 3e3e 2055 6e6b  Adapter] >>> Unk
-00006950: 6e6f 776e 2065 7272 6f72 7320 6861 7070  nown errors happ
-00006960: 656e 2e20 5468 6973 2069 7320 6d61 696e  en. This is main
-00006970: 6c79 2064 7565 2074 6f20 6162 6e6f 726d  ly due to abnorm
-00006980: 616c 2065 7869 7473 206f 6620 6368 696c  al exits of chil
-00006990: 6420 7072 6f63 6573 7365 732e 5c30 3333  d processes.\033
-000069a0: 5b30 6d22 0d0a 2020 2020 2020 2020 2020  [0m"..          
-000069b0: 2020 290d 0a0d 0a20 2020 2064 6566 2065    )....    def e
-000069c0: 6163 685f 6772 6964 2873 656c 6629 3a0d  ach_grid(self):.
-000069d0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
-000069e0: 2073 6561 7263 6820 666f 7220 6561 6368   search for each
-000069f0: 206b 696e 6420 6f66 2070 6172 616d 2e22   kind of param."
-00006a00: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
-00006a10: 6b65 792c 2076 616c 7320 696e 207a 6970  key, vals in zip
-00006a20: 2873 656c 662e 7061 7261 6d73 2c20 7365  (self.params, se
-00006a30: 6c66 2e76 616c 7565 7329 3a0d 0a20 2020  lf.values):..   
-00006a40: 2020 2020 2020 2020 2066 6f72 2076 616c           for val
-00006a50: 2069 6e20 7661 6c73 3a0d 0a20 2020 2020   in vals:..     
-00006a60: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00006a70: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
-00006a80: 5453 207c 207b 6b65 793a 2076 616c 7d0d  TS | {key: val}.
-00006a90: 0a0d 0a20 2020 2064 6566 2070 726f 6475  ...    def produ
-00006aa0: 6374 5f67 7269 6428 7365 6c66 293a 0d0a  ct_grid(self):..
-00006ab0: 2020 2020 2020 2020 2222 2247 7269 6420          """Grid 
-00006ac0: 7365 6172 6368 2061 6372 6f73 7320 616c  search across al
-00006ad0: 6c20 636f 6d62 696e 6174 696f 6e20 6f66  l combination of
-00006ae0: 2070 6172 616d 7322 2222 0d0a 2020 2020   params"""..    
-00006af0: 2020 2020 666f 7220 7661 6c73 2069 6e20      for vals in 
-00006b00: 7072 6f64 7563 7428 2a73 656c 662e 7661  product(*self.va
-00006b10: 6c75 6573 293a 0d0a 2020 2020 2020 2020  lues):..        
-00006b20: 2020 2020 7969 656c 6420 7365 6c66 2e63      yield self.c
-00006b30: 6667 2e44 4546 4155 4c54 5320 7c20 7b6f  fg.DEFAULTS | {o
-00006b40: 7074 696f 6e3a 7661 6c20 666f 7220 6f70  ption:val for op
-00006b50: 7469 6f6e 2c20 7661 6c20 696e 207a 6970  tion, val in zip
-00006b60: 2873 656c 662e 7061 7261 6d73 2c20 7661  (self.params, va
-00006b70: 6c73 297d 0d0a 0d0a 2020 2020 6465 6620  ls)}....    def 
-00006b80: 7361 7665 5f63 6865 636b 706f 696e 7428  save_checkpoint(
-00006b90: 7365 6c66 2c20 736f 7572 6365 3a20 4c69  self, source: Li
-00006ba0: 7374 2920 2d3e 204e 6f6e 653a 0d0a 2020  st) -> None:..  
-00006bb0: 2020 2020 2020 2222 2253 6176 6520 7468        """Save th
-00006bc0: 6520 7265 7374 206f 6620 7061 7261 6d73  e rest of params
-00006bd0: 2e22 2222 0d0a 2020 2020 2020 2020 7061  ."""..        pa
-00006be0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-00006bf0: 6e28 7365 6c66 2e63 6667 2e43 4f52 455f  n(self.cfg.CORE_
-00006c00: 4348 4543 4b50 4f49 4e54 5f50 4154 482c  CHECKPOINT_PATH,
-00006c10: 2073 656c 662e 6366 672e 4348 4543 4b50   self.cfg.CHECKP
-00006c20: 4f49 4e54 5f46 494c 454e 414d 4529 0d0a  OINT_FILENAME)..
-00006c30: 2020 2020 2020 2020 6368 6563 6b70 6f69          checkpoi
-00006c40: 6e74 203d 2064 6963 7428 290d 0a20 2020  nt = dict()..   
-00006c50: 2020 2020 2063 6865 636b 706f 696e 745b       checkpoint[
-00006c60: 2773 6f75 7263 6527 5d20 3d20 736f 7572  'source'] = sour
-00006c70: 6365 0d0a 2020 2020 2020 2020 746f 7263  ce..        torc
-00006c80: 682e 7361 7665 2863 6865 636b 706f 696e  h.save(checkpoin
-00006c90: 742c 2070 6174 6829 0d0a 0d0a 2020 2020  t, path)....    
-00006ca0: 4074 696d 656d 6574 6572 2822 436f 6163  @timemeter("Coac
-00006cb0: 682f 7265 7375 6d65 2229 0d0a 2020 2020  h/resume")..    
-00006cc0: 6465 6620 6c6f 6164 5f63 6865 636b 706f  def load_checkpo
-00006cd0: 696e 7428 7365 6c66 2920 2d3e 2069 6e74  int(self) -> int
-00006ce0: 3a0d 0a20 2020 2020 2020 2022 2222 4c6f  :..        """Lo
-00006cf0: 6164 2074 6865 2072 6573 7420 6f66 2070  ad the rest of p
-00006d00: 6172 616d 732e 2222 220d 0a20 2020 2020  arams."""..     
-00006d10: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
-00006d20: 5b43 6f61 6368 5d20 3e3e 3e20 4c6f 6164  [Coach] >>> Load
-00006d30: 2074 6865 2072 6563 656e 7420 6368 6563   the recent chec
-00006d40: 6b70 6f69 6e74 202e 2e2e 2229 0d0a 2020  kpoint ...")..  
-00006d50: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
-00006d60: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00006d70: 6667 2e43 4f52 455f 4348 4543 4b50 4f49  fg.CORE_CHECKPOI
-00006d80: 4e54 5f50 4154 482c 2073 656c 662e 6366  NT_PATH, self.cf
-00006d90: 672e 4348 4543 4b50 4f49 4e54 5f46 494c  g.CHECKPOINT_FIL
-00006da0: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
-00006db0: 6368 6563 6b70 6f69 6e74 203d 2074 6f72  checkpoint = tor
-00006dc0: 6368 2e6c 6f61 6428 7061 7468 290d 0a20  ch.load(path).. 
-00006dd0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-00006de0: 6563 6b70 6f69 6e74 5b27 736f 7572 6365  eckpoint['source
-00006df0: 275d 0d0a 0d0a 2020 2020 6465 6620 7265  ']....    def re
-00006e00: 7375 6d65 2873 656c 6629 3a0d 0a20 2020  sume(self):..   
-00006e10: 2020 2020 2022 2222 5265 7375 6d65 2066       """Resume f
-00006e20: 726f 6d20 7468 6520 7265 6365 6e74 2063  rom the recent c
-00006e30: 6865 636b 706f 696e 742e 2222 220d 0a20  heckpoint.""".. 
-00006e40: 2020 2020 2020 2073 6f75 7263 6520 3d20         source = 
-00006e50: 7365 6c66 2e65 6163 685f 6772 6964 2829  self.each_grid()
-00006e60: 2069 6620 7365 6c66 2e63 6667 2e45 5843   if self.cfg.EXC
-00006e70: 4c55 5349 5645 2065 6c73 6520 7365 6c66  LUSIVE else self
-00006e80: 2e70 726f 6475 6374 5f67 7269 6428 290d  .product_grid().
-00006e90: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
-00006ea0: 3d20 6c69 7374 2873 6f75 7263 6529 5b3a  = list(source)[:
-00006eb0: 3a2d 315d 0d0a 2020 2020 2020 2020 736f  :-1]..        so
-00006ec0: 7572 6365 203d 2073 656c 662e 6c6f 6164  urce = self.load
-00006ed0: 5f63 6865 636b 706f 696e 7428 2920 6966  _checkpoint() if
-00006ee0: 2073 656c 662e 6366 672e 7265 7375 6d65   self.cfg.resume
-00006ef0: 2065 6c73 6520 736f 7572 6365 0d0a 2020   else source..  
-00006f00: 2020 2020 2020 7265 7475 726e 2073 6f75        return sou
-00006f10: 7263 650d 0a0d 0a20 2020 2064 6566 2072  rce....    def r
-00006f20: 756e 2873 656c 662c 2063 6f6d 6d61 6e64  un(self, command
-00006f30: 3a20 7374 722c 2070 6172 616d 733a 2044  : str, params: D
-00006f40: 6963 7429 3a0d 0a20 2020 2020 2020 2022  ict):..        "
-00006f50: 2222 5374 6172 7420 6120 6e65 7720 7375  ""Start a new su
-00006f60: 6270 726f 6365 7373 2222 220d 0a20 2020  bprocess"""..   
-00006f70: 2020 2020 2069 6d70 6f72 7420 7375 6270       import subp
-00006f80: 726f 6365 7373 2c20 7368 6c65 780d 0a20  rocess, shlex.. 
-00006f90: 2020 2020 2020 2066 6f72 206f 7074 696f         for optio
-00006fa0: 6e2c 2076 616c 2069 6e20 7061 7261 6d73  n, val in params
-00006fb0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00006fc0: 2020 2020 2020 2063 6f6d 6d61 6e64 202b         command +
-00006fd0: 3d20 7365 6c66 2e67 6574 5f6f 7074 696f  = self.get_optio
-00006fe0: 6e28 6f70 7469 6f6e 2c20 7661 6c29 0d0a  n(option, val)..
-00006ff0: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
-00007000: 6572 2866 225c 3033 335b 303b 3331 3b34  er(f"\033[0;31;4
-00007010: 376d 7b63 6f6d 6d61 6e64 7d5c 3033 335b  7m{command}\033[
-00007020: 306d 2229 0d0a 2020 2020 2020 2020 7265  0m")..        re
-00007030: 7475 726e 2073 7562 7072 6f63 6573 732e  turn subprocess.
-00007040: 506f 7065 6e28 7368 6c65 782e 7370 6c69  Popen(shlex.spli
-00007050: 7428 636f 6d6d 616e 6429 290d 0a0d 0a20  t(command)).... 
-00007060: 2020 2064 6566 2077 6169 7428 7365 6c66     def wait(self
-00007070: 2c20 7461 736b 733a 204c 6973 7429 3a0d  , tasks: List):.
-00007080: 0a20 2020 2020 2020 2022 2222 5761 6974  .        """Wait
-00007090: 2075 7469 6c20 616c 6c20 7072 6f63 6573   util all proces
-000070a0: 7365 7320 7465 726d 696e 6174 652e 2222  ses terminate.""
-000070b0: 220d 0a20 2020 2020 2020 2074 6173 6b73  "..        tasks
-000070c0: 203d 205b 7461 736b 2066 6f72 2074 6173   = [task for tas
-000070d0: 6b20 696e 2074 6173 6b73 2069 6620 7461  k in tasks if ta
-000070e0: 736b 2069 7320 6e6f 7420 4e6f 6e65 5d0d  sk is not None].
-000070f0: 0a20 2020 2020 2020 2066 6f72 2070 726f  .        for pro
-00007100: 6365 7373 5f2c 2069 645f 2c20 6c6f 6750  cess_, id_, logP
-00007110: 6174 682c 2070 6172 616d 7320 696e 2074  ath, params in t
-00007120: 6173 6b73 3a0d 0a20 2020 2020 2020 2020  asks:..         
-00007130: 2020 2070 726f 6365 7373 5f2e 7761 6974     process_.wait
-00007140: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00007150: 7365 6c66 2e77 7269 7465 2869 645f 2c20  self.write(id_, 
-00007160: 6c6f 6750 6174 682c 2070 6172 616d 7329  logPath, params)
-00007170: 0d0a 0d0a 2020 2020 6465 6620 706f 6c6c  ....    def poll
-00007180: 2873 656c 662c 2074 6173 6b73 3a20 4c69  (self, tasks: Li
-00007190: 7374 293a 0d0a 2020 2020 2020 2020 2222  st):..        ""
-000071a0: 2257 6169 7420 7574 696c 2061 6e79 2070  "Wait util any p
-000071b0: 726f 6365 7373 2074 6572 6d69 6e61 7465  rocess terminate
-000071c0: 732e 2222 220d 0a20 2020 2020 2020 2064  s."""..        d
-000071d0: 6566 2069 735f 6e75 6c6c 2874 6173 6b29  ef is_null(task)
-000071e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000071f0: 6574 7572 6e20 7461 736b 2069 7320 4e6f  eturn task is No
-00007200: 6e65 0d0a 2020 2020 2020 2020 6275 6666  ne..        buff
-00007210: 6572 5f73 6f75 7263 6520 3d20 5b74 6173  er_source = [tas
-00007220: 6b5b 2d31 5d20 666f 7220 7461 736b 2069  k[-1] for task i
-00007230: 6e20 7461 736b 7320 6966 2074 6173 6b20  n tasks if task 
-00007240: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
-00007250: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00007260: 2831 2920 2320 666f 7220 756e 6971 7565  (1) # for unique
-00007270: 2069 640d 0a20 2020 2020 2020 2077 6869   id..        whi
-00007280: 6c65 206e 6f74 2061 6e79 286d 6170 2869  le not any(map(i
-00007290: 735f 6e75 6c6c 2c20 7461 736b 7329 293a  s_null, tasks)):
-000072a0: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-000072b0: 6d65 2e73 6c65 6570 2837 290d 0a20 2020  me.sleep(7)..   
-000072c0: 2020 2020 2020 2020 2062 7566 6665 725f           buffer_
-000072d0: 736f 7572 6365 203d 205b 5d0d 0a20 2020  source = []..   
-000072e0: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-000072f0: 2870 726f 6365 7373 5f2c 2069 645f 2c20  (process_, id_, 
-00007300: 6c6f 6750 6174 682c 2070 6172 616d 7329  logPath, params)
-00007310: 2069 6e20 656e 756d 6572 6174 6528 7461   in enumerate(ta
-00007320: 736b 7329 3a0d 0a20 2020 2020 2020 2020  sks):..         
-00007330: 2020 2020 2020 2069 6620 7072 6f63 6573         if proces
-00007340: 735f 2e70 6f6c 6c28 2920 6973 206e 6f74  s_.poll() is not
-00007350: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00007360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007370: 2e77 7269 7465 2869 645f 2c20 6c6f 6750  .write(id_, logP
-00007380: 6174 682c 2070 6172 616d 7329 0d0a 2020  ath, params)..  
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 7461 736b 735b 695d 203d 204e 6f6e    tasks[i] = Non
-000073b0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000073c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000073d0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
-000073e0: 6666 6572 5f73 6f75 7263 652e 6170 7065  ffer_source.appe
-000073f0: 6e64 2870 6172 616d 7329 0d0a 2020 2020  nd(params)..    
-00007400: 2020 2020 7365 6c66 2e73 6176 655f 6368      self.save_ch
-00007410: 6563 6b70 6f69 6e74 2873 656c 662e 736f  eckpoint(self.so
-00007420: 7572 6365 202b 2062 7566 6665 725f 736f  urce + buffer_so
-00007430: 7572 6365 290d 0a20 2020 2020 2020 2072  urce)..        r
-00007440: 6574 7572 6e20 7461 736b 732e 696e 6465  eturn tasks.inde
-00007450: 7828 4e6f 6e65 290d 0a0d 0a20 2020 2064  x(None)....    d
-00007460: 6566 2074 6572 6d69 6e61 7465 2873 656c  ef terminate(sel
-00007470: 662c 2074 6173 6b73 3a20 4c69 7374 293a  f, tasks: List):
-00007480: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
-00007490: 3d20 5b74 6173 6b20 666f 7220 7461 736b  = [task for task
-000074a0: 2069 6e20 7461 736b 7320 6966 2074 6173   in tasks if tas
-000074b0: 6b20 6973 206e 6f74 204e 6f6e 655d 0d0a  k is not None]..
-000074c0: 2020 2020 2020 2020 666f 7220 7072 6f63          for proc
-000074d0: 6573 735f 2c20 5f2c 205f 2c20 5f20 696e  ess_, _, _, _ in
-000074e0: 2074 6173 6b73 3a0d 0a20 2020 2020 2020   tasks:..       
-000074f0: 2020 2020 2069 6620 7072 6f63 6573 735f       if process_
-00007500: 2e70 6f6c 6c28 2920 6973 204e 6f6e 653a  .poll() is None:
-00007510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007520: 2020 7072 6f63 6573 735f 2e74 6572 6d69    process_.termi
-00007530: 6e61 7465 2829 0d0a 2020 2020 2020 2020  nate()..        
-00007540: 7469 6d65 2e73 6c65 6570 2833 290d 0a20  time.sleep(3).. 
-00007550: 2020 2020 2020 2066 6f72 2070 726f 6365         for proce
-00007560: 7373 5f2c 205f 2c20 5f2c 205f 2069 6e20  ss_, _, _, _ in 
-00007570: 7461 736b 733a 0d0a 2020 2020 2020 2020  tasks:..        
-00007580: 2020 2020 6966 2070 726f 6365 7373 5f2e      if process_.
-00007590: 706f 6c6c 2829 2069 7320 4e6f 6e65 3a0d  poll() is None:.
-000075a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000075b0: 2070 726f 6365 7373 5f2e 6b69 6c6c 2829   process_.kill()
-000075c0: 0d0a 2020 2020 2020 2020 7379 732e 6578  ..        sys.ex
-000075d0: 6974 2829 0d0a 0d0a 2020 2020 4074 696d  it()....    @tim
-000075e0: 656d 6574 6572 2822 4164 6170 7465 722f  emeter("Adapter/
-000075f0: 6669 7422 290d 0a20 2020 2064 6566 2066  fit")..    def f
-00007600: 6974 2873 656c 6629 3a0d 0a20 2020 2020  it(self):..     
-00007610: 2020 2022 2222 4772 6964 2073 6561 7263     """Grid searc
-00007620: 682e 2222 220d 0a20 2020 2020 2020 2073  h."""..        s
-00007630: 656c 662e 736f 7572 6365 203d 2073 656c  elf.source = sel
-00007640: 662e 7265 7375 6d65 2829 0d0a 2020 2020  f.resume()..    
-00007650: 2020 2020 7461 736b 7320 3d20 5b4e 6f6e      tasks = [Non
-00007660: 6520 666f 7220 5f20 696e 2072 616e 6765  e for _ in range
-00007670: 286c 656e 2873 656c 662e 6465 7669 6365  (len(self.device
-00007680: 7329 295d 0d0a 0d0a 2020 2020 2020 2020  s))]....        
-00007690: 6465 6620 7369 676e 616c 5f68 616e 646c  def signal_handl
-000076a0: 6572 2873 6967 2c20 6672 616d 6529 3a0d  er(sig, frame):.
-000076b0: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
-000076c0: 6f4c 6f67 6765 7228 6622 5c30 3333 5b30  oLogger(f"\033[0
-000076d0: 3b33 313b 3437 6d3d 3d3d 3d3d 3d3d 3d3d  ;31;47m=========
-000076e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000076f0: 3d3d 3d3d 3d3d 5445 524d 494e 4154 4520  ======TERMINATE 
-00007700: 414c 4c20 5355 4250 524f 4345 5353 4553  ALL SUBPROCESSES
-00007710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c  ===============\
-00007730: 3033 335b 306d 2229 0d0a 2020 2020 2020  033[0m")..      
-00007740: 2020 2020 2020 7365 6c66 2e74 6572 6d69        self.termi
-00007750: 6e61 7465 2874 6173 6b73 290d 0a20 2020  nate(tasks)..   
-00007760: 2020 2020 2073 6967 6e61 6c2e 7369 676e       signal.sign
-00007770: 616c 2873 6967 6e61 6c2e 5349 4749 4e54  al(signal.SIGINT
-00007780: 2c20 7369 676e 616c 5f68 616e 646c 6572  , signal_handler
-00007790: 290d 0a0d 0a20 2020 2020 2020 2074 7279  )....        try
-000077a0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
-000077b0: 6869 6c65 2073 656c 662e 736f 7572 6365  hile self.source
-000077c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000077d0: 2020 2069 6e64 6578 203d 2073 656c 662e     index = self.
-000077e0: 706f 6c6c 2874 6173 6b73 290d 0a20 2020  poll(tasks)..   
-000077f0: 2020 2020 2020 2020 2020 2020 2064 6576               dev
-00007800: 6963 6520 3d20 7365 6c66 2e64 6576 6963  ice = self.devic
-00007810: 6573 5b69 6e64 6578 5d0d 0a20 2020 2020  es[index]..     
-00007820: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00007830: 7320 3d20 7365 6c66 2e73 6f75 7263 652e  s = self.source.
-00007840: 706f 7028 290d 0a20 2020 2020 2020 2020  pop()..         
-00007850: 2020 2020 2020 2063 6f6d 6d61 6e64 2c20         command, 
-00007860: 6964 5f2c 206c 6f67 5061 7468 203d 2073  id_, logPath = s
-00007870: 656c 662e 7265 6769 7374 6572 2864 6576  elf.register(dev
-00007880: 6963 6529 0d0a 2020 2020 2020 2020 2020  ice)..          
-00007890: 2020 2020 2020 7072 6f63 6573 735f 203d        process_ =
-000078a0: 2073 656c 662e 7275 6e28 636f 6d6d 616e   self.run(comman
-000078b0: 642c 2070 6172 616d 7329 0d0a 2020 2020  d, params)..    
-000078c0: 2020 2020 2020 2020 2020 2020 7461 736b              task
-000078d0: 735b 696e 6465 785d 203d 2028 7072 6f63  s[index] = (proc
-000078e0: 6573 735f 2c20 6964 5f2c 206c 6f67 5061  ess_, id_, logPa
-000078f0: 7468 2c20 7061 7261 6d73 290d 0a20 2020  th, params)..   
-00007900: 2020 2020 2066 696e 616c 6c79 3a0d 0a20       finally:.. 
-00007910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007920: 7761 6974 2874 6173 6b73 290d 0a20 2020  wait(tasks)..   
-00007930: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00007940: 726d 696e 6174 6528 7461 736b 7329       rminate(tasks)
+000002d0: 5f5f 203d 205b 0d0a 2020 2020 2743 6869  __ = [..    'Chi
+000002e0: 6566 436f 6163 6827 2c20 2743 6f61 6368  efCoach', 'Coach
+000002f0: 272c 2027 4164 6170 7465 7227 2c0d 0a20  ', 'Adapter',.. 
+00000300: 2020 2027 4765 6e43 6f61 6368 272c 2027     'GenCoach', '
+00000310: 5365 7143 6f61 6368 272c 2027 5365 7373  SeqCoach', 'Sess
+00000320: 436f 6163 6827 0d0a 5d0d 0a0d 0a0d 0a44  Coach'..]......D
+00000330: 4546 4155 4c54 5f4d 4554 5249 4353 203d  EFAULT_METRICS =
+00000340: 207b 0d0a 2020 2020 274c 4f53 5327 3a20   {..    'LOSS': 
+00000350: 6c61 6d62 6461 2078 3a20 782c 0d0a 2020  lambda x: x,..  
+00000360: 2020 2323 2323 2323 2323 2323 2323 230d    #############.
+00000370: 0a20 2020 2027 4d53 4527 3a20 6d65 616e  .    'MSE': mean
+00000380: 5f73 7175 6172 6564 5f65 7272 6f72 2c0d  _squared_error,.
+00000390: 0a20 2020 2027 4d41 4527 3a20 6d65 616e  .    'MAE': mean
+000003a0: 5f61 6273 5f65 7272 6f72 2c0d 0a20 2020  _abs_error,..   
+000003b0: 2027 524d 5345 273a 2072 6f6f 745f 6d73   'RMSE': root_ms
+000003c0: 652c 0d0a 2020 2020 2323 2323 2323 2323  e,..    ########
+000003d0: 2323 2323 230d 0a20 2020 2027 5052 4543  #####..    'PREC
+000003e0: 4953 494f 4e27 3a20 7072 6563 6973 696f  ISION': precisio
+000003f0: 6e2c 0d0a 2020 2020 2752 4543 414c 4c27  n,..    'RECALL'
+00000400: 3a20 7265 6361 6c6c 2c0d 0a20 2020 2027  : recall,..    '
+00000410: 4631 273a 2066 315f 7363 6f72 652c 0d0a  F1': f1_score,..
+00000420: 2020 2020 2741 5543 273a 2061 7572 6f63      'AUC': auroc
+00000430: 2c0d 0a20 2020 2027 4849 5452 4154 4527  ,..    'HITRATE'
+00000440: 3a20 6869 745f 7261 7465 2c0d 0a20 2020  : hit_rate,..   
+00000450: 2023 2323 2323 2323 2323 2323 2323 0d0a   #############..
+00000460: 2020 2020 274e 4443 4727 3a20 6e6f 726d      'NDCG': norm
+00000470: 616c 697a 6564 5f64 6367 2c0d 0a20 2020  alized_dcg,..   
+00000480: 2027 4d52 5227 3a20 6d65 616e 5f72 6563   'MRR': mean_rec
+00000490: 6970 726f 6361 6c5f 7261 6e6b 2c0d 0a20  iprocal_rank,.. 
+000004a0: 2020 2027 4d41 5027 3a20 6d65 616e 5f61     'MAP': mean_a
+000004b0: 7665 7261 6765 5f70 7265 6369 7369 6f6e  verage_precision
+000004c0: 0d0a 7d0d 0a0d 0a44 4546 4155 4c54 5f46  ..}....DEFAULT_F
+000004d0: 4d54 5320 3d20 7b0d 0a20 2020 2027 4c4f  MTS = {..    'LO
+000004e0: 5353 273a 2022 2e35 6622 2c0d 0a20 2020  SS': ".5f",..   
+000004f0: 2023 2323 2323 2323 2323 2323 2323 0d0a   #############..
+00000500: 2020 2020 274d 5345 273a 2022 2e34 6622      'MSE': ".4f"
+00000510: 2c0d 0a20 2020 2027 4d41 4527 3a20 222e  ,..    'MAE': ".
+00000520: 3466 222c 0d0a 2020 2020 2752 4d53 4527  4f",..    'RMSE'
+00000530: 3a20 222e 3466 222c 0d0a 2020 2020 2323  : ".4f",..    ##
+00000540: 2323 2323 2323 2323 2323 230d 0a20 2020  ###########..   
+00000550: 2027 5052 4543 4953 494f 4e27 3a20 222e   'PRECISION': ".
+00000560: 3466 222c 0d0a 2020 2020 2752 4543 414c  4f",..    'RECAL
+00000570: 4c27 3a20 222e 3466 222c 0d0a 2020 2020  L': ".4f",..    
+00000580: 2746 3127 3a20 222e 3466 222c 0d0a 2020  'F1': ".4f",..  
+00000590: 2020 2741 5543 273a 2022 2e34 6622 2c0d    'AUC': ".4f",.
+000005a0: 0a20 2020 2027 4849 5452 4154 4527 3a20  .    'HITRATE': 
+000005b0: 222e 3466 222c 0d0a 2020 2020 2323 2323  ".4f",..    ####
+000005c0: 2323 2323 2323 2323 230d 0a20 2020 2027  #########..    '
+000005d0: 4e44 4347 273a 2022 2e34 6622 2c0d 0a20  NDCG': ".4f",.. 
+000005e0: 2020 2027 4d52 5227 3a20 222e 3466 222c     'MRR': ".4f",
+000005f0: 0d0a 2020 2020 274d 4150 273a 2022 2e34  ..    'MAP': ".4
+00000600: 6622 2c0d 0a7d 0d0a 0d0a 4445 4641 554c  f",..}....DEFAUL
+00000610: 545f 4245 5354 5f43 4153 5445 5220 3d20  T_BEST_CASTER = 
+00000620: 7b0d 0a20 2020 2027 4c4f 5353 273a 206d  {..    'LOSS': m
+00000630: 696e 2c0d 0a20 2020 2023 2323 2323 2323  in,..    #######
+00000640: 2323 2323 2323 0d0a 2020 2020 274d 5345  ######..    'MSE
+00000650: 273a 206d 696e 2c0d 0a20 2020 2027 4d41  ': min,..    'MA
+00000660: 4527 3a20 6d69 6e2c 0d0a 2020 2020 2752  E': min,..    'R
+00000670: 4d53 4527 3a20 6d69 6e2c 0d0a 2020 2020  MSE': min,..    
+00000680: 2323 2323 2323 2323 2323 2323 230d 0a20  #############.. 
+00000690: 2020 2027 5052 4543 4953 494f 4e27 3a20     'PRECISION': 
+000006a0: 6d61 782c 0d0a 2020 2020 2752 4543 414c  max,..    'RECAL
+000006b0: 4c27 3a20 6d61 782c 0d0a 2020 2020 2746  L': max,..    'F
+000006c0: 3127 3a20 6d61 782c 0d0a 2020 2020 2741  1': max,..    'A
+000006d0: 5543 273a 206d 6178 2c0d 0a20 2020 2027  UC': max,..    '
+000006e0: 4849 5452 4154 4527 3a20 6d61 782c 0d0a  HITRATE': max,..
+000006f0: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00000700: 230d 0a20 2020 2027 4e44 4347 273a 206d  #..    'NDCG': m
+00000710: 6178 2c0d 0a20 2020 2027 4d52 5227 3a20  ax,..    'MRR': 
+00000720: 6d61 782c 0d0a 2020 2020 274d 4150 273a  max,..    'MAP':
+00000730: 206d 6178 2c0d 0a7d 0d0a 0d0a 0d0a 636c   max,..}......cl
+00000740: 6173 7320 5f44 756d 6d79 4d6f 6475 6c65  ass _DummyModule
+00000750: 2874 6f72 6368 2e6e 6e2e 4d6f 6475 6c65  (torch.nn.Module
+00000760: 293a 0d0a 2020 2020 2222 2254 6869 7320  ):..    """This 
+00000770: 6973 2061 2064 756d 6d79 206d 6f64 756c  is a dummy modul
+00000780: 6520 7468 6174 2073 6572 7665 7320 6173  e that serves as
+00000790: 2061 2070 6c61 6365 686f 6c64 6572 2066   a placeholder f
+000007a0: 6f72 2061 2072 6561 6c20 6d6f 6465 6c2e  or a real model.
+000007b0: 2222 220d 0a20 2020 2064 6566 2066 6f72  """..    def for
+000007c0: 7761 7264 2873 656c 662c 202a 6172 6773  ward(self, *args
+000007d0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+000007e0: 2020 2020 2020 2222 2244 756d 6d79 2066        """Dummy f
+000007f0: 6f72 7761 7264 206d 6574 686f 6420 7468  orward method th
+00000800: 6174 2072 6169 7365 7320 6120 604e 6f74  at raises a `Not
+00000810: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00000820: 602e 2222 220d 0a20 2020 2020 2020 2072  `."""..        r
+00000830: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+00000840: 7465 6445 7272 6f72 2822 4e6f 206d 6f64  tedError("No mod
+00000850: 656c 2061 7661 696c 6162 6c65 2066 6f72  el available for
+00000860: 2043 6f61 6368 202e 2e2e 2229 0d0a 0d0a   Coach ...")....
+00000870: 2020 2020 6465 6620 7374 6570 2873 656c      def step(sel
+00000880: 662c 202a 6172 6773 2c20 2a2a 6b77 6172  f, *args, **kwar
+00000890: 6773 293a 0d0a 2020 2020 2020 2020 2222  gs):..        ""
+000008a0: 2244 756d 6d79 2073 7465 7020 6d65 7468  "Dummy step meth
+000008b0: 6f64 2074 6861 7420 7261 6973 6573 2061  od that raises a
+000008c0: 2060 4e6f 7449 6d70 6c65 6d65 6e74 6564   `NotImplemented
+000008d0: 4572 726f 7260 2e22 2222 0d0a 2020 2020  Error`."""..    
+000008e0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+000008f0: 6c65 6d65 6e74 6564 4572 726f 7228 224e  lementedError("N
+00000900: 6f20 6f70 7469 6d69 7a65 7220 6f72 206c  o optimizer or l
+00000910: 7220 7363 6865 6475 6c65 7220 6176 6169  r scheduler avai
+00000920: 6c61 626c 6520 666f 7220 436f 6163 6820  lable for Coach 
+00000930: 2e2e 2e22 290d 0a0d 0a20 2020 2064 6566  ...")....    def
+00000940: 2062 6163 6b77 6172 6428 7365 6c66 2c20   backward(self, 
+00000950: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00000960: 3a0d 0a20 2020 2020 2020 2022 2222 4475  :..        """Du
+00000970: 6d6d 7920 6261 636b 7761 7264 206d 6574  mmy backward met
+00000980: 686f 6420 7468 6174 2072 6169 7365 7320  hod that raises 
+00000990: 6120 604e 6f74 496d 706c 656d 656e 7465  a `NotImplemente
+000009a0: 6445 7272 6f72 602e 2222 220d 0a20 2020  dError`."""..   
+000009b0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+000009c0: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
+000009d0: 4e6f 206f 7074 696d 697a 6572 2061 7661  No optimizer ava
+000009e0: 696c 6162 6c65 2066 6f72 2043 6f61 6368  ilable for Coach
+000009f0: 202e 2e2e 2229 0d0a 0d0a 0d0a 636c 6173   ...")......clas
+00000a00: 7320 4368 6965 6643 6f61 6368 286d 6574  s ChiefCoach(met
+00000a10: 6163 6c61 7373 3d61 6263 2e41 4243 4d65  aclass=abc.ABCMe
+00000a20: 7461 293a 0d0a 2020 2020 7222 2222 200d  ta):..    r""" .
+00000a30: 0a20 2020 2054 6865 2060 4368 6965 6643  .    The `ChiefC
+00000a40: 6f61 6368 6020 636c 6173 7320 6973 2074  oach` class is t
+00000a50: 6865 2074 6f70 2d6c 6576 656c 2063 6c61  he top-level cla
+00000a60: 7373 2066 6f72 2072 756e 6e69 6e67 2074  ss for running t
+00000a70: 6865 2074 7261 696e 696e 6720 616e 6420  he training and 
+00000a80: 6576 616c 7561 7469 6f6e 206c 6f6f 7073  evaluation loops
+00000a90: 2e0d 0a0d 0a20 2020 2050 6172 616d 6574  .....    Paramet
+00000aa0: 6572 733a 0d0a 2020 2020 2d2d 2d2d 2d2d  ers:..    ------
+00000ab0: 2d2d 2d2d 2d0d 0a20 2020 2074 7261 696e  -----..    train
+00000ac0: 7069 7065 203a 2049 7465 7244 6174 6150  pipe : IterDataP
+00000ad0: 6970 650d 0a20 2020 2020 2020 2049 7465  ipe..        Ite
+00000ae0: 7261 626c 6520 6461 7461 2070 6970 656c  rable data pipel
+00000af0: 696e 6520 666f 7220 7472 6169 6e69 6e67  ine for training
+00000b00: 2064 6174 612e 0d0a 2020 2020 7661 6c69   data...    vali
+00000b10: 6470 6970 6520 3a20 4974 6572 4461 7461  dpipe : IterData
+00000b20: 5069 7065 2c20 6f70 7469 6f6e 616c 0d0a  Pipe, optional..
+00000b30: 2020 2020 2020 2020 4974 6572 6162 6c65          Iterable
+00000b40: 2064 6174 6120 7069 7065 6c69 6e65 2066   data pipeline f
+00000b50: 6f72 2076 616c 6964 6174 696f 6e20 6461  or validation da
+00000b60: 7461 2e0d 0a20 2020 2020 2020 2049 6620  ta...        If 
+00000b70: 604e 6f6e 6560 2c20 7573 6520 6074 7261  `None`, use `tra
+00000b80: 696e 7069 7065 6020 696e 7374 6561 642e  inpipe` instead.
+00000b90: 0d0a 2020 2020 7465 7374 7069 7065 203a  ..    testpipe :
+00000ba0: 2049 7465 7244 6174 6150 6970 652c 206f   IterDataPipe, o
+00000bb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00000bc0: 2049 7465 7261 626c 6520 6461 7461 2070   Iterable data p
+00000bd0: 6970 656c 696e 6520 666f 7220 7465 7374  ipeline for test
+00000be0: 696e 6720 6461 7461 2e0d 0a20 2020 2020  ing data...     
+00000bf0: 2020 2049 6620 604e 6f6e 6560 2c20 7573     If `None`, us
+00000c00: 6520 6076 616c 6964 7069 7065 6020 696e  e `validpipe` in
+00000c10: 7374 6561 642e 0d0a 2020 2020 6669 656c  stead...    fiel
+00000c20: 6473 203a 2049 7465 7261 626c 655b 4669  ds : Iterable[Fi
+00000c30: 656c 644d 6f64 756c 655d 0d0a 2020 2020  eldModule]..    
+00000c40: 2020 2020 5475 706c 6520 6f66 2060 4669      Tuple of `Fi
+00000c50: 656c 644d 6f64 756c 6560 7320 666f 7220  eldModule`s for 
+00000c60: 6461 7461 7365 7420 6669 656c 6473 2e0d  dataset fields..
+00000c70: 0a20 2020 206d 6f64 656c 203a 2055 6e69  .    model : Uni
+00000c80: 6f6e 5b52 6563 5379 7341 7263 682c 2074  on[RecSysArch, t
+00000c90: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 2c20  orch.nn.Module, 
+00000ca0: 4e6f 6e65 5d0d 0a20 2020 2020 2020 204d  None]..        M
+00000cb0: 6f64 656c 2066 6f72 2074 7261 696e 696e  odel for trainin
+00000cc0: 6720 616e 6420 6576 616c 7561 7469 6e67  g and evaluating
+00000cd0: 2e20 0d0a 2020 2020 2020 2020 4966 2060  . ..        If `
+00000ce0: 4e6f 6e65 602c 2075 7365 205f 4475 6d6d  None`, use _Dumm
+00000cf0: 794d 6f64 756c 6520 696e 7374 6561 642c  yModule instead,
+00000d00: 2077 6869 6368 2073 686f 756c 6420 6e6f   which should no
+00000d10: 7420 6361 6c6c 2060 666f 7277 6172 6460  t call `forward`
+00000d20: 2e0d 0a20 2020 2063 7269 7465 7269 6f6e  ...    criterion
+00000d30: 203a 2055 6e69 6f6e 5b42 6173 6543 7269   : Union[BaseCri
+00000d40: 7465 7269 6f6e 2c20 4361 6c6c 6162 6c65  terion, Callable
+00000d50: 5d0d 0a20 2020 2020 2020 2043 616c 6c61  ]..        Calla
+00000d60: 626c 6520 666f 7220 636f 6d70 7574 696e  ble for computin
+00000d70: 6720 7468 6520 6c6f 7373 2066 756e 6374  g the loss funct
+00000d80: 696f 6e2e 0d0a 2020 2020 6f70 7469 6d69  ion...    optimi
+00000d90: 7a65 7220 3a20 746f 7263 682e 6f70 7469  zer : torch.opti
+00000da0: 6d2e 4f70 7469 6d69 7a65 722c 206f 7074  m.Optimizer, opt
+00000db0: 696f 6e61 6c0d 0a20 2020 2020 2020 204f  ional..        O
+00000dc0: 7074 696d 697a 6572 2066 6f72 2075 7064  ptimizer for upd
+00000dd0: 6174 696e 6720 6d6f 6465 6c20 7061 7261  ating model para
+00000de0: 6d65 7465 7273 2e20 0d0a 2020 2020 2020  meters. ..      
+00000df0: 2020 4966 2060 4e6f 6e65 602c 2075 7365    If `None`, use
+00000e00: 205f 4475 6d6d 794d 6f64 756c 6520 696e   _DummyModule in
+00000e10: 7374 6561 642c 2077 6869 6368 2073 686f  stead, which sho
+00000e20: 756c 6420 6e6f 7420 6361 6c6c 2060 7374  uld not call `st
+00000e30: 6570 6020 616e 6420 6062 6163 6b77 6172  ep` and `backwar
+00000e40: 6460 2e0d 0a20 2020 206c 725f 7363 6865  d`...    lr_sche
+00000e50: 6475 6c65 7220 3a20 746f 7263 682e 6f70  duler : torch.op
+00000e60: 7469 6d2e 6c72 5f73 6368 6564 756c 6572  tim.lr_scheduler
+00000e70: 2e5f 4c52 5363 6865 6475 6c65 722c 206f  ._LRScheduler, o
+00000e80: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00000e90: 204c 6561 726e 696e 6720 7261 7465 2073   Learning rate s
+00000ea0: 6368 6564 756c 6572 2e20 4966 2060 4e6f  cheduler. If `No
+00000eb0: 6e65 602c 2075 7365 205f 4475 6d6d 794d  ne`, use _DummyM
+00000ec0: 6f64 756c 6520 696e 7374 6561 642c 200d  odule instead, .
+00000ed0: 0a20 2020 2020 2020 2077 6869 6368 2073  .        which s
+00000ee0: 686f 756c 6420 6e6f 7420 6361 6c6c 2060  hould not call `
+00000ef0: 7374 6570 602e 0d0a 2020 2020 6465 7669  step`...    devi
+00000f00: 6365 203a 2055 6e69 6f6e 5b74 6f72 6368  ce : Union[torch
+00000f10: 2e64 6576 6963 652c 2073 7472 2c20 696e  .device, str, in
+00000f20: 745d 0d0a 2020 2020 2020 2020 4465 7669  t]..        Devi
+00000f30: 6365 206f 6e20 7768 6963 6820 746f 2072  ce on which to r
+00000f40: 756e 2074 6865 2063 6f6d 7075 7461 7469  un the computati
+00000f50: 6f6e 2e20 0d0a 2020 2020 2020 2020 2020  on. ..          
+00000f60: 2020 2d20 6074 6f72 6368 2e64 6576 6963    - `torch.devic
+00000f70: 6560 0d0a 2020 2020 2020 2020 2020 2020  e`..            
+00000f80: 2d20 6073 7472 603a 204c 696b 6520 6063  - `str`: Like `c
+00000f90: 7075 602c 2060 6375 6461 3a30 602e 0d0a  pu`, `cuda:0`...
+00000fa0: 2020 2020 2020 2020 2020 2020 2d20 6069              - `i
+00000fb0: 6e74 603a 2055 7369 6e67 2063 7564 613a  nt`: Using cuda:
+00000fc0: 6069 6e74 602e 0d0a 2020 2020 2222 220d  `int`...    """.
+00000fd0: 0a0d 0a0d 0a20 2020 2064 6566 205f 5f69  .....    def __i
+00000fe0: 6e69 745f 5f28 0d0a 2020 2020 2020 2020  nit__(..        
+00000ff0: 7365 6c66 2c20 2a2c 0d0a 2020 2020 2020  self, *,..      
+00001000: 2020 7472 6169 6e70 6970 653a 2049 7465    trainpipe: Ite
+00001010: 7244 6174 6150 6970 652c 2076 616c 6964  rDataPipe, valid
+00001020: 7069 7065 3a20 4f70 7469 6f6e 616c 5b49  pipe: Optional[I
+00001030: 7465 7244 6174 6150 6970 655d 2c20 7465  terDataPipe], te
+00001040: 7374 7069 7065 3a20 4f70 7469 6f6e 616c  stpipe: Optional
+00001050: 5b49 7465 7244 6174 6150 6970 655d 2c20  [IterDataPipe], 
+00001060: 6669 656c 6473 3a20 4974 6572 6162 6c65  fields: Iterable
+00001070: 5b46 6965 6c64 4d6f 6475 6c65 5d2c 0d0a  [FieldModule],..
+00001080: 2020 2020 2020 2020 6d6f 6465 6c3a 2055          model: U
+00001090: 6e69 6f6e 5b52 6563 5379 7341 7263 682c  nion[RecSysArch,
+000010a0: 2074 6f72 6368 2e6e 6e2e 4d6f 6475 6c65   torch.nn.Module
+000010b0: 2c20 4e6f 6e65 5d2c 2063 7269 7465 7269  , None], criteri
+000010c0: 6f6e 3a20 556e 696f 6e5b 4261 7365 4372  on: Union[BaseCr
+000010d0: 6974 6572 696f 6e2c 2043 616c 6c61 626c  iterion, Callabl
+000010e0: 655d 2c20 0d0a 2020 2020 2020 2020 6f70  e], ..        op
+000010f0: 7469 6d69 7a65 723a 204f 7074 696f 6e61  timizer: Optiona
+00001100: 6c5b 746f 7263 682e 6f70 7469 6d2e 4f70  l[torch.optim.Op
+00001110: 7469 6d69 7a65 725d 2c20 6c72 5f73 6368  timizer], lr_sch
+00001120: 6564 756c 6572 3a20 4f70 7469 6f6e 616c  eduler: Optional
+00001130: 5b74 6f72 6368 2e6f 7074 696d 2e6c 725f  [torch.optim.lr_
+00001140: 7363 6865 6475 6c65 722e 5f4c 5253 6368  scheduler._LRSch
+00001150: 6564 756c 6572 5d2c 0d0a 2020 2020 2020  eduler],..      
+00001160: 2020 6465 7669 6365 3a20 556e 696f 6e5b    device: Union[
+00001170: 746f 7263 682e 6465 7669 6365 2c20 7374  torch.device, st
+00001180: 722c 2069 6e74 5d0d 0a20 2020 2029 3a0d  r, int]..    ):.
+00001190: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+000011a0: 6669 656c 6473 3a20 4669 656c 6454 7570  fields: FieldTup
+000011b0: 6c65 5b46 6965 6c64 4d6f 6475 6c65 5d20  le[FieldModule] 
+000011c0: 3d20 4669 656c 6454 7570 6c65 2866 6965  = FieldTuple(fie
+000011d0: 6c64 7329 0d0a 2020 2020 2020 2020 7365  lds)..        se
+000011e0: 6c66 2e64 6576 6963 6520 3d20 746f 7263  lf.device = torc
+000011f0: 682e 6465 7669 6365 2864 6576 6963 6529  h.device(device)
+00001200: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00001210: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+00001220: 682e 6375 6461 2e73 6574 5f64 6576 6963  h.cuda.set_devic
+00001230: 6528 7365 6c66 2e64 6576 6963 6529 0d0a  e(self.device)..
+00001240: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+00001250: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
+00001260: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00001270: 2020 2020 2020 6578 6365 7074 2041 7474        except Att
+00001280: 7269 6275 7465 4572 726f 723a 0d0a 2020  ributeError:..  
+00001290: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+000012a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000012b0: 7365 745f 6461 7461 7069 7065 2874 7261  set_datapipe(tra
+000012c0: 696e 7069 7065 2c20 7661 6c69 6470 6970  inpipe, validpip
+000012d0: 652c 2074 6573 7470 6970 6529 0d0a 2020  e, testpipe)..  
+000012e0: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
+000012f0: 6f74 6865 7228 6d6f 6465 6c2c 2063 7269  other(model, cri
+00001300: 7465 7269 6f6e 2c20 6f70 7469 6d69 7a65  terion, optimize
+00001310: 722c 206c 725f 7363 6865 6475 6c65 7229  r, lr_scheduler)
+00001320: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00001330: 2e5f 5f6d 6f64 6520 3d20 2774 7261 696e  .__mode = 'train
+00001340: 270d 0a0d 0a20 2020 2020 2020 2064 6566  '....        def
+00001350: 2063 6c65 616e 2829 3a0d 0a20 2020 2020   clean():..     
+00001360: 2020 2020 2020 2070 6172 656e 7420 3d20         parent = 
+00001370: 7073 7574 696c 2e50 726f 6365 7373 286f  psutil.Process(o
+00001380: 732e 6765 7470 6964 2829 290d 0a20 2020  s.getpid())..   
+00001390: 2020 2020 2020 2020 2063 6869 6c64 7265           childre
+000013a0: 6e20 3d20 7061 7265 6e74 2e63 6869 6c64  n = parent.child
+000013b0: 7265 6e28 7265 6375 7273 6976 653d 5472  ren(recursive=Tr
+000013c0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000013d0: 2066 6f72 2070 726f 6365 7373 2069 6e20   for process in 
+000013e0: 6368 696c 6472 656e 3a0d 0a20 2020 2020  children:..     
+000013f0: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+00001400: 7373 2e73 656e 645f 7369 676e 616c 2873  ss.send_signal(s
+00001410: 6967 6e61 6c2e 5349 4754 4552 4d29 0d0a  ignal.SIGTERM)..
+00001420: 2020 2020 2020 2020 2020 2020 7073 7574              psut
+00001430: 696c 2e77 6169 745f 7072 6f63 7328 6368  il.wait_procs(ch
+00001440: 696c 6472 656e 2c20 7469 6d65 6f75 743d  ildren, timeout=
+00001450: 3529 0d0a 0d0a 2020 2020 2020 2020 6174  5)....        at
+00001460: 6578 6974 2e72 6567 6973 7465 7228 636c  exit.register(cl
+00001470: 6561 6e29 0d0a 0d0a 0d0a 2020 2020 6465  ean)......    de
+00001480: 6620 5f73 6574 5f64 6174 6170 6970 6528  f _set_datapipe(
+00001490: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
+000014a0: 0a20 2020 2020 2020 2074 7261 696e 7069  .        trainpi
+000014b0: 7065 2c0d 0a20 2020 2020 2020 2076 616c  pe,..        val
+000014c0: 6964 7069 7065 3d4e 6f6e 652c 0d0a 2020  idpipe=None,..  
+000014d0: 2020 2020 2020 7465 7374 7069 7065 3d4e        testpipe=N
+000014e0: 6f6e 652c 0d0a 2020 2020 293a 0d0a 2020  one,..    ):..  
+000014f0: 2020 2020 2020 2222 2253 6574 2074 6865        """Set the
+00001500: 2064 6174 6120 7069 7065 2066 6f72 2074   data pipe for t
+00001510: 7261 696e 696e 672c 2076 616c 6964 6174  raining, validat
+00001520: 696f 6e20 616e 6420 7465 7374 2e22 2222  ion and test."""
+00001530: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00001540: 7261 696e 7069 7065 203d 2074 7261 696e  rainpipe = train
+00001550: 7069 7065 0d0a 2020 2020 2020 2020 7365  pipe..        se
+00001560: 6c66 2e76 616c 6964 7069 7065 203d 2073  lf.validpipe = s
+00001570: 656c 662e 7472 6169 6e70 6970 6520 6966  elf.trainpipe if
+00001580: 2076 616c 6964 7069 7065 2069 7320 4e6f   validpipe is No
+00001590: 6e65 2065 6c73 6520 7661 6c69 6470 6970  ne else validpip
+000015a0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000015b0: 7465 7374 7069 7065 203d 2073 656c 662e  testpipe = self.
+000015c0: 7661 6c69 6470 6970 6520 6966 2074 6573  validpipe if tes
+000015d0: 7470 6970 6520 6973 204e 6f6e 6520 656c  tpipe is None el
+000015e0: 7365 2074 6573 7470 6970 650d 0a0d 0a20  se testpipe.... 
+000015f0: 2020 2064 6566 205f 7365 745f 6f74 6865     def _set_othe
+00001600: 7228 0d0a 2020 2020 2020 2020 7365 6c66  r(..        self
+00001610: 2c0d 0a20 2020 2020 2020 206d 6f64 656c  ,..        model
+00001620: 3d4e 6f6e 652c 2063 7269 7465 7269 6f6e  =None, criterion
+00001630: 3d4e 6f6e 652c 206f 7074 696d 697a 6572  =None, optimizer
+00001640: 3d4e 6f6e 652c 206c 725f 7363 6865 6475  =None, lr_schedu
+00001650: 6c65 723d 4e6f 6e65 2c0d 0a20 2020 2029  ler=None,..    )
+00001660: 3a0d 0a20 2020 2020 2020 2022 2222 5365  :..        """Se
+00001670: 7420 7468 6520 6f74 6865 7220 6e65 6365  t the other nece
+00001680: 7373 6172 7920 636f 6d70 6f6e 656e 7473  ssary components
+00001690: 2e22 2222 0d0a 2020 2020 2020 2020 7365  ."""..        se
+000016a0: 6c66 2e63 7269 7465 7269 6f6e 203d 2063  lf.criterion = c
+000016b0: 7269 7465 7269 6f6e 0d0a 2020 2020 2020  riterion..      
+000016c0: 2020 7365 6c66 2e6d 6f64 656c 203d 206d    self.model = m
+000016d0: 6f64 656c 2e74 6f28 7365 6c66 2e64 6576  odel.to(self.dev
+000016e0: 6963 6529 2069 6620 6d6f 6465 6c20 656c  ice) if model el
+000016f0: 7365 205f 4475 6d6d 794d 6f64 756c 6528  se _DummyModule(
+00001700: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00001710: 6f70 7469 6d69 7a65 7220 3d20 6f70 7469  optimizer = opti
+00001720: 6d69 7a65 7220 6966 206f 7074 696d 697a  mizer if optimiz
+00001730: 6572 2065 6c73 6520 5f44 756d 6d79 4d6f  er else _DummyMo
+00001740: 6475 6c65 2829 0d0a 2020 2020 2020 2020  dule()..        
+00001750: 7365 6c66 2e6c 725f 7363 6865 6475 6c65  self.lr_schedule
+00001760: 7220 3d20 6c72 5f73 6368 6564 756c 6572  r = lr_scheduler
+00001770: 2069 6620 6c72 5f73 6368 6564 756c 6572   if lr_scheduler
+00001780: 2065 6c73 6520 5f44 756d 6d79 4d6f 6475   else _DummyModu
+00001790: 6c65 2829 0d0a 0d0a 2020 2020 4070 726f  le()....    @pro
+000017a0: 7065 7274 790d 0a20 2020 2064 6566 206d  perty..    def m
+000017b0: 6f64 6528 7365 6c66 293a 0d0a 2020 2020  ode(self):..    
+000017c0: 2020 2020 2222 2247 6574 2074 6865 2063      """Get the c
+000017d0: 7572 7265 6e74 206d 6f64 6520 6f66 2074  urrent mode of t
+000017e0: 6865 2063 6869 6566 2063 6f61 6368 2e22  he chief coach."
+000017f0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00001800: 726e 2073 656c 662e 5f5f 6d6f 6465 0d0a  rn self.__mode..
+00001810: 0d0a 2020 2020 4074 696d 656d 6574 6572  ..    @timemeter
+00001820: 0d0a 2020 2020 6465 6620 7472 6169 6e28  ..    def train(
+00001830: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
+00001840: 293a 0d0a 2020 2020 2020 2020 2222 2253  ):..        """S
+00001850: 7461 7274 2074 7261 696e 696e 6720 616e  tart training an
+00001860: 6420 7265 7475 726e 2074 6865 2074 7261  d return the tra
+00001870: 696e 696e 6720 6c6f 7373 2e22 2222 0d0a  ining loss."""..
+00001880: 2020 2020 2020 2020 7365 6c66 2e5f 5f6d          self.__m
+00001890: 6f64 6520 3d20 2774 7261 696e 270d 0a20  ode = 'train'.. 
+000018a0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+000018b0: 6c2e 7472 6169 6e28 290d 0a20 2020 2020  l.train()..     
+000018c0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
+000018d0: 7261 696e 5f70 6572 5f65 706f 6368 2865  rain_per_epoch(e
+000018e0: 706f 6368 290d 0a0d 0a20 2020 2040 7469  poch)....    @ti
+000018f0: 6d65 6d65 7465 720d 0a20 2020 2040 746f  memeter..    @to
+00001900: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
+00001910: 2020 2064 6566 2076 616c 6964 2873 656c     def valid(sel
+00001920: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
+00001930: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
+00001940: 7420 7661 6c69 6461 7469 6f6e 2061 6e64  t validation and
+00001950: 2072 6574 7572 6e20 7468 6520 7661 6c69   return the vali
+00001960: 6461 7469 6f6e 206d 6574 7269 6373 2e22  dation metrics."
+00001970: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001980: 2e5f 5f6d 6f64 6520 3d20 2776 616c 6964  .__mode = 'valid
+00001990: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+000019a0: 6d6f 6465 6c2e 6576 616c 2829 0d0a 2020  model.eval()..  
+000019b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000019c0: 662e 6576 616c 7561 7465 2865 706f 6368  f.evaluate(epoch
+000019d0: 3d65 706f 6368 2c20 7072 6566 6978 3d27  =epoch, prefix='
+000019e0: 7661 6c69 6427 290d 0a0d 0a20 2020 2040  valid')....    @
+000019f0: 7469 6d65 6d65 7465 720d 0a20 2020 2040  timemeter..    @
+00001a00: 746f 7263 682e 6e6f 5f67 7261 6428 290d  torch.no_grad().
+00001a10: 0a20 2020 2064 6566 2074 6573 7428 7365  .    def test(se
+00001a20: 6c66 2c20 6570 6f63 683a 2069 6e74 293a  lf, epoch: int):
+00001a30: 0d0a 2020 2020 2020 2020 2222 2253 7461  ..        """Sta
+00001a40: 7274 2074 6573 7469 6e67 2061 6e64 2072  rt testing and r
+00001a50: 6574 7572 6e20 7468 6520 7465 7374 206d  eturn the test m
+00001a60: 6574 7269 6373 2e22 2222 0d0a 2020 2020  etrics."""..    
+00001a70: 2020 2020 7365 6c66 2e5f 5f6d 6f64 6520      self.__mode 
+00001a80: 3d20 2774 6573 7427 0d0a 2020 2020 2020  = 'test'..      
+00001a90: 2020 7365 6c66 2e6d 6f64 656c 2e65 7661    self.model.eva
+00001aa0: 6c28 290d 0a20 2020 2020 2020 2072 6574  l()..        ret
+00001ab0: 7572 6e20 7365 6c66 2e65 7661 6c75 6174  urn self.evaluat
+00001ac0: 6528 6570 6f63 683d 6570 6f63 682c 2070  e(epoch=epoch, p
+00001ad0: 7265 6669 783d 2774 6573 7427 290d 0a0d  refix='test')...
+00001ae0: 0a20 2020 2040 6162 632e 6162 7374 7261  .    @abc.abstra
+00001af0: 6374 6d65 7468 6f64 0d0a 2020 2020 6465  ctmethod..    de
+00001b00: 6620 7472 6169 6e5f 7065 725f 6570 6f63  f train_per_epoc
+00001b10: 6828 7365 6c66 2c20 6570 6f63 683a 2069  h(self, epoch: i
+00001b20: 6e74 293a 0d0a 2020 2020 2020 2020 7261  nt):..        ra
+00001b30: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00001b40: 6564 4572 726f 7228 0d0a 2020 2020 2020  edError(..      
+00001b50: 2020 2020 2020 6622 7b73 656c 662e 5f5f        f"{self.__
+00001b60: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00001b70: 7d2e 7472 6169 6e5f 7065 725f 6570 6f63  }.train_per_epoc
+00001b80: 6828 2920 7368 6f75 6c64 2062 6520 696d  h() should be im
+00001b90: 706c 656d 656e 7465 6420 2e2e 2e22 0d0a  plemented ..."..
+00001ba0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00001bb0: 2040 6162 632e 6162 7374 7261 6374 6d65   @abc.abstractme
+00001bc0: 7468 6f64 0d0a 2020 2020 6465 6620 6576  thod..    def ev
+00001bd0: 616c 7561 7465 2873 656c 662c 2065 706f  aluate(self, epo
+00001be0: 6368 3a20 696e 742c 2070 7265 6669 783a  ch: int, prefix:
+00001bf0: 2073 7472 203d 2027 7661 6c69 6427 293a   str = 'valid'):
+00001c00: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
+00001c10: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00001c20: 726f 7228 0d0a 2020 2020 2020 2020 2020  ror(..          
+00001c30: 2020 6622 7b73 656c 662e 5f5f 636c 6173    f"{self.__clas
+00001c40: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d2e 6576  s__.__name__}.ev
+00001c50: 616c 7561 7465 2829 2073 686f 756c 6420  aluate() should 
+00001c60: 6265 2069 6d70 6c65 6d65 6e74 6564 202e  be implemented .
+00001c70: 2e2e 220d 0a20 2020 2020 2020 2029 0d0a  .."..        )..
+00001c80: 0d0a 2020 2020 6465 6620 7265 6769 7374  ..    def regist
+00001c90: 6572 5f6d 6574 7269 6328 0d0a 2020 2020  er_metric(..    
+00001ca0: 2020 2020 7365 6c66 2c20 6e61 6d65 3a20      self, name: 
+00001cb0: 7374 722c 2066 756e 633a 2043 616c 6c61  str, func: Calla
+00001cc0: 626c 652c 200d 0a20 2020 2020 2020 2066  ble, ..        f
+00001cd0: 6d74 3a20 7374 7220 3d20 272e 3466 272c  mt: str = '.4f',
+00001ce0: 2062 6573 745f 6361 7374 6572 3a20 4361   best_caster: Ca
+00001cf0: 6c6c 6162 6c65 203d 206d 6178 0d0a 2020  llable = max..  
+00001d00: 2020 2920 2d3e 204e 6f6e 653a 0d0a 2020    ) -> None:..  
+00001d10: 2020 2020 2020 7222 2222 0d0a 2020 2020        r"""..    
+00001d20: 2020 2020 5265 6769 7374 6572 2061 206d      Register a m
+00001d30: 6574 7269 632e 0d0a 0d0a 2020 2020 2020  etric.....      
+00001d40: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00001d50: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00001d60: 0d0a 2020 2020 2020 2020 6e61 6d65 203a  ..        name :
+00001d70: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00001d80: 2020 5468 6520 636f 6d70 6c65 7465 206e    The complete n
+00001d90: 616d 6520 6f66 2074 6865 206d 6574 7269  ame of the metri
+00001da0: 632c 2073 7563 6820 6173 2060 4c4f 5353  c, such as `LOSS
+00001db0: 3260 2e0d 0a20 2020 2020 2020 2020 2020  2`...           
+00001dc0: 2054 6865 206e 6f74 6174 696f 6e20 6040   The notation `@
+00001dd0: 6020 7368 6f75 6c64 206e 6f74 2062 6520  ` should not be 
+00001de0: 696e 636c 7564 6564 2c20 692e 652e 2c20  included, i.e., 
+00001df0: 274c 4f53 5340 3227 2069 7320 696e 7661  'LOSS@2' is inva
+00001e00: 6c69 642e 0d0a 2020 2020 2020 2020 6675  lid...        fu
+00001e10: 6e63 203a 2043 616c 6c61 626c 650d 0a20  nc : Callable.. 
+00001e20: 2020 2020 2020 2020 2020 2054 6865 2066             The f
+00001e30: 756e 6374 696f 6e20 746f 2070 726f 6365  unction to proce
+00001e40: 7373 2074 6865 2064 6174 6120 666f 7220  ss the data for 
+00001e50: 7468 6520 6d65 7472 6963 2e0d 0a20 2020  the metric...   
+00001e60: 2020 2020 2066 6d74 203a 2073 7472 2c20       fmt : str, 
+00001e70: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00001e80: 2020 2020 2020 5468 6520 666f 726d 6174        The format
+00001e90: 2074 6f20 7573 6520 7768 656e 2070 7269   to use when pri
+00001ea0: 6e74 696e 6720 7468 6520 6d65 7472 6963  nting the metric
+00001eb0: 2c20 6465 6661 756c 7473 2074 6f20 6027  , defaults to `'
+00001ec0: 2e34 6627 602e 0d0a 2020 2020 2020 2020  .4f'`...        
+00001ed0: 6265 7374 5f63 6173 7465 7220 3a20 4361  best_caster : Ca
+00001ee0: 6c6c 6162 6c65 2c20 6f70 7469 6f6e 616c  llable, optional
+00001ef0: 0d0a 2020 2020 2020 2020 2020 2020 4120  ..            A 
+00001f00: 6675 6e63 7469 6f6e 2075 7365 6420 746f  function used to
+00001f10: 2063 6173 7420 7468 6520 6265 7374 2076   cast the best v
+00001f20: 616c 7565 206f 6620 7468 6520 6d65 7472  alue of the metr
+00001f30: 6963 2c20 6465 6661 756c 7473 2074 6f20  ic, defaults to 
+00001f40: 606d 6178 602e 0d0a 2020 2020 2020 2020  `max`...        
+00001f50: 2020 2020 0d0a 2020 2020 2020 2020 5265      ..        Re
+00001f60: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+00001f70: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00001f80: 4e6f 6e65 0d0a 2020 2020 2020 2020 0d0a  None..        ..
+00001f90: 2020 2020 2020 2020 5261 6973 6573 0d0a          Raises..
+00001fa0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
+00001fb0: 2020 2020 2020 2020 4173 7365 7274 696f          Assertio
+00001fc0: 6e45 7272 6f72 0d0a 2020 2020 2020 2020  nError..        
+00001fd0: 2020 2020 5768 656e 2060 6e61 6d65 6020      When `name` 
+00001fe0: 6861 7320 616c 7265 6164 7920 6265 656e  has already been
+00001ff0: 2072 6567 6973 7465 7265 6420 6f72 2063   registered or c
+00002000: 6f6e 7461 696e 7320 7468 6520 6e6f 7461  ontains the nota
+00002010: 7469 6f6e 2060 4060 2e0d 0a20 2020 2020  tion `@`...     
+00002020: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
+00002030: 2020 6e61 6d65 203d 206e 616d 652e 7570    name = name.up
+00002040: 7065 7228 290d 0a20 2020 2020 2020 2061  per()..        a
+00002050: 7373 6572 7420 4445 4641 554c 545f 4d45  ssert DEFAULT_ME
+00002060: 5452 4943 532e 6765 7428 6e61 6d65 2c20  TRICS.get(name, 
+00002070: 4e6f 6e65 2920 6973 204e 6f6e 652c 2066  None) is None, f
+00002080: 2254 6865 206d 6574 7269 6320 7b6e 616d  "The metric {nam
+00002090: 657d 2061 6c72 6561 6479 2065 7869 7374  e} already exist
+000020a0: 7320 2e2e 2e22 0d0a 2020 2020 2020 2020  s ..."..        
+000020b0: 6173 7365 7274 2027 4027 206e 6f74 2069  assert '@' not i
+000020c0: 6e20 6e61 6d65 2c20 6622 5468 6520 6d65  n name, f"The me
+000020d0: 7472 6963 206e 616d 6520 6861 7320 696e  tric name has in
+000020e0: 7661 6c69 6420 6e6f 7461 7469 6f6e 206f  valid notation o
+000020f0: 6620 6040 2720 2e2e 2e22 0d0a 2020 2020  f `@' ..."..    
+00002100: 2020 2020 4445 4641 554c 545f 4d45 5452      DEFAULT_METR
+00002110: 4943 535b 6e61 6d65 5d20 3d20 6675 6e63  ICS[name] = func
+00002120: 0d0a 2020 2020 2020 2020 4445 4641 554c  ..        DEFAUL
+00002130: 545f 464d 5453 5b6e 616d 655d 203d 2066  T_FMTS[name] = f
+00002140: 6d74 0d0a 2020 2020 2020 2020 4445 4641  mt..        DEFA
+00002150: 554c 545f 4245 5354 5f43 4153 5445 525b  ULT_BEST_CASTER[
+00002160: 6e61 6d65 5d20 3d20 6265 7374 5f63 6173  name] = best_cas
+00002170: 7465 720d 0a0d 0a0d 0a63 6c61 7373 2043  ter......class C
+00002180: 6f61 6368 2843 6869 6566 436f 6163 6829  oach(ChiefCoach)
+00002190: 3a0d 0a20 2020 2022 2222 5468 6520 6672  :..    """The fr
+000021a0: 616d 6577 6f72 6b20 666f 7220 7472 6169  amework for trai
+000021b0: 6e69 6e67 2e22 2222 0d0a 0d0a 2020 2020  ning."""....    
+000021c0: 6465 6620 7072 6570 6172 655f 6461 7461  def prepare_data
+000021d0: 6c6f 6164 6572 2873 656c 6629 202d 3e20  loader(self) -> 
+000021e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2022  None:..        "
+000021f0: 2222 5072 6570 6172 6520 6461 7461 206c  ""Prepare data l
+00002200: 6f61 6465 7273 2066 6f72 2074 7261 696e  oaders for train
+00002210: 696e 672c 2076 616c 6964 6174 696f 6e2c  ing, validation,
+00002220: 2061 6e64 2074 6573 7469 6e67 2064 6174   and testing dat
+00002230: 612e 2222 220d 0a20 2020 2020 2020 2073  a."""..        s
+00002240: 656c 662e 7472 6169 6e6c 6f61 6465 7220  elf.trainloader 
+00002250: 3d20 4461 7461 4c6f 6164 6572 280d 0a20  = DataLoader(.. 
+00002260: 2020 2020 2020 2020 2020 2064 6174 6170             datap
+00002270: 6970 653d 7365 6c66 2e74 7261 696e 7069  ipe=self.trainpi
+00002280: 7065 2c20 0d0a 2020 2020 2020 2020 2020  pe, ..          
+00002290: 2020 6e75 6d5f 776f 726b 6572 733d 7365    num_workers=se
+000022a0: 6c66 2e63 6667 2e6e 756d 5f77 6f72 6b65  lf.cfg.num_worke
+000022b0: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+000022c0: 2070 696e 5f6d 656d 6f72 793d 7365 6c66   pin_memory=self
+000022d0: 2e63 6667 2e70 696e 5f6d 656d 6f72 790d  .cfg.pin_memory.
+000022e0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+000022f0: 2020 2020 7365 6c66 2e76 616c 6964 6c6f      self.validlo
+00002300: 6164 6572 203d 2044 6174 614c 6f61 6465  ader = DataLoade
+00002310: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00002320: 6461 7461 7069 7065 3d73 656c 662e 7661  datapipe=self.va
+00002330: 6c69 6470 6970 652c 200d 0a20 2020 2020  lidpipe, ..     
+00002340: 2020 2020 2020 206e 756d 5f77 6f72 6b65         num_worke
+00002350: 7273 3d73 656c 662e 6366 672e 6e75 6d5f  rs=self.cfg.num_
+00002360: 776f 726b 6572 732c 0d0a 2020 2020 2020  workers,..      
+00002370: 2020 2020 2020 7069 6e5f 6d65 6d6f 7279        pin_memory
+00002380: 3d73 656c 662e 6366 672e 7069 6e5f 6d65  =self.cfg.pin_me
+00002390: 6d6f 7279 0d0a 2020 2020 2020 2020 290d  mory..        ).
+000023a0: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+000023b0: 7374 6c6f 6164 6572 203d 2044 6174 614c  stloader = DataL
+000023c0: 6f61 6465 7228 0d0a 2020 2020 2020 2020  oader(..        
+000023d0: 2020 2020 6461 7461 7069 7065 3d73 656c      datapipe=sel
+000023e0: 662e 7465 7374 7069 7065 2c20 0d0a 2020  f.testpipe, ..  
+000023f0: 2020 2020 2020 2020 2020 6e75 6d5f 776f            num_wo
+00002400: 726b 6572 733d 7365 6c66 2e63 6667 2e6e  rkers=self.cfg.n
+00002410: 756d 5f77 6f72 6b65 7273 2c0d 0a20 2020  um_workers,..   
+00002420: 2020 2020 2020 2020 2070 696e 5f6d 656d           pin_mem
+00002430: 6f72 793d 7365 6c66 2e63 6667 2e70 696e  ory=self.cfg.pin
+00002440: 5f6d 656d 6f72 790d 0a20 2020 2020 2020  _memory..       
+00002450: 2029 0d0a 2020 2020 0d0a 2020 2020 4070   )..    ..    @p
+00002460: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00002470: 2064 6174 616c 6f61 6465 7228 7365 6c66   dataloader(self
+00002480: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00002490: 6574 7572 6e20 7468 6520 636f 7272 6573  eturn the corres
+000024a0: 706f 6e64 696e 6720 6461 7461 206c 6f61  ponding data loa
+000024b0: 6465 7220 6465 7065 6e64 696e 6720 6f6e  der depending on
+000024c0: 2074 6865 2063 7572 7265 6e74 206d 6f64   the current mod
+000024d0: 652e 2222 220d 0a20 2020 2020 2020 2069  e."""..        i
+000024e0: 6620 7365 6c66 2e6d 6f64 6520 3d3d 2027  f self.mode == '
+000024f0: 7472 6169 6e27 3a0d 0a20 2020 2020 2020  train':..       
+00002500: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002510: 2e74 7261 696e 6c6f 6164 6572 0d0a 2020  .trainloader..  
+00002520: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00002530: 6d6f 6465 203d 3d20 2776 616c 6964 273a  mode == 'valid':
+00002540: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00002550: 7475 726e 2073 656c 662e 7661 6c69 646c  turn self.validl
+00002560: 6f61 6465 720d 0a20 2020 2020 2020 2065  oader..        e
+00002570: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002580: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
+00002590: 7374 6c6f 6164 6572 0d0a 0d0a 2020 2020  stloader....    
+000025a0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+000025b0: 6566 206d 6f6e 6974 6f72 7328 7365 6c66  ef monitors(self
+000025c0: 2920 2d3e 204d 6f6e 6974 6f72 3a0d 0a20  ) -> Monitor:.. 
+000025d0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000025e0: 2074 6865 206d 6f6e 6974 6f72 2064 6963   the monitor dic
+000025f0: 7469 6f6e 6172 7920 666f 7220 7468 6520  tionary for the 
+00002600: 6469 6666 6572 656e 7420 6d6f 6465 7320  different modes 
+00002610: 2827 7472 6169 6e27 2c20 2776 616c 6964  ('train', 'valid
+00002620: 272c 2027 7465 7374 2729 2e22 2222 0d0a  ', 'test')."""..
+00002630: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002640: 656c 662e 5f5f 6d6f 6e69 746f 7273 0d0a  elf.__monitors..
+00002650: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00002660: 0a20 2020 2064 6566 206d 6574 6572 3462  .    def meter4b
+00002670: 6573 7428 7365 6c66 293a 0d0a 2020 2020  est(self):..    
+00002680: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002690: 5f5f 6265 7374 5f6d 6574 6572 0d0a 0d0a  __best_meter....
+000026a0: 2020 2020 406d 6574 6572 3462 6573 742e      @meter4best.
+000026b0: 7365 7474 6572 0d0a 2020 2020 6465 6620  setter..    def 
+000026c0: 6d65 7465 7234 6265 7374 2873 656c 662c  meter4best(self,
+000026d0: 206d 6574 6572 3a20 4176 6572 6167 654d   meter: AverageM
+000026e0: 6574 6572 293a 0d0a 2020 2020 2020 2020  eter):..        
+000026f0: 7365 6c66 2e5f 5f62 6573 745f 6d65 7465  self.__best_mete
+00002700: 7220 3d20 6d65 7465 720d 0a20 2020 2020  r = meter..     
+00002710: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+00002720: 5b43 6f61 6368 5d20 3e3e 3e20 5365 7420  [Coach] >>> Set 
+00002730: 6265 7374 206d 6574 6572 3a20 7b6d 6574  best meter: {met
+00002740: 6572 2e6e 616d 657d 2022 290d 0a0d 0a20  er.name} ").... 
+00002750: 2020 2040 7469 6d65 6d65 7465 720d 0a20     @timemeter.. 
+00002760: 2020 2064 6566 2063 6f6d 7069 6c65 280d     def compile(.
+00002770: 0a20 2020 2020 2020 2073 656c 662c 2063  .        self, c
+00002780: 6667 3a20 436f 6e66 6967 2c20 6d6f 6e69  fg: Config, moni
+00002790: 746f 7273 3a20 4c69 7374 5b73 7472 5d2c  tors: List[str],
+000027a0: 200d 0a20 2020 2020 2020 2077 6869 6368   ..        which
+000027b0: 3462 6573 743a 2073 7472 203d 2027 4c4f  4best: str = 'LO
+000027c0: 5353 270d 0a20 2020 2029 3a0d 0a20 2020  SS'..    ):..   
+000027d0: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
+000027e0: 2020 204c 6f61 6420 7468 6520 636f 6e66     Load the conf
+000027f0: 6967 7572 6174 696f 6e20 616e 6420 7365  iguration and se
+00002800: 7420 7570 206d 6f6e 6974 6f72 7320 666f  t up monitors fo
+00002810: 7220 7472 6169 6e69 6e67 2e0d 0a0d 0a20  r training..... 
+00002820: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00002830: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00002840: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2063  -----..        c
+00002850: 6667 203a 2043 6f6e 6669 670d 0a20 2020  fg : Config..   
+00002860: 2020 2020 2020 2020 2041 2063 6f6e 6669           A confi
+00002870: 6775 7261 7469 6f6e 206f 626a 6563 7420  guration object 
+00002880: 7769 7468 2074 6865 2074 7261 696e 696e  with the trainin
+00002890: 6720 6465 7461 696c 732e 0d0a 2020 2020  g details...    
+000028a0: 2020 2020 6d6f 6e69 746f 7273 203a 204c      monitors : L
+000028b0: 6973 745b 7374 725d 0d0a 2020 2020 2020  ist[str]..      
+000028c0: 2020 2020 2020 4120 6c69 7374 206f 6620        A list of 
+000028d0: 6d65 7472 6963 206e 616d 6573 2074 6f20  metric names to 
+000028e0: 6265 206d 6f6e 6974 6f72 6564 2064 7572  be monitored dur
+000028f0: 696e 6720 7472 6169 6e69 6e67 2e0d 0a20  ing training... 
+00002900: 2020 2020 2020 2077 6869 6368 3462 6573         which4bes
+00002910: 7420 3a20 7374 722c 2064 6566 6175 6c74  t : str, default
+00002920: 7320 604c 4f53 5327 0d0a 2020 2020 2020  s `LOSS'..      
+00002930: 2020 2020 2020 5468 6520 6d65 7472 6963        The metric
+00002940: 2075 7365 6420 666f 7220 7365 6c65 6374   used for select
+00002950: 696e 6720 7468 6520 6265 7374 2063 6865  ing the best che
+00002960: 636b 706f 696e 742e 0d0a 0d0a 2020 2020  ckpoint.....    
+00002970: 2020 2020 4578 616d 706c 6573 0d0a 2020      Examples..  
+00002980: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a        --------..
+00002990: 2020 2020 2020 2020 3e3e 3e20 636f 6163          >>> coac
+000029a0: 683a 2043 6f61 6368 0d0a 2020 2020 2020  h: Coach..      
+000029b0: 2020 3e3e 3e20 636f 6163 682e 636f 6d70    >>> coach.comp
+000029c0: 696c 6528 6366 672c 206d 6f6e 6974 6f72  ile(cfg, monitor
+000029d0: 733d 5b27 6c6f 7373 272c 2027 7265 6361  s=['loss', 'reca
+000029e0: 6c6c 4031 3027 2c20 2772 6563 616c 6c40  ll@10', 'recall@
+000029f0: 3230 272c 2027 6e64 6367 4031 3027 2c20  20', 'ndcg@10', 
+00002a00: 276e 6463 6740 3230 275d 290d 0a20 2020  'ndcg@20'])..   
+00002a10: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002a20: 2020 7365 6c66 2e63 6667 203d 2063 6667    self.cfg = cfg
+00002a30: 0d0a 2020 2020 2020 2020 2320 6d65 7465  ..        # mete
+00002a40: 7273 2066 6f72 2074 7261 696e 7c76 616c  rs for train|val
+00002a50: 6964 7c74 6573 740d 0a20 2020 2020 2020  id|test..       
+00002a60: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
+00002a70: 203d 204d 6f6e 6974 6f72 2829 0d0a 2020   = Monitor()..  
+00002a80: 2020 2020 2020 7365 6c66 2e5f 5f6d 6f6e        self.__mon
+00002a90: 6974 6f72 735b 2774 7261 696e 275d 203d  itors['train'] =
+00002aa0: 2064 6566 6175 6c74 6469 6374 286c 6973   defaultdict(lis
+00002ab0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
+00002ac0: 2e5f 5f6d 6f6e 6974 6f72 735b 2776 616c  .__monitors['val
+00002ad0: 6964 275d 203d 2064 6566 6175 6c74 6469  id'] = defaultdi
+00002ae0: 6374 286c 6973 7429 0d0a 2020 2020 2020  ct(list)..      
+00002af0: 2020 7365 6c66 2e5f 5f6d 6f6e 6974 6f72    self.__monitor
+00002b00: 735b 2774 6573 7427 5d20 3d20 6465 6661  s['test'] = defa
+00002b10: 756c 7464 6963 7428 6c69 7374 290d 0a0d  ultdict(list)...
+00002b20: 0a20 2020 2020 2020 2064 6566 2073 6574  .        def set
+00002b30: 5f6d 6f6e 6974 6f72 280d 0a20 2020 2020  _monitor(..     
+00002b40: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
+00002b50: 2c20 6c61 7374 6e61 6d65 3a20 7374 722c  , lastname: str,
+00002b60: 2070 7265 6669 783a 2073 7472 203d 2027   prefix: str = '
+00002b70: 7472 6169 6e27 2c20 2a2a 6b77 6172 6773  train', **kwargs
+00002b80: 0d0a 2020 2020 2020 2020 293a 0d0a 2020  ..        ):..  
+00002b90: 2020 2020 2020 2020 2020 2222 2241 6464            """Add
+00002ba0: 2061 206d 6f6e 6974 6f72 2066 6f72 2074   a monitor for t
+00002bb0: 6865 2073 7065 6369 6669 6564 206d 6574  he specified met
+00002bc0: 7269 632e 2222 220d 0a20 2020 2020 2020  ric."""..       
+00002bd0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00002be0: 2020 2020 2020 2020 2020 206d 6574 6572             meter
+00002bf0: 203d 2041 7665 7261 6765 4d65 7465 7228   = AverageMeter(
+00002c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002c10: 2020 2020 2020 2020 2020 6e61 6d65 3d6e            name=n
+00002c20: 616d 652c 0d0a 2020 2020 2020 2020 2020  ame,..          
+00002c30: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00002c40: 7472 6963 3d70 6172 7469 616c 2844 4546  tric=partial(DEF
+00002c50: 4155 4c54 5f4d 4554 5249 4353 5b6c 6173  AULT_METRICS[las
+00002c60: 746e 616d 655d 2c20 2a2a 6b77 6172 6773  tname], **kwargs
+00002c70: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00002c80: 2020 2020 2020 2020 2020 2020 666d 743d              fmt=
+00002c90: 4445 4641 554c 545f 464d 5453 5b6c 6173  DEFAULT_FMTS[las
+00002ca0: 746e 616d 655d 2c0d 0a20 2020 2020 2020  tname],..       
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2062 6573 745f 6361 7374 6572 3d44 4546   best_caster=DEF
+00002cd0: 4155 4c54 5f42 4553 545f 4341 5354 4552  AULT_BEST_CASTER
+00002ce0: 5b6c 6173 746e 616d 655d 0d0a 2020 2020  [lastname]..    
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002d10: 2020 2073 656c 662e 5f5f 6d6f 6e69 746f     self.__monito
+00002d20: 7273 5b70 7265 6669 785d 5b6c 6173 746e  rs[prefix][lastn
+00002d30: 616d 655d 2e61 7070 656e 6428 6d65 7465  ame].append(mete
+00002d40: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+00002d50: 6578 6365 7074 204b 6579 4572 726f 723a  except KeyError:
+00002d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d70: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
+00002d80: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00002d90: 2020 2020 2020 2066 2254 6865 206d 6574         f"The met
+00002da0: 7269 6320 6f66 207b 6c61 7374 6e61 6d65  ric of {lastname
+00002db0: 7d20 6973 206e 6f74 2069 6e63 6c75 6465  } is not include
+00002dc0: 642e 2022 0d0a 2020 2020 2020 2020 2020  d. "..          
+00002dd0: 2020 2020 2020 2020 2020 6622 596f 7520            f"You 
+00002de0: 6361 6e20 7265 6769 7374 6572 2062 7920  can register by 
+00002df0: 6361 6c6c 696e 6720 6072 6567 6973 7465  calling `registe
+00002e00: 725f 6d65 7472 6963 282e 2e2e 2927 202e  r_metric(...)' .
+00002e10: 2e2e 220d 0a20 2020 2020 2020 2020 2020  .."..           
+00002e20: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00002e30: 2020 2020 7265 7475 726e 206d 6574 6572      return meter
+00002e40: 0d0a 0d0a 2020 2020 2020 2020 2320 5550  ....        # UP
+00002e50: 5045 520d 0a20 2020 2020 2020 2077 6869  PER..        whi
+00002e60: 6368 3462 6573 7420 3d20 7768 6963 6834  ch4best = which4
+00002e70: 6265 7374 2e75 7070 6572 2829 0d0a 2020  best.upper()..  
+00002e80: 2020 2020 2020 6d6f 6e69 746f 7273 203d        monitors =
+00002e90: 205b 274c 4f53 5327 5d20 2b20 5b6e 616d   ['LOSS'] + [nam
+00002ea0: 652e 7570 7065 7228 2920 666f 7220 6e61  e.upper() for na
+00002eb0: 6d65 2069 6e20 6d6f 6e69 746f 7273 5d20  me in monitors] 
+00002ec0: 2b20 5b77 6869 6368 3462 6573 745d 0d0a  + [which4best]..
+00002ed0: 2020 2020 2020 2020 6d6f 6e69 746f 7273          monitors
+00002ee0: 203d 2073 6f72 7465 6428 7365 7428 6d6f   = sorted(set(mo
+00002ef0: 6e69 746f 7273 292c 206b 6579 3d6d 6f6e  nitors), key=mon
+00002f00: 6974 6f72 732e 696e 6465 7829 0d0a 0d0a  itors.index)....
+00002f10: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+00002f20: 2069 6e20 6d6f 6e69 746f 7273 3a0d 0a20   in monitors:.. 
+00002f30: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00002f40: 7265 6669 7820 696e 2028 2774 7261 696e  refix in ('train
+00002f50: 272c 2027 7661 6c69 6427 2c20 2774 6573  ', 'valid', 'tes
+00002f60: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
+00002f70: 2020 2020 2020 6966 2027 4027 2069 6e20        if '@' in 
+00002f80: 6e61 6d65 3a0d 0a20 2020 2020 2020 2020  name:..         
+00002f90: 2020 2020 2020 2020 2020 206c 6173 746e             lastn
+00002fa0: 616d 652c 204b 203d 206e 616d 652e 7370  ame, K = name.sp
+00002fb0: 6c69 7428 2740 2729 0d0a 2020 2020 2020  lit('@')..      
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00002fd0: 7465 7220 3d20 7365 745f 6d6f 6e69 746f  ter = set_monito
+00002fe0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00002ff0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00003000: 3d6e 616d 652c 0d0a 2020 2020 2020 2020  =name,..        
+00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003020: 6c61 7374 6e61 6d65 3d6c 6173 746e 616d  lastname=lastnam
+00003030: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00003040: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+00003050: 6978 3d70 7265 6669 782c 0d0a 2020 2020  ix=prefix,..    
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 2020 2020 6b3d 696e 7428 4b29 0d0a 2020      k=int(K)..  
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+000030a0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 6c61 7374 6e61 6d65 203d 206e 616d 650d  lastname = name.
+000030d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000030e0: 2020 2020 206d 6574 6572 203d 2073 6574       meter = set
+000030f0: 5f6d 6f6e 6974 6f72 280d 0a20 2020 2020  _monitor(..     
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 206e 616d 653d 6e61 6d65 2c0d 0a20     name=name,.. 
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2020 2020 206c 6173 746e 616d 653d         lastname=
+00003140: 6c61 7374 6e61 6d65 2c0d 0a20 2020 2020  lastname,..     
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 2020 2070 7265 6669 783d 7072 6566 6978     prefix=prefix
+00003170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003180: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00003190: 2020 2020 2020 2020 2069 6620 7072 6566           if pref
+000031a0: 6978 203d 3d20 2776 616c 6964 2720 616e  ix == 'valid' an
+000031b0: 6420 6e61 6d65 203d 3d20 7768 6963 6834  d name == which4
+000031c0: 6265 7374 3a0d 0a20 2020 2020 2020 2020  best:..         
+000031d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000031e0: 6d65 7465 7234 6265 7374 203d 206d 6574  meter4best = met
+000031f0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00003200: 2020 2020 2020 2020 7365 6c66 2e5f 6265          self._be
+00003210: 7374 203d 202d 666c 6f61 7428 2769 6e66  st = -float('inf
+00003220: 2729 2069 6620 6d65 7465 722e 6361 7374  ') if meter.cast
+00003230: 6572 2069 7320 6d61 7820 656c 7365 2066  er is max else f
+00003240: 6c6f 6174 2827 696e 6627 290d 0a20 2020  loat('inf')..   
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2073 656c 662e 5f62 6573 745f 6570 6f63   self._best_epoc
+00003270: 6820 3d20 300d 0a0d 0a20 2020 2020 2020  h = 0....       
+00003280: 2023 2050 7265 7061 7265 2064 6174 6120   # Prepare data 
+00003290: 6c6f 6164 6572 730d 0a20 2020 2020 2020  loaders..       
+000032a0: 2073 656c 662e 7072 6570 6172 655f 6461   self.prepare_da
+000032b0: 7461 6c6f 6164 6572 2829 0d0a 0d0a 2020  taloader()....  
+000032c0: 2020 6465 6620 7361 7665 2873 656c 6629    def save(self)
+000032d0: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+000032e0: 2020 2022 2222 5361 7665 2074 6865 206d     """Save the m
+000032f0: 6f64 656c 2222 220d 0a20 2020 2020 2020  odel"""..       
+00003300: 2074 6f72 6368 2e73 6176 6528 7365 6c66   torch.save(self
+00003310: 2e6d 6f64 656c 2e73 7461 7465 5f64 6963  .model.state_dic
+00003320: 7428 292c 206f 732e 7061 7468 2e6a 6f69  t(), os.path.joi
+00003330: 6e28 7365 6c66 2e63 6667 2e4c 4f47 5f50  n(self.cfg.LOG_P
+00003340: 4154 482c 2073 656c 662e 6366 672e 5341  ATH, self.cfg.SA
+00003350: 5645 445f 4649 4c45 4e41 4d45 2929 0d0a  VED_FILENAME))..
+00003360: 0d0a 2020 2020 6465 6620 6c6f 6164 2873  ..    def load(s
+00003370: 656c 662c 2070 6174 683a 2073 7472 2c20  elf, path: str, 
+00003380: 6669 6c65 6e61 6d65 3a20 4f70 7469 6f6e  filename: Option
+00003390: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c20  al[str] = None, 
+000033a0: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
+000033b0: 653a 0d0a 2020 2020 2020 2020 6669 6c65  e:..        file
+000033c0: 6e61 6d65 203d 2073 656c 662e 6366 672e  name = self.cfg.
+000033d0: 5341 5645 445f 4649 4c45 4e41 4d45 2069  SAVED_FILENAME i
+000033e0: 6620 6669 6c65 6e61 6d65 2069 7320 4e6f  f filename is No
+000033f0: 6e65 2065 6c73 6520 6669 6c65 6e61 6d65  ne else filename
+00003400: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+00003410: 6f64 656c 2e6c 6f61 645f 7374 6174 655f  odel.load_state_
+00003420: 6469 6374 2874 6f72 6368 2e6c 6f61 6428  dict(torch.load(
+00003430: 6f73 2e70 6174 682e 6a6f 696e 2870 6174  os.path.join(pat
+00003440: 682c 2066 696c 656e 616d 6529 2c20 2a2a  h, filename), **
+00003450: 6b77 6172 6773 2929 0d0a 0d0a 2020 2020  kwargs))....    
+00003460: 6465 6620 7361 7665 5f63 6865 636b 706f  def save_checkpo
+00003470: 696e 7428 7365 6c66 2c20 6570 6f63 683a  int(self, epoch:
+00003480: 2069 6e74 2920 2d3e 204e 6f6e 653a 0d0a   int) -> None:..
+00003490: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
+000034a0: 2020 2020 2020 5361 7665 2063 7572 7265        Save curre
+000034b0: 6e74 2063 6865 636b 706f 696e 7420 6174  nt checkpoint at
+000034c0: 2065 706f 6368 2e0d 0a0d 0a20 2020 2020   epoch.....     
+000034d0: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
+000034e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000034f0: 2d2d 2d0d 0a20 2020 2020 2020 2020 2020  ---..           
+00003500: 2065 706f 6368 203a 696e 7420 4375 7272   epoch :int Curr
+00003510: 656e 7420 6570 6f63 6820 6e75 6d62 6572  ent epoch number
+00003520: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00003530: 7572 6e73 3a0d 0a20 2020 2020 2020 202d  urns:..        -
+00003540: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00003550: 2020 2020 204e 6f6e 650d 0a20 2020 2020       None..     
+00003560: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00003570: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00003580: 6f69 6e28 7365 6c66 2e63 6667 2e43 4845  oin(self.cfg.CHE
+00003590: 434b 504f 494e 545f 5041 5448 2c20 7365  CKPOINT_PATH, se
+000035a0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+000035b0: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
+000035c0: 2020 2020 2063 6865 636b 706f 696e 7420       checkpoint 
+000035d0: 3d20 6469 6374 2829 0d0a 2020 2020 2020  = dict()..      
+000035e0: 2020 6368 6563 6b70 6f69 6e74 5b27 6570    checkpoint['ep
+000035f0: 6f63 6827 5d20 3d20 6570 6f63 680d 0a20  och'] = epoch.. 
+00003600: 2020 2020 2020 2066 6f72 206d 6f64 756c         for modul
+00003610: 6520 696e 2073 656c 662e 6366 672e 4348  e in self.cfg.CH
+00003620: 4543 4b50 4f49 4e54 5f4d 4f44 554c 4553  ECKPOINT_MODULES
+00003630: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00003640: 6865 636b 706f 696e 745b 6d6f 6475 6c65  heckpoint[module
+00003650: 5d20 3d20 6765 7461 7474 7228 7365 6c66  ] = getattr(self
+00003660: 2c20 6d6f 6475 6c65 292e 7374 6174 655f  , module).state_
+00003670: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
+00003680: 6368 6563 6b70 6f69 6e74 5b27 6d6f 6e69  checkpoint['moni
+00003690: 746f 7273 275d 203d 2073 656c 662e 6d6f  tors'] = self.mo
+000036a0: 6e69 746f 7273 2e73 7461 7465 5f64 6963  nitors.state_dic
+000036b0: 7428 290d 0a20 2020 2020 2020 2074 6f72  t()..        tor
+000036c0: 6368 2e73 6176 6528 6368 6563 6b70 6f69  ch.save(checkpoi
+000036d0: 6e74 2c20 7061 7468 290d 0a0d 0a20 2020  nt, path)....   
+000036e0: 2064 6566 206c 6f61 645f 6368 6563 6b70   def load_checkp
+000036f0: 6f69 6e74 2873 656c 6629 202d 3e20 696e  oint(self) -> in
+00003700: 743a 0d0a 2020 2020 2020 2020 7222 2222  t:..        r"""
+00003710: 0d0a 2020 2020 2020 2020 4c6f 6164 206c  ..        Load l
+00003720: 6173 7420 7361 7665 6420 6368 6563 6b70  ast saved checkp
+00003730: 6f69 6e74 2e0d 0a0d 0a20 2020 2020 2020  oint.....       
+00003740: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00003750: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
+00003760: 2020 2020 2065 706f 6368 3a20 696e 7420       epoch: int 
+00003770: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00003780: 6520 6570 6f63 6820 6e75 6d62 6572 206c  e epoch number l
+00003790: 6f61 6465 6420 6672 6f6d 2074 6865 2063  oaded from the c
+000037a0: 6865 636b 706f 696e 742e 0d0a 2020 2020  heckpoint...    
+000037b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000037c0: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
+000037d0: 6a6f 696e 2873 656c 662e 6366 672e 4348  join(self.cfg.CH
+000037e0: 4543 4b50 4f49 4e54 5f50 4154 482c 2073  ECKPOINT_PATH, s
+000037f0: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
+00003800: 4e54 5f46 494c 454e 414d 4529 0d0a 2020  NT_FILENAME)..  
+00003810: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
+00003820: 203d 2074 6f72 6368 2e6c 6f61 6428 7061   = torch.load(pa
+00003830: 7468 290d 0a20 2020 2020 2020 2066 6f72  th)..        for
+00003840: 206d 6f64 756c 6520 696e 2073 656c 662e   module in self.
+00003850: 6366 672e 4348 4543 4b50 4f49 4e54 5f4d  cfg.CHECKPOINT_M
+00003860: 4f44 554c 4553 3a0d 0a20 2020 2020 2020  ODULES:..       
+00003870: 2020 2020 2067 6574 6174 7472 2873 656c       getattr(sel
+00003880: 662c 206d 6f64 756c 6529 2e6c 6f61 645f  f, module).load_
+00003890: 7374 6174 655f 6469 6374 2863 6865 636b  state_dict(check
+000038a0: 706f 696e 745b 6d6f 6475 6c65 5d29 0d0a  point[module])..
+000038b0: 2020 2020 2020 2020 7365 6c66 2e6d 6f6e          self.mon
+000038c0: 6974 6f72 732e 6c6f 6164 5f73 7461 7465  itors.load_state
+000038d0: 5f64 6963 7428 6368 6563 6b70 6f69 6e74  _dict(checkpoint
+000038e0: 5b27 6d6f 6e69 746f 7273 275d 290d 0a20  ['monitors']).. 
+000038f0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+00003900: 6563 6b70 6f69 6e74 5b27 6570 6f63 6827  eckpoint['epoch'
+00003910: 5d0d 0a0d 0a20 2020 2064 6566 2073 6176  ]....    def sav
+00003920: 655f 6265 7374 2873 656c 6629 202d 3e20  e_best(self) -> 
+00003930: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2074  None:..        t
+00003940: 6f72 6368 2e73 6176 6528 7365 6c66 2e6d  orch.save(self.m
+00003950: 6f64 656c 2e73 7461 7465 5f64 6963 7428  odel.state_dict(
+00003960: 292c 206f 732e 7061 7468 2e6a 6f69 6e28  ), os.path.join(
+00003970: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
+00003980: 482c 2073 656c 662e 6366 672e 4245 5354  H, self.cfg.BEST
+00003990: 5f46 494c 454e 414d 4529 290d 0a0d 0a20  _FILENAME)).... 
+000039a0: 2020 2064 6566 206c 6f61 645f 6265 7374     def load_best
+000039b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+000039c0: 0a20 2020 2020 2020 2069 6e66 6f4c 6f67  .        infoLog
+000039d0: 6765 7228 6622 5b43 6f61 6368 5d20 3e3e  ger(f"[Coach] >>
+000039e0: 3e20 4c6f 6164 2062 6573 7420 6d6f 6465  > Load best mode
+000039f0: 6c20 4045 706f 6368 207b 7365 6c66 2e5f  l @Epoch {self._
+00003a00: 6265 7374 5f65 706f 6368 3a3c 3464 7d20  best_epoch:<4d} 
+00003a10: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003a20: 2e6d 6f64 656c 2e6c 6f61 645f 7374 6174  .model.load_stat
+00003a30: 655f 6469 6374 2874 6f72 6368 2e6c 6f61  e_dict(torch.loa
+00003a40: 6428 6f73 2e70 6174 682e 6a6f 696e 2873  d(os.path.join(s
+00003a50: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00003a60: 2c20 7365 6c66 2e63 6667 2e42 4553 545f  , self.cfg.BEST_
+00003a70: 4649 4c45 4e41 4d45 2929 290d 0a0d 0a20  FILENAME))).... 
+00003a80: 2020 2064 6566 2063 6865 636b 5f62 6573     def check_bes
+00003a90: 7428 7365 6c66 2c20 6570 6f63 683a 2069  t(self, epoch: i
+00003aa0: 6e74 2920 2d3e 204e 6f6e 653a 0d0a 2020  nt) -> None:..  
+00003ab0: 2020 2020 2020 2222 2255 7064 6174 6520        """Update 
+00003ac0: 6265 7374 2076 616c 7565 2e22 2222 0d0a  best value."""..
+00003ad0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003ae0: 6d65 7465 7234 6265 7374 2e61 6374 6976  meter4best.activ
+00003af0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003b00: 6265 7374 5f20 3d20 7365 6c66 2e6d 6574  best_ = self.met
+00003b10: 6572 3462 6573 742e 7768 6963 685f 6973  er4best.which_is
+00003b20: 5f62 6574 7465 7228 7365 6c66 2e5f 6265  _better(self._be
+00003b30: 7374 290d 0a20 2020 2020 2020 2020 2020  st)..           
+00003b40: 2069 6620 6265 7374 5f20 213d 2073 656c   if best_ != sel
+00003b50: 662e 5f62 6573 743a 0d0a 2020 2020 2020  f._best:..      
+00003b60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003b70: 6265 7374 203d 2062 6573 745f 0d0a 2020  best = best_..  
+00003b80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003b90: 6c66 2e5f 6265 7374 5f65 706f 6368 203d  lf._best_epoch =
+00003ba0: 2065 706f 6368 0d0a 2020 2020 2020 2020   epoch..        
+00003bb0: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
+00003bc0: 6572 2866 225b 436f 6163 685d 203e 3e3e  er(f"[Coach] >>>
+00003bd0: 2042 6574 7465 7220 2a2a 2a7b 7365 6c66   Better ***{self
+00003be0: 2e6d 6574 6572 3462 6573 742e 6e61 6d65  .meter4best.name
+00003bf0: 7d2a 2a2a 206f 6620 2a2a 2a7b 7365 6c66  }*** of ***{self
+00003c00: 2e5f 6265 7374 3a2e 3466 7d2a 2a2a 2022  ._best:.4f}*** "
+00003c10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003c20: 2020 2073 656c 662e 7361 7665 5f62 6573     self.save_bes
+00003c30: 7428 290d 0a0d 0a20 2020 2064 6566 2065  t()....    def e
+00003c40: 7661 6c5f 6174 5f62 6573 7428 7365 6c66  val_at_best(self
+00003c50: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+00003c60: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003c70: 6c66 2e6c 6f61 645f 6265 7374 2829 0d0a  lf.load_best()..
+00003c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003c90: 2e76 616c 6964 2873 656c 662e 5f62 6573  .valid(self._bes
+00003ca0: 745f 6570 6f63 6829 0d0a 2020 2020 2020  t_epoch)..      
+00003cb0: 2020 2020 2020 7365 6c66 2e74 6573 7428        self.test(
+00003cc0: 7365 6c66 2e5f 6265 7374 5f65 706f 6368  self._best_epoch
+00003cd0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00003ce0: 656c 662e 7374 6570 2873 656c 662e 5f62  elf.step(self._b
+00003cf0: 6573 745f 6570 6f63 6829 0d0a 2020 2020  est_epoch)..    
+00003d00: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+00003d10: 6428 7365 6c66 2e63 6667 2e4c 4f47 5f50  d(self.cfg.LOG_P
+00003d20: 4154 482c 2073 656c 662e 6366 672e 5341  ATH, self.cfg.SA
+00003d30: 5645 445f 4649 4c45 4e41 4d45 290d 0a20  VED_FILENAME).. 
+00003d40: 2020 2020 2020 2065 7863 6570 7420 4669         except Fi
+00003d50: 6c65 4e6f 7446 6f75 6e64 4572 726f 723a  leNotFoundError:
+00003d60: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00003d70: 666f 4c6f 6767 6572 2866 225b 436f 6163  foLogger(f"[Coac
+00003d80: 685d 203e 3e3e 204e 6f20 6265 7374 206d  h] >>> No best m
+00003d90: 6f64 656c 2077 6173 2072 6563 6f72 6465  odel was recorde
+00003da0: 642e 2053 6b69 7020 6974 202e 2e2e 2229  d. Skip it ...")
+00003db0: 0d0a 0d0a 2020 2020 6465 6620 6561 7379  ....    def easy
+00003dc0: 5f72 6563 6f72 645f 6265 7374 2873 656c  _record_best(sel
+00003dd0: 662c 2062 6573 743a 2064 6566 6175 6c74  f, best: default
+00003de0: 6469 6374 293a 0d0a 2020 2020 2020 2020  dict):..        
+00003df0: 7222 2222 0d0a 2020 2020 2020 2020 5265  r"""..        Re
+00003e00: 636f 7264 2074 6865 2062 6573 7420 7265  cord the best re
+00003e10: 7375 6c74 7320 6f6e 2074 6573 7420 7365  sults on test se
+00003e20: 742e 0d0a 2020 2020 2020 2020 4974 206d  t...        It m
+00003e30: 616b 6520 6561 7379 2074 6f20 7761 7463  ake easy to watc
+00003e40: 6820 6f6e 2074 656e 736f 7262 6f61 7264  h on tensorboard
+00003e50: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00003e60: 0d0a 2020 2020 2020 2020 666f 7220 6c61  ..        for la
+00003e70: 7374 6e61 6d65 2c20 6d65 7465 7273 2069  stname, meters i
+00003e80: 6e20 7365 6c66 2e6d 6f6e 6974 6f72 735b  n self.monitors[
+00003e90: 2774 6573 7427 5d2e 6974 656d 7328 293a  'test'].items():
+00003ea0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00003eb0: 7220 6d65 7465 7220 696e 206d 6574 6572  r meter in meter
+00003ec0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00003ed0: 2020 2020 2320 536b 6970 2074 686f 7365      # Skip those
+00003ee0: 206d 6574 6572 7320 6e65 7665 7220 6163   meters never ac
+00003ef0: 7469 7661 7465 642e 0d0a 2020 2020 2020  tivated...      
+00003f00: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00003f10: 286d 6574 6572 2e68 6973 746f 7279 2920  (meter.history) 
+00003f20: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00003f30: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00003f40: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
+00003f50: 2020 2020 2023 204e 6f74 6520 7468 6174       # Note that
+00003f60: 206d 6574 6572 2e68 6973 746f 7279 5b2d   meter.history[-
+00003f70: 315d 2069 7320 7468 6520 7265 7375 6c74  1] is the result
+00003f80: 2061 7420 7468 6520 6265 7374 2063 6865   at the best che
+00003f90: 636b 706f 696e 742e 0d0a 2020 2020 2020  ckpoint...      
+00003fa0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+00003fb0: 6d65 7465 722e 6869 7374 6f72 795b 2d31  meter.history[-1
+00003fc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00003fd0: 2020 2062 6573 745b 2762 6573 7427 5d5b     best['best'][
+00003fe0: 6d65 7465 722e 6e61 6d65 5d20 3d20 7661  meter.name] = va
+00003ff0: 6c0d 0a0d 0a20 2020 2020 2020 2065 7870  l....        exp
+00004000: 6f72 745f 7069 636b 6c65 2862 6573 742c  ort_pickle(best,
+00004010: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00004020: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
+00004030: 2073 656c 662e 6366 672e 4441 5441 5f44   self.cfg.DATA_D
+00004040: 4952 2c20 7365 6c66 2e63 6667 2e4d 4f4e  IR, self.cfg.MON
+00004050: 4954 4f52 5f42 4553 545f 4649 4c45 4e41  ITOR_BEST_FILENA
+00004060: 4d45 2929 0d0a 0d0a 2020 2020 6465 6620  ME))....    def 
+00004070: 7265 7375 6d65 2873 656c 6629 202d 3e20  resume(self) -> 
+00004080: 696e 743a 0d0a 2020 2020 2020 2020 7222  int:..        r"
+00004090: 2222 0d0a 2020 2020 2020 2020 5265 7375  ""..        Resu
+000040a0: 6d65 2074 7261 696e 696e 6720 6672 6f6d  me training from
+000040b0: 2074 6865 206c 6173 7420 6368 6563 6b70   the last checkp
+000040c0: 6f69 6e74 2e0d 0a0d 0a20 2020 2020 2020  oint.....       
+000040d0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+000040e0: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
+000040f0: 2020 2020 2073 7461 7274 5f65 706f 6368       start_epoch
+00004100: 3a20 696e 740d 0a20 2020 2020 2020 2020  : int..         
+00004110: 2020 2054 6865 2065 706f 6368 206e 756d     The epoch num
+00004120: 6265 7220 746f 2072 6573 756d 6520 7472  ber to resume tr
+00004130: 6169 6e69 6e67 2066 726f 6d2e 0d0a 2020  aining from...  
+00004140: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004150: 2020 2073 7461 7274 5f65 706f 6368 3a20     start_epoch: 
+00004160: 696e 7420 3d20 300d 0a20 2020 2020 2020  int = 0..       
+00004170: 2069 6620 7365 6c66 2e63 6667 2e72 6573   if self.cfg.res
+00004180: 756d 653a 0d0a 2020 2020 2020 2020 2020  ume:..          
+00004190: 2020 7374 6172 745f 6570 6f63 6820 3d20    start_epoch = 
+000041a0: 7365 6c66 2e6c 6f61 645f 6368 6563 6b70  self.load_checkp
+000041b0: 6f69 6e74 2829 0d0a 2020 2020 2020 2020  oint()..        
+000041c0: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
+000041d0: 225b 436f 6163 685d 203e 3e3e 204c 6f61  "[Coach] >>> Loa
+000041e0: 6420 6c61 7374 2063 6865 636b 706f 696e  d last checkpoin
+000041f0: 7420 616e 6420 7472 6169 6e20 6672 6f6d  t and train from
+00004200: 2065 706f 6368 3a20 7b73 7461 7274 5f65   epoch: {start_e
+00004210: 706f 6368 7d22 290d 0a20 2020 2020 2020  poch}")..       
+00004220: 2072 6574 7572 6e20 7374 6172 745f 6570   return start_ep
+00004230: 6f63 680d 0a0d 0a20 2020 2040 746f 7263  och....    @torc
+00004240: 682e 6e6f 5f67 7261 6428 290d 0a20 2020  h.no_grad()..   
+00004250: 2064 6566 206d 6f6e 6974 6f72 280d 0a20   def monitor(.. 
+00004260: 2020 2020 2020 2073 656c 662c 202a 7661         self, *va
+00004270: 6c75 6573 2c0d 0a20 2020 2020 2020 206e  lues,..        n
+00004280: 3a20 696e 7420 3d20 312c 206d 6f64 653a  : int = 1, mode:
+00004290: 2073 7472 203d 2027 6d65 616e 272c 200d   str = 'mean', .
+000042a0: 0a20 2020 2020 2020 2070 7265 6669 783a  .        prefix:
+000042b0: 2073 7472 203d 2027 7472 6169 6e27 2c20   str = 'train', 
+000042c0: 706f 6f6c 3a20 4f70 7469 6f6e 616c 5b49  pool: Optional[I
+000042d0: 7465 7261 626c 655d 203d 204e 6f6e 650d  terable] = None.
+000042e0: 0a20 2020 2029 3a0d 0a0d 0a20 2020 2020  .    ):....     
+000042f0: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
+00004300: 204c 6f67 2064 6174 6120 7661 6c75 6573   Log data values
+00004310: 2074 6f20 7370 6563 6966 6963 206d 6f6e   to specific mon
+00004320: 6974 6f72 732e 0d0a 0d0a 2020 2020 2020  itors.....      
+00004330: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
+00004340: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00004350: 2d2d 0d0a 2020 2020 2020 2020 2a76 616c  --..        *val
+00004360: 7565 7320 3a20 6461 7461 0d0a 2020 2020  ues : data..    
+00004370: 2020 2020 2020 2020 5468 6520 6461 7461          The data
+00004380: 2076 616c 7565 7320 746f 2062 6520 6c6f   values to be lo
+00004390: 6767 6564 2e0d 0a20 2020 2020 2020 206e  gged...        n
+000043a0: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
+000043b0: 2020 2020 5468 6520 6261 7463 6820 7369      The batch si
+000043c0: 7a65 2069 6e20 6765 6e65 7261 6c2e 0d0a  ze in general...
+000043d0: 2020 2020 2020 2020 6d6f 6465 203a 2073          mode : s
+000043e0: 7472 2c20 6f70 7469 6f6e 616c 0d0a 2020  tr, optional..  
+000043f0: 2020 2020 2020 2020 2020 5468 6520 6d6f            The mo
+00004400: 6465 2074 6f20 636f 6d70 7574 6520 7468  de to compute th
+00004410: 6520 6d65 7472 6963 2e20 4361 6e20 6265  e metric. Can be
+00004420: 2027 7375 6d27 206f 7220 276d 6561 6e27   'sum' or 'mean'
+00004430: 2028 6465 6661 756c 7429 2e0d 0a20 2020   (default)...   
+00004440: 2020 2020 2070 7265 6669 7820 3a20 7374       prefix : st
+00004450: 722c 206f 7074 696f 6e61 6c0d 0a20 2020  r, optional..   
+00004460: 2020 2020 2020 2020 2054 6865 2070 7265           The pre
+00004470: 6669 7820 7374 7269 6e67 2069 6e64 6963  fix string indic
+00004480: 6174 696e 6720 7768 6963 6820 6d6f 6465  ating which mode
+00004490: 2074 6865 2076 616c 7565 7320 6265 6c6f   the values belo
+000044a0: 6e67 2074 6f2e 2043 616e 2062 6520 2774  ng to. Can be 't
+000044b0: 7261 696e 272c 2027 7465 7374 2720 6f72  rain', 'test' or
+000044c0: 2027 7661 6c69 6427 2e0d 0a20 2020 2020   'valid'...     
+000044d0: 2020 2070 6f6f 6c20 3a20 4c69 7374 5b73     pool : List[s
+000044e0: 7472 5d2c 206f 7074 696f 6e61 6c0d 0a20  tr], optional.. 
+000044f0: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
+00004500: 7420 6f66 206d 6574 7269 6320 6e61 6d65  t of metric name
+00004510: 7320 746f 206c 6f67 2e20 4966 204e 6f6e  s to log. If Non
+00004520: 652c 2061 6c6c 206d 6574 7269 6373 2069  e, all metrics i
+00004530: 6e20 7468 6520 706f 6f6c 206f 6620 6070  n the pool of `p
+00004540: 7265 6669 7860 2077 696c 6c20 6265 206c  refix` will be l
+00004550: 6f67 6765 642e 0d0a 2020 2020 2020 2020  ogged...        
+00004560: 2222 220d 0a0d 0a20 2020 2020 2020 206d  """....        m
+00004570: 6574 7269 6373 3a20 4469 6374 5b4c 6973  etrics: Dict[Lis
+00004580: 745d 203d 2073 656c 662e 6d6f 6e69 746f  t] = self.monito
+00004590: 7273 5b70 7265 6669 785d 0d0a 2020 2020  rs[prefix]..    
+000045a0: 2020 2020 706f 6f6c 203d 206d 6574 7269      pool = metri
+000045b0: 6373 2069 6620 706f 6f6c 2069 7320 4e6f  cs if pool is No
+000045c0: 6e65 2065 6c73 6520 706f 6f6c 0d0a 2020  ne else pool..  
+000045d0: 2020 2020 2020 666f 7220 6c61 7374 6e61        for lastna
+000045e0: 6d65 2069 6e20 706f 6f6c 3a0d 0a20 2020  me in pool:..   
+000045f0: 2020 2020 2020 2020 2066 6f72 206d 6574           for met
+00004600: 6572 2069 6e20 6d65 7472 6963 732e 6765  er in metrics.ge
+00004610: 7428 6c61 7374 6e61 6d65 2e75 7070 6572  t(lastname.upper
+00004620: 2829 2c20 5b5d 293a 0d0a 2020 2020 2020  (), []):..      
+00004630: 2020 2020 2020 2020 2020 6d65 7465 7228            meter(
+00004640: 2a76 616c 7565 732c 206e 3d6e 2c20 6d6f  *values, n=n, mo
+00004650: 6465 3d6d 6f64 6529 0d0a 0d0a 2020 2020  de=mode)....    
+00004660: 6465 6620 7374 6570 2873 656c 662c 2065  def step(self, e
+00004670: 706f 6368 3a20 696e 7429 3a0d 0a20 2020  poch: int):..   
+00004680: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
+00004690: 2020 2050 7269 6e74 7320 7472 6169 6e69     Prints traini
+000046a0: 6e67 2073 7461 7475 7320 616e 6420 6576  ng status and ev
+000046b0: 616c 7561 7469 6f6e 2072 6573 756c 7473  aluation results
+000046c0: 2066 6f72 2065 6163 6820 6570 6f63 682c   for each epoch,
+000046d0: 200d 0a20 2020 2020 2020 2061 6e64 2072   ..        and r
+000046e0: 6573 6574 7320 7468 6520 636f 7272 6573  esets the corres
+000046f0: 706f 6e64 696e 6720 6041 7665 7261 6765  ponding `Average
+00004700: 4d65 7465 7260 2069 6e73 7461 6e63 6573  Meter` instances
+00004710: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00004720: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00004730: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
+00004740: 2020 2020 2020 2065 706f 6368 203a 2069         epoch : i
+00004750: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00004760: 5468 6520 6570 6f63 6820 6e75 6d62 6572  The epoch number
+00004770: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00004780: 7572 6e73 3a0d 0a20 2020 2020 2020 202d  urns:..        -
+00004790: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+000047a0: 204e 6f6e 650d 0a20 2020 2020 2020 2022   None..        "
+000047b0: 2222 0d0a 2020 2020 2020 2020 6d65 7472  ""..        metr
+000047c0: 6963 733a 2044 6963 745b 7374 722c 204c  ics: Dict[str, L
+000047d0: 6973 745b 4176 6572 6167 654d 6574 6572  ist[AverageMeter
+000047e0: 5d5d 0d0a 2020 2020 2020 2020 666f 7220  ]]..        for 
+000047f0: 7072 6566 6978 2c20 6d65 7472 6963 7320  prefix, metrics 
+00004800: 696e 2073 656c 662e 6d6f 6e69 746f 7273  in self.monitors
+00004810: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00004820: 2020 2020 2020 2069 6e66 6f73 203d 205b         infos = [
+00004830: 6622 5b43 6f61 6368 5d20 3e3e 3e20 7b70  f"[Coach] >>> {p
+00004840: 7265 6669 782e 7570 7065 7228 293a 357d  refix.upper():5}
+00004850: 2040 4570 6f63 683a 207b 6570 6f63 683a   @Epoch: {epoch:
+00004860: 3c34 647d 203e 3e3e 2022 5d0d 0a20 2020  <4d} >>> "]..   
+00004870: 2020 2020 2020 2020 2066 6f72 206d 6574           for met
+00004880: 6572 7320 696e 206d 6574 7269 6373 2e76  ers in metrics.v
+00004890: 616c 7565 7328 293a 0d0a 2020 2020 2020  alues():..      
+000048a0: 2020 2020 2020 2020 2020 696e 666f 7320            infos 
+000048b0: 2b3d 205b 6d65 7465 722e 7374 6570 2829  += [meter.step()
+000048c0: 2066 6f72 206d 6574 6572 2069 6e20 6d65   for meter in me
+000048d0: 7465 7273 2069 6620 6d65 7465 722e 6163  ters if meter.ac
+000048e0: 7469 7665 5d0d 0a20 2020 2020 2020 2020  tive]..         
+000048f0: 2020 2069 6e66 6f4c 6f67 6765 7228 2720     infoLogger(' 
+00004900: 7c7c 2027 2e6a 6f69 6e28 696e 666f 7329  || '.join(infos)
+00004910: 290d 0a0d 0a20 2020 2040 7469 6d65 6d65  )....    @timeme
+00004920: 7465 720d 0a20 2020 2064 6566 2073 756d  ter..    def sum
+00004930: 6d61 7279 2873 656c 6629 3a0d 0a20 2020  mary(self):..   
+00004940: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
+00004950: 2020 2053 756d 6d61 7279 2074 6865 2077     Summary the w
+00004960: 686f 6c65 2074 7261 696e 696e 6720 7072  hole training pr
+00004970: 6f63 6573 732e 0d0a 0d0a 2020 2020 2020  ocess.....      
+00004980: 2020 4765 6e65 7261 7465 2061 2073 756d    Generate a sum
+00004990: 6d61 7279 206f 6620 7468 6520 656e 7469  mary of the enti
+000049a0: 7265 2074 7261 696e 696e 6720 7072 6f63  re training proc
+000049b0: 6573 732c 2069 6e63 6c75 6469 6e67 2074  ess, including t
+000049c0: 6865 2068 6973 746f 7269 6361 6c20 6576  he historical ev
+000049d0: 616c 7561 7469 6f6e 2072 6573 756c 7473  aluation results
+000049e0: 2c20 7468 6520 6265 7374 0d0a 2020 2020  , the best..    
+000049f0: 2020 2020 6869 7374 6f72 6963 616c 2072      historical r
+00004a00: 6573 756c 7473 2c20 616e 6420 7468 6520  esults, and the 
+00004a10: 6375 7276 6573 206f 6620 6869 7374 6f72  curves of histor
+00004a20: 6963 616c 2072 6573 756c 7473 2e20 5468  ical results. Th
+00004a30: 6520 7265 7375 6c74 696e 6720 7375 6d6d  e resulting summ
+00004a40: 6172 7920 6973 2073 6176 6564 2074 6f20  ary is saved to 
+00004a50: 6120 4d61 726b 646f 776e 2066 696c 6520  a Markdown file 
+00004a60: 6e61 6d65 640d 0a20 2020 2020 2020 2022  named..        "
+00004a70: 5375 6d6d 6172 792e 6d64 2220 696e 2074  Summary.md" in t
+00004a80: 6865 2060 7365 6c66 2e63 6667 2e4c 4f47  he `self.cfg.LOG
+00004a90: 5f50 4154 4860 2064 6972 6563 746f 7279  _PATH` directory
+00004aa0: 2e0d 0a0d 0a20 2020 2020 2020 2041 6464  .....        Add
+00004ab0: 6974 696f 6e61 6c6c 792c 2074 6865 2062  itionally, the b
+00004ac0: 6573 7420 6869 7374 6f72 6963 616c 2072  est historical r
+00004ad0: 6573 756c 7473 2061 7265 2073 6176 6564  esults are saved
+00004ae0: 2074 6f20 6120 6269 6e61 7279 2066 696c   to a binary fil
+00004af0: 6520 6e61 6d65 6420 6073 656c 662e 6366  e named `self.cf
+00004b00: 672e 4d4f 4e49 544f 525f 4245 5354 5f46  g.MONITOR_BEST_F
+00004b10: 494c 454e 414d 4560 2e0d 0a20 2020 2020  ILENAME`...     
+00004b20: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004b30: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
+00004b40: 2070 640d 0a0d 0a20 2020 2020 2020 2073   pd....        s
+00004b50: 203d 2022 7c20 207b 7072 6566 6978 7d20   = "|  {prefix} 
+00004b60: 207c 2020 207b 6e61 6d65 7d20 2020 7c20   |   {name}   | 
+00004b70: 2020 7b76 616c 7d20 2020 7c20 2020 7b65    {val}   |   {e
+00004b80: 706f 6368 7d20 2020 7c20 2020 7b69 6d67  poch}   |   {img
+00004b90: 7d20 2020 7c5c 6e22 0d0a 2020 2020 2020  }   |\n"..      
+00004ba0: 2020 696e 666f 203d 2022 220d 0a20 2020    info = ""..   
+00004bb0: 2020 2020 2069 6e66 6f20 2b3d 2022 7c20       info += "| 
+00004bc0: 2050 7265 6669 7820 207c 2020 204d 6574   Prefix  |   Met
+00004bd0: 7269 6320 2020 7c20 2020 4265 7374 2020  ric   |   Best  
+00004be0: 207c 2020 2040 4570 6f63 6820 2020 7c20   |   @Epoch   | 
+00004bf0: 2020 496d 6720 2020 7c5c 6e22 0d0a 2020    Img   |\n"..  
+00004c00: 2020 2020 2020 696e 666f 202b 3d20 227c        info += "|
+00004c10: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
+00004c20: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+00004c30: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
+00004c40: 203a 2d2d 2d2d 2d2d 2d3a 207c 5c6e 220d   :-------: |\n".
+00004c50: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00004c60: 5b5d 0d0a 2020 2020 2020 2020 6265 7374  []..        best
+00004c70: 203d 2064 6566 6175 6c74 6469 6374 2864   = defaultdict(d
+00004c80: 6963 7429 0d0a 0d0a 2020 2020 2020 2020  ict)....        
+00004c90: 666f 7220 7072 6566 6978 2c20 6d65 7472  for prefix, metr
+00004ca0: 6963 7320 696e 2073 656c 662e 6d6f 6e69  ics in self.moni
+00004cb0: 746f 7273 2e69 7465 6d73 2829 3a0d 0a20  tors.items():.. 
+00004cc0: 2020 2020 2020 2020 2020 206d 6574 7269             metri
+00004cd0: 6373 3a20 6465 6661 756c 7464 6963 745b  cs: defaultdict[
+00004ce0: 7374 722c 204c 6973 745b 4176 6572 6167  str, List[Averag
+00004cf0: 654d 6574 6572 5d5d 0d0a 2020 2020 2020  eMeter]]..      
+00004d00: 2020 2020 2020 6672 6571 203d 2031 2069        freq = 1 i
+00004d10: 6620 7072 6566 6978 203d 3d20 2774 7261  f prefix == 'tra
+00004d20: 696e 2720 656c 7365 2073 656c 662e 6366  in' else self.cf
+00004d30: 672e 4556 414c 5f46 5245 510d 0a20 2020  g.EVAL_FREQ..   
+00004d40: 2020 2020 2020 2020 2066 6f72 206c 6173           for las
+00004d50: 746e 616d 652c 206d 6574 6572 7320 696e  tname, meters in
+00004d60: 206d 6574 7269 6373 2e69 7465 6d73 2829   metrics.items()
+00004d70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004d80: 2020 2066 6f72 206d 6574 6572 2069 6e20     for meter in 
+00004d90: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+00004da0: 2020 2020 2020 2020 2020 2020 2023 2053               # S
+00004db0: 6b69 7020 7468 6f73 6520 6d65 7465 7273  kip those meters
+00004dc0: 206e 6576 6572 2061 6374 6976 6174 6564   never activated
+00004dd0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00004de0: 2020 2020 2020 2069 6620 6c65 6e28 6d65         if len(me
+00004df0: 7465 722e 6869 7374 6f72 7929 203d 3d20  ter.history) == 
+00004e00: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00004e10: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00004e20: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
+00004e30: 2020 2020 2020 2020 2020 6d65 7465 722e            meter.
+00004e40: 706c 6f74 2866 7265 713d 6672 6571 290d  plot(freq=freq).
+00004e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004e60: 2020 2020 2069 6d67 6e61 6d65 203d 206d       imgname = m
+00004e70: 6574 6572 2e73 6176 6528 7061 7468 3d6f  eter.save(path=o
+00004e80: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+00004e90: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
+00004ea0: 656c 662e 6366 672e 5355 4d4d 4152 595f  elf.cfg.SUMMARY_
+00004eb0: 4449 5229 2c20 7072 6566 6978 3d70 7265  DIR), prefix=pre
+00004ec0: 6669 7829 0d0a 2020 2020 2020 2020 2020  fix)..          
+00004ed0: 2020 2020 2020 2020 2020 6570 6f63 682c            epoch,
+00004ee0: 2076 616c 203d 206d 6574 6572 2e61 7267   val = meter.arg
+00004ef0: 6265 7374 2866 7265 7129 0d0a 2020 2020  best(freq)..    
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f10: 696e 666f 202b 3d20 732e 666f 726d 6174  info += s.format
+00004f20: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00004f30: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00004f40: 783d 7072 6566 6978 2c20 6e61 6d65 3d6d  x=prefix, name=m
+00004f50: 6574 6572 2e6e 616d 652c 0d0a 2020 2020  eter.name,..    
+00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f70: 2020 2020 7661 6c3d 7661 6c2c 2065 706f      val=val, epo
+00004f80: 6368 3d65 706f 6368 2c20 696d 673d 6622  ch=epoch, img=f"
+00004f90: 215b 5d28 7b69 6d67 6e61 6d65 7d29 220d  ![]({imgname})".
+00004fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fb0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00004fc0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00004fd0: 2e61 7070 656e 6428 5b70 7265 6669 782c  .append([prefix,
+00004fe0: 206d 6574 6572 2e6e 616d 652c 2076 616c   meter.name, val
+00004ff0: 2c20 6570 6f63 685d 290d 0a20 2020 2020  , epoch])..     
+00005000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005010: 6620 7661 6c20 213d 202d 313a 2023 204f  f val != -1: # O
+00005020: 6e6c 7920 7361 7665 2061 7661 696c 6162  nly save availab
+00005030: 6c65 2064 6174 612e 0d0a 2020 2020 2020  le data...      
+00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005050: 2020 6265 7374 5b70 7265 6669 785d 5b6d    best[prefix][m
+00005060: 6574 6572 2e6e 616d 655d 203d 2076 616c  eter.name] = val
+00005070: 0d0a 0d0a 2020 2020 2020 2020 6669 6c65  ....        file
+00005080: 5f20 3d20 6f73 2e70 6174 682e 6a6f 696e  _ = os.path.join
+00005090: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
+000050a0: 5448 2c20 7365 6c66 2e63 6667 2e53 554d  TH, self.cfg.SUM
+000050b0: 4d41 5259 5f44 4952 2c20 7365 6c66 2e63  MARY_DIR, self.c
+000050c0: 6667 2e53 554d 4d41 5259 5f46 494c 454e  fg.SUMMARY_FILEN
+000050d0: 414d 4529 0d0a 2020 2020 2020 2020 7769  AME)..        wi
+000050e0: 7468 206f 7065 6e28 6669 6c65 5f2c 2022  th open(file_, "
+000050f0: 7722 2c20 656e 636f 6469 6e67 3d22 7574  w", encoding="ut
+00005100: 6638 2229 2061 7320 6668 3a0d 0a20 2020  f8") as fh:..   
+00005110: 2020 2020 2020 2020 2066 682e 7772 6974           fh.writ
+00005120: 6528 696e 666f 290d 0a0d 0a20 2020 2020  e(info)....     
+00005130: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
+00005140: 7261 6d65 2864 6174 612c 2063 6f6c 756d  rame(data, colum
+00005150: 6e73 3d5b 2750 7265 6669 7827 2c20 274d  ns=['Prefix', 'M
+00005160: 6574 7269 6327 2c20 2742 6573 7427 2c20  etric', 'Best', 
+00005170: 2740 4570 6f63 6827 5d29 0d0a 2020 2020  '@Epoch'])..    
+00005180: 2020 2020 696e 666f 4c6f 6767 6572 2873      infoLogger(s
+00005190: 7472 2864 6629 290d 0a20 2020 2020 2020  tr(df))..       
+000051a0: 2069 6e66 6f4c 6f67 6765 7228 6622 5b4c   infoLogger(f"[L
+000051b0: 6f47 5f50 6154 485d 203e 3e3e 207b 7365  oG_PaTH] >>> {se
+000051c0: 6c66 2e63 6667 2e4c 4f47 5f50 4154 487d  lf.cfg.LOG_PATH}
+000051d0: 2229 0d0a 0d0a 2020 2020 2020 2020 7365  ")....        se
+000051e0: 6c66 2e6d 6f6e 6974 6f72 732e 7772 6974  lf.monitors.writ
+000051f0: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
+00005200: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00005210: 2c20 7365 6c66 2e63 6667 2e53 554d 4d41  , self.cfg.SUMMA
+00005220: 5259 5f44 4952 2929 2023 2074 656e 736f  RY_DIR)) # tenso
+00005230: 7262 6f61 7264 0d0a 2020 2020 2020 2020  rboard..        
+00005240: 7365 6c66 2e6d 6f6e 6974 6f72 732e 7361  self.monitors.sa
+00005250: 7665 286f 732e 7061 7468 2e6a 6f69 6e28  ve(os.path.join(
+00005260: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
+00005270: 482c 2073 656c 662e 6366 672e 4441 5441  H, self.cfg.DATA
+00005280: 5f44 4952 292c 2073 656c 662e 6366 672e  _DIR), self.cfg.
+00005290: 4d4f 4e49 544f 525f 4649 4c45 4e41 4d45  MONITOR_FILENAME
+000052a0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
+000052b0: 7572 6e20 6265 7374 0d0a 2020 2020 2020  urn best..      
+000052c0: 2020 2020 2020 0d0a 2020 2020 4074 696d        ..    @tim
+000052d0: 656d 6574 6572 0d0a 2020 2020 6465 6620  emeter..    def 
+000052e0: 6669 7428 7365 6c66 293a 0d0a 0d0a 2020  fit(self):....  
+000052f0: 2020 2020 2020 6465 6620 7369 676e 616c        def signal
+00005300: 5f68 616e 646c 6572 2873 6967 2c20 6672  _handler(sig, fr
+00005310: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
+00005320: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+00005330: 5c30 3333 5b30 3b33 313b 3437 6d3d 3d3d  \033[0;31;47m===
+00005340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5445 524d  ============TERM
+00005360: 494e 4154 4520 4355 5252 454e 5420 5052  INATE CURRENT PR
+00005370: 4f43 4553 533d 3d3d 3d3d 3d3d 3d3d 3d3d  OCESS===========
+00005380: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005390: 3d3d 3d3d 5c30 3333 5b30 6d22 290d 0a20  ====\033[0m").. 
+000053a0: 2020 2020 2020 2020 2020 2073 7973 2e65             sys.e
+000053b0: 7869 7428 290d 0a20 2020 2020 2020 2073  xit()..        s
+000053c0: 6967 6e61 6c2e 7369 676e 616c 2873 6967  ignal.signal(sig
+000053d0: 6e61 6c2e 5349 4749 4e54 2c20 7369 676e  nal.SIGINT, sign
+000053e0: 616c 5f68 616e 646c 6572 290d 0a0d 0a20  al_handler).... 
+000053f0: 2020 2020 2020 2073 7461 7274 5f65 706f         start_epo
+00005400: 6368 203d 2073 656c 662e 7265 7375 6d65  ch = self.resume
+00005410: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00005420: 6570 6f63 6820 696e 2072 616e 6765 2873  epoch in range(s
+00005430: 7461 7274 5f65 706f 6368 2c20 7365 6c66  tart_epoch, self
+00005440: 2e63 6667 2e65 706f 6368 7329 3a0d 0a20  .cfg.epochs):.. 
+00005450: 2020 2020 2020 2020 2020 2069 6620 6570             if ep
+00005460: 6f63 6820 2520 7365 6c66 2e63 6667 2e43  och % self.cfg.C
+00005470: 4845 434b 504f 494e 545f 4652 4551 203d  HECKPOINT_FREQ =
+00005480: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00005490: 2020 2020 2020 7365 6c66 2e73 6176 655f        self.save_
+000054a0: 6368 6563 6b70 6f69 6e74 2865 706f 6368  checkpoint(epoch
+000054b0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+000054c0: 6620 6570 6f63 6820 2520 7365 6c66 2e63  f epoch % self.c
+000054d0: 6667 2e45 5641 4c5f 4652 4551 203d 3d20  fg.EVAL_FREQ == 
+000054e0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000054f0: 2020 2020 6966 2073 656c 662e 6366 672e      if self.cfg.
+00005500: 4556 414c 5f56 414c 4944 3a0d 0a20 2020  EVAL_VALID:..   
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2073 656c 662e 7661 6c69 6428 6570 6f63   self.valid(epoc
+00005530: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+00005540: 2020 2020 6966 2073 656c 662e 6366 672e      if self.cfg.
+00005550: 4556 414c 5f54 4553 543a 0d0a 2020 2020  EVAL_TEST:..    
+00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005570: 7365 6c66 2e74 6573 7428 6570 6f63 6829  self.test(epoch)
+00005580: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005590: 6c66 2e63 6865 636b 5f62 6573 7428 6570  lf.check_best(ep
+000055a0: 6f63 6829 0d0a 2020 2020 2020 2020 2020  och)..          
+000055b0: 2020 7365 6c66 2e73 7465 7028 6570 6f63    self.step(epoc
+000055c0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+000055d0: 7365 6c66 2e74 7261 696e 2865 706f 6368  self.train(epoch
+000055e0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+000055f0: 662e 7361 7665 2829 0d0a 0d0a 2020 2020  f.save()....    
+00005600: 2020 2020 2320 6c61 7374 2065 706f 6368      # last epoch
+00005610: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
+00005620: 616c 6964 2873 656c 662e 6366 672e 6570  alid(self.cfg.ep
+00005630: 6f63 6873 290d 0a20 2020 2020 2020 2073  ochs)..        s
+00005640: 656c 662e 7465 7374 2873 656c 662e 6366  elf.test(self.cf
+00005650: 672e 6570 6f63 6873 290d 0a20 2020 2020  g.epochs)..     
+00005660: 2020 2073 656c 662e 6368 6563 6b5f 6265     self.check_be
+00005670: 7374 2873 656c 662e 6366 672e 6570 6f63  st(self.cfg.epoc
+00005680: 6873 290d 0a20 2020 2020 2020 2073 656c  hs)..        sel
+00005690: 662e 7374 6570 2873 656c 662e 6366 672e  f.step(self.cfg.
+000056a0: 6570 6f63 6873 290d 0a0d 0a20 2020 2020  epochs)....     
+000056b0: 2020 2062 6573 7420 3d20 7365 6c66 2e73     best = self.s
+000056c0: 756d 6d61 7279 2829 0d0a 0d0a 2020 2020  ummary()....    
+000056d0: 2020 2020 7365 6c66 2e65 7661 6c5f 6174      self.eval_at
+000056e0: 5f62 6573 7428 290d 0a20 2020 2020 2020  _best()..       
+000056f0: 2073 656c 662e 6561 7379 5f72 6563 6f72   self.easy_recor
+00005700: 645f 6265 7374 2862 6573 7429 0d0a 0d0a  d_best(best)....
+00005710: 0d0a 636c 6173 7320 4765 6e43 6f61 6368  ..class GenCoach
+00005720: 2843 6f61 6368 293a 0d0a 0d0a 2020 2020  (Coach):....    
+00005730: 6465 6620 6576 616c 7561 7465 2873 656c  def evaluate(sel
+00005740: 662c 2065 706f 6368 3a20 696e 742c 2070  f, epoch: int, p
+00005750: 7265 6669 783a 2073 7472 203d 2027 7661  refix: str = 'va
+00005760: 6c69 6427 293a 0d0a 2020 2020 2020 2020  lid'):..        
+00005770: 7222 2222 0d0a 2020 2020 2020 2020 4576  r"""..        Ev
+00005780: 616c 7561 7465 2072 6563 6f6d 6d65 6e64  aluate recommend
+00005790: 6572 2062 7920 7361 6d70 6c65 642d 6261  er by sampled-ba
+000057a0: 7365 6420 6f72 2066 756c 6c20 7261 6e6b  sed or full rank
+000057b0: 696e 670d 0a20 2020 2020 2020 2061 6363  ing..        acc
+000057c0: 6f72 6469 6e67 2074 6f20 7468 6520 666f  ording to the fo
+000057d0: 726d 206f 6620 6064 6174 6160 3a0d 0a0d  rm of `data`:...
+000057e0: 0a20 2020 2020 2020 2031 2e20 2875 7365  .        1. (use
+000057f0: 7273 2c20 706f 6f6c 293a 0d0a 2020 2020  rs, pool):..    
+00005800: 2020 2020 2020 2020 7573 6572 733a 2074          users: t
+00005810: 6f72 6368 2e54 656e 736f 722c 2028 422c  orch.Tensor, (B,
+00005820: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
+00005830: 2070 6f6f 6c3a 2074 6f72 6368 2e54 656e   pool: torch.Ten
+00005840: 736f 722c 2028 422c 2031 3031 290d 0a20  sor, (B, 101).. 
+00005850: 2020 2020 2020 2032 2e20 2875 7365 7273         2. (users
+00005860: 2c20 756e 7365 656e 2c20 7365 656e 293a  , unseen, seen):
+00005870: 0d0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+00005880: 6572 733a 2042 7566 6665 7246 6965 6c64  ers: BufferField
+00005890: 0d0a 2020 2020 2020 2020 2020 2020 756e  ..            un
+000058a0: 7365 656e 3a20 4275 6666 6572 4669 656c  seen: BufferFiel
+000058b0: 640d 0a20 2020 2020 2020 2020 2020 2073  d..            s
+000058c0: 6565 6e3a 2042 7566 6665 7246 6965 6c64  een: BufferField
+000058d0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000058e0: 2020 2020 2020 2075 7365 7246 6561 7473         userFeats
+000058f0: 2c20 6974 656d 4665 6174 7320 3d20 7365  , itemFeats = se
+00005900: 6c66 2e6d 6f64 656c 2e72 6563 6f6d 6d65  lf.model.recomme
+00005910: 6e64 2829 0d0a 2020 2020 2020 2020 666f  nd()..        fo
+00005920: 7220 6461 7461 2069 6e20 7365 6c66 2e64  r data in self.d
+00005930: 6174 616c 6f61 6465 723a 0d0a 2020 2020  ataloader:..    
+00005940: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
+00005950: 6174 6129 203d 3d20 323a 0d0a 2020 2020  ata) == 2:..    
+00005960: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00005970: 732c 2070 6f6f 6c20 3d20 5b63 6f6c 2e74  s, pool = [col.t
+00005980: 6f28 7365 6c66 2e64 6576 6963 6529 2066  o(self.device) f
+00005990: 6f72 2063 6f6c 2069 6e20 6461 7461 5d0d  or col in data].
+000059a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059b0: 2075 7365 7273 203d 2075 7365 7246 6561   users = userFea
+000059c0: 7473 5b75 7365 7273 5d20 2320 2842 2c20  ts[users] # (B, 
+000059d0: 312c 2044 290d 0a20 2020 2020 2020 2020  1, D)..         
+000059e0: 2020 2020 2020 2069 7465 6d73 203d 2069         items = i
+000059f0: 7465 6d46 6561 7473 5b70 6f6f 6c5d 2023  temFeats[pool] #
+00005a00: 2028 422c 204b 2c20 4429 0d0a 2020 2020   (B, K, D)..    
+00005a10: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
+00005a20: 6573 203d 2075 7365 7273 2e6d 756c 2869  es = users.mul(i
+00005a30: 7465 6d73 292e 7375 6d28 2d31 290d 0a20  tems).sum(-1).. 
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005a50: 6172 6765 7473 203d 2074 6f72 6368 2e7a  argets = torch.z
+00005a60: 6572 6f73 5f6c 696b 6528 7363 6f72 6573  eros_like(scores
+00005a70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005a80: 2020 2074 6172 6765 7473 5b3a 2c20 305d     targets[:, 0]
+00005a90: 2e66 696c 6c5f 2831 290d 0a20 2020 2020  .fill_(1)..     
+00005aa0: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
+00005ab0: 6461 7461 2920 3d3d 2033 3a0d 0a20 2020  data) == 3:..   
+00005ac0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00005ad0: 7273 2c20 756e 7365 656e 2c20 7365 656e  rs, unseen, seen
+00005ae0: 203d 2064 6174 610d 0a20 2020 2020 2020   = data..       
+00005af0: 2020 2020 2020 2020 2075 7365 7273 203d           users =
+00005b00: 2075 7365 7273 2e74 6f28 7365 6c66 2e64   users.to(self.d
+00005b10: 6576 6963 6529 2e64 6174 610d 0a20 2020  evice).data..   
+00005b20: 2020 2020 2020 2020 2020 2020 2073 6565               see
+00005b30: 6e20 3d20 7365 656e 2e74 6f5f 6373 7228  n = seen.to_csr(
+00005b40: 292e 746f 2873 656c 662e 6465 7669 6365  ).to(self.device
+00005b50: 292e 746f 5f64 656e 7365 2829 2e62 6f6f  ).to_dense().boo
+00005b60: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
+00005b70: 2020 2020 2074 6172 6765 7473 203d 2075       targets = u
+00005b80: 6e73 6565 6e2e 746f 5f63 7372 2829 2e74  nseen.to_csr().t
+00005b90: 6f28 7365 6c66 2e64 6576 6963 6529 2e74  o(self.device).t
+00005ba0: 6f5f 6465 6e73 6528 290d 0a20 2020 2020  o_dense()..     
+00005bb0: 2020 2020 2020 2020 2020 2075 7365 7273             users
+00005bc0: 203d 2075 7365 7246 6561 7473 5b75 7365   = userFeats[use
+00005bd0: 7273 5d2e 666c 6174 7465 6e28 3129 2023  rs].flatten(1) #
+00005be0: 2042 2078 2044 0d0a 2020 2020 2020 2020   B x D..        
+00005bf0: 2020 2020 2020 2020 6974 656d 7320 3d20          items = 
+00005c00: 6974 656d 4665 6174 732e 666c 6174 7465  itemFeats.flatte
+00005c10: 6e28 3129 2023 204e 2078 2044 0d0a 2020  n(1) # N x D..  
+00005c20: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00005c30: 6f72 6573 203d 2075 7365 7273 2e6d 6174  ores = users.mat
+00005c40: 6d75 6c28 6974 656d 732e 5429 2023 2042  mul(items.T) # B
+00005c50: 2078 204e 0d0a 2020 2020 2020 2020 2020   x N..          
+00005c60: 2020 2020 2020 7363 6f72 6573 5b73 6565        scores[see
+00005c70: 6e5d 203d 202d 3165 3233 0d0a 2020 2020  n] = -1e23..    
+00005c80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00005ca0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+00005cb0: 7465 6445 7272 6f72 280d 0a20 2020 2020  tedError(..     
+00005cc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005cd0: 2247 656e 436f 6163 6827 7320 6065 7661  "GenCoach's `eva
+00005ce0: 6c75 6174 6560 2065 7870 6563 7473 2074  luate` expects t
+00005cf0: 6865 2060 6461 7461 6020 746f 2062 6520  he `data` to be 
+00005d00: 7468 6520 6c65 6e67 7468 206f 6620 3220  the length of 2 
+00005d10: 6f72 2033 2c20 6275 7420 7b6c 656e 2864  or 3, but {len(d
+00005d20: 6174 6129 7d20 7265 6365 6976 6564 202e  ata)} received .
+00005d30: 2e2e 220d 0a20 2020 2020 2020 2020 2020  .."..           
+00005d40: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00005d50: 2020 2020 2020 7365 6c66 2e6d 6f6e 6974        self.monit
+00005d60: 6f72 280d 0a20 2020 2020 2020 2020 2020  or(..           
+00005d70: 2020 2020 2073 636f 7265 732c 2074 6172       scores, tar
+00005d80: 6765 7473 2c0d 0a20 2020 2020 2020 2020  gets,..         
+00005d90: 2020 2020 2020 206e 3d6c 656e 2875 7365         n=len(use
+00005da0: 7273 292c 206d 6f64 653d 226d 6561 6e22  rs), mode="mean"
+00005db0: 2c20 7072 6566 6978 3d70 7265 6669 782c  , prefix=prefix,
+00005dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005dd0: 2020 706f 6f6c 3d5b 2748 4954 5241 5445    pool=['HITRATE
+00005de0: 272c 2027 5052 4543 4953 494f 4e27 2c20  ', 'PRECISION', 
+00005df0: 2752 4543 414c 4c27 2c20 274e 4443 4727  'RECALL', 'NDCG'
+00005e00: 2c20 274d 5252 275d 0d0a 2020 2020 2020  , 'MRR']..      
+00005e10: 2020 2020 2020 290d 0a0d 0a0d 0a63 6c61        )......cla
+00005e20: 7373 2053 6571 436f 6163 6828 436f 6163  ss SeqCoach(Coac
+00005e30: 6829 3a0d 0a0d 0a20 2020 2064 6566 2065  h):....    def e
+00005e40: 7661 6c75 6174 6528 7365 6c66 2c20 6570  valuate(self, ep
+00005e50: 6f63 683a 2069 6e74 2c20 7072 6566 6978  och: int, prefix
+00005e60: 3a20 7374 7220 3d20 2776 616c 6964 2729  : str = 'valid')
+00005e70: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
+00005e80: 0a20 2020 2020 2020 2045 7661 6c75 6174  .        Evaluat
+00005e90: 6520 7265 636f 6d6d 656e 6465 7220 6279  e recommender by
+00005ea0: 2073 616d 706c 6564 2d62 6173 6564 206f   sampled-based o
+00005eb0: 7220 6675 6c6c 2072 616e 6b69 6e67 0d0a  r full ranking..
+00005ec0: 2020 2020 2020 2020 6163 636f 7264 696e          accordin
+00005ed0: 6720 746f 2074 6865 2066 6f72 6d20 6f66  g to the form of
+00005ee0: 2060 6461 7461 603a 0d0a 0d0a 2020 2020   `data`:....    
+00005ef0: 2020 2020 312e 2028 7573 6572 732c 2073      1. (users, s
+00005f00: 6571 732c 2070 6f6f 6c29 3a0d 0a20 2020  eqs, pool):..   
+00005f10: 2020 2020 2020 2020 2075 7365 7273 3a20           users: 
+00005f20: 746f 7263 682e 5465 6e73 6f72 2c20 2842  torch.Tensor, (B
+00005f30: 2c20 3129 0d0a 2020 2020 2020 2020 2020  , 1)..          
+00005f40: 2020 7365 7173 3a20 746f 7263 682e 5465    seqs: torch.Te
+00005f50: 6e73 6f72 2c20 2842 2c20 5329 0d0a 2020  nsor, (B, S)..  
+00005f60: 2020 2020 2020 2020 2020 706f 6f6c 3a20            pool: 
+00005f70: 746f 7263 682e 5465 6e73 6f72 2c20 2842  torch.Tensor, (B
+00005f80: 2c20 3130 3129 0d0a 2020 2020 2020 2020  , 101)..        
+00005f90: 322e 2028 7573 6572 732c 2073 6571 732c  2. (users, seqs,
+00005fa0: 2075 6e73 6565 6e2c 2073 6565 6e29 3a0d   unseen, seen):.
+00005fb0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00005fc0: 7273 3a20 4275 6666 6572 4669 656c 640d  rs: BufferField.
+00005fd0: 0a20 2020 2020 2020 2020 2020 2073 6571  .            seq
+00005fe0: 733a 2042 7566 6665 7246 6965 6c64 0d0a  s: BufferField..
+00005ff0: 2020 2020 2020 2020 2020 2020 756e 7365              unse
+00006000: 656e 3a20 4275 6666 6572 4669 656c 640d  en: BufferField.
+00006010: 0a20 2020 2020 2020 2020 2020 2073 6565  .            see
+00006020: 6e3a 2042 7566 6665 7246 6965 6c64 0d0a  n: BufferField..
+00006030: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00006040: 2020 2020 2066 6f72 2064 6174 6120 696e       for data in
+00006050: 2073 656c 662e 6461 7461 6c6f 6164 6572   self.dataloader
+00006060: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00006070: 6620 6c65 6e28 6461 7461 2920 3d3d 2033  f len(data) == 3
+00006080: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006090: 2020 2075 7365 7273 2c20 7365 7173 2c20     users, seqs, 
+000060a0: 706f 6f6c 203d 205b 636f 6c2e 746f 2873  pool = [col.to(s
+000060b0: 656c 662e 6465 7669 6365 2920 666f 7220  elf.device) for 
+000060c0: 636f 6c20 696e 2064 6174 615d 0d0a 2020  col in data]..  
+000060d0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000060e0: 6f72 6573 203d 2073 656c 662e 6d6f 6465  ores = self.mode
+000060f0: 6c2e 7265 636f 6d6d 656e 6428 7573 6572  l.recommend(user
+00006100: 733d 7573 6572 732c 2073 6571 733d 7365  s=users, seqs=se
+00006110: 7173 2c20 706f 6f6c 3d70 6f6f 6c29 0d0a  qs, pool=pool)..
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 7461 7267 6574 7320 3d20 746f 7263 682e  targets = torch.
+00006140: 7a65 726f 735f 6c69 6b65 2873 636f 7265  zeros_like(score
+00006150: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00006160: 2020 2020 7461 7267 6574 735b 3a2c 2030      targets[:, 0
+00006170: 5d2e 6669 6c6c 5f28 3129 0d0a 2020 2020  ].fill_(1)..    
+00006180: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
+00006190: 2864 6174 6129 203d 3d20 343a 0d0a 2020  (data) == 4:..  
+000061a0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+000061b0: 6572 732c 2073 6571 732c 2075 6e73 6565  ers, seqs, unsee
+000061c0: 6e2c 2073 6565 6e20 3d20 6461 7461 0d0a  n, seen = data..
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 7573 6572 7320 3d20 7573 6572 732e 746f  users = users.to
+000061f0: 2873 656c 662e 6465 7669 6365 292e 6461  (self.device).da
+00006200: 7461 0d0a 2020 2020 2020 2020 2020 2020  ta..            
+00006210: 2020 2020 7365 7173 203d 2073 6571 732e      seqs = seqs.
+00006220: 746f 2873 656c 662e 6465 7669 6365 292e  to(self.device).
+00006230: 6461 7461 0d0a 2020 2020 2020 2020 2020  data..          
+00006240: 2020 2020 2020 7363 6f72 6573 203d 2073        scores = s
+00006250: 656c 662e 6d6f 6465 6c2e 7265 636f 6d6d  elf.model.recomm
+00006260: 656e 6428 7573 6572 733d 7573 6572 732c  end(users=users,
+00006270: 2073 6571 733d 7365 7173 290d 0a20 2020   seqs=seqs)..   
+00006280: 2020 2020 2020 2020 2020 2020 2073 6565               see
+00006290: 6e20 3d20 7365 656e 2e74 6f5f 6373 7228  n = seen.to_csr(
+000062a0: 292e 746f 2873 656c 662e 6465 7669 6365  ).to(self.device
+000062b0: 292e 746f 5f64 656e 7365 2829 2e62 6f6f  ).to_dense().boo
+000062c0: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
+000062d0: 2020 2020 2073 636f 7265 735b 7365 656e       scores[seen
+000062e0: 5d20 3d20 2d31 6532 330d 0a20 2020 2020  ] = -1e23..     
+000062f0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00006300: 7473 203d 2075 6e73 6565 6e2e 746f 5f63  ts = unseen.to_c
+00006310: 7372 2829 2e74 6f28 7365 6c66 2e64 6576  sr().to(self.dev
+00006320: 6963 6529 2e74 6f5f 6465 6e73 6528 290d  ice).to_dense().
+00006330: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006340: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00006350: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00006360: 6c65 6d65 6e74 6564 4572 726f 7228 0d0a  lementedError(..
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 6622 5365 7143 6f61 6368 2773      f"SeqCoach's
+00006390: 2060 6576 616c 7561 7465 6020 6578 7065   `evaluate` expe
+000063a0: 6374 7320 7468 6520 6064 6174 6160 2074  cts the `data` t
+000063b0: 6f20 6265 2074 6865 206c 656e 6774 6820  o be the length 
+000063c0: 6f66 2033 206f 7220 342c 2062 7574 207b  of 3 or 4, but {
+000063d0: 6c65 6e28 6461 7461 297d 2072 6563 6569  len(data)} recei
+000063e0: 7665 6420 2e2e 2e22 0d0a 2020 2020 2020  ved ..."..      
+000063f0: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00006400: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006410: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00006420: 2020 2020 2020 2020 2020 7363 6f72 6573            scores
+00006430: 2c20 7461 7267 6574 732c 0d0a 2020 2020  , targets,..    
+00006440: 2020 2020 2020 2020 2020 2020 6e3d 6c65              n=le
+00006450: 6e28 7573 6572 7329 2c20 6d6f 6465 3d22  n(users), mode="
+00006460: 6d65 616e 222c 2070 7265 6669 783d 7072  mean", prefix=pr
+00006470: 6566 6978 2c0d 0a20 2020 2020 2020 2020  efix,..         
+00006480: 2020 2020 2020 2070 6f6f 6c3d 5b27 4849         pool=['HI
+00006490: 5452 4154 4527 2c20 2750 5245 4349 5349  TRATE', 'PRECISI
+000064a0: 4f4e 272c 2027 5245 4341 4c4c 272c 2027  ON', 'RECALL', '
+000064b0: 4e44 4347 272c 2027 4d52 5227 5d0d 0a20  NDCG', 'MRR'].. 
+000064c0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+000064d0: 0d0a 636c 6173 7320 5365 7373 436f 6163  ..class SessCoac
+000064e0: 6828 436f 6163 6829 3a0d 0a0d 0a20 2020  h(Coach):....   
+000064f0: 2064 6566 2065 7661 6c75 6174 6528 7365   def evaluate(se
+00006500: 6c66 2c20 6570 6f63 683a 2069 6e74 2c20  lf, epoch: int, 
+00006510: 7072 6566 6978 3a20 7374 7220 3d20 2776  prefix: str = 'v
+00006520: 616c 6964 2729 3a0d 0a20 2020 2020 2020  alid'):..       
+00006530: 2072 2222 220d 0a20 2020 2020 2020 2045   r"""..        E
+00006540: 7661 6c75 6174 6520 7265 636f 6d6d 656e  valuate recommen
+00006550: 6465 7220 6279 2073 616d 706c 6564 2d62  der by sampled-b
+00006560: 6173 6564 206f 7220 6675 6c6c 2072 616e  ased or full ran
+00006570: 6b69 6e67 0d0a 2020 2020 2020 2020 6163  king..        ac
+00006580: 636f 7264 696e 6720 746f 2074 6865 2066  cording to the f
+00006590: 6f72 6d20 6f66 2060 6461 7461 603a 0d0a  orm of `data`:..
+000065a0: 0d0a 2020 2020 2020 2020 312e 2028 7573  ..        1. (us
+000065b0: 6572 732c 2073 6571 732c 2070 6f6f 6c29  ers, seqs, pool)
+000065c0: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
+000065d0: 7365 7273 3a20 746f 7263 682e 5465 6e73  sers: torch.Tens
+000065e0: 6f72 2c20 2842 2c20 3129 0d0a 2020 2020  or, (B, 1)..    
+000065f0: 2020 2020 2020 2020 7365 7173 3a20 746f          seqs: to
+00006600: 7263 682e 5465 6e73 6f72 2c20 2842 2c20  rch.Tensor, (B, 
+00006610: 5329 0d0a 2020 2020 2020 2020 2020 2020  S)..            
+00006620: 706f 6f6c 3a20 746f 7263 682e 5465 6e73  pool: torch.Tens
+00006630: 6f72 2c20 2842 2c20 3130 3129 0d0a 2020  or, (B, 101)..  
+00006640: 2020 2020 2020 322e 2028 7573 6572 732c        2. (users,
+00006650: 2073 6571 732c 2075 6e73 6565 6e2c 2073   seqs, unseen, s
+00006660: 6565 6e29 3a0d 0a20 2020 2020 2020 2020  een):..         
+00006670: 2020 2075 7365 7273 3a20 4275 6666 6572     users: Buffer
+00006680: 4669 656c 640d 0a20 2020 2020 2020 2020  Field..         
+00006690: 2020 2073 6571 733a 2042 7566 6665 7246     seqs: BufferF
+000066a0: 6965 6c64 0d0a 2020 2020 2020 2020 2020  ield..          
+000066b0: 2020 756e 7365 656e 3a20 4275 6666 6572    unseen: Buffer
+000066c0: 4669 656c 640d 0a20 2020 2020 2020 2020  Field..         
+000066d0: 2020 2073 6565 6e3a 2042 7566 6665 7246     seen: BufferF
+000066e0: 6965 6c64 0d0a 2020 2020 2020 2020 2222  ield..        ""
+000066f0: 220d 0a20 2020 2020 2020 2066 6f72 2064  "..        for d
+00006700: 6174 6120 696e 2073 656c 662e 6461 7461  ata in self.data
+00006710: 6c6f 6164 6572 3a0d 0a20 2020 2020 2020  loader:..       
+00006720: 2020 2020 2069 6620 6c65 6e28 6461 7461       if len(data
+00006730: 2920 3d3d 2033 3a0d 0a20 2020 2020 2020  ) == 3:..       
+00006740: 2020 2020 2020 2020 2073 6573 7365 732c           sesses,
+00006750: 2073 6571 732c 2070 6f6f 6c20 3d20 5b63   seqs, pool = [c
+00006760: 6f6c 2e74 6f28 7365 6c66 2e64 6576 6963  ol.to(self.devic
+00006770: 6529 2066 6f72 2063 6f6c 2069 6e20 6461  e) for col in da
+00006780: 7461 5d0d 0a20 2020 2020 2020 2020 2020  ta]..           
+00006790: 2020 2020 2073 636f 7265 7320 3d20 7365       scores = se
+000067a0: 6c66 2e6d 6f64 656c 2e72 6563 6f6d 6d65  lf.model.recomme
+000067b0: 6e64 2873 6573 7365 733d 7365 7373 6573  nd(sesses=sesses
+000067c0: 2c20 7365 7173 3d73 6571 732c 2070 6f6f  , seqs=seqs, poo
+000067d0: 6c3d 706f 6f6c 290d 0a20 2020 2020 2020  l=pool)..       
+000067e0: 2020 2020 2020 2020 2074 6172 6765 7473           targets
+000067f0: 203d 2074 6f72 6368 2e7a 6572 6f73 5f6c   = torch.zeros_l
+00006800: 696b 6528 7363 6f72 6573 290d 0a20 2020  ike(scores)..   
+00006810: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00006820: 6765 7473 5b3a 2c20 305d 2e66 696c 6c5f  gets[:, 0].fill_
+00006830: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
+00006840: 2065 6c69 6620 6c65 6e28 6461 7461 2920   elif len(data) 
+00006850: 3d3d 2034 3a0d 0a20 2020 2020 2020 2020  == 4:..         
+00006860: 2020 2020 2020 2073 6573 7365 732c 2073         sesses, s
+00006870: 6571 732c 2075 6e73 6565 6e2c 2073 6565  eqs, unseen, see
+00006880: 6e20 3d20 6461 7461 0d0a 2020 2020 2020  n = data..      
+00006890: 2020 2020 2020 2020 2020 7365 7373 6573            sesses
+000068a0: 203d 2073 6573 7365 732e 6461 7461 0d0a   = sesses.data..
+000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068c0: 7365 7173 203d 2073 6571 732e 746f 2873  seqs = seqs.to(s
+000068d0: 656c 662e 6465 7669 6365 292e 6461 7461  elf.device).data
+000068e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000068f0: 2020 7363 6f72 6573 203d 2073 656c 662e    scores = self.
+00006900: 6d6f 6465 6c2e 7265 636f 6d6d 656e 6428  model.recommend(
+00006910: 7365 7373 6573 3d73 6573 7365 732c 2073  sesses=sesses, s
+00006920: 6571 733d 7365 7173 290d 0a20 2020 2020  eqs=seqs)..     
+00006930: 2020 2020 2020 2020 2020 2023 2044 6f6e             # Don
+00006940: 2774 2072 656d 6f76 6520 7365 656e 7320  't remove seens 
+00006950: 666f 7220 7365 7373 696f 6e0d 0a20 2020  for session..   
+00006960: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00006970: 6765 7473 203d 2075 6e73 6565 6e2e 746f  gets = unseen.to
+00006980: 5f63 7372 2829 2e74 6f28 7365 6c66 2e64  _csr().to(self.d
+00006990: 6576 6963 6529 2e74 6f5f 6465 6e73 6528  evice).to_dense(
+000069a0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000069b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000069c0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+000069d0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+000069e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000069f0: 2020 2020 2020 6622 5365 7373 436f 6163        f"SessCoac
+00006a00: 6827 7320 6065 7661 6c75 6174 6560 2065  h's `evaluate` e
+00006a10: 7870 6563 7473 2074 6865 2060 6461 7461  xpects the `data
+00006a20: 6020 746f 2062 6520 7468 6520 6c65 6e67  ` to be the leng
+00006a30: 7468 206f 6620 3320 6f72 2034 2c20 6275  th of 3 or 4, bu
+00006a40: 7420 7b6c 656e 2864 6174 6129 7d20 7265  t {len(data)} re
+00006a50: 6365 6976 6564 202e 2e2e 220d 0a20 2020  ceived ..."..   
+00006a60: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00006a70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00006a80: 6c66 2e6d 6f6e 6974 6f72 280d 0a20 2020  lf.monitor(..   
+00006a90: 2020 2020 2020 2020 2020 2020 2073 636f               sco
+00006aa0: 7265 732c 2074 6172 6765 7473 2c0d 0a20  res, targets,.. 
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00006ac0: 3d6c 656e 2873 6573 7365 7329 2c20 6d6f  =len(sesses), mo
+00006ad0: 6465 3d22 6d65 616e 222c 2070 7265 6669  de="mean", prefi
+00006ae0: 783d 7072 6566 6978 2c0d 0a20 2020 2020  x=prefix,..     
+00006af0: 2020 2020 2020 2020 2020 2070 6f6f 6c3d             pool=
+00006b00: 5b27 4849 5452 4154 4527 2c20 2750 5245  ['HITRATE', 'PRE
+00006b10: 4349 5349 4f4e 272c 2027 5245 4341 4c4c  CISION', 'RECALL
+00006b20: 272c 2027 4e44 4347 272c 2027 4d52 5227  ', 'NDCG', 'MRR'
+00006b30: 5d0d 0a20 2020 2020 2020 2020 2020 2029  ]..            )
+00006b40: 0d0a 0d0a 0d0a 0d0a 636c 6173 7320 4164  ........class Ad
+00006b50: 6170 7465 723a 0d0a 2020 2020 7222 2222  apter:..    r"""
+00006b60: 0d0a 2020 2020 5061 7261 6d73 2074 756e  ..    Params tun
+00006b70: 6572 2e0d 0a0d 0a20 2020 2046 6c6f 7773  er.....    Flows
+00006b80: 3a0d 0a20 2020 202d 2d2d 2d2d 2d0d 0a20  :..    ------.. 
+00006b90: 2020 2031 2e20 636f 6d70 696c 653a 2063     1. compile: c
+00006ba0: 6f6e 6669 6775 7265 2074 6865 2063 6f6d  onfigure the com
+00006bb0: 6d61 6e64 2c20 656e 7669 726f 6e6d 656e  mand, environmen
+00006bc0: 7473 2c20 616e 6420 7061 7261 6d65 7465  ts, and paramete
+00006bd0: 7273 2066 6f72 2074 7261 696e 696e 672e  rs for training.
+00006be0: 0d0a 2020 2020 322e 2061 6c6c 6f63 6174  ..    2. allocat
+00006bf0: 6520 6465 7669 6365 7320 666f 7220 7661  e devices for va
+00006c00: 7269 6f75 7320 7061 7261 6d65 7465 7273  rious parameters
+00006c10: 3a0d 0a20 2020 2020 2020 202d 2072 6567  :..        - reg
+00006c20: 6973 7465 7220 7468 6520 4944 2c20 6c6f  ister the ID, lo
+00006c30: 6720 7061 7468 2c20 616e 6420 6465 7669  g path, and devi
+00006c40: 6365 2066 6972 7374 0d0a 2020 2020 2020  ce first..      
+00006c50: 2020 2d20 6578 6563 7574 6520 7468 6520    - execute the 
+00006c60: 636f 6d6d 616e 640d 0a20 2020 2020 2020  command..       
+00006c70: 202d 2063 6f6c 6c65 6374 2069 6e66 6f72   - collect infor
+00006c80: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
+00006c90: 6c6f 6720 7061 7468 2061 6e64 206f 7574  log path and out
+00006ca0: 7075 7420 746f 2054 656e 736f 7242 6f61  put to TensorBoa
+00006cb0: 7264 0d0a 2020 2020 2020 2020 2d20 7361  rd..        - sa
+00006cc0: 7665 2074 6865 2063 6865 636b 706f 696e  ve the checkpoin
+00006cd0: 740d 0a20 2020 2020 2020 202d 2072 656c  t..        - rel
+00006ce0: 6561 7365 2074 6865 2063 6f72 7265 7370  ease the corresp
+00006cf0: 6f6e 6469 6e67 2064 6576 6963 650d 0a0d  onding device...
+00006d00: 0a20 2020 2045 7861 6d70 6c65 733a 0d0a  .    Examples:..
+00006d10: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0d 0a20      ---------.. 
+00006d20: 2020 203e 3e3e 2063 6667 203d 207b 2763     >>> cfg = {'c
+00006d30: 6f6d 6d61 6e64 273a 2027 7079 7468 6f6e  ommand': 'python
+00006d40: 2078 7878 2e70 7927 2c20 2770 6172 616d   xxx.py', 'param
+00006d50: 7327 3a20 7b27 6f70 7469 6d69 7a65 7227  s': {'optimizer'
+00006d60: 3a20 5b27 7367 6427 2c20 2761 6461 6d27  : ['sgd', 'adam'
+00006d70: 5d7d 7d0d 0a20 2020 203e 3e3e 2074 756e  ]}}..    >>> tun
+00006d80: 6572 203d 2041 6461 7074 6572 2829 0d0a  er = Adapter()..
+00006d90: 2020 2020 3e3e 3e20 7475 6e65 722e 636f      >>> tuner.co
+00006da0: 6d70 696c 6528 6366 6729 0d0a 2020 2020  mpile(cfg)..    
+00006db0: 3e3e 3e20 7475 6e65 722e 6669 7428 290d  >>> tuner.fit().
+00006dc0: 0a20 2020 2022 2222 0d0a 0d0a 2020 2020  .    """....    
+00006dd0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00006de0: 6629 202d 3e20 4e6f 6e65 3a0d 0a20 2020  f) -> None:..   
+00006df0: 2020 2020 2073 656c 662e 7061 7261 6d73       self.params
+00006e00: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
+00006e10: 656c 662e 7661 6c75 6573 203d 205b 5d0d  elf.values = [].
+00006e20: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+00006e30: 7669 6365 7320 3d20 7475 706c 6528 290d  vices = tuple().
+00006e40: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00006e50: 0d0a 2020 2020 6465 6620 434f 4d4d 414e  ..    def COMMAN
+00006e60: 4428 7365 6c66 293a 0d0a 2020 2020 2020  D(self):..      
+00006e70: 2020 7265 7475 726e 2073 656c 662e 6366    return self.cf
+00006e80: 672e 434f 4d4d 414e 440d 0a0d 0a20 2020  g.COMMAND....   
+00006e90: 2064 6566 2072 6567 6973 7465 7228 7365   def register(se
+00006ea0: 6c66 2c20 6465 7669 6365 3a20 7374 7229  lf, device: str)
+00006eb0: 202d 3e20 5475 706c 655b 7374 722c 2073   -> Tuple[str, s
+00006ec0: 7472 5d3a 0d0a 2020 2020 2020 2020 7365  tr]:..        se
+00006ed0: 6c66 2e63 6667 2e45 4e56 535b 2769 6427  lf.cfg.ENVS['id'
+00006ee0: 5d20 3d20 7469 6d65 2e73 7472 6674 696d  ] = time.strftim
+00006ef0: 6528 5449 4d45 290d 0a20 2020 2020 2020  e(TIME)..       
+00006f00: 2073 656c 662e 6366 672e 454e 5653 5b27   self.cfg.ENVS['
+00006f10: 6465 7669 6365 275d 203d 2064 6576 6963  device'] = devic
+00006f20: 650d 0a20 2020 2020 2020 2063 6f6d 6d61  e..        comma
+00006f30: 6e64 203d 2073 656c 662e 434f 4d4d 414e  nd = self.COMMAN
+00006f40: 4420 2b20 7365 6c66 2e67 6574 5f6f 7074  D + self.get_opt
+00006f50: 696f 6e28 2769 6427 2c20 7365 6c66 2e63  ion('id', self.c
+00006f60: 6667 2e45 4e56 532e 6964 290d 0a20 2020  fg.ENVS.id)..   
+00006f70: 2020 2020 2063 6f6d 6d61 6e64 202b 3d20       command += 
+00006f80: 7365 6c66 2e67 6574 5f6f 7074 696f 6e28  self.get_option(
+00006f90: 2764 6576 6963 6527 2c20 7365 6c66 2e63  'device', self.c
+00006fa0: 6667 2e45 4e56 532e 6465 7669 6365 290d  fg.ENVS.device).
+00006fb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00006fc0: 636f 6d6d 616e 642c 2073 656c 662e 6366  command, self.cf
+00006fd0: 672e 454e 5653 2e69 642c 2073 656c 662e  g.ENVS.id, self.
+00006fe0: 6366 672e 4c4f 475f 5041 5448 2e66 6f72  cfg.LOG_PATH.for
+00006ff0: 6d61 7428 2a2a 7365 6c66 2e63 6667 2e45  mat(**self.cfg.E
+00007000: 4e56 5329 0d0a 0d0a 2020 2020 4074 696d  NVS)....    @tim
+00007010: 656d 6574 6572 0d0a 2020 2020 6465 6620  emeter..    def 
+00007020: 636f 6d70 696c 6528 7365 6c66 2c20 6366  compile(self, cf
+00007030: 673a 2043 6f6e 6669 6729 202d 3e20 4e6f  g: Config) -> No
+00007040: 6e65 3a0d 0a20 2020 2020 2020 2072 2222  ne:..        r""
+00007050: 220d 0a20 2020 2020 2020 2043 6f6e 6669  "..        Confi
+00007060: 6775 7265 2074 6865 2063 6f6d 6d61 6e64  gure the command
+00007070: 2c20 656e 7669 726f 6e6d 656e 7473 2c20  , environments, 
+00007080: 616e 6420 7061 7261 6d65 7465 7273 2066  and parameters f
+00007090: 6f72 2074 7261 696e 696e 672e 0d0a 0d0a  or training.....
+000070a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000070b0: 7273 3a0d 0a20 2020 2020 2020 202d 2d2d  rs:..        ---
+000070c0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+000070d0: 2020 6366 6720 3a20 436f 6e66 6967 0d0a    cfg : Config..
+000070e0: 2020 2020 2020 2020 2020 2020 416e 206f              An o
+000070f0: 626a 6563 7420 7468 6174 2063 6f6e 7461  bject that conta
+00007100: 696e 7320 7468 6520 636f 6d6d 616e 642c  ins the command,
+00007110: 2065 6e76 6972 6f6e 6d65 6e74 732c 2070   environments, p
+00007120: 6172 616d 6574 6572 732c 2061 6e64 2064  arameters, and d
+00007130: 6566 6175 6c74 732e 0d0a 0d0a 2020 2020  efaults.....    
+00007140: 2020 2020 466c 6f77 733a 0d0a 2020 2020      Flows:..    
+00007150: 2020 2020 2d2d 2d2d 2d2d 0d0a 2020 2020      ------..    
+00007160: 2020 2020 312e 2041 6464 2065 6e76 6972      1. Add envir
+00007170: 6f6e 6d65 6e74 616c 2070 6172 616d 6574  onmental paramet
+00007180: 6572 7320 746f 2074 6865 2062 6173 6963  ers to the basic
+00007190: 2060 636f 6d6d 616e 6460 2e0d 0a20 2020   `command`...   
+000071a0: 2020 2020 2032 2e20 5265 6769 7374 6572       2. Register
+000071b0: 2061 6c6c 2061 7661 696c 6162 6c65 2064   all available d
+000071c0: 6576 6963 6573 2e0d 0a20 2020 2020 2020  evices...       
+000071d0: 2033 2e20 436f 6e76 6572 7420 616c 6c20   3. Convert all 
+000071e0: 7061 7261 6d65 7465 7273 2066 726f 6d20  parameters from 
+000071f0: 6063 6667 2e50 4152 414d 5360 2e0d 0a20  `cfg.PARAMS`... 
+00007200: 2020 2020 2020 2034 2e20 436f 6e76 6572         4. Conver
+00007210: 7420 616c 6c20 6465 6661 756c 7473 2066  t all defaults f
+00007220: 726f 6d20 6063 6667 2e44 4546 4155 4c54  rom `cfg.DEFAULT
+00007230: 5360 2e0d 0a0d 0a20 2020 2020 2020 2052  S`.....        R
+00007240: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00007250: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
+00007260: 2020 204e 6f6e 650d 0a20 2020 2020 2020     None..       
+00007270: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00007280: 6c66 2e63 6667 203d 2063 6667 0d0a 2020  lf.cfg = cfg..  
+00007290: 2020 2020 2020 7069 6563 6520 3d20 225c        piece = "\
+000072a0: 747b 6b65 797d 3a20 7b76 616c 737d 205c  t{key}: {vals} \
+000072b0: 6e22 0d0a 2020 2020 2020 2020 656e 7673  n"..        envs
+000072c0: 2c20 7061 7261 6d73 2c20 6465 6661 756c  , params, defaul
+000072d0: 7473 203d 2022 222c 2022 222c 2022 220d  ts = "", "", "".
+000072e0: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
+000072f0: 2c20 7661 6c20 696e 2073 656c 662e 6366  , val in self.cf
+00007300: 672e 454e 5653 2e69 7465 6d73 2829 3a0d  g.ENVS.items():.
+00007310: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007320: 6b65 7920 3d3d 2027 6465 7669 6365 273a  key == 'device':
+00007330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007340: 2020 7365 6c66 2e64 6576 6963 6573 203d    self.devices =
+00007350: 2074 7570 6c65 2876 616c 2e73 706c 6974   tuple(val.split
+00007360: 2827 2c27 2929 0d0a 2020 2020 2020 2020  (','))..        
+00007370: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00007380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007390: 6366 672e 434f 4d4d 414e 4420 2b3d 2073  cfg.COMMAND += s
+000073a0: 656c 662e 6765 745f 6f70 7469 6f6e 286b  elf.get_option(k
+000073b0: 6579 2c20 7661 6c29 0d0a 2020 2020 2020  ey, val)..      
+000073c0: 2020 2020 2020 656e 7673 202b 3d20 7069        envs += pi
+000073d0: 6563 652e 666f 726d 6174 286b 6579 3d6b  ece.format(key=k
+000073e0: 6579 2c20 7661 6c73 3d76 616c 290d 0a20  ey, vals=val).. 
+000073f0: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00007400: 7661 6c73 2069 6e20 7365 6c66 2e63 6667  vals in self.cfg
+00007410: 2e50 4152 414d 532e 6974 656d 7328 293a  .PARAMS.items():
+00007420: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00007430: 2069 7369 6e73 7461 6e63 6528 7661 6c73   isinstance(vals
+00007440: 2c20 2873 7472 2c20 696e 742c 2066 6c6f  , (str, int, flo
+00007450: 6174 2929 3a0d 0a20 2020 2020 2020 2020  at)):..         
+00007460: 2020 2020 2020 2076 616c 7320 3d20 5b76         vals = [v
+00007470: 616c 735d 0d0a 2020 2020 2020 2020 2020  als]..          
+00007480: 2020 7365 6c66 2e64 6570 6c6f 795f 7061    self.deploy_pa
+00007490: 7261 6d73 286b 6579 2c20 7661 6c73 290d  rams(key, vals).
+000074a0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000074b0: 616d 7320 2b3d 2070 6965 6365 2e66 6f72  ams += piece.for
+000074c0: 6d61 7428 6b65 793d 6b65 792c 2076 616c  mat(key=key, val
+000074d0: 733d 7661 6c73 290d 0a20 2020 2020 2020  s=vals)..       
+000074e0: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+000074f0: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
+00007500: 5453 2e69 7465 6d73 2829 3a0d 0a20 2020  TS.items():..   
+00007510: 2020 2020 2020 2020 2073 656c 662e 6366           self.cf
+00007520: 672e 4445 4641 554c 5453 5b6b 6579 5d20  g.DEFAULTS[key] 
+00007530: 3d20 7661 6c0d 0a20 2020 2020 2020 2020  = val..         
+00007540: 2020 2064 6566 6175 6c74 7320 2b3d 2070     defaults += p
+00007550: 6965 6365 2e66 6f72 6d61 7428 6b65 793d  iece.format(key=
+00007560: 6b65 792c 2076 616c 733d 7661 6c29 0d0a  key, vals=val)..
+00007570: 0d0a 2020 2020 2020 2020 6366 675f 696e  ..        cfg_in
+00007580: 666f 7320 3d20 6622 636f 6d6d 616e 643a  fos = f"command:
+00007590: 207b 7365 6c66 2e63 6667 2e43 4f4d 4d41   {self.cfg.COMMA
+000075a0: 4e44 7d20 5c6e 656e 7673 3a20 5c6e 7b65  ND} \nenvs: \n{e
+000075b0: 6e76 737d 7061 7261 6d73 3a20 5c6e 7b70  nvs}params: \n{p
+000075c0: 6172 616d 737d 6465 6661 756c 7473 3a20  arams}defaults: 
+000075d0: 5c6e 7b64 6566 6175 6c74 737d 220d 0a20  \n{defaults}".. 
+000075e0: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
+000075f0: 7228 6622 5c30 3333 5b30 3b33 313b 3437  r(f"\033[0;31;47
+00007600: 6d7b 6366 675f 696e 666f 737d 5c30 3333  m{cfg_infos}\033
+00007610: 5b30 6d22 290d 0a0d 0a20 2020 2064 6566  [0m")....    def
+00007620: 2064 6570 6c6f 795f 7061 7261 6d73 2873   deploy_params(s
+00007630: 656c 662c 206b 6579 3a20 7374 722c 2076  elf, key: str, v
+00007640: 616c 733a 2049 7465 7261 626c 6529 3a0d  als: Iterable):.
+00007650: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+00007660: 7261 6d73 2e61 7070 656e 6428 6b65 7929  rams.append(key)
+00007670: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
+00007680: 616c 7565 732e 6170 7065 6e64 2876 616c  alues.append(val
+00007690: 7329 0d0a 0d0a 2020 2020 4073 7461 7469  s)....    @stati
+000076a0: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
+000076b0: 2067 6574 5f6f 7074 696f 6e28 6b65 793a   get_option(key:
+000076c0: 2073 7472 2c20 7661 6c3a 2041 6e79 293a   str, val: Any):
+000076d0: 0d0a 2020 2020 2020 2020 7222 2222 0d0a  ..        r"""..
+000076e0: 2020 2020 2020 2020 436f 6e76 6572 7420          Convert 
+000076f0: 286b 6579 2c20 7661 6c29 2074 6f20 272d  (key, val) to '-
+00007700: 2d6b 6579 3d76 616c 272e 0d0a 0d0a 2020  -key=val'.....  
+00007710: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00007720: 3a0d 0a20 2020 2020 2020 202d 2d2d 2d2d  :..        -----
+00007730: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00007740: 6b65 7920 3a20 7374 720d 0a20 2020 2020  key : str..     
+00007750: 2020 2020 2020 2054 6865 206b 6579 206f         The key o
+00007760: 6620 7468 6520 7061 7261 6d65 7465 722e  f the parameter.
+00007770: 0d0a 2020 2020 2020 2020 7661 6c20 3a20  ..        val : 
+00007780: 416e 790d 0a20 2020 2020 2020 2020 2020  Any..           
+00007790: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
+000077a0: 6520 7061 7261 6d65 7465 722e 0d0a 0d0a  e parameter.....
+000077b0: 2020 2020 2020 2020 4e6f 7465 733a 0d0a          Notes:..
+000077c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
+000077d0: 2020 2020 2020 2020 416c 6c20 275f 2720          All '_' 
+000077e0: 696e 2060 6b65 7960 2077 696c 6c20 6265  in `key` will be
+000077f0: 2072 6570 6c61 6365 6420 6279 2027 2d27   replaced by '-'
+00007800: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00007810: 7572 6e73 3a0d 0a20 2020 2020 2020 202d  urns:..        -
+00007820: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00007830: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00007840: 2020 5468 6520 7061 7261 6d65 7465 7220    The parameter 
+00007850: 7769 7468 2066 6f72 6d61 7420 272d 2d6b  with format '--k
+00007860: 6579 3d76 616c 272e 0d0a 0d0a 2020 2020  ey=val'.....    
+00007870: 2020 2020 4578 616d 706c 6573 3a0d 0a20      Examples:.. 
+00007880: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00007890: 0d0a 2020 2020 2020 2020 3e3e 3e20 4164  ..        >>> Ad
+000078a0: 6170 7465 722e 6765 745f 6f70 7469 6f6e  apter.get_option
+000078b0: 2827 6c72 272c 2027 3165 2d33 2729 0d0a  ('lr', '1e-3')..
+000078c0: 2020 2020 2020 2020 272d 2d6c 723d 3165          '--lr=1e
+000078d0: 2d33 270d 0a20 2020 2020 2020 203e 3e3e  -3'..        >>>
+000078e0: 2041 6461 7074 6572 2e67 6574 5f6f 7074   Adapter.get_opt
+000078f0: 696f 6e28 276c 6561 726e 696e 675f 7261  ion('learning_ra
+00007900: 7465 272c 2027 3165 2d33 2729 0d0a 2020  te', '1e-3')..  
+00007910: 2020 2020 2020 272d 2d6c 6561 726e 696e        '--learnin
+00007920: 672d 7261 7465 3d31 652d 3327 0d0a 2020  g-rate=1e-3'..  
+00007930: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00007940: 2020 2072 6574 7572 6e20 6622 202d 2d7b     return f" --{
+00007950: 6b65 792e 7265 706c 6163 6528 275f 272c  key.replace('_',
+00007960: 2027 2d27 297d 3d7b 7661 6c7d 220d 0a0d   '-')}={val}"...
+00007970: 0a20 2020 2064 6566 206c 6f61 645f 6265  .    def load_be
+00007980: 7374 2873 656c 662c 206c 6f67 5061 7468  st(self, logPath
+00007990: 3a20 7374 7229 3a0d 0a20 2020 2020 2020  : str):..       
+000079a0: 2022 2222 4c6f 6164 2062 6573 742e 7069   """Load best.pi
+000079b0: 636b 6c65 2066 726f 6d20 6c6f 6750 6174  ckle from logPat
+000079c0: 6820 6f66 2063 6f72 7265 7370 6f6e 6469  h of correspondi
+000079d0: 6e67 2e22 2222 0d0a 2020 2020 2020 2020  ng."""..        
+000079e0: 6669 6c65 5f20 3d20 6f73 2e70 6174 682e  file_ = os.path.
+000079f0: 6a6f 696e 286c 6f67 5061 7468 2c20 7365  join(logPath, se
+00007a00: 6c66 2e63 6667 2e44 4154 415f 4449 522c  lf.cfg.DATA_DIR,
+00007a10: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
+00007a20: 525f 4245 5354 5f46 494c 454e 414d 4529  R_BEST_FILENAME)
+00007a30: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00007a40: 2069 6d70 6f72 745f 7069 636b 6c65 2866   import_pickle(f
+00007a50: 696c 655f 290d 0a0d 0a20 2020 2064 6566  ile_)....    def
+00007a60: 2077 7269 7465 2873 656c 662c 2069 645f   write(self, id_
+00007a70: 3a20 7374 722c 206c 6f67 5061 7468 3a20  : str, logPath: 
+00007a80: 7374 722c 2070 6172 616d 733a 2044 6963  str, params: Dic
+00007a90: 7429 3a0d 0a20 2020 2020 2020 2072 2222  t):..        r""
+00007aa0: 220d 0a20 2020 2020 2020 2057 7269 7465  "..        Write
+00007ab0: 2065 7870 6572 696d 656e 7420 7265 7375   experiment resu
+00007ac0: 6c74 7320 746f 2074 656e 736f 7262 6f61  lts to tensorboa
+00007ad0: 7264 2e0d 0a0d 0a20 2020 2020 2020 2050  rd.....        P
+00007ae0: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00007af0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d      -----------.
+00007b00: 0a20 2020 2020 2020 2069 645f 3a20 7374  .        id_: st
+00007b10: 720d 0a20 2020 2020 2020 2020 2020 2045  r..            E
+00007b20: 7870 6572 696d 656e 7420 4944 2e0d 0a20  xperiment ID... 
+00007b30: 2020 2020 2020 206c 6f67 5061 7468 3a20         logPath: 
+00007b40: 7374 720d 0a20 2020 2020 2020 2020 2020  str..           
+00007b50: 2050 6174 6820 746f 2074 6865 2065 7870   Path to the exp
+00007b60: 6572 696d 656e 7420 6c6f 6773 2e0d 0a20  eriment logs... 
+00007b70: 2020 2020 2020 2070 6172 616d 733a 2044         params: D
+00007b80: 6963 740d 0a20 2020 2020 2020 2020 2020  ict..           
+00007b90: 2043 6f6e 6669 6775 7261 7469 6f6e 2070   Configuration p
+00007ba0: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
+00007bb0: 2065 7870 6572 696d 656e 742e 0d0a 0d0a   experiment.....
+00007bc0: 2020 2020 2020 2020 466c 6f77 733a 0d0a          Flows:..
+00007bd0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0d0a          ------..
+00007be0: 2020 2020 2020 2020 312e 204c 6f61 6420          1. Load 
+00007bf0: 7468 6520 6265 7374 2064 6174 6120 6672  the best data fr
+00007c00: 6f6d 2060 6c6f 6750 6174 6860 2e0d 0a20  om `logPath`... 
+00007c10: 2020 2020 2020 2032 2e20 5772 6974 6520         2. Write 
+00007c20: 7468 6520 6265 7374 2064 6174 6120 746f  the best data to
+00007c30: 2074 656e 736f 7262 6f61 7264 2077 6974   tensorboard wit
+00007c40: 6820 6070 6172 616d 7360 2e0d 0a0d 0a20  h `params`..... 
+00007c50: 2020 2020 2020 204e 6f74 6573 3a0d 0a20         Notes:.. 
+00007c60: 2020 2020 2020 202d 2d2d 2d2d 2d0d 0a20         ------.. 
+00007c70: 2020 2020 2020 2049 6620 796f 7520 6669         If you fi
+00007c80: 6e64 2060 2d31 6020 6170 7065 6172 696e  nd `-1` appearin
+00007c90: 6720 696e 2074 6865 2074 656e 736f 7262  g in the tensorb
+00007ca0: 6f61 7264 2c0d 0a20 2020 2020 2020 2069  oard,..        i
+00007cb0: 7420 636f 756c 6420 6d65 616e 2074 6861  t could mean tha
+00007cc0: 7420 7468 6520 6461 7461 2069 7320 6f66  t the data is of
+00007cd0: 2060 7374 7260 2074 7970 652c 0d0a 2020   `str` type,..  
+00007ce0: 2020 2020 2020 7768 6963 6820 7769 6c6c        which will
+00007cf0: 2063 6175 7365 2061 6e20 6572 726f 7220   cause an error 
+00007d00: 6966 2069 7420 6973 2073 656e 7420 746f  if it is sent to
+00007d10: 2074 656e 736f 7262 6f61 7264 2064 6972   tensorboard dir
+00007d20: 6563 746c 7921 0d0a 2020 2020 2020 2020  ectly!..        
+00007d30: 2222 220d 0a20 2020 2020 2020 2074 7279  """..        try
+00007d40: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+00007d50: 6174 6120 3d20 7365 6c66 2e6c 6f61 645f  ata = self.load_
+00007d60: 6265 7374 286c 6f67 5061 7468 290d 0a20  best(logPath).. 
+00007d70: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+00007d80: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+00007d90: 656c 662e 6366 672e 434f 5245 5f4c 4f47  elf.cfg.CORE_LOG
+00007da0: 5f50 4154 482c 2069 645f 290d 0a20 2020  _PATH, id_)..   
+00007db0: 2020 2020 2020 2020 2077 6974 6820 5375           with Su
+00007dc0: 6d6d 6172 7957 7269 7465 7228 6c6f 675f  mmaryWriter(log_
+00007dd0: 6469 723d 7061 7468 2920 6173 2077 7269  dir=path) as wri
+00007de0: 7465 723a 0d0a 2020 2020 2020 2020 2020  ter:..          
+00007df0: 2020 2020 2020 6d65 7472 6963 7320 3d20        metrics = 
+00007e00: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
+00007e10: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
+00007e20: 6978 2c20 6265 7374 2069 6e20 6461 7461  ix, best in data
+00007e30: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00007e50: 6f72 206d 6574 7269 632c 2076 616c 2069  or metric, val i
+00007e60: 6e20 6265 7374 2e69 7465 6d73 2829 3a0d  n best.items():.
+00007e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007e80: 2020 2020 2020 2020 2076 616c 203d 2076           val = v
+00007e90: 616c 2069 6620 6973 696e 7374 616e 6365  al if isinstance
+00007ea0: 2876 616c 2c20 2869 6e74 2c20 666c 6f61  (val, (int, floa
+00007eb0: 7429 2920 656c 7365 202d 310d 0a20 2020  t)) else -1..   
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 206d 6574 7269 6373 5b27 2f27       metrics['/'
+00007ee0: 2e6a 6f69 6e28 5b70 7265 6669 782c 206d  .join([prefix, m
+00007ef0: 6574 7269 635d 295d 203d 2076 616c 0d0a  etric])] = val..
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 7772 6974 6572 2e61 6464 5f68 7061 7261  writer.add_hpara
+00007f20: 6d73 280d 0a20 2020 2020 2020 2020 2020  ms(..           
+00007f30: 2020 2020 2020 2020 2070 6172 616d 732c           params,
+00007f40: 206d 6574 7269 6373 2c0d 0a20 2020 2020   metrics,..     
+00007f50: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00007f60: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00007f70: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
+00007f80: 2020 2020 2069 6e66 6f4c 6f67 6765 7228       infoLogger(
+00007f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007fa0: 2020 6622 5c30 3333 5b30 3b33 313b 3437    f"\033[0;31;47
+00007fb0: 6d5b 4164 6170 7465 725d 203e 3e3e 2055  m[Adapter] >>> U
+00007fc0: 6e6b 6e6f 776e 2065 7272 6f72 7320 6861  nknown errors ha
+00007fd0: 7070 656e 2e20 5468 6973 2069 7320 6d61  ppen. This is ma
+00007fe0: 696e 6c79 2064 7565 2074 6f20 6162 6e6f  inly due to abno
+00007ff0: 726d 616c 2065 7869 7473 206f 6620 6368  rmal exits of ch
+00008000: 696c 6420 7072 6f63 6573 7365 732e 5c30  ild processes.\0
+00008010: 3333 5b30 6d22 0d0a 2020 2020 2020 2020  33[0m"..        
+00008020: 2020 2020 290d 0a0d 0a20 2020 2064 6566      )....    def
+00008030: 2065 6163 685f 6772 6964 2873 656c 6629   each_grid(self)
+00008040: 3a0d 0a20 2020 2020 2020 2022 2222 4772  :..        """Gr
+00008050: 6964 2073 6561 7263 6820 666f 7220 6561  id search for ea
+00008060: 6368 206b 696e 6420 6f66 2070 6172 616d  ch kind of param
+00008070: 2e22 2222 0d0a 2020 2020 2020 2020 666f  ."""..        fo
+00008080: 7220 6b65 792c 2076 616c 7320 696e 207a  r key, vals in z
+00008090: 6970 2873 656c 662e 7061 7261 6d73 2c20  ip(self.params, 
+000080a0: 7365 6c66 2e76 616c 7565 7329 3a0d 0a20  self.values):.. 
+000080b0: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
+000080c0: 616c 2069 6e20 7661 6c73 3a0d 0a20 2020  al in vals:..   
+000080d0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
+000080e0: 6c64 2073 656c 662e 6366 672e 4445 4641  ld self.cfg.DEFA
+000080f0: 554c 5453 207c 207b 6b65 793a 2076 616c  ULTS | {key: val
+00008100: 7d0d 0a0d 0a20 2020 2064 6566 2070 726f  }....    def pro
+00008110: 6475 6374 5f67 7269 6428 7365 6c66 293a  duct_grid(self):
+00008120: 0d0a 2020 2020 2020 2020 2222 2247 7269  ..        """Gri
+00008130: 6420 7365 6172 6368 2061 6372 6f73 7320  d search across 
+00008140: 616c 6c20 636f 6d62 696e 6174 696f 6e20  all combination 
+00008150: 6f66 2070 6172 616d 7322 2222 0d0a 2020  of params"""..  
+00008160: 2020 2020 2020 666f 7220 7661 6c73 2069        for vals i
+00008170: 6e20 7072 6f64 7563 7428 2a73 656c 662e  n product(*self.
+00008180: 7661 6c75 6573 293a 0d0a 2020 2020 2020  values):..      
+00008190: 2020 2020 2020 7969 656c 6420 7365 6c66        yield self
+000081a0: 2e63 6667 2e44 4546 4155 4c54 5320 7c20  .cfg.DEFAULTS | 
+000081b0: 7b6f 7074 696f 6e3a 7661 6c20 666f 7220  {option:val for 
+000081c0: 6f70 7469 6f6e 2c20 7661 6c20 696e 207a  option, val in z
+000081d0: 6970 2873 656c 662e 7061 7261 6d73 2c20  ip(self.params, 
+000081e0: 7661 6c73 297d 0d0a 0d0a 2020 2020 6465  vals)}....    de
+000081f0: 6620 7361 7665 5f63 6865 636b 706f 696e  f save_checkpoin
+00008200: 7428 7365 6c66 2c20 736f 7572 6365 3a20  t(self, source: 
+00008210: 4c69 7374 2920 2d3e 204e 6f6e 653a 0d0a  List) -> None:..
+00008220: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
+00008230: 7468 6520 7265 7374 206f 6620 7061 7261  the rest of para
+00008240: 6d73 2e22 2222 0d0a 2020 2020 2020 2020  ms."""..        
+00008250: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00008260: 6f69 6e28 7365 6c66 2e63 6667 2e43 4f52  oin(self.cfg.COR
+00008270: 455f 4348 4543 4b50 4f49 4e54 5f50 4154  E_CHECKPOINT_PAT
+00008280: 482c 2073 656c 662e 6366 672e 4348 4543  H, self.cfg.CHEC
+00008290: 4b50 4f49 4e54 5f46 494c 454e 414d 4529  KPOINT_FILENAME)
+000082a0: 0d0a 2020 2020 2020 2020 6368 6563 6b70  ..        checkp
+000082b0: 6f69 6e74 203d 2064 6963 7428 290d 0a20  oint = dict().. 
+000082c0: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
+000082d0: 745b 2773 6f75 7263 6527 5d20 3d20 736f  t['source'] = so
+000082e0: 7572 6365 0d0a 2020 2020 2020 2020 746f  urce..        to
+000082f0: 7263 682e 7361 7665 2863 6865 636b 706f  rch.save(checkpo
+00008300: 696e 742c 2070 6174 6829 0d0a 0d0a 2020  int, path)....  
+00008310: 2020 4074 696d 656d 6574 6572 0d0a 2020    @timemeter..  
+00008320: 2020 6465 6620 6c6f 6164 5f63 6865 636b    def load_check
+00008330: 706f 696e 7428 7365 6c66 2920 2d3e 2069  point(self) -> i
+00008340: 6e74 3a0d 0a20 2020 2020 2020 2022 2222  nt:..        """
+00008350: 4c6f 6164 2074 6865 2072 6573 7420 6f66  Load the rest of
+00008360: 2070 6172 616d 732e 2222 220d 0a20 2020   params."""..   
+00008370: 2020 2020 2069 6e66 6f4c 6f67 6765 7228       infoLogger(
+00008380: 6622 5b43 6f61 6368 5d20 3e3e 3e20 4c6f  f"[Coach] >>> Lo
+00008390: 6164 2074 6865 2072 6563 656e 7420 6368  ad the recent ch
+000083a0: 6563 6b70 6f69 6e74 202e 2e2e 2229 0d0a  eckpoint ...")..
+000083b0: 2020 2020 2020 2020 7061 7468 203d 206f          path = o
+000083c0: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+000083d0: 2e63 6667 2e43 4f52 455f 4348 4543 4b50  .cfg.CORE_CHECKP
+000083e0: 4f49 4e54 5f50 4154 482c 2073 656c 662e  OINT_PATH, self.
+000083f0: 6366 672e 4348 4543 4b50 4f49 4e54 5f46  cfg.CHECKPOINT_F
+00008400: 494c 454e 414d 4529 0d0a 2020 2020 2020  ILENAME)..      
+00008410: 2020 6368 6563 6b70 6f69 6e74 203d 2074    checkpoint = t
+00008420: 6f72 6368 2e6c 6f61 6428 7061 7468 290d  orch.load(path).
+00008430: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008440: 6368 6563 6b70 6f69 6e74 5b27 736f 7572  checkpoint['sour
+00008450: 6365 275d 0d0a 0d0a 2020 2020 6465 6620  ce']....    def 
+00008460: 7265 7375 6d65 2873 656c 6629 3a0d 0a20  resume(self):.. 
+00008470: 2020 2020 2020 2022 2222 5265 7375 6d65         """Resume
+00008480: 2066 726f 6d20 7468 6520 7265 6365 6e74   from the recent
+00008490: 2063 6865 636b 706f 696e 742e 2222 220d   checkpoint.""".
+000084a0: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
+000084b0: 3d20 7365 6c66 2e65 6163 685f 6772 6964  = self.each_grid
+000084c0: 2829 2069 6620 7365 6c66 2e63 6667 2e45  () if self.cfg.E
+000084d0: 5843 4c55 5349 5645 2065 6c73 6520 7365  XCLUSIVE else se
+000084e0: 6c66 2e70 726f 6475 6374 5f67 7269 6428  lf.product_grid(
+000084f0: 290d 0a20 2020 2020 2020 2073 6f75 7263  )..        sourc
+00008500: 6520 3d20 6c69 7374 2873 6f75 7263 6529  e = list(source)
+00008510: 5b3a 3a2d 315d 0d0a 2020 2020 2020 2020  [::-1]..        
+00008520: 736f 7572 6365 203d 2073 656c 662e 6c6f  source = self.lo
+00008530: 6164 5f63 6865 636b 706f 696e 7428 2920  ad_checkpoint() 
+00008540: 6966 2073 656c 662e 6366 672e 7265 7375  if self.cfg.resu
+00008550: 6d65 2065 6c73 6520 736f 7572 6365 0d0a  me else source..
+00008560: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008570: 6f75 7263 650d 0a0d 0a20 2020 2064 6566  ource....    def
+00008580: 2072 756e 2873 656c 662c 2063 6f6d 6d61   run(self, comma
+00008590: 6e64 3a20 7374 722c 2070 6172 616d 733a  nd: str, params:
+000085a0: 2044 6963 7429 3a0d 0a20 2020 2020 2020   Dict):..       
+000085b0: 2022 2222 5374 6172 7420 6120 6e65 7720   """Start a new 
+000085c0: 7375 6270 726f 6365 7373 2222 220d 0a20  subprocess""".. 
+000085d0: 2020 2020 2020 2069 6d70 6f72 7420 7375         import su
+000085e0: 6270 726f 6365 7373 2c20 7368 6c65 780d  bprocess, shlex.
+000085f0: 0a20 2020 2020 2020 2066 6f72 206f 7074  .        for opt
+00008600: 696f 6e2c 2076 616c 2069 6e20 7061 7261  ion, val in para
+00008610: 6d73 2e69 7465 6d73 2829 3a0d 0a20 2020  ms.items():..   
+00008620: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
+00008630: 202b 3d20 7365 6c66 2e67 6574 5f6f 7074   += self.get_opt
+00008640: 696f 6e28 6f70 7469 6f6e 2c20 7661 6c29  ion(option, val)
+00008650: 0d0a 2020 2020 2020 2020 696e 666f 4c6f  ..        infoLo
+00008660: 6767 6572 2866 225c 3033 335b 303b 3331  gger(f"\033[0;31
+00008670: 3b34 376d 7b63 6f6d 6d61 6e64 7d5c 3033  ;47m{command}\03
+00008680: 335b 306d 2229 0d0a 2020 2020 2020 2020  3[0m")..        
+00008690: 7265 7475 726e 2073 7562 7072 6f63 6573  return subproces
+000086a0: 732e 506f 7065 6e28 7368 6c65 782e 7370  s.Popen(shlex.sp
+000086b0: 6c69 7428 636f 6d6d 616e 6429 290d 0a0d  lit(command))...
+000086c0: 0a20 2020 2064 6566 2077 6169 7428 7365  .    def wait(se
+000086d0: 6c66 2c20 7461 736b 733a 204c 6973 7429  lf, tasks: List)
+000086e0: 3a0d 0a20 2020 2020 2020 2022 2222 5761  :..        """Wa
+000086f0: 6974 2075 7469 6c20 616c 6c20 7072 6f63  it util all proc
+00008700: 6573 7365 7320 7465 726d 696e 6174 652e  esses terminate.
+00008710: 2222 220d 0a20 2020 2020 2020 2074 6173  """..        tas
+00008720: 6b73 203d 205b 7461 736b 2066 6f72 2074  ks = [task for t
+00008730: 6173 6b20 696e 2074 6173 6b73 2069 6620  ask in tasks if 
+00008740: 7461 736b 2069 7320 6e6f 7420 4e6f 6e65  task is not None
+00008750: 5d0d 0a20 2020 2020 2020 2066 6f72 2070  ]..        for p
+00008760: 726f 6365 7373 5f2c 2069 645f 2c20 6c6f  rocess_, id_, lo
+00008770: 6750 6174 682c 2070 6172 616d 7320 696e  gPath, params in
+00008780: 2074 6173 6b73 3a0d 0a20 2020 2020 2020   tasks:..       
+00008790: 2020 2020 2070 726f 6365 7373 5f2e 7761       process_.wa
+000087a0: 6974 2829 0d0a 2020 2020 2020 2020 2020  it()..          
+000087b0: 2020 7365 6c66 2e77 7269 7465 2869 645f    self.write(id_
+000087c0: 2c20 6c6f 6750 6174 682c 2070 6172 616d  , logPath, param
+000087d0: 7329 0d0a 0d0a 2020 2020 6465 6620 706f  s)....    def po
+000087e0: 6c6c 2873 656c 662c 2074 6173 6b73 3a20  ll(self, tasks: 
+000087f0: 4c69 7374 293a 0d0a 2020 2020 2020 2020  List):..        
+00008800: 2222 2257 6169 7420 7574 696c 2061 6e79  """Wait util any
+00008810: 2070 726f 6365 7373 2074 6572 6d69 6e61   process termina
+00008820: 7465 732e 2222 220d 0a20 2020 2020 2020  tes."""..       
+00008830: 2064 6566 2069 735f 6e75 6c6c 2874 6173   def is_null(tas
+00008840: 6b29 3a0d 0a20 2020 2020 2020 2020 2020  k):..           
+00008850: 2072 6574 7572 6e20 7461 736b 2069 7320   return task is 
+00008860: 4e6f 6e65 0d0a 2020 2020 2020 2020 6275  None..        bu
+00008870: 6666 6572 5f73 6f75 7263 6520 3d20 5b74  ffer_source = [t
+00008880: 6173 6b5b 2d31 5d20 666f 7220 7461 736b  ask[-1] for task
+00008890: 2069 6e20 7461 736b 7320 6966 2074 6173   in tasks if tas
+000088a0: 6b20 6973 206e 6f74 204e 6f6e 655d 0d0a  k is not None]..
+000088b0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+000088c0: 6570 2831 2920 2320 666f 7220 756e 6971  ep(1) # for uniq
+000088d0: 7565 2069 640d 0a20 2020 2020 2020 2077  ue id..        w
+000088e0: 6869 6c65 206e 6f74 2061 6e79 286d 6170  hile not any(map
+000088f0: 2869 735f 6e75 6c6c 2c20 7461 736b 7329  (is_null, tasks)
+00008900: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00008910: 7469 6d65 2e73 6c65 6570 2837 290d 0a20  time.sleep(7).. 
+00008920: 2020 2020 2020 2020 2020 2062 7566 6665             buffe
+00008930: 725f 736f 7572 6365 203d 205b 5d0d 0a20  r_source = [].. 
+00008940: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008950: 2c20 2870 726f 6365 7373 5f2c 2069 645f  , (process_, id_
+00008960: 2c20 6c6f 6750 6174 682c 2070 6172 616d  , logPath, param
+00008970: 7329 2069 6e20 656e 756d 6572 6174 6528  s) in enumerate(
+00008980: 7461 736b 7329 3a0d 0a20 2020 2020 2020  tasks):..       
+00008990: 2020 2020 2020 2020 2069 6620 7072 6f63           if proc
+000089a0: 6573 735f 2e70 6f6c 6c28 2920 6973 206e  ess_.poll() is n
+000089b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000089c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000089d0: 6c66 2e77 7269 7465 2869 645f 2c20 6c6f  lf.write(id_, lo
+000089e0: 6750 6174 682c 2070 6172 616d 7329 0d0a  gPath, params)..
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2020 7461 736b 735b 695d 203d 204e      tasks[i] = N
+00008a10: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00008a20: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 6275 6666 6572 5f73 6f75 7263 652e 6170  buffer_source.ap
+00008a50: 7065 6e64 2870 6172 616d 7329 0d0a 2020  pend(params)..  
+00008a60: 2020 2020 2020 7365 6c66 2e73 6176 655f        self.save_
+00008a70: 6368 6563 6b70 6f69 6e74 2873 656c 662e  checkpoint(self.
+00008a80: 736f 7572 6365 202b 2062 7566 6665 725f  source + buffer_
+00008a90: 736f 7572 6365 290d 0a20 2020 2020 2020  source)..       
+00008aa0: 2072 6574 7572 6e20 7461 736b 732e 696e   return tasks.in
+00008ab0: 6465 7828 4e6f 6e65 290d 0a0d 0a20 2020  dex(None)....   
+00008ac0: 2064 6566 2074 6572 6d69 6e61 7465 2873   def terminate(s
+00008ad0: 656c 662c 2074 6173 6b73 3a20 4c69 7374  elf, tasks: List
+00008ae0: 293a 0d0a 2020 2020 2020 2020 7461 736b  ):..        task
+00008af0: 7320 3d20 5b74 6173 6b20 666f 7220 7461  s = [task for ta
+00008b00: 736b 2069 6e20 7461 736b 7320 6966 2074  sk in tasks if t
+00008b10: 6173 6b20 6973 206e 6f74 204e 6f6e 655d  ask is not None]
+00008b20: 0d0a 2020 2020 2020 2020 666f 7220 7072  ..        for pr
+00008b30: 6f63 6573 735f 2c20 5f2c 205f 2c20 5f20  ocess_, _, _, _ 
+00008b40: 696e 2074 6173 6b73 3a0d 0a20 2020 2020  in tasks:..     
+00008b50: 2020 2020 2020 2069 6620 7072 6f63 6573         if proces
+00008b60: 735f 2e70 6f6c 6c28 2920 6973 204e 6f6e  s_.poll() is Non
+00008b70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00008b80: 2020 2020 7072 6f63 6573 735f 2e74 6572      process_.ter
+00008b90: 6d69 6e61 7465 2829 0d0a 2020 2020 2020  minate()..      
+00008ba0: 2020 7469 6d65 2e73 6c65 6570 2833 290d    time.sleep(3).
+00008bb0: 0a20 2020 2020 2020 2066 6f72 2070 726f  .        for pro
+00008bc0: 6365 7373 5f2c 205f 2c20 5f2c 205f 2069  cess_, _, _, _ i
+00008bd0: 6e20 7461 736b 733a 0d0a 2020 2020 2020  n tasks:..      
+00008be0: 2020 2020 2020 6966 2070 726f 6365 7373        if process
+00008bf0: 5f2e 706f 6c6c 2829 2069 7320 4e6f 6e65  _.poll() is None
+00008c00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008c10: 2020 2070 726f 6365 7373 5f2e 6b69 6c6c     process_.kill
+00008c20: 2829 0d0a 2020 2020 2020 2020 7379 732e  ()..        sys.
+00008c30: 6578 6974 2829 0d0a 0d0a 2020 2020 4074  exit()....    @t
+00008c40: 696d 656d 6574 6572 0d0a 2020 2020 6465  imemeter..    de
+00008c50: 6620 6669 7428 7365 6c66 293a 0d0a 2020  f fit(self):..  
+00008c60: 2020 2020 2020 2222 2247 7269 6420 7365        """Grid se
+00008c70: 6172 6368 2e22 2222 0d0a 2020 2020 2020  arch."""..      
+00008c80: 2020 7365 6c66 2e73 6f75 7263 6520 3d20    self.source = 
+00008c90: 7365 6c66 2e72 6573 756d 6528 290d 0a20  self.resume().. 
+00008ca0: 2020 2020 2020 2074 6173 6b73 203d 205b         tasks = [
+00008cb0: 4e6f 6e65 2066 6f72 205f 2069 6e20 7261  None for _ in ra
+00008cc0: 6e67 6528 6c65 6e28 7365 6c66 2e64 6576  nge(len(self.dev
+00008cd0: 6963 6573 2929 5d0d 0a0d 0a20 2020 2020  ices))]....     
+00008ce0: 2020 2064 6566 2073 6967 6e61 6c5f 6861     def signal_ha
+00008cf0: 6e64 6c65 7228 7369 672c 2066 7261 6d65  ndler(sig, frame
+00008d00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00008d10: 696e 666f 4c6f 6767 6572 2866 225c 3033  infoLogger(f"\03
+00008d20: 335b 303b 3331 3b34 376d 3d3d 3d3d 3d3d  3[0;31;47m======
+00008d30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008d40: 3d3d 3d3d 3d3d 3d3d 3d54 4552 4d49 4e41  =========TERMINA
+00008d50: 5445 2041 4c4c 2053 5542 5052 4f43 4553  TE ALL SUBPROCES
+00008d60: 5345 533d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  SES=============
+00008d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008d80: 3d3d 5c30 3333 5b30 6d22 290d 0a20 2020  ==\033[0m")..   
+00008d90: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00008da0: 726d 696e 6174 6528 7461 736b 7329 0d0a  rminate(tasks)..
+00008db0: 2020 2020 2020 2020 7369 676e 616c 2e73          signal.s
+00008dc0: 6967 6e61 6c28 7369 676e 616c 2e53 4947  ignal(signal.SIG
+00008dd0: 494e 542c 2073 6967 6e61 6c5f 6861 6e64  INT, signal_hand
+00008de0: 6c65 7229 0d0a 0d0a 2020 2020 2020 2020  ler)....        
+00008df0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00008e00: 2020 7768 696c 6520 7365 6c66 2e73 6f75    while self.sou
+00008e10: 7263 653a 0d0a 2020 2020 2020 2020 2020  rce:..          
+00008e20: 2020 2020 2020 696e 6465 7820 3d20 7365        index = se
+00008e30: 6c66 2e70 6f6c 6c28 7461 736b 7329 0d0a  lf.poll(tasks)..
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 6465 7669 6365 203d 2073 656c 662e 6465  device = self.de
+00008e60: 7669 6365 735b 696e 6465 785d 0d0a 2020  vices[index]..  
+00008e70: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00008e80: 7261 6d73 203d 2073 656c 662e 736f 7572  rams = self.sour
+00008e90: 6365 2e70 6f70 2829 0d0a 2020 2020 2020  ce.pop()..      
+00008ea0: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+00008eb0: 642c 2069 645f 2c20 6c6f 6750 6174 6820  d, id_, logPath 
+00008ec0: 3d20 7365 6c66 2e72 6567 6973 7465 7228  = self.register(
+00008ed0: 6465 7669 6365 290d 0a20 2020 2020 2020  device)..       
+00008ee0: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00008ef0: 5f20 3d20 7365 6c66 2e72 756e 2863 6f6d  _ = self.run(com
+00008f00: 6d61 6e64 2c20 7061 7261 6d73 290d 0a20  mand, params).. 
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00008f20: 6173 6b73 5b69 6e64 6578 5d20 3d20 2870  asks[index] = (p
+00008f30: 726f 6365 7373 5f2c 2069 645f 2c20 6c6f  rocess_, id_, lo
+00008f40: 6750 6174 682c 2070 6172 616d 7329 0d0a  gPath, params)..
+00008f50: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+00008f60: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00008f70: 6c66 2e77 6169 7428 7461 736b 7329 0d0a  lf.wait(tasks)..
+00008f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008f90: 2e74 6572 6d69 6e61 7465 2874 6173 6b73  .terminate(tasks
+00008fa0: 29                                       )
```

### Comparing `freerec-0.4.1/freerec/metrics.py` & `freerec-0.4.3/freerec/metrics.py`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/freerec/parser.py` & `freerec-0.4.3/freerec/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,23 +157,24 @@
             fh.write(info)
 
     def reset(self):
         self.clear()
         for key, val in CONFIG.items():
             self[key] = val
 
-    @timemeter("Parser/parse")
+    @timemeter
     def parse(self):
         """Add command-line arguments to the parser."""
 
         self.parser = argparse.ArgumentParser()
 
         self.add_argument("--root", type=str, default=".", help="data")
         self.add_argument("--dataset", type=str, default="RecDataSet", help="useless if no need to automatically select a dataset")
-        self.add_argument("--config", type=str, default=None, help="config.yml")
+        self.add_argument("--config", type=str, default=None, help="config.yaml")
+        self.add_argument("--ranking", type=str, choices=('full', 'pool'), default='full', help="full: full ranking; pool: sampled-based ranking")
 
         self.add_argument("--device", default=torch.cuda.current_device() if torch.cuda.is_available() else 'cpu', help="device")
 
         # model
         self.add_argument("--optimizer", type=str, default="adam", help="Optimizer: adam (default), sgd, ...")
         self.add_argument("--nesterov", action="store_true", default=False, help="nesterov for SGD")
         self.add_argument("-mom", "--momentum", type=float, default=0.9, help="the momentum used for SGD")
@@ -243,15 +244,15 @@
             if '=' in arg:
                 key = arg.split('=')[0]
             else:
                 key = arg.split(' ')[0]
             args.add(self._options[key])
         return args
 
-    @timemeter("Parser/load")
+    @timemeter
     def load(self, args: ArgumentParser):
         r"""
         Load config.yaml.
 
         Parameters:
         -----------
         args : argparse.ArgumentParser
@@ -271,15 +272,15 @@
                         defaults[key.upper()] = val
                     elif key in self:
                         defaults[key] = val
                     else:
                         raise KeyError(f"Unexpected parameter of `{key}' in `{args.config}' ...")
         return defaults
 
-    @timemeter("Parser/compile")
+    @timemeter
     def compile(self):
         r"""
         Generate the configuration file according to the specified settings.
 
         Flows:
         ------
         1. If the `--config` flag has been specified, load settings from a .yaml file, 
@@ -375,15 +376,15 @@
         for key in ('root', 'dataset', 'device'):
             if self.ENVS.get(key, None) is None:
                 raise KeyError(f"No `{key}' is allocated, calling '--{key}' to specify it")
 
         self.ENVS = Config(self.ENVS)
         self.PARAMS = Config(self.PARAMS)
 
-    @timemeter("Parser/load")
+    @timemeter
     def load(self, args: ArgumentParser) -> None:
         r"""
         Load configuration file.
 
         Parameters:
         -----------
         args : ArgumentParser
@@ -398,15 +399,15 @@
             self.update(**config)
         self.EXCLUSIVE = args.exclusive
         self.resume = args.resume
         for key, val in args._get_kwargs():
             if key in self.ALL_ENVS and val is not None:
                 self.ENVS[key] = val
 
-    @timemeter("CoreParser/compile")
+    @timemeter
     def compile(self, args) -> None:
         r"""
         Generate config file according to settings.
 
         Flows:
         ------
         1. Load settings from xxx.yaml which provides parameters for grid searching.
```

### Comparing `freerec-0.4.1/freerec/utils.py` & `freerec-0.4.3/freerec/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,39 +425,37 @@
     words : str
         The warning message that was logged.
     """
     words = f"\033[1;31m[Warning] >>> {warn} \033[0m"
     LOGGER.info(words)
     return words
 
-def timemeter(prefix=""):
+def timemeter(func):
     r"""
     A decorator to measure the running time of a function.
 
     Parameters:
     -----------
     prefix : str, optional
         A prefix to be displayed in the logging message, by default "".
 
     Returns:
     --------
     wrapper : function
         The decorated function.
     """
-    def decorator(func):
-        def wrapper(*args, **kwargs):
-            start = time.time()
-            results = func(*args, **kwargs)
-            end = time.time()
-            infoLogger(f"[Wall TIME] >>> {prefix} takes {end-start:.6f} seconds ...")
-            return  results
-        wrapper.__doc__ = func.__doc__
-        wrapper.__name__ = func.__name__
-        return wrapper
-    return decorator
+    def wrapper(*args, **kwargs):
+        start = time.time()
+        results = func(*args, **kwargs)
+        end = time.time()
+        infoLogger(f"[Wall TIME] >>> {func.__qualname__} takes {end-start:.6f} seconds ...")
+        return  results
+    wrapper.__doc__ = func.__doc__
+    wrapper.__name__ = func.__name__
+    return wrapper
 
 def mkdirs(*paths: str) -> None:
     r"""
     Create directories.
 
     Parameters:
     -----------
```

### Comparing `freerec-0.4.1/freerec.egg-info/PKG-INFO` & `freerec-0.4.3/freerec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.4.1
+Version: 0.4.3
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freerec-0.4.1/freerec.egg-info/SOURCES.txt` & `freerec-0.4.3/freerec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freerec-0.4.1/setup.py` & `freerec-0.4.3/setup.py`

 * *Files identical despite different names*

