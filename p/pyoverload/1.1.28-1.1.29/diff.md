# Comparing `tmp/pyoverload-1.1.28.tar.gz` & `tmp/pyoverload-1.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverload-1.1.28.tar", last modified: Wed Jul  5 08:20:42 2023, max compression
+gzip compressed data, was "pyoverload-1.1.29.tar", last modified: Wed Jul  5 08:28:39 2023, max compression
```

## Comparing `pyoverload-1.1.28.tar` & `pyoverload-1.1.29.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.434318 pyoverload-1.1.28/
--rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 08:20:42.434166 pyoverload-1.1.28/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)    12301 2023-07-05 08:20:42.000000 pyoverload-1.1.28/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.425484 pyoverload-1.1.28/batorch/
--rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.426555 pyoverload-1.1.28/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.429937 pyoverload-1.1.28/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.431171 pyoverload-1.1.28/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 08:20:41.000000 pyoverload-1.1.28/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.432472 pyoverload-1.1.28/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/metrics.py
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:20:40.000000 pyoverload-1.1.28/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.433075 pyoverload-1.1.28/pyoverload/
--rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload/override.py
--rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload/typehint.py
--rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload/utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.433866 pyoverload-1.1.28/pyoverload.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1809 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       31 2023-07-05 08:20:42.000000 pyoverload-1.1.28/pyoverload.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:20:42.434376 pyoverload-1.1.28/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)    13392 2023-07-05 08:20:42.000000 pyoverload-1.1.28/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.254234 pyoverload-1.1.29/
+-rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 08:28:39.254087 pyoverload-1.1.29/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)    12301 2023-07-05 08:28:39.000000 pyoverload-1.1.29/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.244976 pyoverload-1.1.29/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.246047 pyoverload-1.1.29/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.249690 pyoverload-1.1.29/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.250929 pyoverload-1.1.29/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 08:28:38.000000 pyoverload-1.1.29/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.252448 pyoverload-1.1.29/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2361 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:28:37.000000 pyoverload-1.1.29/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.253034 pyoverload-1.1.29/pyoverload/
+-rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload/override.py
+-rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload/typehint.py
+-rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload/utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.253823 pyoverload-1.1.29/pyoverload.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1809 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       31 2023-07-05 08:28:39.000000 pyoverload-1.1.29/pyoverload.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:28:39.254285 pyoverload-1.1.29/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)    13180 2023-07-05 08:28:39.000000 pyoverload-1.1.29/setup.py
```

### Comparing `pyoverload-1.1.28/PKG-INFO` & `pyoverload-1.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverload
-Version: 1.1.28
+Version: 1.1.29
 Summary: 'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. 
 Home-page: https://github.com/Bertie97/PyZMyc/pyoverload
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pyoverload
```

### Comparing `pyoverload-1.1.28/README.md` & `pyoverload-1.1.29/README.md`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/__init__.py` & `pyoverload-1.1.29/batorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'batorch',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.34',
+    version = '1.0.35',
     contact = 'bertiezhou@163.com',
     keywords = ['torch', 'batch', 'batched data'],
     description = "'batorch' is an extension of package torch, for tensors with batch dimensions. ",
     requires = ['pycamia', 'torch', 'pynvml'],
-    update = '2023-07-05 14:57:53'
+    update = '2023-07-05 16:20:40'
 ).check()
 
 import torch
 distributed = torch.distributed
 autograd = torch.autograd
 random = torch.random
 optim = torch.optim
```

