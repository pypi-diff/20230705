# Comparing `tmp/batorch-1.0.32.tar.gz` & `tmp/batorch-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batorch-1.0.32.tar", last modified: Fri Sep  9 14:37:25 2022, max compression
+gzip compressed data, was "batorch-1.0.33.tar", last modified: Wed Jul  5 06:46:33 2023, max compression
```

## Comparing `batorch-1.0.32.tar` & `batorch-1.0.33.tar`

### file list

```diff
@@ -1,63 +1,73 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.080989 batorch-1.0.32/
--rw-r--r--   0 admin      (501) staff       (20)     4301 2022-09-09 14:37:25.080854 batorch-1.0.32/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     3509 2022-09-09 14:37:24.000000 batorch-1.0.32/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.075351 batorch-1.0.32/batorch/
--rw-r--r--   0 admin      (501) staff       (20)     8678 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6984 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.076806 batorch-1.0.32/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186152 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.079651 batorch-1.0.32/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.080669 batorch-1.0.32/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2919 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20486 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106308 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    39679 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    21004 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2022-09-09 14:37:24.000000 batorch-1.0.32/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 14:37:25.075909 batorch-1.0.32/batorch.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     4301 2022-09-09 14:37:25.000000 batorch-1.0.32/batorch.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1512 2022-09-09 14:37:25.000000 batorch-1.0.32/batorch.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-09-09 14:37:25.000000 batorch-1.0.32/batorch.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       21 2022-09-09 14:37:25.000000 batorch-1.0.32/batorch.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2022-09-09 14:37:25.000000 batorch-1.0.32/batorch.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-09-09 14:37:25.081033 batorch-1.0.32/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     4175 2022-09-09 14:37:24.000000 batorch-1.0.32/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.601273 batorch-1.0.33/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-05 06:46:33.601137 batorch-1.0.33/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     3509 2023-07-05 06:46:33.000000 batorch-1.0.33/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.592966 batorch-1.0.33/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.594663 batorch-1.0.33/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.598368 batorch-1.0.33/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.599617 batorch-1.0.33/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.593651 batorch-1.0.33/batorch.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     4301 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1705 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       21 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       20 2023-07-05 06:46:33.000000 batorch-1.0.33/batorch.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:33.600841 batorch-1.0.33/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 06:46:31.000000 batorch-1.0.33/micomputing/trans.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 06:46:33.601320 batorch-1.0.33/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     4175 2023-07-05 06:46:33.000000 batorch-1.0.33/setup.py
```

### Comparing `batorch-1.0.32/PKG-INFO` & `batorch-1.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.32
+Version: 1.0.33
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.32/README.md` & `batorch-1.0.33/README.md`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/__init__.py` & `batorch-1.0.33/batorch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'batorch',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.31',
+    version = '1.0.32',
     contact = 'bertiezhou@163.com',
     keywords = ['torch', 'batch', 'batched data'],
     description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
-    requires = ['pycamia', 'torch', 'pynvml']
+    requires = ['pycamia', 'torch', 'pynvml'],
+    update = '2022-09-09 22:37:24'
 ).check()
 
 import torch
 distributed = torch.distributed
 autograd = torch.autograd
 random = torch.random
 optim = torch.optim
@@ -31,15 +32,15 @@
 nan = tensor(math.nan)
 inf = tensor(math.inf)
 pi = tensor(math.pi)
 
 from . import nn
 from .device import free_memory_amount, all_memory_amount
 from .tensor import CPU, GPU, GPUs, Tensor, Size, set_device, get_device, to_device, turn_on_autodevice, turn_off_autodevice, get_cpu_memory_used, get_gpu_memory_used, inv, diag, batch_tensor, channel_tensor, zeros, zeros_like, ones, ones_like, empty, empty_like, rand, rand_like, randn, randn_like, full, full_like, randint, randint_like, eye, eye_as, eye_like, cat, stack, t, unsqueeze, squeeze, tensor, tr, trace, bfloat16, bool, cdouble, cfloat, complex128, complex32, complex64, double, float, float16, float32, float64, half, int, int16, int32, int64, int8, long, qint32, qint8, quint8, short, uint8, BFloat16Storage, BoolStorage, ByteStorage, CharStorage, ComplexDoubleStorage, ComplexFloatStorage, DisableTorchFunction, DoubleStorage, FatalError, FloatStorage, HalfStorage, HalfStorageBase, IntStorage, JITException, LongStorage, QInt32Storage, QInt32StorageBase, QInt8Storage, QInt8StorageBase, QUInt8Storage, ShortStorage, Storage, device, dtype, enable_grad, finfo, iinfo, layout, memory_format, no_grad, qscheme, set_grad_enabled, Set, abs, abs_, absolute, acos, acos_, acosh, acosh_, adaptive_avg_pool1d, adaptive_max_pool1d, add, addbmm, addcdiv, addcmul, addmm, addmv, addmv_, addr, affine_grid_generator, align_tensors, all, allclose, alpha_dropout, alpha_dropout_, amax, amin, angle, any, arange, arccos, arccos_, arccosh, arccosh_, arcsin, arcsin_, arcsinh, arcsinh_, arctan, arctan_, arctanh, arctanh_, argmax, argmin, argsort, as_strided, as_strided_, as_tensor, asin, asin_, asinh, asinh_, atan, atan2, atan_, atanh, atanh_, atleast_1d, atleast_2d, atleast_3d, autocast_decrement_nesting, autocast_increment_nesting, avg_pool1d, baddbmm, bartlett_window, batch_norm, batch_norm_backward_elemt, batch_norm_backward_reduce, batch_norm_elemt, batch_norm_gather_stats, batch_norm_gather_stats_with_counts, batch_norm_stats, batch_norm_update_stats, bernoulli, bilinear, binary_cross_entropy_with_logits, bincount, binomial, bitwise_and, bitwise_not, bitwise_or, bitwise_xor, blackman_window, block_diag, bmm, broadcast_tensors, bucketize, can_cast, cartesian_prod, cdist, ceil, ceil_, celu, celu_, chain_matmul, channel_shuffle, cholesky, cholesky_inverse, cholesky_solve, choose_qparams_optimized, chunk, clamp, clamp_, clamp_max, clamp_max_, clamp_min, clamp_min_, clear_autocast_cache, clip, clip_, clone, combinations, compiled_with_cxx11_abi, complex, conj, constant_pad_nd, conv1d, conv2d, conv3d, conv_tbc, conv_transpose1d, conv_transpose2d, conv_transpose3d, convolution, cos, cos_, cosh, cosh_, cosine_embedding_loss, cosine_similarity, count_nonzero, cross, ctc_loss, cudnn_affine_grid_generator, cudnn_batch_norm, cudnn_convolution, cudnn_convolution_transpose, cudnn_grid_sampler, cudnn_is_acceptable, cummax, cummin, cumprod, cumsum, deg2rad, deg2rad_, dequantize, det, detach, detach_, diag_embed, diagflat, diagonal, digamma, dist, div, divide, dot, dropout, dropout_, dsmm, dstack, eig, einsum, embedding, embedding_bag, embedding_renorm_, empty_quantized, empty_strided, eq, equal, erf, erf_, erfc, erfc_, erfinv, exp, exp2, exp2_, exp_, expm1, expm1_, fake_quantize_per_channel_affine, fake_quantize_per_tensor_affine, fbgemm_linear_fp16_weight, fbgemm_linear_fp16_weight_fp32_activation, fbgemm_linear_int8_weight, fbgemm_linear_int8_weight_fp32_activation, fbgemm_linear_quantize_weight, fbgemm_pack_gemm_matrix_fp16, fbgemm_pack_quantized_matrix, feature_alpha_dropout, feature_alpha_dropout_, feature_dropout, feature_dropout_, fill_, fix, fix_, flatten, flip, fliplr, flipud, floor, floor_, floor_divide, fmod, fork, frac, frac_, frobenius_norm, from_file, from_numpy, gather, gcd, gcd_, ge, geqrf, ger, get_default_dtype, get_file_path, get_num_interop_threads, get_num_threads, get_rng_state, greater, greater_equal, grid_sampler, grid_sampler_2d, grid_sampler_3d, group_norm, gru, gru_cell, gt, hamming_window, hann_window, hardshrink, heaviside, hinge_embedding_loss, histc, hsmm, hspmm, hstack, hypot, i0, i0_, imag, import_ir_module, import_ir_module_from_buffer, index_add, index_copy, index_fill, index_put, index_put_, index_select, init_num_threads, initial_seed, instance_norm, int_repr, inverse, is_anomaly_enabled, is_autocast_enabled, is_complex, is_distributed, is_floating_point, is_grad_enabled, is_nonzero, is_same_size, is_signed, is_storage, is_tensor, is_vulkan_available, isclose, isfinite, isinf, isnan, isneginf, isposinf, isreal, istft, kaiser_window, kl_div, kthvalue, layer_norm, lcm, lcm_, le, lerp, less, less_equal, lgamma, linspace, load, lobpcg, log, log10, log10_, log1p, log1p_, log2, log2_, log_, log_softmax, logaddexp, logaddexp2, logcumsumexp, logdet, logical_and, logical_not, logical_or, logical_xor, logit, logit_, logspace, logsumexp, lstm, lstm_cell, lstsq, lt, lu, lu_solve, lu_unpack, manual_seed, margin_ranking_loss, masked_fill, masked_scatter, masked_select, matmul, matrix_exp, matrix_power, matrix_rank, max, max_pool1d, max_pool1d_with_indices, max_pool2d, max_pool3d, maximum, mean, median, merge_type_from_type_comment, meshgrid, min, minimum, miopen_batch_norm, miopen_convolution, miopen_convolution_transpose, miopen_depthwise_convolution, miopen_rnn, mkldnn_adaptive_avg_pool2d, mkldnn_convolution, mkldnn_convolution_backward_weights, mkldnn_max_pool2d, mkldnn_max_pool3d, mm, mode, movedim, mul, multinomial, multiply, mv, mvlgamma, nanquantile, nansum, narrow, native_batch_norm, native_group_norm, native_layer_norm, native_norm, ne, neg, neg_, negative, negative_, nextafter, nonzero, norm, norm_except_dim, normal, not_equal, nuclear_norm, numel, orgqr, ormqr, outer, pairwise_distance, parse_ir, parse_schema, parse_type_comment, pca_lowrank, pdist, pinverse, pixel_shuffle, poisson, poisson_nll_loss, polar, polygamma, pow, prelu, prepare_multiprocessing_environment, prod, promote_types, q_per_channel_axis, q_per_channel_scales, q_per_channel_zero_points, q_scale, q_zero_point, qr, quantile, quantize_per_channel, quantize_per_tensor, quantized_batch_norm, quantized_gru, quantized_gru_cell, quantized_lstm, quantized_lstm_cell, quantized_max_pool1d, quantized_max_pool2d, quantized_rnn_relu_cell, quantized_rnn_tanh_cell, rad2deg, rad2deg_, randperm, range, real, reciprocal, reciprocal_, relu, relu_, remainder, renorm, repeat_interleave, reshape, resize_as_, result_type, rnn_relu, rnn_relu_cell, rnn_tanh, rnn_tanh_cell, roll, rot90, round, round_, rrelu, rrelu_, rsqrt, rsqrt_, rsub, saddmm, save, scalar_tensor, scatter, scatter_add, searchsorted, seed, select, selu, selu_, set_anomaly_enabled, set_autocast_enabled, set_default_dtype, set_default_tensor_type, set_flush_denormal, set_num_interop_threads, set_num_threads, set_printoptions, set_rng_state, sgn, sigmoid, sigmoid_, sign, signbit, sin, sin_, sinh, sinh_, slogdet, smm, softmax, solve, sort, sparse_coo_tensor, split, split_with_sizes, spmm, sqrt, sqrt_, square, square_, sspaddmm, std, std_mean, stft, sub, subtract, sum, svd, svd_lowrank, symeig, take, tan, tan_, tanh, tanh_, tensordot, threshold, threshold_, topk, transpose, trapz, triangular_solve, tril, tril_indices, triplet_margin_loss, triu, triu_indices, true_divide, trunc, trunc_, unbind, unify_type_list, unique, unique_consecutive, unsafe_chunk, unsafe_split, unsafe_split_with_sizes, vander, var, var_mean, vdot, view_as_complex, view_as_real, vstack, wait, where, zero_ #**
-from .tensorfunc import crop_as, pad, decimal, divide, equals, matpow, matprod, dot, down_scale, gaussian_kernel, norm, norm2, Fnorm, Fnorm2, frobenius_norm, meannorm, meannorm2, mean_norm, mean_norm2, Jacobian, grad_image, image_grid, up_scale, one_hot, permute_space, skew_symmetric, cross_matrix, uncross_matrix, summary #*
+from .tensorfunc import crop_as, pad, decimal, divide, equals, matpow, matprod, dot, down_scale, gaussian_kernel, norm, norm2, Fnorm, Fnorm2, frobenius_norm, meannorm, meannorm2, mean_norm, mean_norm2, Jacobian, grad_image, image_grid, up_scale, one_hot, permute_space, skew_symmetric, cross_matrix, uncross_matrix, summary, display #*
 from .optimizer import CSGD, CADAM, Optimization, train, test #*
```

