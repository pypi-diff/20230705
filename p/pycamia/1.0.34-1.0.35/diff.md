# Comparing `tmp/pycamia-1.0.34.tar.gz` & `tmp/pycamia-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycamia-1.0.34.tar", last modified: Wed Jul  5 08:20:42 2023, max compression
+gzip compressed data, was "pycamia-1.0.35.tar", last modified: Wed Jul  5 08:28:39 2023, max compression
```

## Comparing `pycamia-1.0.34.tar` & `pycamia-1.0.35.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.866530 pycamia-1.0.34/
--rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 08:20:42.866278 pycamia-1.0.34/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     7041 2023-07-05 08:20:42.000000 pycamia-1.0.34/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.854308 pycamia-1.0.34/batorch/
--rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.856105 pycamia-1.0.34/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.859820 pycamia-1.0.34/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.861199 pycamia-1.0.34/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 08:20:41.000000 pycamia-1.0.34/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.862533 pycamia-1.0.34/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/metrics.py
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:20:40.000000 pycamia-1.0.34/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.864692 pycamia-1.0.34/pycamia/
--rw-r--r--   0 admin      (501) staff       (20)     1944 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3453 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/decorators.py
--rw-r--r--   0 admin      (501) staff       (20)     9424 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/environment.py
--rw-r--r--   0 admin      (501) staff       (20)     4260 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/exception.py
--rw-r--r--   0 admin      (501) staff       (20)      683 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/functions.py
--rw-r--r--   0 admin      (501) staff       (20)     3814 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/inout.py
--rw-r--r--   0 admin      (501) staff       (20)    15488 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/listop.py
--rw-r--r--   0 admin      (501) staff       (20)     6550 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/logging.py
--rw-r--r--   0 admin      (501) staff       (20)     7135 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/manager.py
--rw-r--r--   0 admin      (501) staff       (20)     5867 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/math.py
--rw-r--r--   0 admin      (501) staff       (20)     1061 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/more.py
--rw-r--r--   0 admin      (501) staff       (20)     1091 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/numpyop.py
--rw-r--r--   0 admin      (501) staff       (20)     9791 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/strop.py
--rw-r--r--   0 admin      (501) staff       (20)    21362 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/system.py
--rw-r--r--   0 admin      (501) staff       (20)    12327 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia/timing.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.865362 pycamia-1.0.34/pycamia.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     2048 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       39 2023-07-05 08:20:42.000000 pycamia-1.0.34/pycamia.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:20:42.866044 pycamia-1.0.34/pyoverload/
--rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 08:20:42.000000 pycamia-1.0.34/pyoverload/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 08:20:42.000000 pycamia-1.0.34/pyoverload/override.py
--rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 08:20:42.000000 pycamia-1.0.34/pyoverload/typehint.py
--rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 08:20:42.000000 pycamia-1.0.34/pyoverload/utils.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:20:42.866586 pycamia-1.0.34/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     8128 2023-07-05 08:20:42.000000 pycamia-1.0.34/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.704927 pycamia-1.0.35/
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 08:28:39.704671 pycamia-1.0.35/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     7041 2023-07-05 08:28:39.000000 pycamia-1.0.35/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.694673 pycamia-1.0.35/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.695856 pycamia-1.0.35/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.699147 pycamia-1.0.35/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.700315 pycamia-1.0.35/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 08:28:38.000000 pycamia-1.0.35/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.701508 pycamia-1.0.35/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2361 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 08:28:37.000000 pycamia-1.0.35/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.703391 pycamia-1.0.35/pycamia/
+-rw-r--r--   0 admin      (501) staff       (20)     1944 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3453 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/decorators.py
+-rw-r--r--   0 admin      (501) staff       (20)     9424 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/environment.py
+-rw-r--r--   0 admin      (501) staff       (20)     4260 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)      683 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/functions.py
+-rw-r--r--   0 admin      (501) staff       (20)     3814 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/inout.py
+-rw-r--r--   0 admin      (501) staff       (20)    15488 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/listop.py
+-rw-r--r--   0 admin      (501) staff       (20)     6550 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/logging.py
+-rw-r--r--   0 admin      (501) staff       (20)     7135 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     5867 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/math.py
+-rw-r--r--   0 admin      (501) staff       (20)     1061 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/more.py
+-rw-r--r--   0 admin      (501) staff       (20)     1091 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/numpyop.py
+-rw-r--r--   0 admin      (501) staff       (20)     9791 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/strop.py
+-rw-r--r--   0 admin      (501) staff       (20)    21362 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/system.py
+-rw-r--r--   0 admin      (501) staff       (20)    12327 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia/timing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.703902 pycamia-1.0.35/pycamia.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     2048 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       39 2023-07-05 08:28:39.000000 pycamia-1.0.35/pycamia.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 08:28:39.704379 pycamia-1.0.35/pyoverload/
+-rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 08:28:39.000000 pycamia-1.0.35/pyoverload/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 08:28:39.000000 pycamia-1.0.35/pyoverload/override.py
+-rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 08:28:39.000000 pycamia-1.0.35/pyoverload/typehint.py
+-rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 08:28:39.000000 pycamia-1.0.35/pyoverload/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 08:28:39.705004 pycamia-1.0.35/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     7720 2023-07-05 08:28:39.000000 pycamia-1.0.35/setup.py
```

### Comparing `pycamia-1.0.34/PKG-INFO` & `pycamia-1.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.34
+Version: 1.0.35
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.34/README.md` & `pycamia-1.0.35/README.md`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/__init__.py` & `pycamia-1.0.35/batorch/__init__.py`

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