### Comparing `pyoverload-1.1.28/batorch/device.py` & `pyoverload-1.1.29/batorch/device.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/_reduction.py` & `pyoverload-1.1.29/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/common_types.py` & `pyoverload-1.1.29/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/functional.py` & `pyoverload-1.1.29/batorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/grad.py` & `pyoverload-1.1.29/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/init.py` & `pyoverload-1.1.29/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/__init__.py` & `pyoverload-1.1.29/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/_functions.py` & `pyoverload-1.1.29/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/activation.py` & `pyoverload-1.1.29/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/adaptive.py` & `pyoverload-1.1.29/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/batchnorm.py` & `pyoverload-1.1.29/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/container.py` & `pyoverload-1.1.29/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/conv.py` & `pyoverload-1.1.29/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/distance.py` & `pyoverload-1.1.29/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/dropout.py` & `pyoverload-1.1.29/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/flatten.py` & `pyoverload-1.1.29/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/fold.py` & `pyoverload-1.1.29/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/instancenorm.py` & `pyoverload-1.1.29/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/linear.py` & `pyoverload-1.1.29/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/loss.py` & `pyoverload-1.1.29/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/module.py` & `pyoverload-1.1.29/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/normalization.py` & `pyoverload-1.1.29/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/padding.py` & `pyoverload-1.1.29/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/pixelshuffle.py` & `pyoverload-1.1.29/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/pooling.py` & `pyoverload-1.1.29/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/rnn.py` & `pyoverload-1.1.29/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/sparse.py` & `pyoverload-1.1.29/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/transformer.py` & `pyoverload-1.1.29/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/upsampling.py` & `pyoverload-1.1.29/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/modules/utils.py` & `pyoverload-1.1.29/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/parameter.py` & `pyoverload-1.1.29/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/clip_grad.py` & `pyoverload-1.1.29/batorch/nn/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/convert_parameters.py` & `pyoverload-1.1.29/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/fusion.py` & `pyoverload-1.1.29/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/memory_format.py` & `pyoverload-1.1.29/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/prune.py` & `pyoverload-1.1.29/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/rnn.py` & `pyoverload-1.1.29/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/spectral_norm.py` & `pyoverload-1.1.29/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/nn/utils/weight_norm.py` & `pyoverload-1.1.29/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/optimizer.py` & `pyoverload-1.1.29/batorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/tensor.py` & `pyoverload-1.1.29/batorch/tensor.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/tensor2.py` & `pyoverload-1.1.29/batorch/tensor2.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/tensorfunc.py` & `pyoverload-1.1.29/batorch/tensorfunc.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/torch_namespace.py` & `pyoverload-1.1.29/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/batorch/torchext.py` & `pyoverload-1.1.29/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/__init__.py` & `pyoverload-1.1.29/micomputing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.34',
+    version = '1.1.35',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-05 14:57:53'
+    update = '2023-07-05 16:20:40',
+    package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
 from .funcs import reorient, rescale, reflect, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
```

### Comparing `pyoverload-1.1.28/micomputing/data.py` & `pyoverload-1.1.29/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/funcs.py` & `pyoverload-1.1.29/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/metrics.py` & `pyoverload-1.1.29/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/network.py` & `pyoverload-1.1.29/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/plot.py` & `pyoverload-1.1.29/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/stdio.py` & `pyoverload-1.1.29/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/test.py` & `pyoverload-1.1.29/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/micomputing/trans.py` & `pyoverload-1.1.29/micomputing/trans.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/pyoverload/__init__.py` & `pyoverload-1.1.29/pyoverload/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'pyoverload',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.27',
+    version = '1.1.28',
     contact = 'bertiezhou@163.com',
     keywords = ['overload'],
     description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. ",
     requires = ['pycamia'],
-    update = '2023-07-05 14:57:54'
+    update = '2023-07-05 16:20:42'
 ).check()
 
 from .typehint import isofsubclass, inheritable, isitertype, iterable, isarray, isdtype, isatype, isoftype, isclassmethod, typename, Type, params, Bool, Int, Float, Str, Set, List, Tuple, Dict, Class, Callable, Function, Method, Lambda, Functional, Real, real, Null, null, Sequence, sequence, Array, Iterable, Scalar, IntScalar, FloatScalar #*
 from .override import override, overload, params #*
```

### Comparing `pyoverload-1.1.28/pyoverload/override.py` & `pyoverload-1.1.29/pyoverload/override.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/pyoverload/typehint.py` & `pyoverload-1.1.29/pyoverload/typehint.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/pyoverload/utils.py` & `pyoverload-1.1.29/pyoverload/utils.py`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/pyoverload.egg-info/PKG-INFO` & `pyoverload-1.1.29/pyoverload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverload
-Version: 1.1.28
+Version: 1.1.29
 Summary: 'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. 
 Home-page: https://github.com/Bertie97/PyZMyc/pyoverload
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pyoverload
```