### Comparing `batorch-1.0.32/batorch/device.py` & `batorch-1.0.33/batorch/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     @property
     def working_devices(self):
         if self._working_devices is None:
             if self.auto: self.auto_select()
             else: self._working_devices = [d if isinstance(d, int) else (-1 if d.index is None else d.index) for d in self.default_devices]
         return self._working_devices
-    
+
     @alias("device_id")
     @property
     def main_device_id(self): return self.working_devices[0] if self.auto else -1
         
     @alias("device")
     @property
     def main_device(self): return device_by_id(self.main_device_id)
```

### Comparing `batorch-1.0.32/batorch/nn/_reduction.py` & `batorch-1.0.33/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/common_types.py` & `batorch-1.0.33/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/functional.py` & `batorch-1.0.33/batorch/nn/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 conv3d = torch.conv3d
 
 conv_transpose1d = torch.conv_transpose1d
 
 conv_transpose2d = torch.conv_transpose2d
 
+conv_transpose3d = torch.conv_transpose3d
+
 conv_tbc = torch.conv_tbc
 
 
 # Pooling
 avg_pool1d = torch.avg_pool1d
```

### Comparing `batorch-1.0.32/batorch/nn/grad.py` & `batorch-1.0.33/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/init.py` & `batorch-1.0.33/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/__init__.py` & `batorch-1.0.33/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/_functions.py` & `batorch-1.0.33/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/activation.py` & `batorch-1.0.33/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/adaptive.py` & `batorch-1.0.33/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/batchnorm.py` & `batorch-1.0.33/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/container.py` & `batorch-1.0.33/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/conv.py` & `batorch-1.0.33/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/distance.py` & `batorch-1.0.33/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/dropout.py` & `batorch-1.0.33/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/flatten.py` & `batorch-1.0.33/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/fold.py` & `batorch-1.0.33/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/instancenorm.py` & `batorch-1.0.33/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/linear.py` & `batorch-1.0.33/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/loss.py` & `batorch-1.0.33/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/module.py` & `batorch-1.0.33/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/normalization.py` & `batorch-1.0.33/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/padding.py` & `batorch-1.0.33/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/pixelshuffle.py` & `batorch-1.0.33/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/pooling.py` & `batorch-1.0.33/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/rnn.py` & `batorch-1.0.33/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/sparse.py` & `batorch-1.0.33/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/transformer.py` & `batorch-1.0.33/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/upsampling.py` & `batorch-1.0.33/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/modules/utils.py` & `batorch-1.0.33/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/parameter.py` & `batorch-1.0.33/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/clip_grad.py` & `batorch-1.0.33/batorch/nn/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/convert_parameters.py` & `batorch-1.0.33/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/fusion.py` & `batorch-1.0.33/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/memory_format.py` & `batorch-1.0.33/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/prune.py` & `batorch-1.0.33/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/rnn.py` & `batorch-1.0.33/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/spectral_norm.py` & `batorch-1.0.33/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/nn/utils/weight_norm.py` & `batorch-1.0.33/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/optimizer.py` & `batorch-1.0.33/batorch/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,29 +328,34 @@
     def optimizer(self, i):
         state_dict = self._optimizer.state_dict()
         for param_state_dict in state_dict['param_groups']:
             for k in self.hyper:
                 param_state_dict[k] = self.hyper[k](i)
         self._optimizer.load_state_dict(state_dict)
         return self._optimizer
+    
+    def new_iter(self):
+        optimizer = self.optimizer(self._index)
+        self._index += 1
+        return optimizer
             
     def minimize(self, loss, **kwargs):
         if callable(loss): self.loss.append((1, loss)); return
         optimizer = self.optimizer(self._index)
         optimizer.zero_grad()
         loss.backward(**kwargs)
         optimizer.step()
         self._index += 1
 
     def maximize(self, loss, **kwargs):
         if callable(loss): self.loss.append((-1, loss)); return
         optimizer = self.optimizer(self._index)
-        self.optimizer.zero_grad()
+        optimizer.zero_grad()
         (-loss).backward(**kwargs)
