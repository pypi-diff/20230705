# Comparing `tmp/scikit-gstat-1.0.8.tar.gz` & `tmp/scikit-gstat-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-gstat-1.0.8.tar", last modified: Tue Dec  6 06:11:12 2022, max compression
+gzip compressed data, was "scikit-gstat-1.0.9.tar", last modified: Wed Jan 11 19:05:36 2023, max compression
```

## Comparing `scikit-gstat-1.0.8.tar` & `scikit-gstat-1.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.568032 scikit-gstat-1.0.8/
--rw-r--r--   0 mirko      (501) staff       (20)      321 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/.coveragerc
--rw-r--r--   0 mirko      (501) staff       (20)      618 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/Dockerfile
--rw-r--r--   0 mirko      (501) staff       (20)     1161 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/Dockerfile.legacy
--rw-r--r--   0 mirko      (501) staff       (20)     1071 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)      226 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/MANIFEST.in
--rw-r--r--   0 mirko      (501) staff       (20)     5152 2022-12-06 06:11:12.567836 scikit-gstat-1.0.8/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     4362 2022-12-03 10:17:16.000000 scikit-gstat-1.0.8/README.rst
--rw-r--r--   0 mirko      (501) staff       (20)      396 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/classifiers.txt
--rw-r--r--   0 mirko      (501) staff       (20)       61 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/requirements.txt
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.554095 scikit-gstat-1.0.8/scikit_gstat.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)     5152 2022-12-06 06:11:12.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     1955 2022-12-06 06:11:12.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2022-12-06 06:11:12.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2022-12-03 09:54:27.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/not-zip-safe
--rw-r--r--   0 mirko      (501) staff       (20)       86 2022-12-06 06:11:12.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/requires.txt
--rw-r--r--   0 mirko      (501) staff       (20)        8 2022-12-06 06:11:12.000000 scikit-gstat-1.0.8/scikit_gstat.egg-info/top_level.txt
--rw-r--r--   0 mirko      (501) staff       (20)       38 2022-12-06 06:11:12.568075 scikit-gstat-1.0.8/setup.cfg
--rw-r--r--   0 mirko      (501) staff       (20)     1072 2022-12-03 09:54:14.000000 scikit-gstat-1.0.8/setup.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.558020 scikit-gstat-1.0.8/skgstat/
--rw-r--r--   0 mirko      (501) staff       (20)    30248 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/DirectionalVariogram.py
--rw-r--r--   0 mirko      (501) staff       (20)    17552 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/Kriging.py
--rw-r--r--   0 mirko      (501) staff       (20)    28110 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/MetricSpace.py
--rw-r--r--   0 mirko      (501) staff       (20)    51948 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/SpaceTimeVariogram.py
--rw-r--r--   0 mirko      (501) staff       (20)    97549 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/Variogram.py
--rw-r--r--   0 mirko      (501) staff       (20)      537 2022-12-06 06:10:42.000000 scikit-gstat-1.0.8/skgstat/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)       21 2022-12-06 06:10:48.000000 scikit-gstat-1.0.8/skgstat/__version__.py
--rw-r--r--   0 mirko      (501) staff       (20)     9903 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/binning.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.558432 scikit-gstat-1.0.8/skgstat/data/
--rw-r--r--   0 mirko      (501) staff       (20)     9465 2022-12-05 18:53:01.000000 scikit-gstat-1.0.8/skgstat/data/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     4350 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/data/_loader.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.559587 scikit-gstat-1.0.8/skgstat/data/rf/
--rw-r--r--   0 mirko      (501) staff       (20)   180781 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/data/rf/aniso.png
--rw-r--r--   0 mirko      (501) staff       (20)   390126 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/data/rf/pancake.png
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.560416 scikit-gstat-1.0.8/skgstat/data/samples/
--rw-r--r--   0 mirko      (501) staff       (20)      471 2022-12-03 09:48:12.000000 scikit-gstat-1.0.8/skgstat/data/samples/README.md
--rw-r--r--   0 mirko      (501) staff       (20)    10520 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/data/samples/meuse.txt
--rw-r--r--   0 mirko      (501) staff       (20)     9973 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/estimators.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.561148 scikit-gstat-1.0.8/skgstat/interfaces/
--rw-r--r--   0 mirko      (501) staff       (20)      162 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/interfaces/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     5531 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/interfaces/gstools.py
--rw-r--r--   0 mirko      (501) staff       (20)     2688 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/interfaces/pykrige.py
--rw-r--r--   0 mirko      (501) staff       (20)     6329 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/interfaces/variogram_estimator.py
--rw-r--r--   0 mirko      (501) staff       (20)    13763 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/models.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.562980 scikit-gstat-1.0.8/skgstat/plotting/
--rw-r--r--   0 mirko      (501) staff       (20)     1279 2022-12-06 06:10:31.000000 scikit-gstat-1.0.8/skgstat/plotting/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     3338 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/directtional_variogram.py
--rw-r--r--   0 mirko      (501) staff       (20)     4809 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/stvariogram_marginal.py
--rw-r--r--   0 mirko      (501) staff       (20)     3715 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/plotting/stvariogram_plot2d.py
--rw-r--r--   0 mirko      (501) staff       (20)     3985 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/stvariogram_plot3d.py
--rw-r--r--   0 mirko      (501) staff       (20)     1935 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/variogram_dd_plot.py
--rw-r--r--   0 mirko      (501) staff       (20)     3732 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/variogram_location_trend.py
--rw-r--r--   0 mirko      (501) staff       (20)     5433 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/variogram_plot.py
--rw-r--r--   0 mirko      (501) staff       (20)     2903 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/plotting/variogram_scattergram.py
--rw-r--r--   0 mirko      (501) staff       (20)     6626 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/stmodels.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.566278 scikit-gstat-1.0.8/skgstat/tests/
--rw-r--r--   0 mirko      (501) staff       (20)     1058 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     4376 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_binning.py
--rw-r--r--   0 mirko      (501) staff       (20)     3156 2022-12-06 06:10:42.000000 scikit-gstat-1.0.8/skgstat/tests/test_cross_utility.py
--rw-r--r--   0 mirko      (501) staff       (20)     1431 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_data_loader.py
--rw-r--r--   0 mirko      (501) staff       (20)     4791 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_directionalvariogram.py
--rw-r--r--   0 mirko      (501) staff       (20)     3107 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_estimator.py
--rw-r--r--   0 mirko      (501) staff       (20)    10884 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/tests/test_interfaces.py
--rw-r--r--   0 mirko      (501) staff       (20)      582 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_isotropic.py
--rw-r--r--   0 mirko      (501) staff       (20)     6723 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_kriging.py
--rw-r--r--   0 mirko      (501) staff       (20)     2274 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_likelihood.py
--rw-r--r--   0 mirko      (501) staff       (20)     4688 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/tests/test_metric_space.py
--rw-r--r--   0 mirko      (501) staff       (20)     5228 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_models.py
--rw-r--r--   0 mirko      (501) staff       (20)      736 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_plotting_backend.py
--rw-r--r--   0 mirko      (501) staff       (20)     6206 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_spacetimevariogram.py
--rw-r--r--   0 mirko      (501) staff       (20)     3764 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/tests/test_stmodels.py
--rw-r--r--   0 mirko      (501) staff       (20)     3104 2022-12-04 10:59:40.000000 scikit-gstat-1.0.8/skgstat/tests/test_util.py
--rw-r--r--   0 mirko      (501) staff       (20)    42719 2022-12-03 09:59:26.000000 scikit-gstat-1.0.8/skgstat/tests/test_variogram.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2022-12-06 06:11:12.567561 scikit-gstat-1.0.8/skgstat/util/
--rw-r--r--   0 mirko      (501) staff       (20)       36 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/util/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     2858 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/util/cross_validation.py
--rw-r--r--   0 mirko      (501) staff       (20)     3608 2022-12-06 06:10:42.000000 scikit-gstat-1.0.8/skgstat/util/cross_variogram.py
--rw-r--r--   0 mirko      (501) staff       (20)     5301 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/util/likelihood.py
--rw-r--r--   0 mirko      (501) staff       (20)      922 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/util/shannon.py
--rw-r--r--   0 mirko      (501) staff       (20)     6820 2022-12-03 07:42:58.000000 scikit-gstat-1.0.8/skgstat/util/uncertainty.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.950127 scikit-gstat-1.0.9/
+-rw-r--r--   0 mirko      (501) staff       (20)      321 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/.coveragerc
+-rw-r--r--   0 mirko      (501) staff       (20)      618 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/Dockerfile
+-rw-r--r--   0 mirko      (501) staff       (20)     1161 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/Dockerfile.legacy
+-rw-r--r--   0 mirko      (501) staff       (20)     1071 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/LICENSE
+-rw-r--r--   0 mirko      (501) staff       (20)      226 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/MANIFEST.in
+-rw-r--r--   0 mirko      (501) staff       (20)     5152 2023-01-11 19:05:36.949927 scikit-gstat-1.0.9/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     4362 2022-12-03 10:17:16.000000 scikit-gstat-1.0.9/README.rst
+-rw-r--r--   0 mirko      (501) staff       (20)      396 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/classifiers.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       61 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/requirements.txt
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.931476 scikit-gstat-1.0.9/scikit_gstat.egg-info/
+-rw-r--r--   0 mirko      (501) staff       (20)     5152 2023-01-11 19:05:36.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     1955 2023-01-11 19:05:36.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/SOURCES.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        1 2023-01-11 19:05:36.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/dependency_links.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        1 2022-12-03 09:54:27.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/not-zip-safe
+-rw-r--r--   0 mirko      (501) staff       (20)       86 2023-01-11 19:05:36.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/requires.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        8 2023-01-11 19:05:36.000000 scikit-gstat-1.0.9/scikit_gstat.egg-info/top_level.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       38 2023-01-11 19:05:36.950172 scikit-gstat-1.0.9/setup.cfg
+-rw-r--r--   0 mirko      (501) staff       (20)     1072 2022-12-03 09:54:14.000000 scikit-gstat-1.0.9/setup.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.935499 scikit-gstat-1.0.9/skgstat/
+-rw-r--r--   0 mirko      (501) staff       (20)    30248 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/DirectionalVariogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)    17552 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/Kriging.py
+-rw-r--r--   0 mirko      (501) staff       (20)    28110 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/MetricSpace.py
+-rw-r--r--   0 mirko      (501) staff       (20)    51948 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/SpaceTimeVariogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)    97549 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/Variogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)      537 2023-01-11 08:29:28.000000 scikit-gstat-1.0.9/skgstat/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)       21 2023-01-11 18:52:55.000000 scikit-gstat-1.0.9/skgstat/__version__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    10067 2023-01-11 08:29:28.000000 scikit-gstat-1.0.9/skgstat/binning.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.936117 scikit-gstat-1.0.9/skgstat/data/
+-rw-r--r--   0 mirko      (501) staff       (20)    13770 2023-01-11 09:45:28.000000 scikit-gstat-1.0.9/skgstat/data/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4350 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/data/_loader.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.937340 scikit-gstat-1.0.9/skgstat/data/rf/
+-rw-r--r--   0 mirko      (501) staff       (20)   180781 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/data/rf/aniso.png
+-rw-r--r--   0 mirko      (501) staff       (20)   390126 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/data/rf/pancake.png
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.938309 scikit-gstat-1.0.9/skgstat/data/samples/
+-rw-r--r--   0 mirko      (501) staff       (20)      471 2022-12-03 09:48:12.000000 scikit-gstat-1.0.9/skgstat/data/samples/README.md
+-rw-r--r--   0 mirko      (501) staff       (20)    10520 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/data/samples/meuse.txt
+-rw-r--r--   0 mirko      (501) staff       (20)     9973 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/estimators.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.939112 scikit-gstat-1.0.9/skgstat/interfaces/
+-rw-r--r--   0 mirko      (501) staff       (20)      162 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/interfaces/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5531 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/interfaces/gstools.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2688 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/interfaces/pykrige.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6329 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/interfaces/variogram_estimator.py
+-rw-r--r--   0 mirko      (501) staff       (20)    13763 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/models.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.940944 scikit-gstat-1.0.9/skgstat/plotting/
+-rw-r--r--   0 mirko      (501) staff       (20)     1279 2022-12-06 06:10:31.000000 scikit-gstat-1.0.9/skgstat/plotting/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3338 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/directtional_variogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4809 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/stvariogram_marginal.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3715 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/plotting/stvariogram_plot2d.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3985 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/stvariogram_plot3d.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1935 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/variogram_dd_plot.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3732 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/variogram_location_trend.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5433 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/variogram_plot.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2903 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/plotting/variogram_scattergram.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6626 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/stmodels.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.948606 scikit-gstat-1.0.9/skgstat/tests/
+-rw-r--r--   0 mirko      (501) staff       (20)     1058 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4376 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_binning.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3156 2023-01-11 08:29:28.000000 scikit-gstat-1.0.9/skgstat/tests/test_cross_utility.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2759 2023-01-11 09:45:28.000000 scikit-gstat-1.0.9/skgstat/tests/test_data_loader.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4791 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_directionalvariogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3107 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_estimator.py
+-rw-r--r--   0 mirko      (501) staff       (20)    10884 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/tests/test_interfaces.py
+-rw-r--r--   0 mirko      (501) staff       (20)      582 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_isotropic.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6723 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_kriging.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2274 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_likelihood.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4688 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/tests/test_metric_space.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5228 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_models.py
+-rw-r--r--   0 mirko      (501) staff       (20)      736 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_plotting_backend.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6206 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_spacetimevariogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3764 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/tests/test_stmodels.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3104 2022-12-04 10:59:40.000000 scikit-gstat-1.0.9/skgstat/tests/test_util.py
+-rw-r--r--   0 mirko      (501) staff       (20)    42719 2022-12-03 09:59:26.000000 scikit-gstat-1.0.9/skgstat/tests/test_variogram.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2023-01-11 19:05:36.949676 scikit-gstat-1.0.9/skgstat/util/
+-rw-r--r--   0 mirko      (501) staff       (20)       36 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/util/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2858 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/util/cross_validation.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3608 2023-01-11 08:29:28.000000 scikit-gstat-1.0.9/skgstat/util/cross_variogram.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5301 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/util/likelihood.py
+-rw-r--r--   0 mirko      (501) staff       (20)      922 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/util/shannon.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6820 2022-12-03 07:42:58.000000 scikit-gstat-1.0.9/skgstat/util/uncertainty.py
```

### Comparing `scikit-gstat-1.0.8/Dockerfile` & `scikit-gstat-1.0.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/Dockerfile.legacy` & `scikit-gstat-1.0.9/Dockerfile.legacy`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/LICENSE` & `scikit-gstat-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/PKG-INFO` & `scikit-gstat-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gstat
-Version: 1.0.8
+Version: 1.0.9
 Summary: Geostatistical expansion in the scipy style
 Author: Mirko Maelicke
 Author-email: mirko.maelicke@kit.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scikit-gstat-1.0.8/README.rst` & `scikit-gstat-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/scikit_gstat.egg-info/PKG-INFO` & `scikit-gstat-1.0.9/scikit_gstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gstat
-Version: 1.0.8
+Version: 1.0.9
 Summary: Geostatistical expansion in the scipy style
 Author: Mirko Maelicke
 Author-email: mirko.maelicke@kit.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scikit-gstat-1.0.8/scikit_gstat.egg-info/SOURCES.txt` & `scikit-gstat-1.0.9/scikit_gstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/setup.py` & `scikit-gstat-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/DirectionalVariogram.py` & `scikit-gstat-1.0.9/skgstat/DirectionalVariogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/Kriging.py` & `scikit-gstat-1.0.9/skgstat/Kriging.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/MetricSpace.py` & `scikit-gstat-1.0.9/skgstat/MetricSpace.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/SpaceTimeVariogram.py` & `scikit-gstat-1.0.9/skgstat/SpaceTimeVariogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/Variogram.py` & `scikit-gstat-1.0.9/skgstat/Variogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/__init__.py` & `scikit-gstat-1.0.9/skgstat/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/binning.py` & `scikit-gstat-1.0.9/skgstat/binning.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,14 +154,18 @@
     The :class:`KMeans <sklearn.cluster.KMeans>` that is used under the hood is not
     a deterministic algorithm, as the starting cluster centroids are seeded
     randomly. This can yield slightly different results on reach run.
     Thus, for this application, the random_state on KMeans is fixed to a
     specific value. You can change the seed by passing another seed to
     :class:`Variogram <skgstat.Variogram>` as `binning_random_state`.
 
+    .. versionchanged:: 1.0.9
+        KMeans is now initialized as ``KMeans(n_init=10)`` as this default value
+        will change in SciKit-Learn 1.4.
+
     """
     # maxlags larger than maximum separating distance will be ignored
     if maxlag is None or maxlag > np.nanmax(distances):
         maxlag = np.nanmax(distances)
 
     # filter for distances < maxlag
     d = distances[np.where(distances <= maxlag)]
@@ -169,15 +173,15 @@
     # filter the sklearn convervence warning, because working with 
     # undefined state in binning does not make any sense
     with warnings.catch_warnings():
         warnings.filterwarnings('error')
 
         # cluster the filtered distances
         try:
-            km = KMeans(n_clusters=n, random_state=binning_random_state).fit(d.reshape(-1, 1))
+            km = KMeans(n_clusters=n, random_state=binning_random_state, n_init=10).fit(d.reshape(-1, 1))
         except ConvergenceWarning:
             raise ValueError("KMeans failed to converge. Maybe you need to use a different n_lags.")
 
     # get the centers
     _centers = np.sort(km.cluster_centers_.flatten())
 
     # build the upper edges
```