### Comparing `pycamia-1.0.34/batorch/device.py` & `pycamia-1.0.35/batorch/device.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/_reduction.py` & `pycamia-1.0.35/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/common_types.py` & `pycamia-1.0.35/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/functional.py` & `pycamia-1.0.35/batorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/grad.py` & `pycamia-1.0.35/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/init.py` & `pycamia-1.0.35/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/__init__.py` & `pycamia-1.0.35/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/_functions.py` & `pycamia-1.0.35/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/activation.py` & `pycamia-1.0.35/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/adaptive.py` & `pycamia-1.0.35/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/batchnorm.py` & `pycamia-1.0.35/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/container.py` & `pycamia-1.0.35/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/conv.py` & `pycamia-1.0.35/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/distance.py` & `pycamia-1.0.35/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/dropout.py` & `pycamia-1.0.35/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/flatten.py` & `pycamia-1.0.35/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/fold.py` & `pycamia-1.0.35/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/instancenorm.py` & `pycamia-1.0.35/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/linear.py` & `pycamia-1.0.35/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/loss.py` & `pycamia-1.0.35/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/module.py` & `pycamia-1.0.35/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/normalization.py` & `pycamia-1.0.35/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/padding.py` & `pycamia-1.0.35/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/pixelshuffle.py` & `pycamia-1.0.35/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/pooling.py` & `pycamia-1.0.35/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/rnn.py` & `pycamia-1.0.35/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/sparse.py` & `pycamia-1.0.35/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/transformer.py` & `pycamia-1.0.35/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/upsampling.py` & `pycamia-1.0.35/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/modules/utils.py` & `pycamia-1.0.35/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/parameter.py` & `pycamia-1.0.35/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/clip_grad.py` & `pycamia-1.0.35/batorch/nn/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/convert_parameters.py` & `pycamia-1.0.35/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/fusion.py` & `pycamia-1.0.35/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/memory_format.py` & `pycamia-1.0.35/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/prune.py` & `pycamia-1.0.35/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/rnn.py` & `pycamia-1.0.35/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/spectral_norm.py` & `pycamia-1.0.35/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/nn/utils/weight_norm.py` & `pycamia-1.0.35/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/optimizer.py` & `pycamia-1.0.35/batorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/tensor.py` & `pycamia-1.0.35/batorch/tensor.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/tensor2.py` & `pycamia-1.0.35/batorch/tensor2.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/tensorfunc.py` & `pycamia-1.0.35/batorch/tensorfunc.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/torch_namespace.py` & `pycamia-1.0.35/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/batorch/torchext.py` & `pycamia-1.0.35/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/__init__.py` & `pycamia-1.0.35/micomputing/__init__.py`

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

### Comparing `pycamia-1.0.34/micomputing/data.py` & `pycamia-1.0.35/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/funcs.py` & `pycamia-1.0.35/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/metrics.py` & `pycamia-1.0.35/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/network.py` & `pycamia-1.0.35/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/plot.py` & `pycamia-1.0.35/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/stdio.py` & `pycamia-1.0.35/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/test.py` & `pycamia-1.0.35/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/micomputing/trans.py` & `pycamia-1.0.35/micomputing/trans.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/__init__.py` & `pycamia-1.0.35/pycamia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from .manager import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = '<main>',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.33',
-    update = '2023-07-05 14:57:55',
+    version = '1.0.34',
+    update = '2023-07-05 16:20:42',
     contact = 'bertiezhou@163.com',
     keywords = ['environment', 'path', 'touch'],
     description = 'The main package and a background support of project PyCAMIA. ',
     requires = []
 ).check()
 
 from .environment import get_environ_vars, get_environ_globals, get_environ_locals, update_locals_by_environ, get_args_expression, get_declaration, EnvironVars #*