-        self.optimizer.step()
+        optimizer.step()
         self._index += 1
 
     @alias("optimize")
     def train(self, max_epoch=10, n_epoch_valid=1, n_batch=4):
         """
         Optimize the function [train the model] by this optimizer. 
         Warning: Requires Dataset element in package `micomputing`.
```

### Comparing `batorch-1.0.32/batorch/tensor.py` & `batorch-1.0.33/batorch/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,22 +192,22 @@
         for i, a in enumerate(args):
 
             if isinstance(a, list):
                 if batch_dim == ndim:
                     batch_dim = i
                 else:
                     raise TypeError("Only one batch dimension is allowed.")
-                raw_args.append(a[0])
+                raw_args.append(a[0] if len(a) > 0 else -1)
 
-            elif isinstance(a, set):
+            elif isinstance(a, (set, dict)):
                 if channel_dim == ndim:
                     channel_dim = i
                 else:
                     raise TypeError("Only one channel dimension is allowed.")
-                raw_args.append(list(a)[0])
+                raw_args.append(list(a)[0] if len(a) > 0 else -1)
 
             else: raw_args.append(a)
 
         self = super().__new__(cls, raw_args)
         self.ndim = ndim
         return self.set_special_(kwargs.get('batch_dim', batch_dim), kwargs.get('channel_dim', channel_dim))
 
@@ -665,15 +665,15 @@
                 self = super()._make_subclass(cls, arg, rg)
                 if dev != cpu: self = self.to(dev)
                 return self.set_special_(batch_dim, channel_dim)
             elif hasattr(arg, '__tensor__'): return arg.__tensor__()
             elif hasattr(arg, 'shape') or isinstance(arg, list):
                 rg = kwargs.get('requires_grad', getattr(arg, 'requires_grad', False))
                 self = super().__new__(cls, arg)
-                if dev != cpu: self = self.to(dev)
+                avouch(self.device == cpu)
                 self.requires_grad = rg
                 self.special_from_(arg)
                 return self.set_special_(batch_dim, channel_dim)
             elif isinstance(arg, tuple): args = arg
             else: raise TypeError(f"Unrecognized initialization of 'Tensor': {arg}. ")
 
         # args is a tuple of integers (or a Size)
@@ -1385,14 +1385,16 @@
 
         new_size = self.shape[:source] + size + self.shape[source + 1:]
         prod = 1
         ni = None
         for i, x in enumerate(size):
             if isinstance(x, list) and len(x) == 1: x = x[0]
             elif isinstance(x, set) and len(x) == 1: x = list(x)[0]
+            elif isinstance(x, list) and len(x) == 0: x = -1
+            elif isinstance(x, dict) and len(x) == 0: x = -1
             if x != -1: prod *= x; continue
             ni = i
         if ni is not None:
             x = self.shape[source] // prod
             if size.batch_dimension == ni: x = [x]
             elif size.channel_dimension == ni: x = {x}
             new_size = new_size[:source + ni] + bt.Size(x) + new_size[source + ni + 1:]
@@ -1589,15 +1591,16 @@
                 res = super(torch.Tensor, self.view(sa + space1[-2:])).__matmul__(other.view(sb + space2[-2:]))
             if rem: res.squeeze_(-1)
             if rem and res.size(-1) == 1: res.squeeze_(-1)
             return res.as_subclass(Tensor).special_from_(sa)
         return super().__matmul__(other, **kwargs).as_subclass(Tensor).special_from_()
 
     def __op__(self, opname, other, **kwargs):
-        if not isinstance(other, Tensor): other = tensor(other)
+        if not isinstance(other, torch.Tensor): other = tensor(other, device=self.device)
+        elif not isinstance(other, Tensor): other = other.as_subclass(Tensor)
         if self.has_special and len(other.shape) > 0 or other.has_special:
             a, b = self.shape ^ other.shape
             with torch._C.DisableTorchFunction():
                 res = getattr(super(Tensor, self.view(a).as_subclass(Tensor)), opname)(other.view(b))
             return res.as_subclass(Tensor).special_from_(a)
         sp = None
         if self.has_special: sp = self
@@ -1669,17 +1672,21 @@
             string = string.rstrip(')') + f', shape={self.shape})'
         return string.replace("tensor", "Tensor")
 
     def __hash__(self): return super().__hash__()
     
     @property
     def grad(self):
-        g = super().grad
+        g = getattr(self, '_grad_override', super().grad)
         if not isinstance(g, torch.Tensor): return g
         return g.as_subclass(Tensor).special_from_(self)
+    
+    @grad.setter
+    def grad(self, value):
+        self._grad_override = value
 
     @staticmethod
     def __torch_function_convert__(ret, cls):
         with torch._C.DisableTorchFunction():
             if isinstance(ret, torch.Tensor):
                 ret = ret.as_subclass(cls)
             if isinstance(ret, (tuple, list)):
@@ -2299,15 +2306,16 @@
     elif isinstance(dim, dict) and len(dim) == 0:
         avouch(ALL([x.has_channel for x in list_of_tensors]), "Tensors can only be concatenated along channel dimension when all of them have one. ")
         dim = pivot.channel_dim; ichannel = dim
     elif isinstance(dim, INT): pass
     else: raise TypeError(f"Not identified dimension for concatenation: {dim}.")
     if dim < 0: dim += list_of_tensors[0].ndim
     self = [t for t in list_of_tensors if isinstance(t, Tensor)]
-    if len(self) == 0: return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_().set_special_(batch_dim=ibatch, channel_dim=ichannel)
+    if len(list_of_tensors) == 0: return torch.tensor([]).as_subclass(Tensor)
+    elif len(self) == 0: return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_().set_special_(batch_dim=ibatch, channel_dim=ichannel)
     return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_(self[0]).set_special_(batch_dim=ibatch, channel_dim=ichannel)
 
 def stack(*list_of_tensors, dim=None, **kwargs) -> Tensor:
     if dim is None:
         if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], torch.Tensor):
             dim = list_of_tensors[-1]
             list_of_tensors = list_of_tensors[:-1]
@@ -2379,18 +2387,14 @@
     if isinstance(device, AutoDevice): device = device.device
     if isinstance(data, (INT, FLOAT)):
         out = torch.tensor(data, device=device, requires_grad=requires_grad).as_subclass(Tensor).special_from_()
     elif isinstance(data, Tensor):
         out = data.clone()
     elif isinstance(data, torch.Tensor):
         out = data.as_subclass(Tensor).special_from_()
-    elif 'numpy' in str(type(data)):
-        import numpy as np
-        if 'uint' in str(data.dtype): data = data.astype(np.uint8)
-        out = Tensor(data, device=device, requires_grad=requires_grad)
     else: out = Tensor(data, device=device, requires_grad=requires_grad)
     if batch_dim is not None: out.batch_dim = batch_dim
     if channel_dim is not None: out.channel_dim = channel_dim
     return out
 
 def batch_tensor(*args, **kwargs) -> Tensor:
     if len(args) == 1 and not isinstance(args[0], (INT, FLOAT)): args = args[0]
```

### Comparing `batorch-1.0.32/batorch/tensor2.py` & `batorch-1.0.33/batorch/tensor2.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,27 +24,28 @@
     inv
     diag
     batch_tensor
     channel_tensor
 """.split()
 
 import builtins, sys
+from collections import defaultdict
 from functools import wraps
 from typing import Generator
 from .tensorfunc import __all__ as tf_list
 from .torch_namespace import *
 from .device import GB, CPU, GPU, GPUs, AutoDevice, FixedDevice
 
 with __info__:
     import torch
     import batorch as bt
     from pycamia import ByteSize
     from pycamia import avouch, touch, alias, execblock, void
-    from pycamia import get_alphas, arg_tuple, max_argmax
-    from pycamia import argmax as _argmax, item, to_list
+    from pycamia import get_alphas, arg_extract, max_argmax
+    from pycamia import argmax as _argmax, item, to_list, tokenize, identity_function
     from pyoverload import Type, Array, isoftype, Iterable
 
 _int = builtins.int
 _min = builtins.min
 _max = builtins.max
 _abs = builtins.abs
 _any = builtins.any
