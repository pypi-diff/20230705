# Comparing `tmp/tslearn-0.6.0.tar.gz` & `tmp/tslearn-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tslearn-0.6.0.tar", last modified: Mon Jul  3 19:34:58 2023, max compression
+gzip compressed data, was "tslearn-0.6.1.tar", last modified: Wed Jul  5 12:12:01 2023, max compression
```

## Comparing `tslearn-0.6.0.tar` & `tslearn-0.6.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.022307 tslearn-0.6.0/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1320 2017-06-28 16:18:01.000000 tslearn-0.6.0/LICENSE
--rw-r--r--   0 tavenard_r   (504) staff       (20)      254 2021-01-25 14:47:09.634369 tslearn-0.6.0/MANIFEST.in
--rw-r--r--   0 tavenard_r   (504) staff       (20)    14218 2023-07-03 19:34:58.022631 tslearn-0.6.0/PKG-INFO
--rw-r--r--   0 tavenard_r   (504) staff       (20)    13726 2023-07-03 19:27:41.054001 tslearn-0.6.0/README.md
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1166 2020-05-25 20:30:29.832352 tslearn-0.6.0/conftest.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)       59 2023-01-20 12:41:18.658875 tslearn-0.6.0/pyproject.toml
--rw-r--r--   0 tavenard_r   (504) staff       (20)      234 2020-05-25 20:30:29.833775 tslearn-0.6.0/setup.cfg
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1494 2023-07-03 19:27:41.069213 tslearn-0.6.0/setup.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.760754 tslearn-0.6.0/tslearn/
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.764247 tslearn-0.6.0/tslearn/.cached_datasets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)   442330 2017-06-22 13:28:03.000000 tslearn-0.6.0/tslearn/.cached_datasets/Trace.npz
--rw-r--r--   0 tavenard_r   (504) staff       (20)      757 2023-07-03 19:30:24.909402 tslearn-0.6.0/tslearn/__init__.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.800317 tslearn-0.6.0/tslearn/backend/
--rwxr-xr-x   0 tavenard_r   (504) staff       (20)      387 2023-07-03 19:27:41.069966 tslearn-0.6.0/tslearn/backend/__init__.py
--rwxr-xr-x   0 tavenard_r   (504) staff       (20)     5097 2023-07-03 19:27:41.070559 tslearn-0.6.0/tslearn/backend/backend.py
--rwxr-xr-x   0 tavenard_r   (504) staff       (20)     3909 2023-07-03 19:27:41.070918 tslearn-0.6.0/tslearn/backend/numpy_backend.py
--rwxr-xr-x   0 tavenard_r   (504) staff       (20)     7737 2023-07-03 19:27:41.071513 tslearn-0.6.0/tslearn/backend/pytorch_backend.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.832884 tslearn-0.6.0/tslearn/barycenters/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1160 2021-01-05 10:39:33.337401 tslearn-0.6.0/tslearn/barycenters/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    26086 2021-01-06 07:38:50.170547 tslearn-0.6.0/tslearn/barycenters/dba.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1095 2023-01-20 12:41:18.661707 tslearn-0.6.0/tslearn/barycenters/euclidean.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3647 2023-01-20 12:41:18.662160 tslearn-0.6.0/tslearn/barycenters/softdtw.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      285 2021-01-05 10:39:33.339083 tslearn-0.6.0/tslearn/barycenters/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.845351 tslearn-0.6.0/tslearn/bases/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      120 2021-01-05 10:39:33.340758 tslearn-0.6.0/tslearn/bases/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7807 2021-01-05 10:39:33.447118 tslearn-0.6.0/tslearn/bases/bases.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.851216 tslearn-0.6.0/tslearn/clustering/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      611 2023-07-03 19:27:41.072334 tslearn-0.6.0/tslearn/clustering/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    31792 2023-07-03 19:27:41.072990 tslearn-0.6.0/tslearn/clustering/kmeans.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     9994 2021-01-07 10:45:54.581839 tslearn-0.6.0/tslearn/clustering/kshape.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8445 2023-01-20 12:41:18.662711 tslearn-0.6.0/tslearn/clustering/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.856207 tslearn-0.6.0/tslearn/datasets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      359 2023-01-20 12:41:18.662963 tslearn-0.6.0/tslearn/datasets/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2843 2021-01-05 10:39:33.344441 tslearn-0.6.0/tslearn/datasets/cached.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2274 2021-01-05 10:39:33.344827 tslearn-0.6.0/tslearn/datasets/datasets.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    13833 2023-07-03 18:23:27.324761 tslearn-0.6.0/tslearn/datasets/ucr_uea.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.858847 tslearn-0.6.0/tslearn/early_classification/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      525 2021-01-05 10:39:33.346065 tslearn-0.6.0/tslearn/early_classification/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    21713 2021-01-05 10:39:33.440889 tslearn-0.6.0/tslearn/early_classification/early_classification.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.862117 tslearn-0.6.0/tslearn/generators/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      210 2021-01-05 10:39:33.348452 tslearn-0.6.0/tslearn/generators/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3556 2021-01-05 10:39:33.440389 tslearn-0.6.0/tslearn/generators/generators.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.870667 tslearn-0.6.0/tslearn/hdftools/
--rw-r--r--   0 tavenard_r   (504) staff       (20)       81 2021-01-05 10:39:33.349590 tslearn-0.6.0/tslearn/hdftools/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4488 2023-01-20 12:41:18.663583 tslearn-0.6.0/tslearn/hdftools/hdftools.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.873036 tslearn-0.6.0/tslearn/matrix_profile/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      361 2021-01-05 10:39:33.350226 tslearn-0.6.0/tslearn/matrix_profile/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8825 2021-01-05 10:39:33.439263 tslearn-0.6.0/tslearn/matrix_profile/matrix_profile.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.950061 tslearn-0.6.0/tslearn/metrics/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2200 2023-07-03 19:27:41.073788 tslearn-0.6.0/tslearn/metrics/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    14019 2023-07-03 19:27:41.075224 tslearn-0.6.0/tslearn/metrics/ctw.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   375335 2021-01-06 07:40:59.972248 tslearn-0.6.0/tslearn/metrics/cycc.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4103 2023-01-20 12:41:18.664293 tslearn-0.6.0/tslearn/metrics/cycc.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   423280 2021-01-06 07:41:00.252084 tslearn-0.6.0/tslearn/metrics/cysax.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7323 2023-01-20 12:41:18.664522 tslearn-0.6.0/tslearn/metrics/cysax.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    82613 2023-07-03 19:27:41.076292 tslearn-0.6.0/tslearn/metrics/dtw_variants.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     2183 2023-07-03 19:27:41.076866 tslearn-0.6.0/tslearn/metrics/sax.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)   281647 2021-01-06 07:41:00.441314 tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.c
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8199 2023-07-03 19:27:41.077390 tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     5245 2023-07-03 19:27:41.077789 tslearn-0.6.0/tslearn/metrics/soft_dtw_loss_pytorch.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    26296 2023-07-03 19:27:41.078376 tslearn-0.6.0/tslearn/metrics/softdtw_variants.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3319 2023-07-03 19:27:41.079312 tslearn-0.6.0/tslearn/metrics/utils.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.956267 tslearn-0.6.0/tslearn/neighbors/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      348 2023-01-20 12:41:18.666986 tslearn-0.6.0/tslearn/neighbors/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    28740 2021-01-05 10:39:33.422420 tslearn-0.6.0/tslearn/neighbors/neighbors.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.961028 tslearn-0.6.0/tslearn/neural_network/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      415 2021-01-05 10:39:33.362297 tslearn-0.6.0/tslearn/neural_network/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     5509 2021-01-05 10:39:33.421725 tslearn-0.6.0/tslearn/neural_network/neural_network.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.968274 tslearn-0.6.0/tslearn/piecewise/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      419 2021-01-05 10:39:33.363393 tslearn-0.6.0/tslearn/piecewise/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    24187 2023-01-20 12:41:18.667327 tslearn-0.6.0/tslearn/piecewise/piecewise.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.972110 tslearn-0.6.0/tslearn/preprocessing/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      318 2021-01-05 10:39:33.365690 tslearn-0.6.0/tslearn/preprocessing/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8690 2021-01-05 10:39:33.419089 tslearn-0.6.0/tslearn/preprocessing/preprocessing.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.976615 tslearn-0.6.0/tslearn/shapelets/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      509 2023-07-03 19:27:41.080084 tslearn-0.6.0/tslearn/shapelets/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    33169 2023-07-03 19:27:41.080848 tslearn-0.6.0/tslearn/shapelets/shapelets.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:57.979601 tslearn-0.6.0/tslearn/svm/
--rw-r--r--   0 tavenard_r   (504) staff       (20)      340 2021-01-05 10:39:33.368177 tslearn-0.6.0/tslearn/svm/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    20958 2023-07-03 19:27:41.081441 tslearn-0.6.0/tslearn/svm/svm.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.018719 tslearn-0.6.0/tslearn/tests/
--rw-r--r--   0 tavenard_r   (504) staff       (20)        0 2020-05-25 20:30:29.875851 tslearn-0.6.0/tslearn/tests/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    25004 2023-01-20 12:41:18.669171 tslearn-0.6.0/tslearn/tests/sklearn_patches.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3983 2020-05-25 20:30:29.876986 tslearn-0.6.0/tslearn/tests/test_barycenters.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     8032 2021-01-05 10:39:33.369380 tslearn-0.6.0/tslearn/tests/test_clustering.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7926 2023-07-03 19:27:41.081939 tslearn-0.6.0/tslearn/tests/test_estimators.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      721 2020-06-15 19:11:12.798796 tslearn-0.6.0/tslearn/tests/test_matrixprofile.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    24535 2023-07-03 19:27:41.082645 tslearn-0.6.0/tslearn/tests/test_metrics.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1994 2021-01-05 10:39:33.370832 tslearn-0.6.0/tslearn/tests/test_neighbors.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3698 2020-06-02 06:20:08.173618 tslearn-0.6.0/tslearn/tests/test_piecewise.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      508 2021-01-05 10:39:33.372803 tslearn-0.6.0/tslearn/tests/test_preprocessing.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     7750 2023-07-03 19:27:41.083347 tslearn-0.6.0/tslearn/tests/test_serialize_models.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     4205 2020-06-15 13:06:56.005238 tslearn-0.6.0/tslearn/tests/test_shapelets.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)      806 2023-07-03 19:27:41.084192 tslearn-0.6.0/tslearn/tests/test_svm.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3005 2021-01-05 10:39:33.374191 tslearn-0.6.0/tslearn/tests/test_utils.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)     3620 2020-06-11 08:08:55.932129 tslearn-0.6.0/tslearn/tests/test_variablelength.py
-drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-03 19:34:58.022204 tslearn-0.6.0/tslearn/utils/
--rw-r--r--   0 tavenard_r   (504) staff       (20)     1605 2023-01-20 12:41:18.670358 tslearn-0.6.0/tslearn/utils/__init__.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    23572 2023-01-20 12:41:18.670786 tslearn-0.6.0/tslearn/utils/cast.py
--rw-r--r--   0 tavenard_r   (504) staff       (20)    21371 2023-07-03 19:27:41.085116 tslearn-0.6.0/tslearn/utils/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.865461 tslearn-0.6.1/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1320 2017-06-28 16:18:01.000000 tslearn-0.6.1/LICENSE
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      254 2021-01-25 14:47:09.634369 tslearn-0.6.1/MANIFEST.in
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    14218 2023-07-05 12:12:01.865944 tslearn-0.6.1/PKG-INFO
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    13726 2023-07-03 19:27:41.054001 tslearn-0.6.1/README.md
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1166 2020-05-25 20:30:29.832352 tslearn-0.6.1/conftest.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)       59 2023-01-20 12:41:18.658875 tslearn-0.6.1/pyproject.toml
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      234 2020-05-25 20:30:29.833775 tslearn-0.6.1/setup.cfg
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1494 2023-07-03 19:27:41.069213 tslearn-0.6.1/setup.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.425165 tslearn-0.6.1/tslearn/
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.426522 tslearn-0.6.1/tslearn/.cached_datasets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   442330 2017-06-22 13:28:03.000000 tslearn-0.6.1/tslearn/.cached_datasets/Trace.npz
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      757 2023-07-05 12:10:14.406049 tslearn-0.6.1/tslearn/__init__.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.433392 tslearn-0.6.1/tslearn/backend/
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)      261 2023-07-05 12:09:08.797959 tslearn-0.6.1/tslearn/backend/__init__.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     5097 2023-07-03 19:27:41.070559 tslearn-0.6.1/tslearn/backend/backend.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     3909 2023-07-03 19:27:41.070918 tslearn-0.6.1/tslearn/backend/numpy_backend.py
+-rwxr-xr-x   0 tavenard_r   (504) staff       (20)     8782 2023-07-05 12:09:08.798395 tslearn-0.6.1/tslearn/backend/pytorch_backend.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.440894 tslearn-0.6.1/tslearn/barycenters/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1160 2021-01-05 10:39:33.337401 tslearn-0.6.1/tslearn/barycenters/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    26086 2021-01-06 07:38:50.170547 tslearn-0.6.1/tslearn/barycenters/dba.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1095 2023-01-20 12:41:18.661707 tslearn-0.6.1/tslearn/barycenters/euclidean.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3647 2023-01-20 12:41:18.662160 tslearn-0.6.1/tslearn/barycenters/softdtw.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      285 2021-01-05 10:39:33.339083 tslearn-0.6.1/tslearn/barycenters/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.443756 tslearn-0.6.1/tslearn/bases/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      120 2021-01-05 10:39:33.340758 tslearn-0.6.1/tslearn/bases/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7807 2021-01-05 10:39:33.447118 tslearn-0.6.1/tslearn/bases/bases.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.454896 tslearn-0.6.1/tslearn/clustering/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      611 2023-07-03 19:27:41.072334 tslearn-0.6.1/tslearn/clustering/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    31792 2023-07-03 19:27:41.072990 tslearn-0.6.1/tslearn/clustering/kmeans.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     9994 2021-01-07 10:45:54.581839 tslearn-0.6.1/tslearn/clustering/kshape.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8445 2023-01-20 12:41:18.662711 tslearn-0.6.1/tslearn/clustering/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.473097 tslearn-0.6.1/tslearn/datasets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      359 2023-01-20 12:41:18.662963 tslearn-0.6.1/tslearn/datasets/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2843 2021-01-05 10:39:33.344441 tslearn-0.6.1/tslearn/datasets/cached.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2274 2021-01-05 10:39:33.344827 tslearn-0.6.1/tslearn/datasets/datasets.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    13833 2023-07-03 18:23:27.324761 tslearn-0.6.1/tslearn/datasets/ucr_uea.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.475580 tslearn-0.6.1/tslearn/early_classification/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      525 2021-01-05 10:39:33.346065 tslearn-0.6.1/tslearn/early_classification/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    21713 2021-01-05 10:39:33.440889 tslearn-0.6.1/tslearn/early_classification/early_classification.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.480063 tslearn-0.6.1/tslearn/generators/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      210 2021-01-05 10:39:33.348452 tslearn-0.6.1/tslearn/generators/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3556 2021-01-05 10:39:33.440389 tslearn-0.6.1/tslearn/generators/generators.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.485602 tslearn-0.6.1/tslearn/hdftools/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)       81 2021-01-05 10:39:33.349590 tslearn-0.6.1/tslearn/hdftools/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4488 2023-01-20 12:41:18.663583 tslearn-0.6.1/tslearn/hdftools/hdftools.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.490325 tslearn-0.6.1/tslearn/matrix_profile/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      361 2021-01-05 10:39:33.350226 tslearn-0.6.1/tslearn/matrix_profile/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8825 2021-01-05 10:39:33.439263 tslearn-0.6.1/tslearn/matrix_profile/matrix_profile.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.545693 tslearn-0.6.1/tslearn/metrics/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2200 2023-07-03 19:27:41.073788 tslearn-0.6.1/tslearn/metrics/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    14019 2023-07-03 19:27:41.075224 tslearn-0.6.1/tslearn/metrics/ctw.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   375335 2021-01-06 07:40:59.972248 tslearn-0.6.1/tslearn/metrics/cycc.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4103 2023-01-20 12:41:18.664293 tslearn-0.6.1/tslearn/metrics/cycc.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   423280 2021-01-06 07:41:00.252084 tslearn-0.6.1/tslearn/metrics/cysax.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7323 2023-01-20 12:41:18.664522 tslearn-0.6.1/tslearn/metrics/cysax.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    82613 2023-07-03 19:27:41.076292 tslearn-0.6.1/tslearn/metrics/dtw_variants.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     2183 2023-07-03 19:27:41.076866 tslearn-0.6.1/tslearn/metrics/sax.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)   281647 2021-01-06 07:41:00.441314 tslearn-0.6.1/tslearn/metrics/soft_dtw_fast.c
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8199 2023-07-03 19:27:41.077390 tslearn-0.6.1/tslearn/metrics/soft_dtw_fast.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     5245 2023-07-03 19:27:41.077789 tslearn-0.6.1/tslearn/metrics/soft_dtw_loss_pytorch.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    26296 2023-07-03 19:27:41.078376 tslearn-0.6.1/tslearn/metrics/softdtw_variants.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3319 2023-07-03 19:27:41.079312 tslearn-0.6.1/tslearn/metrics/utils.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.548856 tslearn-0.6.1/tslearn/neighbors/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      348 2023-01-20 12:41:18.666986 tslearn-0.6.1/tslearn/neighbors/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    28740 2021-01-05 10:39:33.422420 tslearn-0.6.1/tslearn/neighbors/neighbors.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.589235 tslearn-0.6.1/tslearn/neural_network/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      415 2021-01-05 10:39:33.362297 tslearn-0.6.1/tslearn/neural_network/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     5509 2021-01-05 10:39:33.421725 tslearn-0.6.1/tslearn/neural_network/neural_network.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.674453 tslearn-0.6.1/tslearn/piecewise/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      419 2021-01-05 10:39:33.363393 tslearn-0.6.1/tslearn/piecewise/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    24187 2023-01-20 12:41:18.667327 tslearn-0.6.1/tslearn/piecewise/piecewise.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.728133 tslearn-0.6.1/tslearn/preprocessing/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      318 2021-01-05 10:39:33.365690 tslearn-0.6.1/tslearn/preprocessing/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8690 2021-01-05 10:39:33.419089 tslearn-0.6.1/tslearn/preprocessing/preprocessing.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.745494 tslearn-0.6.1/tslearn/shapelets/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      509 2023-07-03 19:27:41.080084 tslearn-0.6.1/tslearn/shapelets/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    33169 2023-07-03 19:27:41.080848 tslearn-0.6.1/tslearn/shapelets/shapelets.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.775015 tslearn-0.6.1/tslearn/svm/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      340 2021-01-05 10:39:33.368177 tslearn-0.6.1/tslearn/svm/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    20958 2023-07-03 19:27:41.081441 tslearn-0.6.1/tslearn/svm/svm.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.856944 tslearn-0.6.1/tslearn/tests/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)        0 2020-05-25 20:30:29.875851 tslearn-0.6.1/tslearn/tests/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    25004 2023-01-20 12:41:18.669171 tslearn-0.6.1/tslearn/tests/sklearn_patches.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3983 2020-05-25 20:30:29.876986 tslearn-0.6.1/tslearn/tests/test_barycenters.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8032 2021-01-05 10:39:33.369380 tslearn-0.6.1/tslearn/tests/test_clustering.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     8099 2023-07-05 12:09:08.799096 tslearn-0.6.1/tslearn/tests/test_estimators.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      721 2020-06-15 19:11:12.798796 tslearn-0.6.1/tslearn/tests/test_matrixprofile.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    24122 2023-07-05 12:09:08.799650 tslearn-0.6.1/tslearn/tests/test_metrics.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1994 2021-01-05 10:39:33.370832 tslearn-0.6.1/tslearn/tests/test_neighbors.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3698 2020-06-02 06:20:08.173618 tslearn-0.6.1/tslearn/tests/test_piecewise.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      508 2021-01-05 10:39:33.372803 tslearn-0.6.1/tslearn/tests/test_preprocessing.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     7750 2023-07-03 19:27:41.083347 tslearn-0.6.1/tslearn/tests/test_serialize_models.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     4205 2020-06-15 13:06:56.005238 tslearn-0.6.1/tslearn/tests/test_shapelets.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)      806 2023-07-03 19:27:41.084192 tslearn-0.6.1/tslearn/tests/test_svm.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3005 2021-01-05 10:39:33.374191 tslearn-0.6.1/tslearn/tests/test_utils.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     3620 2020-06-11 08:08:55.932129 tslearn-0.6.1/tslearn/tests/test_variablelength.py
+drwxr-xr-x   0 tavenard_r   (504) staff       (20)        0 2023-07-05 12:12:01.864995 tslearn-0.6.1/tslearn/utils/
+-rw-r--r--   0 tavenard_r   (504) staff       (20)     1605 2023-01-20 12:41:18.670358 tslearn-0.6.1/tslearn/utils/__init__.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    23572 2023-01-20 12:41:18.670786 tslearn-0.6.1/tslearn/utils/cast.py
+-rw-r--r--   0 tavenard_r   (504) staff       (20)    21371 2023-07-03 19:27:41.085116 tslearn-0.6.1/tslearn/utils/utils.py
```

### Comparing `tslearn-0.6.0/LICENSE` & `tslearn-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/PKG-INFO` & `tslearn-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tslearn
-Version: 0.6.0
+Version: 0.6.1
 Summary: A machine learning toolkit dedicated to time-series data
 Home-page: http://tslearn.readthedocs.io/
 Author: Romain Tavenard
 Author-email: romain.tavenard@univ-rennes2.fr
 License: BSD-2-Clause
 Project-URL: Source, https://github.com/tslearn-team/tslearn
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tslearn Version: 0.6.0 Summary: A machine learning
+Metadata-Version: 2.1 Name: tslearn Version: 0.6.1 Summary: A machine learning
 toolkit dedicated to time-series data Home-page: http://tslearn.readthedocs.io/
 Author: Romain Tavenard Author-email: romain.tavenard@univ-rennes2.fr License:
 BSD-2-Clause Project-URL: Source, https://github.com/tslearn-team/tslearn
 Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
 pytorch License-File: LICENSE
                                **** tslearn ****