```

### Comparing `pycamia-1.0.34/pycamia/decorators.py` & `pycamia-1.0.35/pycamia/decorators.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/environment.py` & `pycamia-1.0.35/pycamia/environment.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/exception.py` & `pycamia-1.0.35/pycamia/exception.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/functions.py` & `pycamia-1.0.35/pycamia/functions.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/inout.py` & `pycamia-1.0.35/pycamia/inout.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/listop.py` & `pycamia-1.0.35/pycamia/listop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/logging.py` & `pycamia-1.0.35/pycamia/logging.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/manager.py` & `pycamia-1.0.35/pycamia/manager.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/math.py` & `pycamia-1.0.35/pycamia/math.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/more.py` & `pycamia-1.0.35/pycamia/more.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/numpyop.py` & `pycamia-1.0.35/pycamia/numpyop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/strop.py` & `pycamia-1.0.35/pycamia/strop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/system.py` & `pycamia-1.0.35/pycamia/system.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia/timing.py` & `pycamia-1.0.35/pycamia/timing.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pycamia.egg-info/PKG-INFO` & `pycamia-1.0.35/pycamia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.34
+Version: 1.0.35
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.34/pycamia.egg-info/SOURCES.txt` & `pycamia-1.0.35/pycamia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pyoverload/__init__.py` & `pycamia-1.0.35/pyoverload/__init__.py`

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

### Comparing `pycamia-1.0.34/pyoverload/override.py` & `pycamia-1.0.35/pyoverload/override.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pyoverload/typehint.py` & `pycamia-1.0.35/pyoverload/typehint.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/pyoverload/utils.py` & `pycamia-1.0.35/pyoverload/utils.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.34/setup.py` & `pycamia-1.0.35/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'pycamia',
-	version = '1.0.34',
+	version = '1.0.35',
 	keywords = ['pip', 'pymyc', 'pycamia', 'environment', 'path', 'touch'],
 	description = 'The main package and a background support of project PyCAMIA. ',
 	long_description = '# pycamia\n\n## Introduction\n\n[`pycamia`](https://github.com/Bertie97/pycamia/tree/main/pycamia) is the base package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a collection of different useful tools necessary in python programming. `pycamia` was designed for `python v3.6+`. It is consist of the following sub-packages. \n\n1. **environment** is a package containing functions to inspect the context. e.g. get the local variables in the context that calls a function. \n2. **strop** is a collection of advanced functions for strings. e.g. tokenize a string by spliting outside brackets OR find all indices for matched sub-strings.\n3. **listop** is a collection of advanced functions for lists. e.g. flatten a nested list.\n4. **manager** is a package to manage file and package infos. e.g. easily check the dependencies OR easy update the version. \n5. **functions** is a package of special (and commonly trivial) functions. e.g. empty functions. \n6. **exceptions** is a package to handle exceptions. e.g. touch a function and suppress the error OR assert with comment OR quickly create an Error.\n7. **inout** is a package to extend the input/output. e.g. printing to a string OR suppressing the console output. \n8. **timing** is a package to time the executions. e.g. use `with` structure to record time spent for a set of commands. \n9. **more** is a collection of uncategorized functions, one need to import them from `pycamia.more`.\n\n## Installation\n\nThis package can be installed by `pip install pycamia` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pycamia\n```\n\n## Package `environment`\n\nThis package fetches the surrounding environment of the call. It is likely that no more functions would be added to it. If there\'s any suggestion, please contact the developer. \n1. Use `v = get_environ_locals()` or `v = get_environ_globals()` to get the dictionary of local or global variables in the parent environment. If the result is out of expectations, please contact the developer. \n2. Use `v[\'name\']` to read variable `name` and `v[\'name\'] = value` to add variable to the environment. \n\n## Package `strop`\n\nThis package cope with str objects. \n1. Use `str_len` to find the ASCII length for a string, with a length `2` for wide characters.\n2. Use `str_slice` to slice a string by given indices.\n3. Use `find_all` to obtain all the indices of a given string. `str_slice(s, find_all(s, k))` is equivalent to `s.split(k)`. \n4. Use `sorted_dict_repr` to create a repr string for a dictionary with ordered key.\n5. Use `enclosed_object` to find the first object enclosed by brackets. \n6. Use `tokenize` to split a string without breaking enclosed objects. This is useful in breaking text of dictionary structures or arguments. e.g. one can use `tokenize(args, sep=[\',\', \'=\'])[::2]` to find the argument names if `args` is a string in the format `key1=value1, key2 = value2, ...`.\n\n## Package `listop`\n\nThis package cope with list objects. More useful functions will be added to it in the future. \n1. Use `argmin(list, domain)` to find the indices for the minimal value in list. The function only search in the indices `domain`. A list is output as there may be multiple entries. \n2. Use `argmax` to find the indices for the maximal value, similar to `argmin`. \n3. Use `flatten_list` to unwrap the list elements to create a list with no element in type `list`. \n4. Use `prod` to obtain the product of all numbers in the list. \n5. Use `item` to fetch the only element in the list. An error will be raised if there isn\'t any or are more than 1 elements. \n\n## Package `manager`\n\nThis package manages the info of packages and files. One can use it to organize the project. \n1. Use `__info__ = info_manager(project="PyCAMIA", ...)` to list the properties at the front of files. This serve as a brief introduction to readers.\n2. Use `info_manager` at the beginning of `__init__.py`, `pack.py` uses it to create the portrait of a package. \n3. Use `__info__.check_requires()` to automatically check if the dependencies in attribute `requires` exist or not. This is commonly used in `__init__.py`. One can use `__info__ = info_manager(...).check()` to perform an in-place check.\n4. Use `with __info__:` before importing required dependencies as well to perform a double check. \n\n## Package `functions`\n\nThis package contains simple functions. It is the simplest package in the project so far. \n1. Use `empty_function` for a function that does nothing. One can put any argument to the function but nothing would happen. \n2. Use `const_function(a)` for a function that accepts any argument but does nothing and always return `a`.\n\n## Package `exceptions`\n\nThis package handles exceptions. \n1. Use `touch(function)` to try a function and suppress the error in the mean time. e.g. `touch(lambda: 1/a)` returns `None` to tell you that an exception occurs when `a=0`, but returns `1` when `a=1`. \n2. Use `crashed(function)` to check whether a function fails or not. \n3. Use `avouch(bool_to_be_tested, assertion_text)` to avouch that the given expression is true and output your designed `assertion_text` when the test fails. \n4. Use `Error("name")` to creat a new error type. It is the same as creating an Error tag by `class nameError(Exception): pass`.\n\n## Package `inout`\n\nThis package manipulates the input/output. Currently, it only deal with print. Shell handler or other inout functions will be added here in the future. \n1. Use `with no_print:` to suppress the console output. Although not recommended, one can use `with no_print as out_stream:` and `output = str(out_stream)` inside the `with` structure to fetch the output. \n2. Use `sprint = SPrint()` to create a function `sprint` that collects the printed text. Use `out = sprint()` or `sprint.text` to get the results.\n\n## Package `timing`\n\nThis package use the time spent of commands to perform useful inspection or organization of the codes.\n1. Use `@time_this` to time a function.\n2. Use `with Timer("name"):` to time a series of commands.\n3. Use `with scope("name"):` to nest a series of commands. It is an alias of `Timer`. \n4. Use `with scope("name"), jump:` to jump a series of commands. \n5. Use `with scope("name"), Jump(False):` to disable the jump.\n6. Use `wf = Workflow("step1", "step2")` and `with wf("step1(2)"), wf.jump:` before commands of "step1(2)" to create a workflow. One can change the arguments in the init function to decide which steps to run. \n7. Use `@periodic(seconds, max_repeat)` to run a function repeatedly. \n\n## Package `more`\n\nCurrently, only `once` is contained in the `more` package. \nAdding it in a function to check if the function is run once or not. \n\n## Waiting to Be Imroved\n\n1. More functions will be added in the future, including path handler, tools for shell and so on. \n2. Contact us to make suggestions. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/pycamia',
 	author = 'Yuncheng Zhou',
 	author_email = 'bertiezhou@163.com',
 	packages = find_packages(),
-	include_package_data = True,
+	include_package_data = False,
 	platforms = 'any',
-	install_requires = [],
-	doc_files = ['pycamia/functions.py', 'pycamia/logging.py', 'pycamia/exception.py', 'pycamia/system.py', 'pycamia/.DS_Store', 'pycamia/__init__.py', 'pycamia/numpyop.py', 'pycamia/__pycache__', 'pycamia/README.md', 'pycamia/more.py', 'pycamia/timing.py', 'pycamia/environment.py', 'pycamia/listop.py', 'pycamia/math.py', 'pycamia/inout.py', 'pycamia/strop.py', 'pycamia/manager.py', 'pycamia/decorators.py']
+	install_requires = []
 )
```