@@ -64,14 +65,17 @@
     squeeze squeeze_ transpose transpose_ movedim movedim_ splitdim repeated amplify ample sample pick split flip
     cummin cummax cumsum cumprod sum prod min max median mean std argmin argmax
 """.split()
 one_dim_methods_last = """multiply multiple repeated amplify ample sample split flip""".split()
 one_dim_methods_first = """splitdim""".split()
 avouch(all(x in new_dim_methods for x in new_dim_inherit_methods))
 
+with open(__file__) as fp:
+    __mirror__ = [None] + fp.read().split('\n')
+
 def set_device(device):
     if isinstance(device, AutoDevice): new_device = device
     elif isinstance(device, torch.device): new_device = FixedDevice(device)
     else: raise TypeError("Invalid device type. ")
     global _device
     _device = new_device
 
@@ -122,32 +126,38 @@
         n_sequence_dim = kwargs.get("n_sequence_dim", 0)
         avouch(isinstance(with_batch, bool), f"Invalid initialization of bt.Size (non bool argument 'with_batch': {type(with_batch)}; If you did not input it manually, reach out for developers with Error Code: B522).")
         avouch(isinstance(n_sequence_dim, int), f"Invalid initialization of bt.Size (non int argument 'n_sequence_dim': {type(n_sequence_dim)}; If you did not input it manually, reach out for developers with Error Code: B523).")
         avouch(feature_range is None or isinstance(feature_range, list) and len(feature_range) == 2, f"Invalid initialization of bt.Size (non list argument 'feature_range': {type(feature_range)}; If you did not input it manually, reach out for developers with Error Code: B524).")
         input_feature = feature_range is not None
 
         raw_size = []
+        began_sequence = False
         for i, x in enumerate(shape):
-            # time/sequence dimension
-            if isinstance(x, list) and len(x) == 1 and isinstance(x[0], list):
-                if len(x[0]) > 0: raw_size.extend(x[0]); n_sequence_dim += len(x[0])
-                else: n_sequence_dim += 1; raw_size.append(-1)
+            # time/sequence dimensions
+            if x == ...:
+                avouch(not began_sequence, f"Invalid initialization of bt.Size (more than one conflict ellipsis): {shape}.")
+                began_sequence = True
+                avouch(n_sequence_dim == 0, f"Invalid initialization of bt.Size (positive n_sequence_dim conflicts with '...' expression): {shape}.")
                 continue
-            avouch(n_sequence_dim == 0, f"Invalid initialization of bt.Size (sequence dimensions can only be the last dimensions): {shape}.")
+            # normal/space dimensions
             if isinstance(x, _int):
-                avouch(x >= -1, "Invalid initialization of bt.Size (Size cannot have negative values except -1 indicating an arbitrary number): {shape}.")
-                raw_size.append(x); continue
-            # batch dimension
+                avouch(x >= -1, f"Invalid initialization of bt.Size (Size cannot have negative values except -1 indicating an arbitrary number): {shape}.")
+                raw_size.append(x)
+                if began_sequence: n_sequence_dim += 1
+                continue
+            if began_sequence:
+                avouch(None, f"Invalid initialization of bt.Size (no special dimension is allowed in time dimensions): {shape}.")
+            # batch dimensions
             if isinstance(x, dict) and len(x) == 0:
                 avouch(i == 0, f"Invalid initialization of bt.Size (batch dimension can only be the first dimension): {shape}.")
                 raw_size.append(-1); with_batch = True; continue
             if isinstance(x, set) and len(x) == 1:
                 avouch(i == 0, f"Invalid initialization of bt.Size (batch dimension can only be the first dimension): {shape}.")
                 raw_size.append(x.pop()); with_batch = True; continue
-            # feature dimension
+            # feature dimensions
             if feature_range is not None: i += feature_range[1] - feature_range[0] - 1
             if isinstance(x, list):
                 avouch(feature_range is None or feature_range[1] == 0 or feature_range[1] == i, f"Invalid initialization of bt.Size (feature dimensions should be neighboring dimensions): {shape}.")
                 avouch(all([isinstance(y, _int) for y in x]), f"Invalid initialization of bt.Size (representation for feature dimensions should be a list of integers): {shape}.")
                 if len(x) == 0: raw_size.append(-1); len_feat = 1
                 else: raw_size.extend(x); len_feat = len(x)
                 if feature_range is None: feature_range = [i, i + len_feat]
@@ -428,34 +438,38 @@
     ## all dimensions:
     @alias("nele")
     @property
     def n_ele(self):
         p = 1
         for i in range(self.n_dim): p *= self[i]
         return p
+    
+    def transpose(self, i, j):
+        if i > j: i, j = j, i
+        return self[:i] + self[j:j+1] + self[i+1:j] + self[i:i+1] + self[j+1:]
 
     ## methods:
     @alias("clone")
     def copy(self): return Size(self)
 
     @alias("raw")
     def tuple(self): return tuple(self)
 
     @property
     def python_repr(self):
-        batch = {self[0]}
+        batch = set(list(self[:self.with_batch]))
         feature = list(self[self.feature_start: self.feature_stop])
-        sequence = [list(self[self.sequence_start:])]
+        sequence = (...,) + tuple(self[self.sequence_start:])
         return (((batch,) if self.with_batch else tuple()) + self[self.n_batch_dim: self.feature_start] + 
-                ((feature,) if len(feature) > 0 else tuple()) + self[self.feature_stop: self.sequence_start] + ((sequence,) if self.n_sequence_dim > 0 else tuple())).tuple()
+                ((feature,) if len(feature) > 0 else tuple()) + self[self.feature_stop: self.sequence_start] + (sequence if self.n_sequence_dim > 0 else tuple())).tuple()
 
     @alias("__repr__")
     def __str__(self):
         rep = self.python_repr
-        return f"batorch.Size{rep}".replace(',)', ')')
+        return f"batorch.Size{rep}".replace(',)', ')').replace('Ellipsis', '...')
     
     ## operations:
     def __getitem__(self, k):
         if isinstance(k, _int): return super().__getitem__(k)
         avouch(isinstance(k, slice), f"Slicing of 'bt.Size' only takes integers or slices, not {k}. ")
         s, e = k.start, k.stop
         if s is None: s = 0
@@ -547,15 +561,15 @@
         if not self.has_batch and other.has_batch: self, other = other, self; swap = True
         if self.has_batch and not other.has_batch: other = Size({1}) + other
         if swap: self, other = other, self
         
         # sequence:
         swap = False
         if not self.has_sequence and other.has_sequence: self, other = other, self; swap = True
-        if self.has_sequence and not other.has_sequence: other = other + Size([[1] * self.n_sequence_dim])
+        if self.has_sequence and not other.has_sequence: other = other + Size((...,) + (1,) * self.n_sequence_dim)
         if swap: self, other = other, self
         avouch(self.n_sequence_dim == other.n_sequence_dim, f"Mismatched sequence dimensions: {self.sequence} and {other.sequence}.")
         
         # feature:
         swap = False
         if not self.has_feature and other.has_feature: self, other = other, self; swap = True
         if self.has_feature and not other.has_feature:
@@ -576,110 +590,154 @@
         swap = False
         if self.right_space_dim == 0 and other.right_space_dim > 0: self, other = other, self; swap = True
         if self.right_space_dim > 0 and other.right_space_dim == 0: other = other[:other.feature_stop] + Size((1,) * self.right_space_dim) + other[other.feature_stop:]
         if swap: self, other = other, self
         avouch(self.right_space_dim == other.right_space_dim, f"Mismatched space dimensions: {self.space} and {other.space}.")
         
         return self, other
-            
-        # avouch(self.with_batch and other.has_feature or self.has_feature and other.with_batch, f"Inner problem: 'bt.Size.__xor__' failed to match sizes {self} and {other}. Please contact the developers for more information (Error Code: B529). ")
-        # if isinstance(other, Size) and not self.has_special: self, other = other, self
-        # if not isinstance(other, Size) or not other.has_special:
-        #     if len(other) == self.n_dim: pass
-        #     elif len(other) == self.n_space_dim: other = ((1,) if self.with_batch else tuple()) + other[:self.feature_start - self.n_batch_dim] + (1,) * self.n_feature_dim + other[self.feature_start - self.n_batch_dim:]
-        #     elif len(other) == self.n_feature_dim: other = (1,) * self.feature_start + other + (1,) * (self.n_dim - self.n_feature_dim - self.feature_start)
-        #     elif len(other) == self.n_dim - 1 and self.with_batch: other = (1,) + other
-        #     else: avouch(None, f"Cannot match Sizes: tuple {other} to {self}")
-        #     return self, other
-        # if self.has_feature and other.has_feature:
-        #     avouch(self.n_feature_dim == other.n_feature_dim, f"Cannot match Sizes with different feature size: {self} and {other}")
-        #     if self.right_space_dim == 0 and other.left_space_dim == 0: other = other[:_int(other.with_batch)] + other[other.feature_stop:] + other.feature
-        #     if other.right_space_dim == 0 and self.left_space_dim == 0: other = other[:_int(other.with_batch)] + other.feature + other[_int(other.with_batch):other.feature_start]
-        #     if self.left_space_dim > 1 and other.left_space_dim == 1 and not other.with_batch: other.with_batch_(True)
-        #     if other.left_space_dim > 1 and self.left_space_dim == 1 and not self.with_batch: self.with_batch_(True)
-        #     if self.left_space_dim == 0: self = self[:self.n_batch_dim] + (1,) * other.left_space_dim + self[self.n_batch_dim:]
-        #     if other.left_space_dim == 0: other = other[:_int(other.with_batch)] + (1,) * self.left_space_dim + other[_int(other.with_batch):]
-        #     if self.right_space_dim == 0: self = self + (1,) * other.right_space_dim
-        #     if other.right_space_dim == 0: other = other + (1,) * self.right_space_dim
-        #     if self.left_space_dim == other.left_space_dim + 1 and not self.with_batch: self.with_batch_(True)
-        #     if other.left_space_dim == self.left_space_dim + 1 and not other.with_batch: other.with_batch_(True)
-        #     avouch(self.left_space_dim == other.left_space_dim and self.right_space_dim == other.right_space_dim, f"Inner problem: 'bt.Size.__xor__' failed to match sizes {self} and {other}. Please contact the developers for more information (Error Code: B528). ")
-        #     if self.with_batch and not other.with_batch: other = ((1,) + other).with_batch_(True)
-        #     if not self.with_batch and other.with_batch: self = ((1,) + self).with_batch_(True)
-        #     avouch(self.with_batch == other.with_batch, "Inner problem: if 'bt.Size.__xor__' is not called manually, please contact the developers with Error Code: B527")
-        #     return self, other
-        # if not self.has_feature and not other.has_feature:
-        #     if self.n_space_dim > 1 and other.n_space_dim == 1 and not other.with_batch: other.with_batch_(True)
-        #     if other.n_space_dim > 1 and self.n_space_dim == 1 and not self.with_batch: self.with_batch_(True)
-        #     if self.n_space_dim == 0: self = self + (1,) * other.n_space_dim
-        #     if other.n_space_dim == 0: other = other + (1,) * self.n_space_dim
-        #     if self.n_space_dim == other.n_space_dim + 1 and not self.with_batch: self.with_batch_(True)
-        #     if other.n_space_dim == self.n_space_dim + 1 and not other.with_batch: other.with_batch_(True)
-        #     avouch(self.n_space_dim == other.n_space_dim, f"Inner problem: 'bt.Size.__xor__' failed to match sizes {self} and {other}. Please contact the developers for more information (Error Code: B528). ")
-        #     if self.with_batch and not other.with_batch: other = ((1,) + other).with_batch_(True)
-        #     if not self.with_batch and other.with_batch: self = ((1,) + self).with_batch_(True)
-        #     avouch(self.with_batch == other.with_batch, "Inner problem: if 'bt.Size.__xor__' is not called manually, please contact the developers with Error Code: B527")
-        #     return self, other
-        # if self.with_batch == other.with_batch:
-        #     self_right, other_right = self[self.n_batch_dim:] ^ other[_int(other.with_batch):]
-        #     return self[:self.n_batch_dim] + self_right, other[:_int(other.with_batch)] + other_right
-        # avouch(self.with_batch and other.has_feature or self.has_feature and other.with_batch, f"Inner problem: 'bt.Size.__xor__' failed to match sizes {self} and {other}. Please contact the developers for more information (Error Code: B529). ")
-        # avouch(None, "bt.Size.__xor__ does not accept two sizes with batch in one of them and feature in the other. ")
-
-def tensor(data, *, dtype=None, device=None, requires_grad=False, pin_memory=False): ...
-def as_tensor(data, dtype=None, device=None): ...
-def empty(*size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False, pin_memory=False, memory_format=torch.contiguous_format): ...
-def ones(*size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False): ...
-def zeros(*size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False): ...
-def empty_like(input, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
-def ones_like(input, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
-def zeros_like(input, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
+
+size_mapping = defaultdict(lambda: identity_function,
+)
+
+def get_updated_code(func, mode='function'):
+    line_no = func.__code__.co_firstlineno
+    declaration = __mirror__[line_no].strip()
+    if declaration.startswith('@'): avouch(None, "Internal error: no decorator is allowed for auto generated functions in batorch.tensor (Please contact the developer with Error Code: B531). ")
+    _def, _fname, _args, *_tail = tokenize(declaration, sep=[' ', '(', ')', '\n'])
+    inner_codes = ""
+    if not _tail[-1] in ('...', 'pass'):
+        l = line_no
+        indent = __mirror__[l].split('def')[0]
+        inner_codes = [''] # Due to the indent issue, a blank line was added at the front. 
+        while True:
+            l += 1
+            line = __mirror__[l]
+            if line.strip() and line.split('def')[0] == indent:
+                break
+            inner_line = line[len(indent):]
+            if inner_line.strip().startswith('return'):
+                inner_line = inner_line.replace('return', 'obj =')
+            if inner_line.startswith('\t'):
+                count = 0
+                for x in inner_line:
+                    if x != '\t': break
+                    count += 1
+                inner_line = '    ' * count + inner_line.strip('\t')
+            inner_line = '    ' + inner_line
+            inner_codes.append(inner_line)
+        inner_codes = '\n'.join(inner_codes)
+    ant = func.__annotations__
+    tensor_args = []
+    size_args = []
+    for a, t in ant.items():
+        if t == 'Tensor': tensor_args.append(a)
+        if t == Size: size_args.append(a)
+    parts = []
+    for x in _args.split(','):
+        x = x.strip()
+        if x == '*': continue
+        if ':' in x: x = x.split(':')[0]
+        if '=' not in x: parts.append(x); continue
+        param = x.split('=', 1)[0]
+        parts.append(param + '=' + param.strip())
+    if mode == 'method': x, *parts = parts
+    inherit_args = ','.join(parts)
+
+    reshape_op = ""
+    if len(tensor_args) >= 2:
+        x = tensor_args[0]
+        reshape_op = [f"x_shape = {x}.shape"]
+        for y in tensor_args[1:]:
+            reshape_op.append(f"x_shape, y_shape = x_shape ^ {y}.shape")
+            reshape_op.append(f"{y} = {y}.view(y_shape)")
+        for y in tensor_args[1:-1]:
+            reshape_op.append(f"_, y_shape = x_shape ^ {y}.shape")
+            reshape_op.append(f"{y} = {y}.view(y_shape)")
+        reshape_op.append(f"{x} = {x}.view(x_shape)")
+        reshape_op = '; '.join(reshape_op)
+    cast = '; '.join([f"{x} = torch.tensor({x}) if not isinstance({x}, torch.Tensor) else {x}; {x} = {x}.as_subclass(Tensor).with_shape({x}.shape) if not isinstance({x}, Tensor) else {x}" for x in tensor_args])
+    get_size = '; '.join([f"{x}_shape={x}.shape" for x in tensor_args] + [f'{x}={x}[0] if isinstance({x}, tuple) and isinstance({x}[0], Size) else Size({x})' for x in size_args])
+    if len(tensor_args) >= 2:
+        size_reference = "x_shape"
+    else:
+        size_reference = ', '.join([f'{x}_shape' for x in tensor_args] + size_args)
+        size_reference = f"size_mapping['{func.__name__}']({size_reference})"
+    parent = f'super(Tensor, {x})' if mode == 'method' else 'torch'
+    if not inner_codes: inner_codes = f"obj = {parent}.{_fname}({inherit_args})"
+    if '.with_shape' not in inner_codes:
+        inner_codes += f"\n        obj = obj.as_subclass(Tensor).with_shape({size_reference})"
+    return f"""
+    {_def} {_fname}({_args}, with_batch=None, feature_range=void, n_sequence_dim=0):
+        {cast} # Cast all arguments to the 'Tensor' or 'Size' type as we want. 
+        {reshape_op} # For '__operations__', reshape all the available tensors to a same size. 
+        {get_size} # Obtain available sized in arguments (which will be fed into size function). 
+        {inner_codes} # Use the given inner codes if they are provided. 
+        if with_batch is not None: obj.with_batch = with_batch
+        if feature_range is not void: obj.feature_range = feature_range
+        if n_sequence_dim != 0: obj.n_sequence_dim = n_sequence_dim
+        return obj
+    """
 
 class Tensor(torch.Tensor):
     
     @staticmethod
-    def _make_subclass(cls, torch_tensor, requires_grad=None, device=None, with_batch=None, feature_range=void, **_):
+    def _make_subclass(cls, torch_tensor, requires_grad=None, device=None, with_batch=None, feature_range=void, n_sequence_dim=0, **_):
         avouch(not _, "bt.Tensor only accept keyword arguments requires_grad, device, with_batch and feature_range")
         if device is not None and torch_tensor.device != device:
             avouch(isinstance(device, AutoDevice), "Please use `AutoDevice` in batorch.Tensor._make_subclass. Please contact the developers if you did not use Tensor._make_subclass directly (Error Code: B530). ")
             torch_tensor = device(torch_tensor)
         if isinstance(torch_tensor, Tensor) and cls == Tensor:
+            if not hasattr(torch_tensor, 'requires_grad'): torch_tensor.requires_grad = False
+            if not hasattr(torch_tensor, 'feature_range'): torch_tensor.feature_range = None
+            if not hasattr(torch_tensor, 'n_sequence_dim'): torch_tensor.n_sequence_dim = 0
             if requires_grad is not None: torch_tensor.requires_grad = requires_grad
             if with_batch is not None: torch_tensor.with_batch = with_batch
             if feature_range is not void: torch_tensor.feature_range = feature_range
+            if n_sequence_dim != 0: torch_tensor.n_sequence_dim = n_sequence_dim
             return torch_tensor
         if requires_grad is None: requires_grad = torch_tensor.requires_grad
         self = torch.Tensor._make_subclass(cls, torch_tensor, requires_grad)
         if with_batch is None: with_batch = torch_tensor.with_batch if isinstance(torch_tensor, Tensor) else False
         if feature_range is void: feature_range = torch_tensor.feature_range if isinstance(torch_tensor, Tensor) else None
         self.with_batch = with_batch
         self.feature_range = feature_range
+        self.n_sequence_dim = n_sequence_dim
         return self
 
     @collect_memory
     def __new__(cls, *args, **kwargs):
         """bt.Tensor
         Usages:
-            bt.Tensor(tensor: list/torch.Tensor/bt.Tensor/tensor with 'shape'/tensor with method '__tensor__', requires_grad=None, device=None, with_batch=None, feature_range=void)
-            bt.Tensor(shape: tuple, requires_grad=None, device=None, with_batch=None, feature_range=void)
-            bt.Tensor(*shape: int, requires_grad=None, device=None, with_batch=None, feature_range=void)
+            bt.Tensor(tensor: list/torch.Tensor/bt.Tensor/tensor with 'shape'/tensor with method '__tensor__', requires_grad=None, device=None, with_batch=None, feature_range=void, n_sequence_dim=0)
+            bt.Tensor(shape: tuple, requires_grad=None, device=None, with_batch=None, feature_range=void, n_sequence_dim=0)
+            bt.Tensor(*shape: int, requires_grad=None, device=None, with_batch=None, feature_range=void, n_sequence_dim=0)
         """
         if len(args) >= 1 and isinstance(args[0], torch.Tensor): return Tensor._make_subclass(cls, *args, **kwargs)
         if len(args) >= 1 and hasattr(args[0], '__tensor__'): return Tensor._make_subclass(cls, args[0].__tensor__(), *args[1:], **kwargs)
         device = kwargs.pop('device', _device)
         if isinstance(device, AutoDevice): device = device.main_device
         if len(args) >= 1 and hasattr(args[0], 'shape') or isinstance(args[0], list): return Tensor._make_subclass(cls, torch.tensor(args[0], requires_grad=False, device=device), *args[1:], **kwargs)
         return Tensor._make_subclass(cls, super().__new__(torch.Tensor, *args, device=device), **kwargs)
 
     def __init__(self, *args, **kwargs):
         self.with_batch = self.with_batch
         self.feature_range = self.feature_range
+        self.n_sequence_dim = self.n_sequence_dim
 
     @property
-    def shape(self): return Size.__new_raw__(super().shape, with_batch=self.with_batch, feature_range=self.feature_range)
+    def shape(self): return Size.__new_raw__(super().shape, with_batch=self.with_batch, feature_range=self.feature_range, n_sequence_dim=self.n_sequence_dim)
+    
+    def with_shape(self, *x):
+        x = arg_extract(x)
+        if isinstance(x, Tensor): x = x.shape
+        if not isinstance(x, Size): x = Size(x)
+        self.with_batch = x.with_batch
+        self.feature_range = x.feature_range
+        self.n_sequence_dim = x.n_sequence_dim
+        return self
 
     @alias("__str__")
     def __repr__(self, *args, **kwargs):
         string = super().__repr__(*args, **kwargs)
         if 'shape=' not in string:
             string = string.rstrip(')') + f', shape={self.shape})'
         return string.replace("tensor", "Tensor")
@@ -733,7 +791,115 @@
         torch_dt = getattr(torch, dtype_map.get(dt_name, dt_name), None)
         avouch(torch_dt is not None, f"Invalid dtype {dt}: {dt_name} cannot be converted into torch dtype.")
         return super().type(torch_dt).as_subclass(self.__class__)
 
     def type(self, dt=None):
         if dt is None: return super().type().replace("torch.", "bt.")
         else: return self.astype(dt)
+
+    basic_vars = list(locals().keys()) + ['basic_vars']
+    def __add__(self: 'Tensor', other: 'Tensor'): ...
+    def __iadd__(self: 'Tensor', other: 'Tensor'): ...
+    def __radd__(self: 'Tensor', other: 'Tensor'): ...
+    def __sub__(self: 'Tensor', other: 'Tensor'): ...
+    def __isub__(self: 'Tensor', other: 'Tensor'): ...
+    def __rsub__(self: 'Tensor', other: 'Tensor'): ...
+    def __mul__(self: 'Tensor', other: 'Tensor'): ...
+    def __imul__(self: 'Tensor', other: 'Tensor'): ...
+    def __rmul__(self: 'Tensor', other: 'Tensor'): ...
+    def __div__(self: 'Tensor', other: 'Tensor'): ...
+    def __idiv__(self: 'Tensor', other: 'Tensor'): ...
+    def __rdiv__(self: 'Tensor', other: 'Tensor'): ...
+    def __pow__(self: 'Tensor', other: 'Tensor'): ...
+    def __ipow__(self: 'Tensor', other: 'Tensor'): ...
+    def __rpow__(self: 'Tensor', other: 'Tensor'): ...
+    def __mod__(self: 'Tensor', other: 'Tensor'): ...
+    def __imod__(self: 'Tensor', other: 'Tensor'): ...
+    def __rmod__(self: 'Tensor', other: 'Tensor'): ...
+    def __truediv__(self: 'Tensor', other: 'Tensor'): ...
+    def __itruediv__(self: 'Tensor', other: 'Tensor'): ...
+    def __rtruediv__(self: 'Tensor', other: 'Tensor'): ...
+    def __floordiv__(self: 'Tensor', other: 'Tensor'): ...
+    def __ifloordiv__(self: 'Tensor', other: 'Tensor'): ...
+    def __rfloordiv__(self: 'Tensor', other: 'Tensor'): ...
+    def __eq__(self: 'Tensor', other: 'Tensor'): ...
+    def __ieq__(self: 'Tensor', other: 'Tensor'): ...
+    def __req__(self: 'Tensor', other: 'Tensor'): ...
+    def __ne__(self: 'Tensor', other: 'Tensor'): ...
+    def __ine__(self: 'Tensor', other: 'Tensor'): ...
+    def __rne__(self: 'Tensor', other: 'Tensor'): ...
+    def __or__(self: 'Tensor', other: 'Tensor'): ...
+    def __ior__(self: 'Tensor', other: 'Tensor'): ...
+    def __ror__(self: 'Tensor', other: 'Tensor'): ...
+    def __and__(self: 'Tensor', other: 'Tensor'): ...
+    def __iand__(self: 'Tensor', other: 'Tensor'): ...
+    def __rand__(self: 'Tensor', other: 'Tensor'): ...
+    def __xor__(self: 'Tensor', other: 'Tensor'): ...
+    def __ixor__(self: 'Tensor', other: 'Tensor'): ...
+    def __rxor__(self: 'Tensor', other: 'Tensor'): ...
+    def __lt__(self: 'Tensor', other: 'Tensor'): ...
+    def __le__(self: 'Tensor', other: 'Tensor'): ...
+    def __gt__(self: 'Tensor', other: 'Tensor'): ...
+    def __ge__(self: 'Tensor', other: 'Tensor'): ...
+    def reshape(self, *size: Size): ...
+    def reshape_as(self, other: 'Tensor'): ...
+    def view(self, *size: Size): ...
+    def view_as(self, other: 'Tensor'): ...
+    def t(self): ...
+    additional_methods = list(set(locals()) - set(basic_vars))
+    
+    for f in additional_methods:
+        execblock(get_updated_code(eval(f), mode='method'))
+
+    # @classmethod
+    # def __torch_function__(cls, func, types, args=(), kwargs=None):
+    #     try:
+    #         if Tensor in types and cls != Tensor: return NotImplemented # Donnot accept calls from outside batorch
+    #         if len(args) == 0: return super().__torch_function__(func, types, args, kwargs) # let non-torch-operation torch functions to run
+            
+    #         func_name = func.__name__
+    #         if func_name in ('__get__', '__set__', '__delete__'):
+    #             return super().__torch_function__(func, types, args, kwargs)
+            
+    #         with torch._C.DisableTorchFunction():
+    #             obj = super().__torch_function__(func, types, args, kwargs)
+    #         return obj.as_subclass(Tensor).with_shape(shape_mapping[func_name]())
+
+            # sfunc = str(func)
+            # if sfunc.startswith('<attribute') or sfunc.startswith('<property'):
+            #     return super().__torch_function__(func, types, args, kwargs)
+
+            # func_name = sfunc.split(' of ')[0].split(' at ')[0].split()[-1].strip("'").split('.')[-1]
+            # if func_name in ('__get__', '__set__', '__delete__'):
+            #     return super().__torch_function__(func, types, args, kwargs)
+
+            # self = args[0]
+            # types = tuple(cls if t in [torch.nn.Parameter, bt.nn.Parameter] else t for t in types)
+            # torch_func_name = Tensor.__torch_function_map__.get(func_name, None)
+            # if isinstance(self, Tensor) and self.init and self.has_special: pass
+            # elif torch_func_name in ('__torch_function_resizing_func__', '__torch_function_full_func__', '__torch_function_resizing_as_func__', '__torch_function_randint_func__'): pass
+            # else:
+            #     with torch._C.DisableTorchFunction():
+            #         ret = super().__torch_function__(func, types, args, kwargs)
+            #     def apply(r): r.special_from_()
+            #     return Tensor.__torch_function_convert_apply__(ret, apply, cls)
+
+            # if torch_func_name is None: return Tensor.__torch_function_default_func__(func, types, args, kwargs)
+            # else: return getattr(Tensor, torch_func_name)(func, types, args, kwargs)
+            
+        # except Exception as e:
+        #     print(f"In function {func}:")
+        #     raise e#.with_traceback(None)
+
+basic_locals = list(locals().keys()) + ['basic_locals']
+def tensor(data: Tensor, *, dtype=None, device=None, requires_grad=False, pin_memory=False): ...
+def as_tensor(data: Tensor, dtype=None, device=None): ...
+def empty(*size: Size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False, pin_memory=False, memory_format=torch.contiguous_format): ...
+def ones(*size: Size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False): ...
+def zeros(*size: Size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False): ...
+def empty_like(input: Tensor, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
+def ones_like(input: Tensor, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
+def zeros_like(input: Tensor, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format): ...
+additional_functions = [f for f in locals() if f not in basic_locals]
+
+for f in additional_functions:
+    execblock(get_updated_code(eval(f)))
```

### Comparing `batorch-1.0.32/batorch/tensorfunc.py` & `batorch-1.0.33/batorch/tensorfunc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = "PyCAMIA",
     package = "batorch",
     fileinfo = "Tensor functions for `batorch`.",
-    requires = "torch"
+    requires = ["torch", "pycamia", "pyoverload", "matplotlib"]
 )
 
 __all__ = """
     crop_as
     pad
     decimal
     divide