```

### Comparing `tslearn-0.6.0/README.md` & `tslearn-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/conftest.py` & `tslearn-0.6.1/conftest.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/setup.py` & `tslearn-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/.cached_datasets/Trace.npz` & `tslearn-0.6.1/tslearn/.cached_datasets/Trace.npz`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/__init__.py` & `tslearn-0.6.1/tslearn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 __author__ = 'Romain Tavenard romain.tavenard[at]univ-rennes2.fr'
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __bibtex__ = r"""@article{JMLR:v21:20-091,
   author  = {Romain Tavenard and Johann Faouzi and Gilles Vandewiele and
              Felix Divo and Guillaume Androz and Chester Holtz and
              Marie Payne and Roman Yurchak and Marc Ru{\ss}wurm and
              Kushal Kolar and Eli Woods},
   title   = {Tslearn, A Machine Learning Toolkit for Time Series Data},
   journal = {Journal of Machine Learning Research},
```

### Comparing `tslearn-0.6.0/tslearn/backend/backend.py` & `tslearn-0.6.1/tslearn/backend/backend.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/backend/numpy_backend.py` & `tslearn-0.6.1/tslearn/backend/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/backend/pytorch_backend.py` & `tslearn-0.6.1/tslearn/backend/pytorch_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,238 +11,251 @@
 Bernhard Kainz, Claire Donnat, Susan Holmes and Xavier Pennec.
 Geomstats:  A Python Package for Riemannian Geometry in Machine Learning,
 Journal of Machine Learning Research, 2020, volume 21, number 223, pages 1-9,
 http://jmlr.org/papers/v21/19-027.html, https://github.com/geomstats/geomstats/
 """
 
 import numpy as _np
-import torch as _torch
 
+try:
+    import torch as _torch
 
-class PyTorchBackend(object):
-    """Class for the PyTorch  backend."""
-
-    def __init__(self):
-        self.backend_string = "pytorch"
-
-        self.linalg = PyTorchLinalg()
-        self.random = PyTorchRandom()
-        self.testing = PyTorchTesting()
-
-        self.int8 = _torch.int8
-        self.int16 = _torch.int16
-        self.int32 = _torch.int32
-        self.int64 = _torch.int64
-        self.float32 = _torch.float32
-        self.float64 = _torch.float64
-        self.complex64 = _torch.complex64
-        self.complex128 = _torch.complex128
-
-        self.abs = _torch.abs
-        self.any = _torch.any
-        self.arange = _torch.arange
-        self.argmax = _torch.argmax
-        self.argmin = _torch.argmin
-        self.dbl_max = _torch.finfo(_torch.double).max
-        self.ceil = _torch.ceil
-        self.diag = _torch.diag
-        self.empty = _torch.empty
-        self.exp = _torch.exp
-        self.eye = _torch.eye
-        self.floor = _torch.floor
-        self.full = _torch.full
-        self.hstack = _torch.hstack
-        self.inf = _torch.inf
-        self.is_array = _torch.is_tensor
-        self.isfinite = _torch.isfinite
-        self.isnan = _torch.isnan
-        self.log = _torch.log
-        self.max = _torch.max
-        self.mean = _torch.mean
-        self.median = _torch.median
-        self.min = _torch.min
-        self.nan = _torch.nan
-        self.pairwise_euclidean_distances = _torch.cdist
-        self.reshape = _torch.reshape
-        self.round = _torch.round
-        self.sum = _torch.sum
-        self.vstack = _torch.vstack
-        self.zeros = _torch.zeros
-        self.zeros_like = _torch.zeros_like
-
-    @staticmethod
-    def all(x, axis=None):
-        if not _torch.is_tensor(x):
-            x = _torch.tensor(x)
-        if axis is None:
-            return x.bool().all()
-        if isinstance(axis, int):
-            return _torch.all(x.bool(), axis)
-        if len(axis) == 1:
-            return _torch.all(x, *axis)
-        axis = list(axis)
-        for i_axis, one_axis in enumerate(axis):
-            if one_axis < 0:
-                axis[i_axis] = x.ndim() + one_axis
-        new_axis = tuple(k - 1 if k >= 0 else k for k in axis[1:])
-        return all(_torch.all(x.bool(), axis[0]), new_axis)
-
-    def array(self, val, dtype=None):
-        if _torch.is_tensor(val):
-            if dtype is None or val.dtype == dtype:
-                return val.clone()
-            return self.cast(val, dtype=dtype)
-
-        elif isinstance(val, _np.ndarray):
-            tensor = self.from_numpy(val)
-            if dtype is not None and tensor.dtype != dtype:
-                tensor = self.cast(tensor, dtype=dtype)
-
-            return tensor
-
-        elif isinstance(val, (list, tuple)) and len(val):
-            tensors = [self.array(tensor, dtype=dtype) for tensor in val]
-            return _torch.stack(tensors)
-
-        return _torch.tensor(val, dtype=dtype)
-
-    def cast(self, x, dtype):
-        if _torch.is_tensor(x):
-            return x.to(dtype=dtype)
-        return self.array(x, dtype=dtype)
-
-    @staticmethod
-    def cdist(x, y, metric="euclidean", p=None):
-        if metric == "euclidean":
-            return _torch.cdist(x, y)
-        if metric == "sqeuclidean":
-            return _torch.cdist(x, y) ** 2
-        if metric == "minkowski":
-            return _torch.cdist(x, y, p=p)
-        raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
-
-    @staticmethod
-    def copy(x):
-        return x.clone()
-
-    @staticmethod
-    def from_numpy(x):
-        return _torch.from_numpy(x)
-
-    @staticmethod
-    def iscomplex(x):
-        if isinstance(x, complex):
-            return True
-        return x.dtype.is_complex
-
-    @staticmethod
-    def is_float(x):
-        if isinstance(x, float):
-            return True
-        return x.dtype.is_floating_point
-
-    @staticmethod
-    def is_float32(x):
-        return isinstance(x, _torch.float32)
-
-    @staticmethod
-    def is_float64(x):
-        return isinstance(x, _torch.float64)
-
-    @staticmethod
-    def ndim(x):
-        return x.dim()
-
-    @staticmethod
-    def pairwise_distances(X, Y=None, metric="euclidean"):
-        if Y is None:
-            Y = X
-        if metric == "euclidean":
-            return _torch.cdist(X, Y)
-        if metric == "sqeuclidean":
-            return _torch.cdist(X, Y) ** 2
-        if callable(metric):
-            distance_matrix = _torch.zeros(X.shape[0], Y.shape[0])
-            for i in range(X.shape[0]):
-                for j in range(Y.shape[0]):
-                    distance_matrix[i, j] = metric(X[i, ...], Y[j, ...])
-            return distance_matrix
-        raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
-
-    @staticmethod
-    def pdist(x, metric="euclidean", p=None):
-        if metric == "euclidean":
-            return _torch.pdist(x)
-        if metric == "sqeuclidean":
-            return _torch.pdist(x) ** 2
-        if metric == "minkowski":
-            return _torch.pdist(x, p=p)
-        raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
-
-    def shape(self, data):
-        if not self.is_array(data):
-            data = self.array(data)
-        return tuple(_torch.Tensor.size(data))
-
-    def sqrt(self, x, out=None):
-        if not self.is_array(x):
-            x = self.array(x)
-        return _torch.sqrt(x, out=out)
-
-    @staticmethod
-    def to_numpy(x):
-        return x.detach().cpu().numpy()
-
-    @staticmethod
-    def tril(mat, k=0):
-        return _torch.tril(mat, diagonal=k)
-
-    @staticmethod
-    def tril_indices(n, k=0, m=None):
-        if m is None:
-            m = n
-        x = _torch.tril_indices(row=n, col=m, offset=k)
-        return x[0], x[1]
-
-    @staticmethod
-    def triu(mat, k=0):
-        return _torch.triu(mat, diagonal=k)
-
-    @staticmethod
-    def triu_indices(n, k=0, m=None):
-        if m is None:
-            m = n
-        x = _torch.triu_indices(row=n, col=m, offset=k)
-        return x[0], x[1]
-
-
-class PyTorchLinalg:
-    def __init__(self):
-        self.inv = _torch.linalg.inv
-        self.norm = _torch.linalg.norm
-
-
-class PyTorchRandom:
-    def __init__(self):
-        self.rand = _torch.rand
-        self.randint = _torch.randint
-        self.randn = _torch.randn
-
-    @staticmethod
-    def normal(loc=0.0, scale=1.0, size=(1,)):
-        if not hasattr(size, "__iter__"):
-            size = (size,)
-        return _torch.normal(mean=loc, std=scale, size=size)
-
-    @staticmethod
-    def uniform(low=0.0, high=1.0, size=(1,), dtype=None):
-        if not hasattr(size, "__iter__"):
-            size = (size,)
-        if low >= high:
-            raise ValueError("Upper bound must be higher than lower bound")
-        return (high - low) * _torch.rand(*size, dtype=dtype) + low
-
-
-class PyTorchTesting:
-    def __init__(self):
-        self.assert_allclose = _torch.allclose
-        self.assert_equal = _torch.testing.assert_close
+    HAS_TORCH = True
+except ImportError:
+    HAS_TORCH = False
+
+
+if not HAS_TORCH:
+
+    class PyTorchBackend:
+        def __init__(self):
+            raise ValueError(
+                "Could not use the PyTorch backend since torch is not installed"
+            )
+
+else:
+
+    class PyTorchBackend(object):
+        """Class for the PyTorch  backend."""
+
+        def __init__(self):
+            self.backend_string = "pytorch"
+
+            self.linalg = PyTorchLinalg()
+            self.random = PyTorchRandom()
+            self.testing = PyTorchTesting()
+
+            self.int8 = _torch.int8
+            self.int16 = _torch.int16
+            self.int32 = _torch.int32
+            self.int64 = _torch.int64
+            self.float32 = _torch.float32
+            self.float64 = _torch.float64
+            self.complex64 = _torch.complex64
+            self.complex128 = _torch.complex128
+
+            self.abs = _torch.abs
+            self.any = _torch.any
+            self.arange = _torch.arange
+            self.argmax = _torch.argmax
+            self.argmin = _torch.argmin
+            self.dbl_max = _torch.finfo(_torch.double).max
+            self.ceil = _torch.ceil
+            self.diag = _torch.diag
+            self.empty = _torch.empty
+            self.exp = _torch.exp
+            self.eye = _torch.eye
+            self.floor = _torch.floor
+            self.full = _torch.full
+            self.hstack = _torch.hstack
+            self.inf = _torch.inf
+            self.is_array = _torch.is_tensor
+            self.isfinite = _torch.isfinite
+            self.isnan = _torch.isnan
+            self.log = _torch.log
+            self.max = _torch.max
+            self.mean = _torch.mean
+            self.median = _torch.median
+            self.min = _torch.min
+            self.nan = _torch.nan
+            self.pairwise_euclidean_distances = _torch.cdist
+            self.reshape = _torch.reshape
+            self.round = _torch.round
+            self.sum = _torch.sum
+            self.vstack = _torch.vstack
+            self.zeros = _torch.zeros
+            self.zeros_like = _torch.zeros_like
+
+        @staticmethod
+        def all(x, axis=None):
+            if not _torch.is_tensor(x):
+                x = _torch.tensor(x)
+            if axis is None:
+                return x.bool().all()
+            if isinstance(axis, int):
+                return _torch.all(x.bool(), axis)
+            if len(axis) == 1:
+                return _torch.all(x, *axis)
+            axis = list(axis)
+            for i_axis, one_axis in enumerate(axis):
+                if one_axis < 0:
+                    axis[i_axis] = x.ndim() + one_axis
+            new_axis = tuple(k - 1 if k >= 0 else k for k in axis[1:])
+            return all(_torch.all(x.bool(), axis[0]), new_axis)
+
+        def array(self, val, dtype=None):
+            if _torch.is_tensor(val):
+                if dtype is None or val.dtype == dtype:
+                    return val.clone()
+                return self.cast(val, dtype=dtype)
+
+            elif isinstance(val, _np.ndarray):
+                tensor = self.from_numpy(val)
+                if dtype is not None and tensor.dtype != dtype:
+                    tensor = self.cast(tensor, dtype=dtype)
+
+                return tensor
+
+            elif isinstance(val, (list, tuple)) and len(val):
+                tensors = [self.array(tensor, dtype=dtype) for tensor in val]
+                return _torch.stack(tensors)
+
+            return _torch.tensor(val, dtype=dtype)
+
+        def cast(self, x, dtype):
+            if _torch.is_tensor(x):
+                return x.to(dtype=dtype)
+            return self.array(x, dtype=dtype)
+
+        @staticmethod
+        def cdist(x, y, metric="euclidean", p=None):
+            if metric == "euclidean":
+                return _torch.cdist(x, y)
+            if metric == "sqeuclidean":
+                return _torch.cdist(x, y) ** 2
+            if metric == "minkowski":
+                return _torch.cdist(x, y, p=p)
+            raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
+
+        @staticmethod
+        def copy(x):
+            return x.clone()
+
+        @staticmethod
+        def from_numpy(x):
+            return _torch.from_numpy(x)
+
+        @staticmethod
+        def iscomplex(x):
+            if isinstance(x, complex):
+                return True
+            return x.dtype.is_complex
+
+        @staticmethod
+        def is_float(x):
+            if isinstance(x, float):
+                return True
+            return x.dtype.is_floating_point
+
+        @staticmethod
+        def is_float32(x):
+            return isinstance(x, _torch.float32)
+
+        @staticmethod
+        def is_float64(x):
+            return isinstance(x, _torch.float64)
+
+        @staticmethod
+        def ndim(x):
+            return x.dim()
+
+        @staticmethod
+        def pairwise_distances(X, Y=None, metric="euclidean"):
+            if Y is None:
+                Y = X
+            if metric == "euclidean":
+                return _torch.cdist(X, Y)
+            if metric == "sqeuclidean":
+                return _torch.cdist(X, Y) ** 2
+            if callable(metric):
+                distance_matrix = _torch.zeros(X.shape[0], Y.shape[0])
+                for i in range(X.shape[0]):
+                    for j in range(Y.shape[0]):
+                        distance_matrix[i, j] = metric(X[i, ...], Y[j, ...])
+                return distance_matrix
+            raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
+
+        @staticmethod
+        def pdist(x, metric="euclidean", p=None):
+            if metric == "euclidean":
+                return _torch.pdist(x)
+            if metric == "sqeuclidean":
+                return _torch.pdist(x) ** 2
+            if metric == "minkowski":
+                return _torch.pdist(x, p=p)
+            raise ValueError(f"Metric {metric} not implemented in PyTorch backend.")
+
+        def shape(self, data):
+            if not self.is_array(data):
+                data = self.array(data)
+            return tuple(_torch.Tensor.size(data))
+
+        def sqrt(self, x, out=None):
+            if not self.is_array(x):
+                x = self.array(x)
+            return _torch.sqrt(x, out=out)
+
+        @staticmethod
+        def to_numpy(x):
+            return x.detach().cpu().numpy()
+
+        @staticmethod
+        def tril(mat, k=0):
+            return _torch.tril(mat, diagonal=k)
+
+        @staticmethod
+        def tril_indices(n, k=0, m=None):
+            if m is None:
+                m = n
+            x = _torch.tril_indices(row=n, col=m, offset=k)
+            return x[0], x[1]
+
+        @staticmethod
+        def triu(mat, k=0):
+            return _torch.triu(mat, diagonal=k)
+
+        @staticmethod
+        def triu_indices(n, k=0, m=None):
+            if m is None:
+                m = n
+            x = _torch.triu_indices(row=n, col=m, offset=k)
+            return x[0], x[1]
+
+    class PyTorchLinalg:
+        def __init__(self):
+            self.inv = _torch.linalg.inv
+            self.norm = _torch.linalg.norm
+
+    class PyTorchRandom:
+        def __init__(self):
+            self.rand = _torch.rand
+            self.randint = _torch.randint
+            self.randn = _torch.randn
+
+        @staticmethod
+        def normal(loc=0.0, scale=1.0, size=(1,)):
+            if not hasattr(size, "__iter__"):
+                size = (size,)
+            return _torch.normal(mean=loc, std=scale, size=size)
+
+        @staticmethod
+        def uniform(low=0.0, high=1.0, size=(1,), dtype=None):
+            if not hasattr(size, "__iter__"):
+                size = (size,)
+            if low >= high:
+                raise ValueError("Upper bound must be higher than lower bound")
+            return (high - low) * _torch.rand(*size, dtype=dtype) + low
+
+    class PyTorchTesting:
+        def __init__(self):
+            self.assert_allclose = _torch.allclose
+            self.assert_equal = _torch.testing.assert_close
```

### Comparing `tslearn-0.6.0/tslearn/barycenters/__init__.py` & `tslearn-0.6.1/tslearn/barycenters/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/barycenters/dba.py` & `tslearn-0.6.1/tslearn/barycenters/dba.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/barycenters/euclidean.py` & `tslearn-0.6.1/tslearn/barycenters/euclidean.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/barycenters/softdtw.py` & `tslearn-0.6.1/tslearn/barycenters/softdtw.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/bases/bases.py` & `tslearn-0.6.1/tslearn/bases/bases.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/clustering/__init__.py` & `tslearn-0.6.1/tslearn/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/clustering/kmeans.py` & `tslearn-0.6.1/tslearn/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/clustering/kshape.py` & `tslearn-0.6.1/tslearn/clustering/kshape.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/clustering/utils.py` & `tslearn-0.6.1/tslearn/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/datasets/cached.py` & `tslearn-0.6.1/tslearn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/datasets/datasets.py` & `tslearn-0.6.1/tslearn/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/datasets/ucr_uea.py` & `tslearn-0.6.1/tslearn/datasets/ucr_uea.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/early_classification/__init__.py` & `tslearn-0.6.1/tslearn/early_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/early_classification/early_classification.py` & `tslearn-0.6.1/tslearn/early_classification/early_classification.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/generators/generators.py` & `tslearn-0.6.1/tslearn/generators/generators.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/hdftools/hdftools.py` & `tslearn-0.6.1/tslearn/hdftools/hdftools.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/matrix_profile/matrix_profile.py` & `tslearn-0.6.1/tslearn/matrix_profile/matrix_profile.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/__init__.py` & `tslearn-0.6.1/tslearn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/ctw.py` & `tslearn-0.6.1/tslearn/metrics/ctw.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/cycc.c` & `tslearn-0.6.1/tslearn/metrics/cycc.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/cycc.py` & `tslearn-0.6.1/tslearn/metrics/cycc.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/cysax.c` & `tslearn-0.6.1/tslearn/metrics/cysax.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/cysax.py` & `tslearn-0.6.1/tslearn/metrics/cysax.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/dtw_variants.py` & `tslearn-0.6.1/tslearn/metrics/dtw_variants.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/sax.py` & `tslearn-0.6.1/tslearn/metrics/sax.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.c` & `tslearn-0.6.1/tslearn/metrics/soft_dtw_fast.c`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/soft_dtw_fast.py` & `tslearn-0.6.1/tslearn/metrics/soft_dtw_fast.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/soft_dtw_loss_pytorch.py` & `tslearn-0.6.1/tslearn/metrics/soft_dtw_loss_pytorch.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/softdtw_variants.py` & `tslearn-0.6.1/tslearn/metrics/softdtw_variants.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/metrics/utils.py` & `tslearn-0.6.1/tslearn/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/neighbors/neighbors.py` & `tslearn-0.6.1/tslearn/neighbors/neighbors.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/neural_network/neural_network.py` & `tslearn-0.6.1/tslearn/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/piecewise/piecewise.py` & `tslearn-0.6.1/tslearn/piecewise/piecewise.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/preprocessing/preprocessing.py` & `tslearn-0.6.1/tslearn/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/shapelets/shapelets.py` & `tslearn-0.6.1/tslearn/shapelets/shapelets.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/svm/svm.py` & `tslearn-0.6.1/tslearn/svm/svm.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/sklearn_patches.py` & `tslearn-0.6.1/tslearn/tests/sklearn_patches.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_barycenters.py` & `tslearn-0.6.1/tslearn/tests/test_barycenters.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_clustering.py` & `tslearn-0.6.1/tslearn/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_estimators.py` & `tslearn-0.6.1/tslearn/tests/test_estimators.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,19 @@
             if name.endswith('shapelets'):
                 # keras is likely not installed
                 warnings.warn('Skipped common tests for shapelets '
                               'as it could not be imported. keras '
                               '(and tensorflow) are probably not '
                               'installed!')
                 continue
+            elif name.endswith('pytorch_backend'):
+                # pytorch is likely not installed
+                continue
             else:
-                raise
+                raise Exception('Could not import module %s' % name)
 
         all_classes.extend(inspect.getmembers(module, inspect.isclass))
     return all_classes
 
 
 def is_abstract(c):
     if not(hasattr(c, '__abstractmethods__')):
```

### Comparing `tslearn-0.6.0/tslearn/tests/test_matrixprofile.py` & `tslearn-0.6.1/tslearn/tests/test_matrixprofile.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_metrics.py` & `tslearn-0.6.1/tslearn/tests/test_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import platform
 import sys
 
 import numpy as np
 import pytest
-import torch
-from scipy.spatial.distance import cdist
-
 import tslearn.clustering
 import tslearn.metrics
+from scipy.spatial.distance import cdist
 from tslearn.backend.backend import Backend
 from tslearn.metrics.dtw_variants import dtw_path
-from tslearn.metrics.soft_dtw_loss_pytorch import _SoftDTWLossPyTorch
 from tslearn.utils import to_time_series
 
 __author__ = "Romain Tavenard romain.tavenard[at]univ-rennes2.fr"
 
+try:
+    import torch
+    backends = ["numpy", "pytorch"]
+except ImportError:
+    backends = ["numpy"]
+
 
 def test_dtw():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         # dtw_path
         path, dist = tslearn.metrics.dtw_path([1, 2, 3], [1.0, 2.0, 2.0, 3.0], be=be)
         np.testing.assert_equal(path, [(0, 0), (1, 1), (1, 2), (2, 3)])
         np.testing.assert_allclose(dist, be.array([0.0]))
 
@@ -48,15 +50,14 @@
         )
         np.testing.assert_allclose(
             dists, be.array([[0.0, 2.44949], [1.0, 1.414214]]), atol=1e-5
         )
 
 
 def test_ctw():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         # ctw_path
         path, cca, dist = tslearn.metrics.ctw_path(
             [1, 2, 3], [1.0, 2.0, 2.0, 3.0], be=be
         )
         np.testing.assert_equal(path, [(0, 0), (1, 1), (1, 2), (2, 3)])
@@ -88,15 +89,14 @@
         )
         np.testing.assert_allclose(
             dists, be.array([[0.0, 2.44949], [1.0, 1.414214]]), atol=1e-5
         )
 
 
 def test_ldtw():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
 
         n1, n2, d = 15, 10, 3
         rng = np.random.RandomState(0)
         x = be.array(rng.randn(n1, d))
         y = be.array(rng.randn(n2, d))
@@ -136,15 +136,14 @@
         np.testing.assert_allclose(
             cost, tslearn.metrics.dtw_limited_warping_length(x, y, n1 + 2, be=be)
         )
         assert len(path) <= n1 + 2
 
 
 def test_lcss():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         sim = tslearn.metrics.lcss([1, 2, 3], [1.0, 2.0, 2.0, 3.0], be=be)
         np.testing.assert_equal(sim, 1.0)
 
         sim = tslearn.metrics.lcss([1, 2, 3], [1.0, 2.0, 2.0, 4.0], be=be)
         np.testing.assert_equal(sim, 1.0)
@@ -153,15 +152,14 @@
         np.testing.assert_equal(round(sim, 2), 0.67)
 
         sim = tslearn.metrics.lcss([1, 2, 3], [1.0, 2.0, 2.0, 2.0, 3.0], eps=0, be=be)
         np.testing.assert_equal(sim, 1.0)
 
 
 def test_lcss_path():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         path, sim = tslearn.metrics.lcss_path(
             [1.0, 2.0, 3.0], [1.0, 2.0, 2.0, 3.0], be=be
         )
         np.testing.assert_equal(sim, 1.0)
         np.testing.assert_equal(path, [(0, 1), (1, 2), (2, 3)])
@@ -182,15 +180,14 @@
             [1.0, 2.0, 3.0], [1.0, 2.0, 2.0, 2.0, 3.0], eps=0, be=be
         )
         np.testing.assert_equal(sim, 1.0)
         np.testing.assert_equal(path, [(0, 0), (1, 3), (2, 4)])
 
 
 def test_lcss_path_from_metric():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         for d in be.arange(1, 5):
             rng = np.random.RandomState(0)
             s1, s2 = rng.randn(10, d), rng.randn(30, d)
             s1, s2 = be.array(s1), be.array(s2)
 
@@ -221,15 +218,14 @@
                 dist_matrix, metric="precomputed", be=be
             )
             np.testing.assert_equal(path, path_ref)
             np.testing.assert_equal(sim, sim_ref)
 
 
 def test_constrained_paths():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         n, d = 10, 3
         rng = np.random.RandomState(0)
         x = rng.randn(n, d)
         y = rng.randn(n, d)
         x, y = be.array(x), be.array(y)
@@ -262,15 +258,14 @@
             global_constraint="itakura",
             itakura_max_slope=2.0,
             be=be,
         )
 
 
 def test_dtw_subseq():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
 
         path, dist = tslearn.metrics.dtw_subsequence_path(
             [2, 3], [1.0, 2.0, 2.0, 3.0, 4.0], be=be
         )
         np.testing.assert_allclose(path, [(0, 2), (1, 3)])
@@ -280,15 +275,14 @@
             [1, 4], [1.0, 2.0, 2.0, 3.0, 4.0], be=be
         )
         np.testing.assert_allclose(path, [(0, 2), (1, 3)])
         np.testing.assert_allclose(dist, np.sqrt(2.0))
 
 
 def test_dtw_subseq_path():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         subseq, longseq = [1, 4], [1.0, 2.0, 2.0, 3.0, 4.0]
         subseq = to_time_series(subseq, be=be)
         longseq = to_time_series(longseq, be=be)
         cost_matrix = tslearn.metrics.subsequence_cost_matrix(subseq, longseq, be=be)
 
@@ -296,15 +290,14 @@
         np.testing.assert_equal(path, [(0, 2), (1, 3)])
 
         path = tslearn.metrics.subsequence_path(cost_matrix, 1, be=be)
         np.testing.assert_equal(path, [(0, 0), (1, 1)])
 
 
 def test_masks():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         sk_mask = tslearn.metrics.sakoe_chiba_mask(4, 4, 1, be=be)
         reference_mask = be.array(
             [
                 [0.0, 0.0, be.inf, be.inf],
                 [0.0, 0.0, 0.0, be.inf],
@@ -403,15 +396,14 @@
         )
         np.testing.assert_allclose(
             estimator1.fit(time_series).labels_, estimator3.fit(time_series).labels_
         )
 
 
 def test_gak():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         # GAK
         g = tslearn.metrics.cdist_gak(
             [[1, 2, 2, 3], [1.0, 2.0, 3.0, 4.0]], sigma=2.0, be=be
         )
         np.testing.assert_allclose(
@@ -459,15 +451,14 @@
 
 @pytest.mark.skipif(
     (sys.version_info.major, sys.version_info.minor) == (3, 9)
     and "mac" in platform.platform().lower(),
     reason="Test failing for MacOS with python3.9 (Segmentation fault)",
 )
 def test_gamma_soft_dtw():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         dataset = be.array([[1, 2, 2, 3], [1.0, 2.0, 3.0, 4.0]])
         gamma = tslearn.metrics.gamma_soft_dtw(
             dataset=dataset, n_samples=200, random_state=0, be=be
         )
         np.testing.assert_allclose(gamma, 8.0)
@@ -475,15 +466,14 @@
 
 @pytest.mark.skipif(
     (sys.version_info.major, sys.version_info.minor) == (3, 9)
     and "mac" in platform.platform().lower(),
     reason="Test failing for MacOS with python3.9 (Segmentation fault)",
 )
 def test_symmetric_cdist():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         rng = np.random.RandomState(0)
         dataset = rng.randn(5, 10, 2)
         dataset = be.array(dataset)
         np.testing.assert_allclose(
             tslearn.metrics.cdist_dtw(dataset, dataset, be=be),
@@ -501,29 +491,27 @@
         np.testing.assert_allclose(
             tslearn.metrics.cdist_soft_dtw_normalized(dataset, dataset, be=be),
             tslearn.metrics.cdist_soft_dtw_normalized(dataset, be=be),
         )
 
 
 def test_lb_keogh():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         ts1 = [1, 2, 3, 2, 1]
         env_low, env_up = tslearn.metrics.lb_envelope(ts1, radius=1, be=be)
         np.testing.assert_allclose(
             env_low, be.array([[1.0], [1.0], [2.0], [1.0], [1.0]])
         )
         np.testing.assert_allclose(
             env_up, be.array([[2.0], [3.0], [3.0], [3.0], [2.0]])
         )
 
 
 def test_dtw_path_from_metric():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         rng = np.random.RandomState(0)
         s1, s2 = rng.rand(10, 2), rng.rand(30, 2)
         s1, s2 = be.array(s1), be.array(s2)
 
         # Use dtw_path as a reference
@@ -553,15 +541,14 @@
             dist_matrix, metric="precomputed", be=be
         )
         np.testing.assert_equal(path, path_ref)
         np.testing.assert_allclose(be.sqrt(dist), dist_ref)
 
 
 def test_softdtw():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         rng = np.random.RandomState(0)
         s1, s2 = rng.rand(10, 2), rng.rand(30, 2)
         s1, s2 = be.array(s1), be.array(s2)
 
         # Use dtw_path as a reference
@@ -574,15 +561,14 @@
         matrix_path, dist = tslearn.metrics.soft_dtw_alignment(s1, s2, gamma=0.0, be=be)
 
         np.testing.assert_equal(dist, dist_ref**2)
         np.testing.assert_allclose(matrix_path, mat_path_ref)
 
 
 def test_dtw_path_with_empty_or_nan_inputs():
-    backends = ["numpy", "pytorch"]
     for backend in backends:
         be = Backend(backend)
         s1 = be.zeros((3, 10))
         s2_empty = be.zeros((0, 10))
         with pytest.raises(ValueError) as excinfo:
             dtw_path(s1, s2_empty, be=be)
         assert (
@@ -594,17 +580,22 @@
         with pytest.raises(ValueError) as excinfo:
             dtw_path(s1, s2_nan, be=be)
         assert (
             str(excinfo.value)
             == "One of the input time series contains only nans or has zero length."
         )
 
-
+@pytest.mark.skipif(
+    len(backends) == 1,
+    reason="Skipping test that requires pytorch backend",
+)
 def test_soft_dtw_loss_pytorch():
     """Tests for the class SoftDTWLossPyTorch."""
+    from tslearn.metrics.soft_dtw_loss_pytorch import _SoftDTWLossPyTorch
+
     b = 5
     m = 10
     n = 12
     d = 8
     batch_ts_1 = torch.zeros((b, m, d), requires_grad=True)
     batch_ts_2 = torch.ones((b, n, d), requires_grad=True)
     soft_dtw_loss_pytorch = tslearn.metrics.SoftDTWLossPyTorch(
```

### Comparing `tslearn-0.6.0/tslearn/tests/test_neighbors.py` & `tslearn-0.6.1/tslearn/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_piecewise.py` & `tslearn-0.6.1/tslearn/tests/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_serialize_models.py` & `tslearn-0.6.1/tslearn/tests/test_serialize_models.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_shapelets.py` & `tslearn-0.6.1/tslearn/tests/test_shapelets.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_svm.py` & `tslearn-0.6.1/tslearn/tests/test_svm.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_utils.py` & `tslearn-0.6.1/tslearn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/tests/test_variablelength.py` & `tslearn-0.6.1/tslearn/tests/test_variablelength.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/utils/__init__.py` & `tslearn-0.6.1/tslearn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/utils/cast.py` & `tslearn-0.6.1/tslearn/utils/cast.py`

 * *Files identical despite different names*

### Comparing `tslearn-0.6.0/tslearn/utils/utils.py` & `tslearn-0.6.1/tslearn/utils/utils.py`

 * *Files identical despite different names*

