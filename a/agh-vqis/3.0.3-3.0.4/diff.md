# Comparing `tmp/agh_vqis-3.0.3.tar.gz` & `tmp/agh_vqis-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-3.0.3.tar", last modified: Sat Jun 17 10:35:19 2023, max compression
+gzip compressed data, was "agh_vqis-3.0.4.tar", last modified: Wed Jul  5 07:18:27 2023, max compression
```

## Comparing `agh_vqis-3.0.3.tar` & `agh_vqis-3.0.4.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/
--rw-rw-rw-   0        0        0     2826 2023-06-09 20:08:24.000000 agh_vqis-3.0.3/LICENSE
--rw-rw-rw-   0        0        0     7317 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6309 2023-06-16 19:04:34.000000 agh_vqis-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.890387 agh_vqis-3.0.3/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0     7317 2023-06-17 10:35:18.000000 agh_vqis-3.0.3/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8111 2023-06-17 10:35:18.000000 agh_vqis-3.0.3/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:35:18.000000 agh_vqis-3.0.3/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-06-17 10:35:18.000000 agh_vqis-3.0.3/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 10:35:18.000000 agh_vqis-3.0.3/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-06-09 20:08:24.000000 agh_vqis-3.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.859016 agh_vqis-3.0.3/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.904057 agh_vqis-3.0.3/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-06-09 20:24:14.000000 agh_vqis-3.0.3/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-06-09 20:24:14.000000 agh_vqis-3.0.3/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-06-09 20:24:14.000000 agh_vqis-3.0.3/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1329 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.859016 agh_vqis-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.906070 agh_vqis-3.0.3/src/agh_vqis/
--rw-rw-rw-   0        0        0      381 2023-06-17 10:33:24.000000 agh_vqis-3.0.3/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    22326 2023-06-16 22:01:17.000000 agh_vqis-3.0.3/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0     1349 2023-06-09 20:08:24.000000 agh_vqis-3.0.3/src/agh_vqis/_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.909511 agh_vqis-3.0.3/src/agh_vqis/binaries/
--rw-rw-rw-   0        0        0    97508 2023-06-09 20:08:24.000000 agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
--rwxrwxrwx   0        0        0   122077 2023-06-17 10:19:50.000000 agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
--rw-rw-rw-   0        0        0    66424 2023-06-09 20:08:24.000000 agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
--rw-rw-rw-   0        0        0  2952245 2023-06-16 14:14:09.000000 agh_vqis-3.0.3/src/agh_vqis/binaries/cygwin1.dll
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:18.859016 agh_vqis-3.0.3/src/agh_vqis/models/
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/
--rw-rw-rw-   0        0        0    21075 2023-05-23 22:55:31.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    21723 2023-05-23 22:55:33.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    14595 2023-05-23 22:55:36.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    15027 2023-05-23 22:55:38.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    32379 2023-05-23 22:56:00.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    35763 2023-05-23 22:56:02.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:04.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    34323 2023-05-23 22:56:06.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:08.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    34035 2023-05-23 22:56:10.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    29643 2023-05-23 22:55:40.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
--rw-rw-rw-   0        0        0    33747 2023-05-23 22:55:42.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
--rw-rw-rw-   0        0        0    28059 2023-05-23 22:55:44.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
--rw-rw-rw-   0        0        0    29787 2023-05-23 22:55:45.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
--rw-rw-rw-   0        0        0    33531 2023-05-23 22:55:46.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
--rw-rw-rw-   0        0        0    29355 2023-05-23 22:55:48.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
--rw-rw-rw-   0        0        0    26691 2023-05-23 22:55:50.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
--rw-rw-rw-   0        0        0    31803 2023-05-23 22:55:52.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:55:58.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
--rw-rw-rw-   0        0        0    30291 2023-05-23 22:55:54.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
--rw-rw-rw-   0        0        0    30795 2023-05-23 22:55:56.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:50.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    26907 2023-05-23 22:56:50.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    38355 2023-05-23 22:56:42.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
--rw-rw-rw-   0        0        0    39075 2023-05-23 22:56:44.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
--rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:46.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
--rw-rw-rw-   0        0        0    37059 2023-05-23 22:56:49.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
--rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:58.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    27339 2023-05-23 22:56:59.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38571 2023-05-23 22:56:51.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
--rw-rw-rw-   0        0        0    39219 2023-05-23 22:56:55.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
--rw-rw-rw-   0        0        0    37923 2023-05-23 22:56:56.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
--rw-rw-rw-   0        0        0    37995 2023-05-23 22:56:57.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
--rw-rw-rw-   0        0        0    27339 2023-05-23 22:57:03.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    27267 2023-05-23 22:57:07.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    38643 2023-05-23 22:57:00.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
--rw-rw-rw-   0        0        0    39363 2023-05-23 22:57:01.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
--rw-rw-rw-   0        0        0    38067 2023-05-23 22:57:01.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
--rw-rw-rw-   0        0        0    38211 2023-05-23 22:57:02.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
--rw-rw-rw-   0        0        0    36915 2023-05-23 22:56:15.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
--rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:16.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
--rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:17.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
--rw-rw-rw-   0        0        0    28779 2023-05-23 22:56:11.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
--rw-rw-rw-   0        0        0    29715 2023-05-23 22:56:13.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
--rw-rw-rw-   0        0        0    30219 2023-05-23 22:56:14.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:23.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
--rw-rw-rw-   0        0        0    38283 2023-05-23 22:56:25.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
--rw-rw-rw-   0        0        0    37563 2023-05-23 22:56:26.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
--rw-rw-rw-   0        0        0    27843 2023-05-23 22:56:18.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
--rw-rw-rw-   0        0        0    27267 2023-05-23 22:56:19.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
--rw-rw-rw-   0        0        0    27699 2023-05-23 22:56:20.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
--rw-rw-rw-   0        0        0    37635 2023-05-23 22:56:30.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
--rw-rw-rw-   0        0        0    37275 2023-05-23 22:56:31.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
--rw-rw-rw-   0        0        0    37851 2023-05-23 22:56:32.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
--rw-rw-rw-   0        0        0    29283 2023-05-23 22:56:27.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
--rw-rw-rw-   0        0        0    27483 2023-05-23 22:56:27.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
--rw-rw-rw-   0        0        0    26979 2023-05-23 22:56:28.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
--rw-rw-rw-   0        0        0    37347 2023-05-23 22:56:37.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
--rw-rw-rw-   0        0        0    38139 2023-05-23 22:56:38.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
--rw-rw-rw-   0        0        0    37779 2023-05-23 22:56:40.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
--rw-rw-rw-   0        0        0    29787 2023-05-23 22:56:33.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
--rw-rw-rw-   0        0        0    27195 2023-05-23 22:56:35.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
--rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:32.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    17835 2023-05-23 22:57:32.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    27411 2023-05-23 22:57:28.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
--rw-rw-rw-   0        0        0    25179 2023-05-23 22:57:30.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
--rw-rw-rw-   0        0        0    22659 2023-05-23 22:57:31.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
--rw-rw-rw-   0        0        0    17259 2023-05-23 22:57:34.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    17187 2023-05-23 22:57:44.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    25395 2023-05-23 22:57:33.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
--rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:34.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:51.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    16827 2023-05-23 22:57:52.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    23667 2023-05-23 22:57:49.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-05-23 22:57:08.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
--rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:09.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
--rw-rw-rw-   0        0        0    22299 2023-05-23 22:57:10.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
--rw-rw-rw-   0        0        0    22155 2023-05-23 22:57:14.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
--rw-rw-rw-   0        0        0    19059 2023-05-23 22:57:12.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
--rw-rw-rw-   0        0        0    18987 2023-05-23 22:57:12.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
--rw-rw-rw-   0        0        0    20571 2023-05-23 22:57:13.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
--rw-rw-rw-   0        0        0    23163 2023-05-23 22:57:20.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:21.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
--rw-rw-rw-   0        0        0    22011 2023-05-23 22:57:15.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
--rw-rw-rw-   0        0        0    20283 2023-05-23 22:57:16.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
--rw-rw-rw-   0        0        0    18123 2023-05-23 22:57:17.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
--rw-rw-rw-   0        0        0    22947 2023-05-23 22:57:25.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-05-23 22:57:26.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
--rw-rw-rw-   0        0        0    22587 2023-05-23 22:57:26.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
--rw-rw-rw-   0        0        0    23955 2023-05-23 22:57:22.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
--rw-rw-rw-   0        0        0    21435 2023-05-23 22:57:23.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
--rw-rw-rw-   0        0        0    18699 2023-05-23 22:57:24.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
--rw-rw-rw-   0        0        0     4587 2023-05-23 22:57:59.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
--rw-rw-rw-   0        0        0     5739 2023-05-23 22:57:53.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
--rw-rw-rw-   0        0        0     6459 2023-05-23 22:57:54.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
--rw-rw-rw-   0        0        0     5307 2023-05-23 22:57:55.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
--rw-rw-rw-   0        0        0     5811 2023-05-23 22:57:56.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
--rw-rw-rw-   0        0        0     4947 2023-05-23 22:57:57.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
--rw-rw-rw-   0        0        0     5379 2023-05-23 22:57:58.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
--rw-rw-rw-   0        0        0     5163 2023-05-23 22:57:57.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
--rw-rw-rw-   0        0        0    40443 2023-05-23 22:58:18.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    43467 2023-05-23 22:58:19.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    39435 2023-05-23 22:58:21.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    42171 2023-05-23 22:58:22.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38787 2023-05-23 22:58:23.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    42747 2023-05-23 22:58:00.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
--rw-rw-rw-   0        0        0    39939 2023-05-23 22:58:01.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
--rw-rw-rw-   0        0        0    41235 2023-05-23 22:58:01.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
--rw-rw-rw-   0        0        0    38931 2023-05-23 22:58:02.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
--rw-rw-rw-   0        0        0    40875 2023-05-23 22:58:03.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
--rw-rw-rw-   0        0        0    37923 2023-05-23 22:58:16.000000 agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/src/agh_vqis/models/ugc/
--rw-rw-rw-   0        0        0   594166 2023-06-13 12:09:35.000000 agh_vqis-3.0.3/src/agh_vqis/models/ugc/12k_all_set.json
-drwxrwxrwx   0        0        0        0 2023-06-17 10:35:19.772883 agh_vqis-3.0.3/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     5470 2023-06-16 19:06:30.000000 agh_vqis-3.0.3/src/agh_vqis/utils/helpers.py
--rw-rw-rw-   0        0        0      754 2023-06-09 21:13:23.000000 agh_vqis-3.0.3/src/agh_vqis/utils/resolution_cast.py
--rw-rw-rw-   0        0        0     5735 2023-06-13 12:52:00.000000 agh_vqis-3.0.3/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.438422 agh_vqis-3.0.4/
+-rw-rw-rw-   0        0        0     2826 2023-01-28 21:45:19.000000 agh_vqis-3.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12782 2023-07-05 07:18:27.438422 agh_vqis-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11774 2023-07-05 07:17:33.000000 agh_vqis-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.130598 agh_vqis-3.0.4/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0    12782 2023-07-05 07:18:27.000000 agh_vqis-3.0.4/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8111 2023-07-05 07:18:27.000000 agh_vqis-3.0.4/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:18:27.000000 agh_vqis-3.0.4/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-07-05 07:18:27.000000 agh_vqis-3.0.4/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-05 07:18:27.000000 agh_vqis-3.0.4/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-01-28 21:02:34.000000 agh_vqis-3.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.070060 agh_vqis-3.0.4/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.138594 agh_vqis-3.0.4/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-01-28 22:00:29.000000 agh_vqis-3.0.4/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-01-28 22:00:29.000000 agh_vqis-3.0.4/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-01-28 22:00:29.000000 agh_vqis-3.0.4/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-07-05 07:18:27.440422 agh_vqis-3.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.071062 agh_vqis-3.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.143593 agh_vqis-3.0.4/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-07-05 07:16:35.000000 agh_vqis-3.0.4/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    22326 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.153596 agh_vqis-3.0.4/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    97508 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+-rwxrwxrwx   0        0        0   122077 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+-rw-rw-rw-   0        0        0    66424 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+-rw-rw-rw-   0        0        0  2952245 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/binaries/cygwin1.dll
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.074068 agh_vqis-3.0.4/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.429425 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.431422 agh_vqis-3.0.4/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-07-05 07:18:27.437421 agh_vqis-3.0.4/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     5470 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-06-21 16:42:58.000000 agh_vqis-3.0.4/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-3.0.3/LICENSE` & `agh_vqis-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-3.0.4/agh_vqis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/python-cpbd/cpbd/compute.py` & `agh_vqis-3.0.4/python-cpbd/cpbd/compute.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/python-cpbd/cpbd/octave.py` & `agh_vqis-3.0.4/python-cpbd/cpbd/octave.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/setup.cfg` & `agh_vqis-3.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2033 2e30 2e33 0d0a 6175  sion = 3.0.3..au
+00000020: 7369 6f6e 203d 2033 2e30 2e34 0d0a 6175  sion = 3.0.4..au
 00000030: 7468 6f72 203d 204a 616b 7562 204e 6177  thor = Jakub Naw
 00000040: 61c5 8261 2c20 4669 6c69 7020 4b6f 7275  a..a, Filip Koru
 00000050: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
 00000060: 3d20 6a61 6b75 622e 6e61 7761 6c61 4061  = jakub.nawala@a
 00000070: 6768 2e65 6475 2e70 6c2c 2066 6b6f 7275  gh.edu.pl, fkoru
 00000080: 7340 7374 7564 656e 742e 6167 682e 6564  s@student.agh.ed
 00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
```

### Comparing `agh_vqis-3.0.3/src/agh_vqis/__main__.py` & `agh_vqis-3.0.4/src/agh_vqis/__main__.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/_logger.py` & `agh_vqis-3.0.4/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt` & `agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe` & `agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/binaries/agh_vqis_binary_x86_mt` & `agh_vqis-3.0.4/src/agh_vqis/binaries/agh_vqis_binary_x86_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/binaries/cygwin1.dll` & `agh_vqis-3.0.4/src/agh_vqis/binaries/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb` & `agh_vqis-3.0.4/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/models/ugc/12k_all_set.json` & `agh_vqis-3.0.4/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/utils/helpers.py` & `agh_vqis-3.0.4/src/agh_vqis/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/utils/resolution_cast.py` & `agh_vqis-3.0.4/src/agh_vqis/utils/resolution_cast.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.0.3/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.0.4/src/agh_vqis/utils/ugc.py`

 * *Files identical despite different names*