@@ -30,24 +30,26 @@
     up_scale
     one_hot
     permute_space
     skew_symmetric
     cross_matrix
     uncross_matrix
     summary
+    display
 """.split()
 
 import math
 
 with __info__:
     import batorch as bt
     from pyoverload import *
     from pycamia import restore_type_wrapper, avouch, alias
     from pycamia import get_environ_vars, get_snakenames, get_args_expression
-    from pycamia import SPrint, Version
+    from pycamia import SPrint, Version, argmin, tokenize
+    from matplotlib import pyplot as plt
     
 def batorch_tensor(x):
     if not isinstance(x, bt.torch.Tensor): return bt.tensor(x)
     elif type(x) != bt.Tensor: return x.as_subclass(bt.Tensor)
     return x
 
 @alias("meannorm2", "mean_norm2", root = False, mean = True)
@@ -427,52 +429,109 @@
     elif n_dim == 3:
         axis[:, 0] = cross_matrix[:, 1, 2]
         axis[:, 1] = cross_matrix[:, 2, 0]
         axis[:, 2] = cross_matrix[:, 0, 1]
     return axis
 
 class summary:
-    def __init__(self, x, thumb = False):
-        var_name = get_args_expression("summary").split(',')[0].strip().split(')')[0]
-        out = SPrint(f"Summary of {var_name}:\n" + "=" * 50 + '\n' + x.__class__.__name__)
-        g = None
-        if not isinstance(x, bt.torch.Tensor): x = batorch_tensor(x)
-        elif not isinstance(x, bt.Tensor):
-            if x.is_leaf and x.grad is not None: g = batorch_tensor(x.grad.clone().detach())
-            x = batorch_tensor(x)
-        xshape = str(x.shape).split('Size')[-1]
-        out(f"{xshape}: [{x.n_special}] + {x.n_space} D tensor of values between [{round(x.min().item(), 4)}, {round(x.max().item(), 4)}].")
-        out(f"Device: {x.device}; Type: {x.type()}; Using gradient: {x.requires_grad}; Gradient func: {x.grad_fn}.")
-        if g is None and (not x.is_leaf or x.grad is None): grad_smy = None
-        else:
-            if g is None: g = x.grad.clone().detach()
-            gshape = str(g.shape).split('Size')[-1]
-            grad_smy = f"Gradient: {gshape} tensor of values [{round(g.min().item(), 4)}, {round(g.max().item(), 4)}].\n"
-            if g.n_space >= 2:
-                if g.has_batch: g = g.pick(0, [])
-                if g.has_channel: g = g.pick(0, {})
-            if g.n_dim == 1: a = min(4, g.size(0)); core_gradient = bt.crop_as(g, (a,)); label = "%ds"%a
-            elif g.n_dim == 2: a = min(4, g.size(0)); b = min(4, g.size(1)); core_gradient = bt.crop_as(g, (a, b)); label = "%d x %d" % (a, b)
-            else: a = min(4, g.size(-2)); b = min(4, g.size(-1)); core_gradient = bt.crop_as(g.flatten(0, g.n_dim - 3)[0], (a, b)); label = "%d x %d" % (a, b)
-            grad_smy += f"Core {label}-window for gradient: \n{core_gradient}\n".replace('Tensor', ' '*6).split(']'*(len(label)//2))[0] + ']'*(len(label)//2)
-        values = x.unique().tolist()
-        if x.nele >> 24 <= 0: out("Quantiles:", str(x.float().quantile(bt.arange(11).float()/10)).replace('Tensor(', '').split(']')[0] + ']')
-        else: out("Quantiles (of first 2^24 elements):", str(x.flatten(0, x.ndim-1).float()[:16777216].quantile(bt.arange(11).float()/10)).replace('Tensor(', '').split(']')[0] + ']')
-        if len(values) <= 10: out(f"Range ({len(values)} unique element{'s' if len(values) > 1 else ''}): [{', '.join(str(round(x, 4)) for x in values)}].")
-        else: out(f"Range ({len(values)} unique elements): \n[{', '.join(str(round(x, 4)) for x in values[:5])}, ..., {', '.join(str(round(x, 4)) for x in values[-5:])}].")
-        if x.n_space >= 2:
-            if x.has_batch: x = x.pick(0, [])
-            if x.has_channel: x = x.pick(0, {})
-        label = "4 x 4"
-        if x.n_dim == 1: a = min(4, x.size(0)); core = bt.crop_as(x, (a,)); label = "%ds"%a
-        elif x.n_dim == 2: a = min(4, x.size(0)); b = min(4, x.size(1)); core = bt.crop_as(x, (a, b)); label = "%d x %d" % (a, b)
-        else: a = min(4, x.size(-2)); b = min(4, x.size(-1)); core = bt.crop_as(x.flatten(0, x.n_dim - 3)[0], (a, b)); label = "%d x %d" % (a, b)
-        out(f"Core 4-window (the central {label}): \n{core}".replace('Tensor', ' '*6).split(']'*(len(label)//2))[0] + ']'*(len(label)//2))
-        if thumb:
-            gaps = bt.floor((bt.channel_tensor(list(x.space)) - 1) / 3).clamp(1).long()
-            down_sample = x[(image_grid(*(4 if s > 4 else s for s in x.space)) * gaps).split(1, {}, squeeze=True)]
-            out(f"Thumb 4-window (down sample to 4{' x 4'*(x.n_space-1)}): \n{down_sample}".replace('Tensor', ' '*6).split(']'*x.n_space)[0] + ']'*x.n_space)
-        if grad_smy is not None: out(grad_smy)
-        self.smy = out.text
-    def show(self): print(self.smy)
+    def __init__(self, *Xs, show_thumb = False, show_core = False, plot = False):
+        self.smys = []
+        self.show_as_plot = plot
+        if plot:
+            n_plots = len(Xs)
+            self.subplot_rows = math.floor(math.sqrt(n_plots))
+            self.subplot_cols = math.ceil(n_plots / self.subplot_rows)
+            self.canvases = []
+        if not hasattr(self, 'var_names'):
+            self.var_names = [vn.strip() for vn in tokenize(get_args_expression("summary"), sep=', ') if '=' not in vn]
+        for i, x in enumerate(Xs):
+            var_name = self.var_names[i]
+            class_name = x.__class__.__name__
+            g = None
+            if not isinstance(x, bt.torch.Tensor): x = batorch_tensor(x)
+            elif not isinstance(x, bt.Tensor):
+                if x.is_leaf and x.grad is not None: g = batorch_tensor(x.grad.clone().detach())
+                x = batorch_tensor(x)
+            batch_dim = f"[{x.n_special}]+" if x.n_special > 0 else ''
+            xshape = str(x.shape).split('Size')[-1]
+            out = SPrint(f">>Summary of {var_name}<<\n")
+            out(f"【Size】{batch_dim}{x.n_space}D {class_name} of size {xshape}")
+            out(f"【Device】{x.device}")
+            out(f"【Type】{x.type()}")
+            out(f"【Using gradient】{x.requires_grad}")
+            if x.requires_grad: out(f"【Gradient func】{x.grad_fn}")
+            nan_mask = bt.isnan(x)
+            num_nans = nan_mask.sum().sum()
+            if num_nans > 0:
+                out(f"【Number of NaNs】{num_nans.long().item()}")
+                out(f"【Center of NaNs】{bt.Size([round(x, 1) for x in (bt.image_grid(*x.shape) * nan_mask.remove_special_()).float().mean().tolist()]).special_from_(x)}")
+                grad_smy = None
+            else:
+                out(f"【MinMax】[{round(x.min().item(), 4)}, {round(x.max().item(), 4)}];")
+                if g is None and (not x.is_leaf or x.grad is None): grad_smy = None
+                else:
+                    if g is None: g = x.grad.clone().detach()
+                    gshape = str(g.shape).split('Size')[-1]
+                    grad_smy = f"【Gradient】{gshape} tensor of values [{round(g.min().item(), 4)}, {round(g.max().item(), 4)}]\n"
+                    if g.n_space >= 2:
+                        if g.has_batch: g = g.pick(0, [])
+                        if g.has_channel: g = g.pick(0, {})
+                    if g.n_dim == 1: a = min(4, g.size(0)); core_gradient = bt.crop_as(g, (a,)); label = "%ds"%a
+                    elif g.n_dim == 2: a = min(4, g.size(0)); b = min(4, g.size(1)); core_gradient = bt.crop_as(g, (a, b)); label = "%d x %d" % (a, b)
+                    else: a = min(4, g.size(-2)); b = min(4, g.size(-1)); core_gradient = bt.crop_as(g.flatten(0, g.n_dim - 3)[0], (a, b)); label = "%d x %d" % (a, b)
+                    if show_core: grad_smy += f"【Core {label}-window for gradient】\n{core_gradient}\n".replace('Tensor', ' '*6).split(']'*(len(label)//2))[0] + ']'*(len(label)//2)
+                values = x.unique().tolist()
+                if x.nele >> 24 <= 0: out("【Quintiles】", [round(u.item(), 4) for u in x.float().quantile(bt.arange(6).float()/5)])
+                else: out("【Quintiles (of first 2^24 elements)】", str(x.flatten(0, x.ndim-1).float()[:16777216].quantile(bt.arange(6).float()/5)).replace('Tensor(', '').split(']')[0] + ']')
+                if len(values) <= 10:
+                    out(f"【Range ({len(values)} unique element{'s' if len(values) > 1 else ''})】")
+                    if len(values) > 6:
+                        out(f">> [{', '.join(str(round(x, 4)) for x in values)}]")
+                    else:
+                        num_pairs = [(round(v, 4), (x == v).sum().sum().item()) for v in values]
+                        out(f">> [{', '.join(f'{v}({n})' for v, n in num_pairs)}]")
+                else: out(f"【Range ({len(values)} unique elements)】\n  [{', '.join(str(round(x, 4)) for x in values[:5])}, ..., {', '.join(str(round(x, 4)) for x in values[-5:])}]")
+            if x.n_space >= 2:
+                if x.has_batch: x = x.pick(0, [])
+                if x.has_channel: x = x.pick(0, {})
+            label = "4 x 4"
+            if x.n_dim == 1: a = min(4, x.size(0)); core = bt.crop_as(x, (a,)); label = "%ds"%a
+            elif x.n_dim == 2: a = min(4, x.size(0)); b = min(4, x.size(1)); core = bt.crop_as(x, (a, b)); label = "%d x %d" % (a, b)
+            else: a = min(4, x.size(-2)); b = min(4, x.size(-1)); core = bt.crop_as(x.flatten(0, x.n_dim - 3)[0], (a, b)); label = "%d x %d" % (a, b)
+            if show_core: out(f"【Core 4-window (the central {label})】\n{core}".replace('Tensor', ' '*6).split(']'*(len(label)//2))[0] + ']'*(len(label)//2))
+            if show_thumb:
+                gaps = bt.floor((bt.channel_tensor(list(x.space)) - 1) / 3).clamp(1).long()
+                down_sample = x[(image_grid(*(4 if s > 4 else s for s in x.space)) * gaps).split(1, {}, squeeze=True)]
+                out(f"【Thumb 4-window (down sampled to 4{' x 4'*(x.n_space-1)})】\n{down_sample}".replace('Tensor', ' '*6).split(']'*x.n_space)[0] + ']'*x.n_space)
+            if grad_smy is not None: out(grad_smy)
+            self.smys.append(out.text)
+            if plot:
+                while x.n_dim > 2:
+                    x = x.pick(0, argmin(list(x.shape))[0])
+                self.canvases.append(x.detach())
+    def show(self):
+        if not self.show_as_plot:
+            print(self)
+            return
+        plt.figure(figsize=(15, 7))
+        for i, x in enumerate(self.canvases):
+            ax = plt.subplot(self.subplot_rows, self.subplot_cols, i+1)
+            old_size = plt.rcParams['font.size']
+            plt.rcParams['font.size'] = 8
+            if x.n_dim == 2:
+                img = plt.imshow(x, cmap=plt.cm.gray)
+                plt.colorbar(mappable=img, ax=ax, orientation='vertical')
+                plt.text(-0.5, -0.5, self.smys[i])
+            elif x.n_dim == 1:
+                plt.plot(bt.arange(len(x)), x)
+                plt.text(0, plt.ylim()[1], self.smys[i])
+            else: raise TypeError("Failed to display 0-dimensional data in plot.")
+            plt.rcParams['font.size'] = old_size
+        plt.show()
     @alias("__repr__")
-    def __str__(self): return self.smy
+    def __str__(self): return ''.join(self.smys)
+
+class display(summary):
+    def __init__(self, *args, **kwargs):
+        kwargs['plot'] = True
+        self.var_names = [vn.strip() for vn in tokenize(get_args_expression("display"), sep=', ') if '=' not in vn]
+        return super().__init__(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `batorch-1.0.32/batorch/torch_namespace.py` & `batorch-1.0.33/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch/torchext.py` & `batorch-1.0.33/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `batorch-1.0.32/batorch.egg-info/PKG-INFO` & `batorch-1.0.33/batorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batorch
-Version: 1.0.32
+Version: 1.0.33
 Summary: 'batorch' is an extension of package torch, for tensors with batch dimensions. 
 Home-page: https://github.com/Bertie97/PyZMyc/batorch
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # batorch
```

### Comparing `batorch-1.0.32/setup.py` & `batorch-1.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'batorch',
-	version = '1.0.32',
+	version = '1.0.33',
 	keywords = ['pip', 'pymyc', 'batorch', 'torch', 'batch', 'batched data'],
 	description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
 	long_description = '# batorch\n\n## Introduction\n\n[batorch](https://github.com/Bertie97/pyctlib/tree/main/batorch) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). We encapsulated a new type on top of `torch` tensers, which we call it `batorch.Tensor`. It has the same function as `torch.Tensor`, but it can automatically select the device it was on and provide batch or channel dimensions. Also, we try to provide more useful module for torch users to make deep learning to be implemented more easily. It relies `python v3.6+` with `torch v 1.7.0+`. ***Note that `torch v1.7.0` was released in 2020,*** *and it is necessary for this package as the inheritance behavior for this version is different from previous versions.* Most original `torch` functions should be able to be applied for `batorch` tensors. \n\n> Special features for `batorch` are still under development. If unknown errors pop our, please use traditional `torch` code to bypass it and meanwhile it would be very kind of you to let us know if anything is needed: please contact us by [e-mail](https://github.com/Bertie97/pycamia#Contributors). \n\n```python\n>>> import batorch as bt\n>>> import batorch.nn as nn\n>>> bt.turn_off_autodevice()\n>>> bt.manual_seed(0)\n<torch._C.Generator object at 0x1071b6730>\n>>> t = bt.randn([3000], 400, requires_grad=True)\n>>> LP = nn.Linear(400, 400)\n>>> a = LP(t)\n>>> a.sum().sum().backward()\n>>> print(t.grad)\nTensor([[-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        ...,\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702],\n        [-0.2986,  0.0267,  0.9059,  ...,  0.4563, -0.1291,  0.5702]], shape=batorch.Size([3000], 400))\n```\n\n`batorch` has all of following appealing features:\n\n1. **Auto assign** the tensors to available `GPU` **device** by default. \n2. Use `[nbatch]` or `{nchannel}` to specify **the batch and channel dimensions**. i.e. `tp.rand([4], {2}, 20, 30)` returns a 2-channel feature tensor of $20\\times30$ matrices with batch size 4. One may also use `tensor.batch_dimension` to access (or assign) batch dimension, channel dimension can be operated likewise. If you find it hard to remember the symbol, just remember brackets enclose paralleled items in matrices hence it represents the batch dimension for paralleled calculation; braces enclose equation systems which are highly related hence it represents the channel (or feature) dimension. \n3. Batch and channel dimension can help **auto matching the sizes** of two tensors in operations. For example, tensors of sizes `(3, [2], 4)` and `(3, 4)` can be automatically added together with axis of size 3 and 4 matched together. Some methods will also use this information. Sampling, for example, will take the batch dimension as priority.\n4. The tensor object is **compatible with original `torch` functions**. \n\n## Installation\n\nThis package can be installed by `pip install batorch` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/batorch/)). \n\n```shell\npip install batorch\n```\n\n## Usages\n\nNot available yet, one may check the codes for usages.\n\n## Acknowledgment\n\n@ Yuncheng Zhou: Developer\n@ Yiteng Zhang: Important functions extraction',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/batorch',
 	author = 'Yuncheng Zhou',
```