### Comparing `scikit-gstat-1.0.8/skgstat/data/_loader.py` & `scikit-gstat-1.0.9/skgstat/data/_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/data/rf/aniso.png` & `scikit-gstat-1.0.9/skgstat/data/rf/aniso.png`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/data/rf/pancake.png` & `scikit-gstat-1.0.9/skgstat/data/rf/pancake.png`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/data/samples/meuse.txt` & `scikit-gstat-1.0.9/skgstat/data/samples/meuse.txt`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/estimators.py` & `scikit-gstat-1.0.9/skgstat/estimators.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/interfaces/gstools.py` & `scikit-gstat-1.0.9/skgstat/interfaces/gstools.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/interfaces/pykrige.py` & `scikit-gstat-1.0.9/skgstat/interfaces/pykrige.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/interfaces/variogram_estimator.py` & `scikit-gstat-1.0.9/skgstat/interfaces/variogram_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/models.py` & `scikit-gstat-1.0.9/skgstat/models.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/__init__.py` & `scikit-gstat-1.0.9/skgstat/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/directtional_variogram.py` & `scikit-gstat-1.0.9/skgstat/plotting/directtional_variogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/stvariogram_marginal.py` & `scikit-gstat-1.0.9/skgstat/plotting/stvariogram_marginal.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/stvariogram_plot2d.py` & `scikit-gstat-1.0.9/skgstat/plotting/stvariogram_plot2d.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/stvariogram_plot3d.py` & `scikit-gstat-1.0.9/skgstat/plotting/stvariogram_plot3d.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/variogram_dd_plot.py` & `scikit-gstat-1.0.9/skgstat/plotting/variogram_dd_plot.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/variogram_location_trend.py` & `scikit-gstat-1.0.9/skgstat/plotting/variogram_location_trend.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/variogram_plot.py` & `scikit-gstat-1.0.9/skgstat/plotting/variogram_plot.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/plotting/variogram_scattergram.py` & `scikit-gstat-1.0.9/skgstat/plotting/variogram_scattergram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/stmodels.py` & `scikit-gstat-1.0.9/skgstat/stmodels.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/__init__.py` & `scikit-gstat-1.0.9/skgstat/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_binning.py` & `scikit-gstat-1.0.9/skgstat/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_cross_utility.py` & `scikit-gstat-1.0.9/skgstat/tests/test_cross_utility.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_directionalvariogram.py` & `scikit-gstat-1.0.9/skgstat/tests/test_directionalvariogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_estimator.py` & `scikit-gstat-1.0.9/skgstat/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_interfaces.py` & `scikit-gstat-1.0.9/skgstat/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_isotropic.py` & `scikit-gstat-1.0.9/skgstat/tests/test_isotropic.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_kriging.py` & `scikit-gstat-1.0.9/skgstat/tests/test_kriging.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_likelihood.py` & `scikit-gstat-1.0.9/skgstat/tests/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_metric_space.py` & `scikit-gstat-1.0.9/skgstat/tests/test_metric_space.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_models.py` & `scikit-gstat-1.0.9/skgstat/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_plotting_backend.py` & `scikit-gstat-1.0.9/skgstat/tests/test_plotting_backend.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_spacetimevariogram.py` & `scikit-gstat-1.0.9/skgstat/tests/test_spacetimevariogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_stmodels.py` & `scikit-gstat-1.0.9/skgstat/tests/test_stmodels.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_util.py` & `scikit-gstat-1.0.9/skgstat/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/tests/test_variogram.py` & `scikit-gstat-1.0.9/skgstat/tests/test_variogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/util/cross_validation.py` & `scikit-gstat-1.0.9/skgstat/util/cross_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/util/cross_variogram.py` & `scikit-gstat-1.0.9/skgstat/util/cross_variogram.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/util/likelihood.py` & `scikit-gstat-1.0.9/skgstat/util/likelihood.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/util/shannon.py` & `scikit-gstat-1.0.9/skgstat/util/shannon.py`

 * *Files identical despite different names*

### Comparing `scikit-gstat-1.0.8/skgstat/util/uncertainty.py` & `scikit-gstat-1.0.9/skgstat/util/uncertainty.py`

 * *Files identical despite different names*