### Comparing `pyoverload-1.1.28/pyoverload.egg-info/SOURCES.txt` & `pyoverload-1.1.29/pyoverload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoverload-1.1.28/setup.py` & `pyoverload-1.1.29/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'pyoverload',
-	version = '1.1.28',
+	version = '1.1.29',
 	keywords = ['pip', 'pymyc', 'pyoverload', 'overload'],
 	description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. ",
 	long_description = '# pyoverload\n\n## Introduction\n\n[`pyoverload`](https://github.com/Bertie97/pycamia/tree/main/pyoverload) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a powerful overloading tools to provide easy overload for `python v3.6+`. `pyoverload` provide multiple usages. The simplest one, however, can be easily implemented as follows. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1)\nfunc1 1\n>>> func("1")\nfunc2 1\n```\n\n`pyoverload` has all of following appealing features:\n\n1. Support of **`Jedi` auto-completion** by keyword decorator `@overload`. This means all main-stream python IDE can hint you the overloaded functions you have defined. \n2. **Multiple usages** that are user friendly for all kinds of users, including `C/Java` language system users and those who are used to `singledispatch` based overload. Also, easy collector of ordinary python functions is also provided. \n3. Support of **all kinds of functions**, including functions, methods, class methods and static methods. One simple implementation for all.\n4. **String types** supported. This means that one can use `"numpy.ndarray"` to mark a numpy array without importing the whole package. \n5. Sufficient **built-in types are provided** for easy representations such as `List[Int]`, `Dict@{str: int}` or `List<<int>>[10]`. \n6. **Available usage listing** when no overload function matches the input arguments. \n7. **Type constraint for an ordinary function** using `@params` decorator. \n\n## Installation\n\nThis package can be installed by `pip install pyoverload` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pyoverload\n```\n\n## Usages\n\n### Usage 1: Decorator Fashion\n\nOne can use `@overload` before the functions with the same function name to build an overloaded function. When the function is called, the inputs will be handed out to the suitable implementation. \n\nThe types of the input arguments are specified by the typehints available in `python3.6+`. All known types can be added after the colon. For package classes like `np.ndarray`, please use a string to represent it. For more types, one can use types from package `types` or `pyoverload.typehint`. \n\nFor usage of `pyoverload.typehint`, please refer to section **Typehints** for more information.\n\nAll implementations of the overloaded function are referenced in the order of definition, but the implementation ends with `__default__` or `__0__` will be used when no usage is available. Note that there are **four** underlines for this notation, **two** on each side. \n\n```python\n>>> from pyoverload import *\n>>> import numpy as np\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n...\n>>> @overload\n... def func(x: str):\n... \tprint("func3", x)\n...\n>>> @overload\n... def func(x: List<<Int>>[4]):\n... \tprint("func4", x)\n...\n>>> @overload\n... def func(x: \'np.ndarray\'):\n... \tprint("func5", x)\n...\n>>> func(1)\nfunc2 1\n>>> func("1")\nfunc3 1\n>>> func([1,2,3,4])\nfunc4 [1, 2, 3, 4]\n>>> func(np.array([1,2,3,4]))\nfunc5 [1 2 3 4]\n>>> func(1.)\nfunc1 1.0\n```\n\nNote that the auto-completion by `Jedi` can only work for this usage. \n\n<img src="https://github.com/Bertie97/pycamia/raw/main/pyoverload/Jedi.jpg" alt="Jedi" style="zoom:50%;" />\n\n### Usage 2: Registering Fashion\n\nAfter using `@overload` decorator, apart from using `@overload` to decorate functions with the same name, one can also use the decorator with the function name `@{fill in the function name}` to decorate other functions with relevant names like `func1`, `func_str`, `first_func` for function `func`. However, omitting sign `_` is recommended for these functions. \n\nIn this fashion, the default function is the one decorated with `@overload` though it can still be changed by adding `__default__` or `__0__` tags in the decorated function names. All typehints are the same as the first usage. \n\nThe following example realized the first three functions in the usage 1 example in a reimplementation. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x):\n... \tprint("func1", x)\n... \n>>> @func\n... def func2(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\nNote that **usage 1** and **usage 2** can be used together though you may need to specify the default function manually like in usage 1 if needed. The last example is rewrote in a combined style. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\n### Usage 3: Collector Fashion\n\nThe last possible usage can not be used along with the previous two, or at least this is not tested by the developer and is not recommended. Another decorator `@override` is used as a collector. \n\nIn this usage, all functions should have different names and all functions with typehints should add decorator `@params` to activate the typehint regularization. Collector `@override` takes additional function list as the arguments indicating these functions should be packed into a single function. \n\nNote that the last function in the function list is the default function. \n\n```python\n>>> from pyoverload import override, params\n>>> @params\n... def func_all(x):\n... \tprint("func1", x)\n... \n>>> @params\n... def func_int(x: int):\n... \tprint("func2", x)\n... \n>>> @params\n... def func_str(x: str):\n... \tprint("func3", x)\n... \n>>> @override(func_int, func_str, func_all)\n... def func(): pass\n... \n```\n\nTheoretically, decorator `@override` can also be used in **usages 1&2**, but this is not recommended either. \n\n## Implementation List\n\nWhen an overloaded function receives arguments that are not suitable for all implementations, the error information will tell you which ones are correct. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1.)\nTraceback (most recent call last):\n  [...omitted...]\nNameError: No func() matches arguments 1.0. All available usages are:\nfunc(x:int)\nfunc(x:str)\n```\n\nThis function is available for all two Implementations but none of them takes `1.`. \n\n## Typehints\n\nDecorator `@params` enables functions to reject inputs with wrong types by raising **`TypeHintError`**. One can use it directly to decorate functions with python typehints or one can add some arguments to it. In the following example, we apply the condition that `a` is a function, `b` is an integer, `k` is a series of integers while function `test_func` needs to return an iterable type of real numbers with length `2`. \n\n```python\n>>> from pyoverload import *\n>>> @params(Func, Int, +Int, __return__ = Real[2])\n... def test_func(a, b=2, *k):\n...     print(a, b, k)\n...     return k\n...\n>>> test_func(lambda x: 1, 3, 4, 5)\n<function <lambda> at 0x7fbdb2027f70> 3 (4, 5)\n(4, 5)\n```\n\nThe basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, \n\n1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. \n2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.\n3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. \n4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.\n5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `batorch` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.Batorch` to identify specific packages. \n6. `Iterable` includes `Array`, `Sequence` and `dict`. \n7. Three types of `Scalar`s support the array variables.\n\nAll these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. \n\nOne can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned. \n\nFor a `Type`, `List` for example, we can do the following operations. Except the first four, these usages are designed for iterable types only. \n\n1. `+List`: This indicates that this is an extendable argument, which means it decorates arguments after `*`. It was used to specify `*args` arguments in `@params` but currently deprecated though adding `+` would not lead to failures. \n\n2. `~List`: This invert the typehint, meaning that all non-list types. \n\n3. `List|Tuple`: This is equivalent to `Type(List, Tuple)` indicating list or tuples. \n\n4. `Type(A)&Callable`: The *and* operator. Note that both indicator should be `Type`s. \n\n   ```python\n   >>> from pyoverload import *\n   >>> class A: pass\n   ...\n   >>> class B(A): pass\n   ...\n   >>> class C(A):\n   ...     def __call__(self): pass\n   ...\n   >>> isoftype(B(), Type(A)&Callable)\n   False\n   >>> isoftype(C(), Type(A)&Callable)\n   True\n   ```\n\n5. `List[5]`: This indicates the length or shape of the variable. For other types such as `Int[5]`, this indicates an iterable of length 5 with integer elements. Note that `Array[3, 4]` represents an array with shape `3 x 4`, but this representation is not available for nested lists. Use `List[List[4]][3]` or `List<<List[4]>>[3]` instead.\n\n6. `List@[int, str]`: This only works for ordered sequence `List` and `Tuple`. It indicates that the list has 2 elements, and the first one is an integer while the second is a string. Note that this is **not** equivalent to `List[int, str]` which represents a list with elements either integer or string.\n\n7. `List@int` or `Dict@{str: int}`: For all Iterables, `A@B` indicates type `A` with all elements of type `B`. `Dict@{str:int}` represents a dictionary with string keys and integer values.  \n\n8. `List[int]`: `=List@int`. A list with integer elements. Note that one can use `List[Int|float]` to directly identify a list of elements that are either `int` or `float`. `List[int, float]` and `Dict[str: int, int:str]` are also valid for multiple element types or key-value pairs. Using list in the blankets will return to the effect of `@` operator: `List[[int, float]]=List@[int, float]`. \n\n9. `List<<int>>[10]`: `=(List@int)[10]=List[int][10]` The first one of the two types should be a `Type`. The representation refers to an integer list of length 10 which is equivalent to `List[10]@int`. The length or shape is not specified if a pair of empty blankets is given. Use `List<<Type(int, Float)>>[]` to represent multiple candidates and `Dict<<(str,int)>>[]=Dict[str:int]` to represent a dictionary. \n\n10. `len(List[10, 20])`: Function `len` returns the length of the array. `200` should be the result for the given example. \n\n## Suggestions\n\n1. The speed of type check for `pyoverload.typehint.Type` is not very fast, hence please try your best to use builtin types, types from module `types` or list of types to do the typehint. \n2. The `overload` takes extra time for delivering the arguments, hence using it for functions require fast speed is not recommended. \n3. Do use `@params` for functions not overloaded but needs typehint constraints instead of using `@overload` without actually has multiple implementations. This is because `@params` is way faster. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/pyoverload',
 	author = 'Yuncheng Zhou',
 	author_email = 'bertiezhou@163.com',
 	packages = find_packages(),
-	include_package_data = True,
+	include_package_data = False,
 	platforms = 'any',
-	install_requires = ['pycamia'],
-	doc_files = ['pyoverload/.DS_Store', 'pyoverload/__init__.py', 'pyoverload/typehint.py', 'pyoverload/__pycache__', 'pyoverload/README.md', 'pyoverload/utils.py', 'pyoverload/Jedi.jpg', 'pyoverload/override.py']
+	install_requires = ['pycamia']
 )
```

