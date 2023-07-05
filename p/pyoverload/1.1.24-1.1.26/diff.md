# Comparing `tmp/pyoverload-1.1.24.tar.gz` & `tmp/pyoverload-1.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverload-1.1.24.tar", last modified: Fri Jan 14 14:16:01 2022, max compression
+gzip compressed data, was "pyoverload-1.1.26.tar", last modified: Wed Jul  5 06:46:34 2023, max compression
```

## Comparing `pyoverload-1.1.24.tar` & `pyoverload-1.1.26.tar`

### file list

```diff
@@ -1,24 +1,78 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-01-14 14:16:01.611017 pyoverload-1.1.24/
--rw-r--r--   0 admin      (501) staff       (20)    14796 2022-01-14 14:16:01.610895 pyoverload-1.1.24/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)    12305 2022-01-14 14:16:01.000000 pyoverload-1.1.24/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-01-14 14:16:01.609226 pyoverload-1.1.24/batorch/
--rw-r--r--   0 admin      (501) staff       (20)      644 2022-01-14 14:16:01.000000 pyoverload-1.1.24/batorch/__init__.py
--rwxr-xr-x   0 admin      (501) staff       (20)      366 2022-01-14 14:16:01.000000 pyoverload-1.1.24/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    70102 2022-01-14 14:16:01.000000 pyoverload-1.1.24/batorch/tensor_tp.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-01-14 14:16:01.609738 pyoverload-1.1.24/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)      925 2022-01-14 14:16:00.000000 pyoverload-1.1.24/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    12277 2022-01-14 14:16:00.000000 pyoverload-1.1.24/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    14933 2022-01-14 14:16:00.000000 pyoverload-1.1.24/micomputing/sim.py
--rw-r--r--   0 admin      (501) staff       (20)    31479 2022-01-14 14:16:00.000000 pyoverload-1.1.24/micomputing/stdio.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-01-14 14:16:01.610246 pyoverload-1.1.24/pyoverload/
--rw-r--r--   0 admin      (501) staff       (20)      889 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    11609 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload/override.py
--rw-r--r--   0 admin      (501) staff       (20)    31736 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload/typehint.py
--rw-r--r--   0 admin      (501) staff       (20)     2289 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload/utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-01-14 14:16:01.610685 pyoverload-1.1.24/pyoverload.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    14796 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      386 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       31 2022-01-14 14:16:01.000000 pyoverload-1.1.24/pyoverload.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-01-14 14:16:01.611061 pyoverload-1.1.24/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)    13174 2022-01-14 14:16:01.000000 pyoverload-1.1.24/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.014128 pyoverload-1.1.26/
+-rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 06:46:34.013996 pyoverload-1.1.26/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)    12301 2023-07-05 06:46:33.000000 pyoverload-1.1.26/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.004448 pyoverload-1.1.26/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.005434 pyoverload-1.1.26/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.009619 pyoverload-1.1.26/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.010938 pyoverload-1.1.26/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 06:46:33.000000 pyoverload-1.1.26/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.012189 pyoverload-1.1.26/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 06:46:31.000000 pyoverload-1.1.26/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.012741 pyoverload-1.1.26/pyoverload/
+-rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload/override.py
+-rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload/typehint.py
+-rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload/utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.013746 pyoverload-1.1.26/pyoverload.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    14792 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1809 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        8 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       31 2023-07-05 06:46:33.000000 pyoverload-1.1.26/pyoverload.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 06:46:34.014176 pyoverload-1.1.26/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)    13179 2023-07-05 06:46:33.000000 pyoverload-1.1.26/setup.py
```

### Comparing `pyoverload-1.1.24/PKG-INFO` & `pyoverload-1.1.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverload
-Version: 1.1.24
+Version: 1.1.26
 Summary: 'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. 
 Home-page: https://github.com/Bertie97/PyZMyc/pyoverload
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pyoverload
         
@@ -210,15 +210,15 @@
         
         The basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, 
         
         1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. 
         2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.
         3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. 
         4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.
-        5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `torchplus` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.TorchPlus` to identify specific packages. 
+        5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `batorch` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.Batorch` to identify specific packages. 
         6. `Iterable` includes `Array`, `Sequence` and `dict`. 
         7. Three types of `Scalar`s support the array variables.
         
         All these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. 
         
         One can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned.
```

### Comparing `pyoverload-1.1.24/README.md` & `pyoverload-1.1.26/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
 The basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, 
 
 1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. 
 2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.
 3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. 
 4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.
-5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `torchplus` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.TorchPlus` to identify specific packages. 
+5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `batorch` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.Batorch` to identify specific packages. 
 6. `Iterable` includes `Array`, `Sequence` and `dict`. 
 7. Three types of `Scalar`s support the array variables.
 
 All these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. 
 
 One can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned.
```

### Comparing `pyoverload-1.1.24/batorch/tensor_tp.py` & `pyoverload-1.1.26/batorch/tensor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,184 @@
-#! python3.8 -u
-#  -*- coding: utf-8 -*-
 
-##############################
-## Project PyCTLib
-## Package torchplus
-##############################
+from pycamia import info_manager
+
+__info__ = info_manager(
+    project = "PyCAMIA",
+    package = "batorch",
+    fileinfo = "The inherited tensor from 'torch' with batch.",
+    requires = "torch"
+)
 
 __all__ = """
-    Device
-    DeviceCPU
+    CPU
+    GPU
+    GPUs
     Tensor
     Size
-    set_autodevice
-    unset_autodevice
-    is_autodevice
+    set_device
+    get_device
+    to_device
+    turn_on_autodevice
+    turn_off_autodevice
+    get_cpu_memory_used
+    get_gpu_memory_used
+    inv
+    diag
+    batch_tensor
+    channel_tensor
 """.split()
 
-try:
-    import torch
-except ImportError:
-    raise ImportError("'pyctlib.torchplus' cannot be used without dependency 'torch'.")
-import typing
-import inspect
-import builtins
-import torchplus as tp
-from .tensorfunc import __all__ as tf_list
-# from pyoverload import overload, override, Tuple, List, Set, params, null, Array, isarray, isoftype, isofsubclass, isint, isdtype, isitertype, isclassmethod
-from pyoverload import *
-from pyctlib import raw_function, return_type_wrapper, touch, vector
-#from pyctlib.visual.debugger import profile
+import builtins, sys
 from functools import wraps
-from types import GeneratorType, MethodWrapperType
-from collections import OrderedDict
+from typing import Generator
+from .tensorfunc import __all__ as tf_list
 from .torch_namespace import *
-from .device import AutoDevice as Device, DeviceCPU
-
-"""
-from torchplus import Tensor
-import torchplus as tp
-"""
-
-# Device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-
-_auto_device = True
+from .device import GB, CPU, GPU, GPUs, AutoDevice, FixedDevice
 
-def set_autodevice(flag=True):
-    global _auto_device
-    _auto_device = flag
-
-def unset_autodevice():
-    global _auto_device
-    _auto_device = False
-
-def is_autodevice():
-    global _auto_device
-    return _auto_device
+with __info__:
+    import torch
+    import batorch as bt
+    from pycamia import ByteSize
+    from pycamia import avouch, alias, execblock
+    from pycamia import get_alphas, arg_tuple, max_argmax
+    from pycamia import argmax as _argmax, item, to_list
+    from pyoverload import Type, Array, isoftype, Iterable
 
 INT = builtins.int
 MIN = builtins.min
 MAX = builtins.max
 ANY = builtins.any
 ALL = builtins.all
+SUM = builtins.sum
 RANGE = builtins.range
 FLOAT = builtins.float
 NUM = (INT, FLOAT)
 
+_device = AutoDevice(verbose=True, always_proceed=True)
+_total_cpu_memory_used = 0
+_total_gpu_memory_used = 0
+
+new_dim_inherit_methods = """multiply multiple""".split()
+new_dim_methods = """unsqueeze unsqueeze_ multiply multiple""".split()
+old_dim_methods = """
+    squeeze squeeze_ transpose transpose_ movedim movedim_ splitdim repeated amplify ample sample pick split flip
+    cummin cummax cumsum cumprod sum prod min max median mean std argmin argmax
+""".split()
+one_dim_methods_last = """multiply multiple repeated amplify ample sample split flip""".split()
+one_dim_methods_first = """splitdim""".split()
+avouch(all(x in new_dim_methods for x in new_dim_inherit_methods))
+
+def set_device(device):
+    if isinstance(device, AutoDevice): new_device = device
+    elif isinstance(device, torch.device): new_device = FixedDevice(device)
+    else: raise TypeError("Invalid device type. ")
+    global _device
+    _device = new_device
+
+def get_device():
+    global _device
+    return _device
+
+def to_device(x):
+    global _device
+    return _device(x)
+
+def turn_on_autodevice(): _device.turn_on()
+def turn_off_autodevice(): _device.turn_off()
+
+def get_cpu_memory_used():
+    global _total_cpu_memory_used
+    return ByteSize(_total_cpu_memory_used)
+
+def get_gpu_memory_used():
+    global _total_gpu_memory_used
+    return ByteSize(_total_gpu_memory_used)
+
 def kwget(kwargs, key, default):
     if kwargs is None: return default
     else: return kwargs.get(key, default)
+    
+def dim_method_wrapper(func):
+    if hasattr(func, '__wrapped__'): name = func.__wrapped__.__name__
+    else: name = func.__name__
+    if name not in new_dim_methods and name not in old_dim_methods: return func
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        single = False
+        domain = args; key = None
+        if 'dim' in kwargs: domain = kwargs['dim']; key = 'dim'
+        elif 'dims' in kwargs: domain = kwargs['dims']; key = 'dims'
+        if not isinstance(domain, tuple): domain = (domain,); single = True
+        pre_args = []
+        post_args = []
+        if len(domain) > 1 and name in one_dim_methods_last:
+            *pre_args, d = domain
+            domain = (d,); single = True
+        if len(domain) > 1 and name in one_dim_methods_first:
+            d, *post_args = domain
+            domain = (d,); single = True
+        
+        new_domain = []
+        if name in new_dim_methods:
+            ibatch = ichannel = None
+            for i, d in enumerate(domain):
+                cls = None
+                if isinstance(d, list) and len(d) == 0: ibatch = 0; d = ibatch; cls = list
+                elif isinstance(d, dict) and len(d) == 0: ichannel = 1 if self.batch_dim == 0 else 0; d = ichannel; cls = set
+                elif isinstance(d, list) and len(d) == 1: ibatch = d[0]; d = ibatch; cls = list
+                elif isinstance(d, set) and len(d) == 1: ichannel = list(d)[0]; d = ichannel; cls = set
+                if isinstance(d, INT):
+                    l, u = - self.ndim - 1, self.ndim
+                    if not l <= d <= u:
+                        raise IndexError(f"Dimension out of range (expected to be in range of [{l}, {u}], but got {d})")
+                    d += self.ndim + i + 1 if d < 0 and 'squeeze' not in name else 0
+                if name in new_dim_inherit_methods and cls is not None: d = cls([d])
+                new_domain.append(d)
+        elif name in old_dim_methods:
+            for d in domain:
+                if isinstance(d, list) and len(d) <= 1: d = self.batch_dimension
+                elif isinstance(d, dict) and len(d) == 0 or isinstance(d, set) and len(d) == 1:
+                    d = self.channel_dimension
+                if isinstance(d, INT): d += self.ndim if d < 0 and 'squeeze' not in name else 0
+                new_domain.append(d)
+
+        domain = tuple(new_domain)
+        if key is None: args = domain
+        else: kwargs[key] = domain[0] if single else domain
+
+        if name in new_dim_methods and name not in new_dim_inherit_methods:
+            if ibatch is not None: kwargs['batch_dim'] = ibatch
+            if ichannel is not None: kwargs['channel_dim'] = ichannel
+
+        args = tuple(pre_args) + args + tuple(post_args)
+        return func(self, *args, **kwargs)
+    return wrapper
 
 class Size(tuple):
 
-    NegSizeError = TypeError("Size cannot have negative values except -1 indicating arbitrary number. ")
+    NegSizeError = TypeError("Size cannot have negative values except -1 indicating an arbitrary number. ")
 
     def __new__(cls, *args, **kwargs):
 
         if len(args) == 1:
             arg = args[0]
             if hasattr(arg, 'shape'): arg = arg.shape
             if isinstance(arg, (INT, set)): pass
+            elif isinstance(arg, Size): args = arg.python_repr
             elif isinstance(arg, tuple): args = arg
-            elif isinstance(arg, GeneratorType):
+            elif isinstance(arg, Generator):
                 self = super().__new__(cls, arg)
                 self.ndim = len(tuple(arg))
-                return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
+                return self.set_special_(kwargs.get('batch_dim', self.ndim), kwargs.get('channel_dim', self.ndim))
             elif isinstance(arg, list):
                 l = len(arg)
                 if l != 1:
                     self = super().__new__(cls, arg)
                     self.ndim = l
-                    return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
+                    return self.set_special_(kwargs.get('batch_dim', self.ndim), kwargs.get('channel_dim', self.ndim))
             elif isinstance(arg, Size):
                 self = super().__new__(cls, arg.tuple())
                 self.ndim = arg.ndim
                 self._special = arg._special
                 self._batch_first = arg._batch_first
                 return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
             else:
@@ -107,63 +192,85 @@
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
-                raw_args.append(a.pop())
+                raw_args.append(list(a)[0] if len(a) > 0 else -1)
 
             else: raw_args.append(a)
 
         self = super().__new__(cls, raw_args)
         self.ndim = ndim
         return self.set_special_(kwargs.get('batch_dim', batch_dim), kwargs.get('channel_dim', channel_dim))
 
     def tuple(self): return super().__new__(tuple, self)
 
+    @alias("b_dim", "batch_dim")
     @property
-    def batch_dimension(self): return self._special[0 if self._batch_first else 1]
+    def batch_dimension(self): return self._batch_dimension if self._batch_dimension < self.ndim else None
 
+    @alias("b_dim", "batch_dim")
     @batch_dimension.setter
-    def batch_dimension(self, batch_dim):
+    def batch_dimension(self, batch_dim): return self.batch_dimension_(batch_dim)
+
+    @property
+    def _batch_dimension(self): return self._special[0 if self._batch_first else 1]
+
+    @_batch_dimension.setter
+    def _batch_dimension(self, batch_dim):
         self.set_special_(batch_dim, None)
 
+    @alias("b_dim_", "batch_dim_", "with_batchdim")
     def batch_dimension_(self, value):
-        self.batch_dimension = value
+        if value is None: value = self.ndim
+        self._batch_dimension = value
         return self
 
+    @alias("n_batch", "nbatch")
     @property
     def batch_size(self):
-        batch_dim = self.batch_dimension
+        batch_dim = self._batch_dimension
         if batch_dim == self.ndim:
             raise ValueError("There is no batch dimension provided. ")
         return self[batch_dim]
 
+    @alias("c_dim", "channel_dim")
     @property
-    def channel_dimension(self): return self._special[1 if self._batch_first else 0]
+    def channel_dimension(self): return self._channel_dimension if self._channel_dimension < self.ndim else None
 
+    @alias("c_dim", "channel_dim")
     @channel_dimension.setter
-    def channel_dimension(self, channel_dim):
+    def channel_dimension(self, channel_dim): return self.channel_dimension_(channel_dim)
+
+    @property
+    def _channel_dimension(self): return self._special[1 if self._batch_first else 0]
+
+    @_channel_dimension.setter
+    def _channel_dimension(self, channel_dim):
         self.set_special_(None, channel_dim)
 
+    @alias("c_dim_", "channel_dim_", "with_channeldim")
     def channel_dimension_(self, value):
-        self.channel_dimension = value
+        if value is None: value = self.ndim
+        self._channel_dimension = value
         return self
 
+    @alias("n_channel", "nchannel")
     @property
     def channel_size(self):
-        channel_dim = self.channel_dimension
+        channel_dim = self._channel_dimension
         if channel_dim is None:
             raise ValueError("There is no channel dimension provided. ")
         return self[channel_dim]
 
     @property
     def special(self): return [x for x in self._special if x < self.ndim]
 
@@ -178,45 +285,50 @@
 
         return self
 
     def add_special_from_(self, other=None):
 
         if isinstance(other, Size):
 
-            doit = False
             batch_dim = None
             channel_dim = None
+            doit = False
 
-            if self.batch_dimension == self.ndim:
-                batch_dim = other.batch_dimension
+            if self._batch_dimension == self.ndim:
+                batch_dim = other._batch_dimension
                 if batch_dim != self.ndim:
                     doit = True
-            if self.channel_dimension == self.ndim:
-                channel_dim = other.channel_dimension
+            if self._channel_dimension == self.ndim:
+                channel_dim = other._channel_dimension
                 if channel_dim != self.ndim:
                     doit = True
             if doit: self.set_special_(batch_dim, channel_dim)
 
         return self
 
     def set_special_(self, batch_dim=None, channel_dim=None):
+        """
+        'batch_dim/channel_dim = None' means skip assignment. 
+        """
 
         if batch_dim is not None:
             if not isinstance(batch_dim, INT): batch_dim = self.ndim
             if batch_dim < 0: batch_dim = batch_dim + self.ndim
             if not 0 <= batch_dim <= self.ndim:
                 raise TypeError(f"batch_dimension should be a dimension index which is smaller than {self.ndim}. ")
-        else: batch_dim = self.ndim
+        else:
+            batch_dim = MIN(self._batch_dimension, self.ndim)
 
         if channel_dim is not None:
             if not isinstance(channel_dim, INT): channel_dim = self.ndim
             if channel_dim < 0: channel_dim = channel_dim + self.ndim
             if not 0 <= channel_dim <= self.ndim:
                 raise TypeError(f"channel_dimension should be a dimension index which is smaller than {self.ndim}. ")
-        else: channel_dim = self.ndim
+        else:
+            channel_dim = MIN(self._channel_dimension, self.ndim)
 
         if batch_dim is None and channel_dim is None: return self
 
         if batch_dim < channel_dim:
             self._batch_first = True
             self._special = [batch_dim, channel_dim]
         elif channel_dim < batch_dim:
@@ -249,44 +361,56 @@
         if s[0] < self.ndim: res += (value,)
         else: return Size(res).special_from_(self)
         res += t[s[0]+1:s[1]]
         if s[1] < self.ndim: res += (value,)
         else: return Size(res).special_from_(self)
         res += t[s[1]+1:]
         return Size(res).special_from_(self)
+    
+    def with_dimsize(self, k, dim):
+        if isinstance(dim, list) and len(dim) in {0, 1}: dim = self.batch_dimension
+        elif isinstance(dim, dict) and len(dim) == 0: dim = self.channel_dimension
+        elif isinstance(dim, set) and len(dim) == 1: dim = self.channel_dimension
+        elif isinstance(dim, INT) and dim < 0: dim += self.n_dim
+
+        return self[:dim] + bt.Size([k] if dim == self.batch_dimension else ({k} if dim == self.channel_dimension else k)) + self[dim+1:]
 
     @property
     def space(self):
         s = self._special
         t = tuple(self)
         return t[:s[0]] + t[s[0]+1:s[1]] + t[s[1]+1:]
 
+    def reset_space(self, *p):
+        p = arg_tuple(p)
+        s = self._special
+        if s[0] == self.n_dim: return bt.Size(p)
+        t = tuple(self)
+        return bt.Size(p[:s[0]] + t[s[0]:s[0]+1] + p[s[0]:s[1]-1] + t[s[1]:s[1]+1] + p[s[1]-1:]).special_from_(self)
+
     @property
     def nele(self):
         p = 1
         for i in self:
             if i == -1: return -1
             p *= i
         return p
 
     def __len__(self): return self.ndim
 
     @property
     def n_dim(self): return self.ndim
 
+    @alias('nspace')
     @property
-    def nspace(self): return self.ndim - (self._special[0] < self.ndim) - (self._special[1] < self.ndim)
+    def n_space(self): return self.ndim - (self._special[0] < self.ndim) - (self._special[1] < self.ndim)
 
+    @alias('nspecial')
     @property
-    def nspecial(self): return (self._special[0] < self.ndim) + (self._special[1] < self.ndim)
-
-    nbatch = batch_size
-    nchannel = channel_size
-    n_space = nspace
-    n_special = nspecial
+    def n_special(self): return (self._special[0] < self.ndim) + (self._special[1] < self.ndim)
 
     @property
     def has_batch(self): return self._special[0 if self._batch_first else 1] < self.ndim
 
     @property
     def has_channel(self): return self._special[1 if self._batch_first else 0] < self.ndim
 
@@ -296,35 +420,35 @@
     def remove_special_(self):
         self._special = [self.ndim, self.ndim]
         self._batch_first = True
         return self
 
     def copy(self): return Size(self)
 
-    def __add__(self, other: [tuple, 'Size']):
+    def __add__(self, other: tuple):
         if not isinstance(other, tuple):
             raise TypeError("Only Size+tuple is available for Size as a python tuple, "
                             "please use size << 1 to increase the size numerically. ")
         if not isinstance(other, Size):
             return Size(tuple(self) + other).special_from_(self)
 
         ndim = self.ndim + other.ndim
         batch_dim = channel_dim = ndim
-        if self.has_batch: batch_dim = self.batch_dimension
+        if self.has_batch: batch_dim = self._batch_dimension
         if other.has_batch:
             if batch_dim < ndim: raise TypeError("Batch dimension conflict in addition. ")
-            batch_dim = self.ndim + other.batch_dimension
-        if self.has_channel: channel_dim = self.channel_dimension
+            batch_dim = self.ndim + other._batch_dimension
+        if self.has_channel: channel_dim = self._channel_dimension
         if other.has_channel:
             if channel_dim < ndim: raise TypeError("Channel dimension conflict in addition. ")
-            channel_dim = self.ndim + other.channel_dimension
+            channel_dim = self.ndim + other._channel_dimension
 
         return Size(tuple(self) + tuple(other), batch_dim=batch_dim, channel_dim=channel_dim)
 
-    def __radd__(self, other: [tuple, 'Size']):
+    def __radd__(self, other: tuple):
         if not isinstance(other, tuple):
             raise TypeError("Only Size+tuple is available for Size as a python tuple, "
                             "please use size << 1 to increase the size numerically. ")
         if not isinstance(other, Size):
             other = Size(other)
         return other + self
     __iadd__ = __add__
@@ -333,15 +457,15 @@
         if not isinstance(value, INT):
             raise TypeError("Only Size*int is available for Size as a python tuple, "
                             "please use size ** 1 to do the multiply numerically. ")
         return Size(tuple(self) * value).special_from_(self)
     __imul__ = __rmul__ = __mul__
 
     @staticmethod
-    def __op__(a: [INT, tuple, 'Size'], b: [INT, tuple, 'Size'], *, op):
+    def __op__(a: Type(INT, tuple), b: Type(INT, tuple), *, op):
 
         def getvalue(x, y, r):
             if x == -2: return y
             if y == -2: return x
             if x == -1 or y == -1: return -1
             if r: z = op(y, x)
             else: z = op(x, y)
@@ -376,31 +500,31 @@
             raise LengthError
         if a.nspace == b.ndim: b = a.insert_special_to_tuple(b, -2)
         if a.ndim == b.ndim:
             if a._special == b._special: return Size(getvalue(x, y, rev) for x, y in zip(a, b)).add_special_from_(a).add_special_from_(b)
             raise TypeError("Only Sizes with same batch/channel dimensions can be operated. ")
         else: raise LengthError
 
-    def __lshift__(self, other: [INT, tuple, 'Size']): return self.__op__(self, other, op=lambda x, y: x + y)
+    def __lshift__(self, other: Type(INT, tuple)): return self.__op__(self, other, op=lambda x, y: x + y)
     __ilshift__ = __rlshift__ = __lshift__
 
-    def __rshift__(self, other: [INT, tuple, 'Size']): return Size.__op__(self, other, op=lambda x, y: x - y)
+    def __rshift__(self, other: Type(INT, tuple)): return Size.__op__(self, other, op=lambda x, y: x - y)
 
-    def __rrshift__(self, other: [INT, tuple, 'Size']): return Size.__op__(other, self, op=lambda x, y: x - y)
+    def __rrshift__(self, other: Type(INT, tuple)): return Size.__op__(other, self, op=lambda x, y: x - y)
     __irshift__ = __rshift__
 
-    def __pow__(self, other: [INT, tuple, 'Size']): return Size.__op__(self, other, op=lambda x, y: x * y)
+    def __pow__(self, other: Type(INT, tuple)): return Size.__op__(self, other, op=lambda x, y: x * y)
     __ipow__ = __rpow__ = __pow__
 
-    def __floordiv__(self, other: [INT, tuple, 'Size']): return Size.__op__(self, other, op=lambda x, y: x // y)
+    def __floordiv__(self, other: Type(INT, tuple)): return Size.__op__(self, other, op=lambda x, y: x // y)
 
-    def __rfloordiv__(self, other: [INT, tuple, 'Size']): return Size.__op__(other, self, op=lambda x, y: x // y)
+    def __rfloordiv__(self, other: Type(INT, tuple)): return Size.__op__(other, self, op=lambda x, y: x // y)
     __ifloordiv__ = __floordiv__
 
-    def __xor__(self, other: [tuple, 'Size']):
+    def __xor__(self, other: tuple):
 
         if not isinstance(other, Size): other = Size(other)
 
         if self.ndim == 0: return (Size(1) * other.ndim).special_from_(other), other
         elif other.ndim == 0: return self, (Size(1) * self.ndim).special_from_(self)
 
         if self.ndim == other.ndim:
@@ -439,95 +563,145 @@
             if self._batch_first: batch_dim, channel_dim = len1, len1 + len2 + 1
             else: batch_dim, channel_dim = len1 + len2 + 1, len1
             exp_self = Size(exp_self, batch_dim=batch_dim, channel_dim=channel_dim)
             exp_other = Size(exp_other, batch_dim=batch_dim, channel_dim=channel_dim)
             return exp_self, exp_other
 
         if self.has_batch and other.has_batch:
-            lp_self, lp_other = self[:self.batch_dimension] ^ other[:other.batch_dimension]
-            rp_self, rp_other = self[self.batch_dimension+1:] ^ other[other.batch_dimension+1:]
+            lp_self, lp_other = self[:self._batch_dimension] ^ other[:other._batch_dimension]
+            rp_self, rp_other = self[self._batch_dimension+1:] ^ other[other._batch_dimension+1:]
             return (
                 lp_self + Size([self.batch_size]) + rp_self,
                 lp_other + Size([other.batch_size]) + rp_other
             )
 
         if self.has_channel and other.has_channel:
-            lp_self, lp_other = self[:self.channel_dimension] ^ other[:other.channel_dimension]
-            rp_self, rp_other = self[self.channel_dimension+1:] ^ other[other.channel_dimension+1:]
+            lp_self, lp_other = self[:self._channel_dimension] ^ other[:other._channel_dimension]
+            rp_self, rp_other = self[self._channel_dimension+1:] ^ other[other._channel_dimension+1:]
             return (
                 lp_self + Size({self.channel_size}) + rp_self,
                 lp_other + Size({other.channel_size}) + rp_other
             )
+        
+        tself = tuple(self)
+        tother = tuple(other)
+        if ALL([a == b for a, b in zip(tself, tother)]):
+            ext_self = tuple()
+            ext_other = tuple()
+            if len(tself) >= len(tother): ext_other = (1,) * (len(tself) - len(tother))
+            else: ext_self = (1,) * (len(tother) - len(tself))
+            return (self + ext_self).add_special_from_(other), (other + ext_other).add_special_from_(self)
+
+        if ALL([a == b for a, b in zip(tself[::-1], tother[::-1])]):
+            ext_self = tuple()
+            ext_other = tuple()
+            if len(tself) >= len(tother): ext_other = (1,) * (len(tself) - len(tother))
+            else: ext_self = (1,) * (len(tother) - len(tself))
+            return (ext_self + self).add_special_from_(other), (ext_other + other).add_special_from_(self)
 
-        raise RuntimeError("Unexpected error occurs in sizes expanding, please contact developers for more information. ")
+        raise RuntimeError(f"Unexpected error occurs in sizes expanding of {self}, {other}. Please confirm that they can be expanded together. Contact the developers for more information (Error Code: B241). ")
     __ixor__ = __rxor__ = __xor__
 
     def __getitem__(self, k):
         if isinstance(k, INT): return super().__getitem__(k)
         return Size(*self.python_repr[k])
 
     @property
     def python_repr(self):
         args = list(self)
-        batch_dim = self.batch_dimension
+        batch_dim = self._batch_dimension
         if batch_dim < self.ndim: args[batch_dim] = [args[batch_dim]]
-        channel_dim = self.channel_dimension
+        channel_dim = self._channel_dimension
         if channel_dim < self.ndim: args[channel_dim] = {args[channel_dim]}
         return tuple(args)
 
     def __str__(self):
         rep = self.python_repr
         if len(rep) == 1: rep = str(rep).replace(',', '')
-        return f"torchplus.Size{rep}"
+        return f"batorch.Size{rep}"
     __repr__ = __str__
 
+def collect_memory(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        ret = func(*args, **kwargs)
+        if ret.device == CPU.main_device:
+            global _total_cpu_memory_used
+            _total_cpu_memory_used += ret.byte_size()
+        else:
+            global _total_gpu_memory_used
+            _total_gpu_memory_used += ret.byte_size()
+        return ret
+    return wrapper
+
 class Tensor(torch.Tensor):
 
     init = False
 
     @staticmethod
-    def _make_subclass(cls, data, auto_device=_auto_device, requires_grad=False, device=None):
-        to_device = None
-        if device is None and auto_device: to_device = Device
-        if device is not None: to_device = device
-        if to_device is not None and to_device != data.device: data = data.to(to_device)
+    def _make_subclass(cls, data, requires_grad=False, device=None):
+        avouch(isinstance(device, AutoDevice), "Please use `AutoDevice` in batorch.Tensor._make_subclass. Please contact the developers if you did not use Tensor._make_subclass directly (Error Code: B242). ")
+        data = device(data)
         self = torch.Tensor._make_subclass(cls, data, requires_grad)
         if isinstance(data, Tensor): return self.special_from_(data)
         return self
 
+    @collect_memory
     def __new__(cls, *args, **kwargs):
-
-        to_device = kwargs.get('device', Device if kwargs.get('auto_device', _auto_device) else None)
+        
+        batch_dim = channel_dim = None
+        for k in kwargs:
+            if 'dim' in k:
+                if k.startswith('b'): batch_dim = kwargs[k]
+                if k.startswith('c'): channel_dim = kwargs[k]
+        dev = kwargs.get('device', _device)
+        if isinstance(dev, AutoDevice): dev = dev.device
+        cpu = torch.device('cpu')
 
         if len(args) == 1:
             arg = args[0]
             if isinstance(arg, INT): pass
-            elif isinstance(arg, torch.Tensor) and (to_device is None or arg.device == to_device):
-                self = arg.as_subclass(Tensor)
-                self.requires_grad = kwargs.get('requires_grad', arg.requires_grad)
-                return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
+            elif isinstance(arg, torch.Tensor):
+                rg = kwargs.get('requires_grad', getattr(arg, 'requires_grad', False))
+                self = super()._make_subclass(cls, arg, rg)
+                if dev != cpu: self = self.to(dev)
+                return self.set_special_(batch_dim, channel_dim)
+            elif hasattr(arg, '__tensor__'): return arg.__tensor__()
             elif hasattr(arg, 'shape') or isinstance(arg, list):
-                if not isinstance(arg, torch.Tensor):
-                    if to_device is None: arg = torch.as_tensor(arg)
-                    else: arg = torch.as_tensor(arg, device=to_device)
-                rg = kwargs.get('requires_grad', arg.requires_grad)
-                if to_device is None or arg.device == to_device:
-                    self = super()._make_subclass(cls, arg, rg)
-                else:
-                    self = super()._make_subclass(cls, arg.to(to_device), rg)
+                rg = kwargs.get('requires_grad', getattr(arg, 'requires_grad', False))
+                self = super().__new__(cls, arg)
+                avouch(self.device == cpu)
+                self.requires_grad = rg
                 self.special_from_(arg)
-                return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
+                return self.set_special_(batch_dim, channel_dim)
             elif isinstance(arg, tuple): args = arg
-            else: raise TypeError("Unrecognized initialization of 'Tensor'. ")
+            else: raise TypeError(f"Unrecognized initialization of 'Tensor': {arg}. ")
 
         # args is a tuple of integers (or a Size)
-        if to_device is None: self = super().__new__(cls, *args, **kwargs)
-        else: self = super().__new__(cls, *args, device=to_device, **kwargs)
+        kwargs.update(dict(device=dev))
+        rg = kwargs.pop('requires_grad', False)
+        dev = kwargs.pop('device', cpu)
+        self = super().__new__(cls, *args, **kwargs)
+        if dev != cpu: self = self.to(dev)
         self.special_from_(args)
-        return self.set_special_(kwargs.get('batch_dim', None), kwargs.get('channel_dim', None))
+        return self.set_special_(batch_dim, channel_dim).requires_grad_(rg)
+
+    # def __del__(self):
+    #     # Release record
+    #     if self.device == CPU.main_device:
+    #         global _total_cpu_memory_used
+    #         _total_cpu_memory_used -= self.byte_size()
+    #     else:
+    #         global _total_gpu_memory_used
+    #         _total_gpu_memory_used -= self.byte_size()
+    #     # Delete self
+        
+    @property
+    def ref_count(self):
+        return sys.getrefcount(self) - 3
 
     def requires_grad_(self, mode=True):
         self.requires_grad = mode
         return self
 
     def refine_names(self, *args, kwargs):
         self.has_names = True
@@ -539,104 +713,122 @@
     @property
     def shape(self):
         shape = Size(super().shape)
         shape.special_from_(self)
         if self.has_names():
             if not shape.has_batch:
                 isbatch = [('batch' in x.lower()) if x else x for x in self.names]
-                if ANY(isbatch):
-                    ibatch = isbatch.index(True)
+                if ANY(isbatch): shape._batch_dimension = isbatch.index(True)
             if not shape.has_channel:
                 ischannel = [('channel' in x.lower()) if x else x for x in self.names]
-                if ANY(ischannel):
-                    ichannel = ischannel.index(True)
+                if ANY(ischannel): shape._channel_dimension = ischannel.index(True)
         return shape
 
     def rename(self, *args, **kwargs):
         ibatch = ichannel = None
-        for i, n in enumerate(args):
-            if not isinstance(n, str): continue
+        for i, x in enumerate(args):
+            if not isinstance(x, str): continue
             elif 'batch' in x.lower():
                 if ibatch is not None:
                     raise TypeError("Multiple batch dimensions not supported. ")
                 ibatch = i
             elif 'channel' in x.lower():
                 if ichannel is not None:
                     raise TypeError("Multiple channel dimensions not supported. ")
                 ichannel = i
             if ibatch is not None and ichannel is not None: break
         return super().rename(*args, **kwargs)
 
     def refine_names(self, *args):
         ibatch = ichannel = None
-        for i, n in enumerate(args):
-            if not isinstance(n, str): continue
+        for i, x in enumerate(args):
+            if not isinstance(x, str): continue
             elif 'batch' in x.lower():
                 if ibatch is not None:
                     raise TypeError("Multiple batch dimensions not supported. ")
                 ibatch = i
             elif 'channel' in x.lower():
                 if ichannel is not None:
                     raise TypeError("Multiple channel dimensions not supported. ")
                 ichannel = i
             if ibatch is not None and ichannel is not None: break
         return super().refine_names(*args)
-        
+
+    @alias("b_dim", "batch_dim")
     @property
-    def batch_dimension(self): return self._special[0 if self._batch_first else 1]
+    def batch_dimension(self): return self._batch_dimension if self._batch_dimension < self.ndim else None
 
+    @alias("b_dim", "batch_dim")
     @batch_dimension.setter
-    def batch_dimension(self, batch_dim):
+    def batch_dimension(self, batch_dim): return self.batch_dimension_(batch_dim)
+
+    @property
+    def _batch_dimension(self): return self._special[0 if self._batch_first else 1]
+
+    @_batch_dimension.setter
+    def _batch_dimension(self, batch_dim):
         self.set_special_(batch_dim, None)
 
+    @alias("b_dim_", "batch_dim_", "with_batchdim")
     def batch_dimension_(self, value):
-        self.batch_dimension = value
+        if value is None: value = self.ndim
+        self._batch_dimension = value
         return self
 
+    @alias("n_batch", "nbatch")
     @property
     def batch_size(self): return self.shape.batch_size
 
+    @alias("c_dim", "channel_dim")
     @property
-    def channel_dimension(self): return self._special[1 if self._batch_first else 0]
+    def channel_dimension(self): return self._channel_dimension if self._channel_dimension < self.ndim else None
 
+    @alias("c_dim", "channel_dim")
     @channel_dimension.setter
-    def channel_dimension(self, channel_dim):
+    def channel_dimension(self, channel_dim): return self.channel_dimension_(channel_dim)
+
+    @property
+    def _channel_dimension(self): return self._special[1 if self._batch_first else 0]
+
+    @_channel_dimension.setter
+    def _channel_dimension(self, channel_dim):
         self.set_special_(None, channel_dim)
 
+    @alias("c_dim_", "channel_dim_", "with_channeldim")
     def channel_dimension_(self, value):
-        self.channel_dimension = value
+        if value is None: value = self.ndim
+        self._channel_dimension = value
         return self
 
+
+    @alias("n_channel", "nchannel")
     @property
     def channel_size(self): return self.shape.channel_size
 
     @property
     def space(self):
         s = self._special
         t = tuple(self.ishape)
         return t[:s[0]] + t[s[0]+1:s[1]] + t[s[1]+1:]
 
+    @alias('nele')
     @property
-    def nele(self): return super().numel()
+    def n_ele(self): return super().numel()
     def numel(self): return super().numel()
 
     @property
     def n_dim(self): return self.ndim
 
+    @alias('nspace')
     @property
-    def nspace(self): return self.ndim if not self.init else (self.ndim - (self._special[0] < self.ndim) - (self._special[1] < self.ndim))
+    def n_space(self): return self.ndim if not self.init else (self.ndim - (self._special[0] < self.ndim) - (self._special[1] < self.ndim))
 
+    @alias('nspecial')
     @property
-    def nspecial(self): return 0 if not self.init else ((self._special[0] < self.ndim) + (self._special[1] < self.ndim))
-
-    nbatch = batch_size
-    nchannel = channel_size
-    n_ele = nele
-    n_space = nspace
-    n_special = nspecial
+    def n_special(self): return 0 if not self.init else ((self._special[0] < self.ndim) + (self._special[1] < self.ndim))
 
     @property
     def has_batch(self): return self.init and self._special[0 if self._batch_first else 1] < self.ndim
 
     @property
     def has_channel(self): return self.init and self._special[1 if self._batch_first else 0] < self.ndim
 
@@ -662,40 +854,43 @@
 
         if isinstance(other, Size):
 
             doit = False
             batch_dim = None
             channel_dim = None
 
-            if self.batch_dimension == self.ndim:
-                batch_dim = other.batch_dimension
+            if self._batch_dimension == self.ndim:
+                batch_dim = other._batch_dimension
                 if batch_dim != self.ndim:
                     doit = True
-            if self.channel_dimension == self.ndim:
-                channel_dim = other.channel_dimension
+            if self._channel_dimension == self.ndim:
+                channel_dim = other._channel_dimension
                 if channel_dim != self.ndim:
                     doit = True
             if doit: self.set_special_(batch_dim, channel_dim)
 
         self.init = True
         return self
 
     def set_special_(self, batch_dim=None, channel_dim=None, *, special=[], bf=True):
+        """
+        batch_dim/channel_dim = None means skip assignment. 
+        """
 
         if batch_dim is None and channel_dim is None:
             if not special:
                 if not self.init: return self.special_from_()
                 else: return self
             a, b = special
             if not isinstance(a, INT): a = self.ndim
             if not isinstance(b, INT): b = self.ndim
             if a < 0: a += self.ndim
             if b < 0: b += self.ndim
             if not 0 <= a <= self.ndim or not 0 <= b <= self.ndim:
-                raise TypeError(f"Special dimension should be a dimension index which is smaller than {self.ndim}. ")
+                raise TypeError(f"Special dimension should be a dimension index which is smaller than {self.ndim}, not {a} and {b}. ")
             if not self.init: self._batch_first = bf
             if a < b:
                 self._special = [a, b]
             else:
                 self._special = [b, a]
                 self._batch_first = not self._batch_first
             self.init = True
@@ -703,25 +898,25 @@
 
         if batch_dim is not None:
             if not isinstance(batch_dim, INT): batch_dim = self.ndim
             if batch_dim < 0: batch_dim = batch_dim + self.ndim
             if not 0 <= batch_dim <= self.ndim:
                 raise TypeError(f"batch_dimension should be a dimension index which is smaller than {self.ndim}. ")
         elif self.init:
-            batch_dim = MIN(self.batch_dimension, self.ndim)
+            batch_dim = MIN(self._batch_dimension, self.ndim)
         else:
             batch_dim = self.ndim
 
         if channel_dim is not None:
             if not isinstance(channel_dim, INT): channel_dim = self.ndim
             if channel_dim < 0: channel_dim = channel_dim + self.ndim
             if not 0 <= channel_dim <= self.ndim:
                 raise TypeError(f"channel_dimension should be a dimension index which is smaller than {self.ndim}. ")
         elif self.init:
-            channel_dim = MIN(self.channel_dimension, self.ndim)
+            channel_dim = MIN(self._channel_dimension, self.ndim)
         else:
             channel_dim = self.ndim
 
         if batch_dim < channel_dim:
             self._batch_first = True
             self._special = [batch_dim, channel_dim]
         elif channel_dim < batch_dim:
@@ -741,15 +936,15 @@
         self._batch_first = True
         return self
 
     def remove_batch_(self):
         return self.set_special_(batch_dim=self.ndim)
 
     def remove_channel_(self):
-        return self.set_special_(channel=self.ndim)
+        return self.set_special_(channel_dim=self.ndim)
 
     def normalize_(self):
         m, M = self.min(), self.max()
         if m == M:
             if M >= 1: return self.one_()
             if m <= 0: return self.zero_()
             return self
@@ -762,289 +957,591 @@
         if m == M:
             if M >= 1: return ones_like(self)
             if m <= 0: return zeros_like(self)
             return self
         return (self - m) / (M - m)
 
     for func in tf_list:
-        exec(f"def {func}(*args, **kwargs): return tp.{func}(*args, **kwargs)")
+        exec(f"def {func}(*args, **kwargs): return bt.{func}(*args, **kwargs)")
 
     def tensor(self): return super()._make_subclass(torch.Tensor, self, self.requires_grad)
-    def numpy(self): return super(torch.Tensor, self.cpu().detach()).numpy()
 
     def one_(self): return self.zero_().add_(1)
     
     def autodevice_(self):
-        if _auto_device and self.device != Device: return self.to(Device)
-        return self
+        return _device(self)
 
-    def device_(self, device):
-        if device != self.device: return self.to(device)
-        return self
+    def device_(self, device: AutoDevice):
+        return device(self)
+    
+    def range(self): return stack(self.flatten().min(-1).values, self.flatten().max(-1).values, -1)
 
-    def size(self, *k: [INT, str]):
+    def size(self, *k: Type(INT, str)):
         if len(k) == 0:
             return self.shape
-        i = [(self.names.index(x) if x in self.names else None) if isoftype(x, str) else x for x in k]
+        i = [(self.names.index(x) if x in self.names else x) if isinstance(x, str) else (
+            self.batch_dimension if isinstance(x, list) else (self.channel_dimension if isinstance(x, (dict, set)) else x)) for x in k]
         if None in i:
-            return super().size(k[i.index(None)])
+            return super().size(*i)
         if len(i) == 1:
             return self.ishape[i[0]]
         return tuple(self.ishape[x] for x in i)
 
-    def squeeze(self, *dims: int, dim=None):
+    def squeeze(self, *dims: INT, dim=None):
         if len(dims) > 0 and dim is not None:
-            raise TypeError("squeeze function only accept either argument or positional argument. But both are given")
-        if len(dims) == 1 and isinstance(dims[0], tuple):
-            dims = dims[0]
+            raise TypeError("squeeze function only accept either argument or positional argument. But both are given. ")
+        dims = arg_tuple(dims, no_list=True)
         if dim is None:
             dim = dims
         if not isinstance(dim, tuple):
             dim = (dim,)
         if len(dim) == 0: dim = tuple(i for i, x in enumerate(self.ishape) if x == 1)[::-1]
         a, b = self._special
         ndim = self.ndim
         bf = self._batch_first
         for d in dim:
-            if isinstance(d, list): d = d[0]
-            if isinstance(d, set): d = d.pop()
+            if d is None: continue
             self = super(Tensor, self).squeeze(d)
+            if d < 0: d = d + ndim
             if a == d: a = ndim
-            if 0 <= d <= a or d + ndim <= a: a -= 1
+            if d <= a: a -= 1
             if b == d: b = ndim
-            if 0 <= d <= b or d + ndim <= b: b -= 1
+            if d <= b: b -= 1
             ndim -= 1
         return self.as_subclass(Tensor).set_special_(special=[a, b], bf=bf)
 
-    def squeeze_(self, *dims:int, dim=None):
+    def squeeze_(self, *dims: INT, dim=None):
         if len(dims) > 0 and dim is not None:
             raise TypeError("squeeze_ function only accept either argument or positional argument. But both are given")
-        if len(dims) == 1 and isinstance(dims[0], tuple):
-            dims = dims[0]
+        dims = arg_tuple(dims, no_list=True)
         if dim is None:
             dim = dims
         if not isinstance(dim, tuple):
             dim = (dim,)
         if len(dim) == 0: dim = tuple(i for i, x in enumerate(self.ishape) if x == 1)
         a, b = self._special
         ndim = self.ndim
         bf = self._batch_first
         for d in dim:
-            if isinstance(d, list): d = d[0]
-            if isinstance(d, set): d = d.pop()
-            self = super(Tensor, self).squeeze_(d)
+            if d is None: continue
+            torch.Tensor.squeeze_(self, d)
+            if d < 0: d = d + ndim
             if a == d: a = ndim
-            if 0 <= d <= a or d + ndim <= a: a -= 1
+            if d <= a: a -= 1
             if b == d: b = ndim
-            if 0 <= d <= b or d + ndim <= b: b -= 1
+            if d <= b: b -= 1
             ndim -= 1
-        return self.as_subclass(Tensor).set_special_(special=[a, b], bf=bf)
+        self.set_special_(special=[a, b], bf=bf)
+        return self
 
-    def unsqueeze(self, *dims: int, dim=None):
+    def unsqueeze(self, *dims: INT, dim=None, batch_dim=None, channel_dim=None):
         if len(dims) > 0 and dim is not None:
             raise TypeError("unsqueeze function only accept either argument or positional argument. But both are given")
-        if len(dims) == 1 and isinstance(dims[0], tuple):
-            dims = dims[0]
+        dims = arg_tuple(dims, no_list=True)
         if dim is None:
             dim = dims
         if not isinstance(dim, tuple):
             dim = (dim,)
-        if len(dim) == 0: dim = (0,)
+        if len(dim) == 0: dim = (SUM([i != self.ndim for i in self._special]),)
         a, b = self._special
         ndim = self.ndim
         bf = self._batch_first
-        ibatch = ichannel = None
         for d in dim:
-            if isinstance(d, list): d = d[0]; ibatch = d
-            if isinstance(d, set): d = d.pop(); ichannel = d
             self = super(Tensor, self).unsqueeze(d)
-            if 0 <= d <= a or d + ndim <= a: a += 1
-            if 0 <= d <= b or d + ndim <= b: b += 1
+            if 0 <= d <= a or d + ndim < a: a += 1
+            if 0 <= d <= b or d + ndim < b: b += 1
             ndim += 1
+        return self.as_subclass(Tensor).set_special_(special=[a, b], bf=bf).set_special_(batch_dim=batch_dim, channel_dim=channel_dim)
 
-        return self.as_subclass(Tensor).set_special_(special=[a, b], bf=bf).set_special_(batch_dim=ibatch, channel_dim=ichannel)
-
-    def unsqueeze_(self, *dims:int, dim=None):
+    def unsqueeze_(self, *dims: INT, dim=None, batch_dim=None, channel_dim=None):
         if len(dims) > 0 and dim is not None:
             raise TypeError("unsqueeze_ function only accept either argument or positional argument. But both are given")
-        if len(dims) == 1 and isinstance(dims[0], tuple):
-            dims = dims[0]
+        dims = arg_tuple(dims, no_list=True)
         if dim is None:
             dim = dims
         if not isinstance(dim, tuple):
             dim = (dim,)
         if len(dim) == 0: dim = (0,)
         a, b = self._special
         ndim = self.ndim
         bf = self._batch_first
-        ibatch = ichannel = None
         for d in dim:
-            if isinstance(d, list): d = d[0]; ibatch = d
-            if isinstance(d, set): d = d.pop(); ichannel = d
-            self = super(Tensor, self).unsqueeze_(d)
-            if 0 <= d <= a or d + ndim <= a: a += 1
-            if 0 <= d <= b or d + ndim <= b: b += 1
+            torch.Tensor.unsqueeze_(self, d)
+            if 0 <= d <= a or d + ndim < a: a += 1
+            if 0 <= d <= b or d + ndim < b: b += 1
             ndim += 1
-        return self.as_subclass(Tensor).set_special_(special=[a, b], bf=bf).set_special_(batch_dim=ibatch, channel_dim=ichannel)
+        # In-place operation
+        self.set_special_(special=[a, b], bf=bf).set_special_(batch_dim=batch_dim, channel_dim=channel_dim)
+        return self
 
-    def expand_to(self, *target):
+    def expand_to(self, *target, axis: list=None, dim: INT=None):
         with torch._C.DisableTorchFunction():
 
             if len(target) == 1 and not isinstance(target[0], INT): target = target[0]
             if isinstance(target, torch.Tensor): target = target.shape
             if not isinstance(target, Size): target = Size(target)
             if self.init and self.nspecial == target.nspecial and target._batch_first != self._batch_first:
                 if self.nspace == 0 and self.ndim == 2: self = self[::-1]
                 else: raise TypeError(f"Batch and channel order not matched for {self.shape} and {target}")
-                
-            axis_map = list(RANGE(self.ndim))
-            p = 0
-            for i, s in enumerate(self.shape):
-                if i == self.batch_dimension:
-                    axis_map[i] = target.batch_dimension
-                    p = target.batch_dimension + 1
-                elif i == self.channel_dimension:
-                    axis_map[i] = target.channel_dimension
-                    p = target.channel_dimension + 1
-                elif s in (1, -1):
-                    axis_map[i] = p
-                    p += 1
-                else:
-                    while p < target.ndim and target[p] not in (s, -1): p += 1
-                    axis_map[i] = p
-                    p += 1
-                if p >= target.ndim  + 1: raise TypeError(f"Unable to expand sizes {self.shape} to {target}. ")
-            res = self.unsqueeze_to(target, axis=axis_map).repeat(tuple(1 if i in axis_map else (x if x >= 0 else 1) for i, x in enumerate(target)))
+
+            if isinstance(dim, list) and len(dim) == 0: dim = target.batch_dimension
+            elif isinstance(dim, dict) and len(dim) == 0: dim = target.channel_dimension
+            elif isinstance(dim, list) and len(dim) == 1: dim = dim[0]
+            elif isinstance(dim, set) and len(dim) == 1: dim = list(dim)[0]
+            if isinstance(dim, INT) and dim < 0: dim += target.ndim
+            if axis is None:
+                axis_map = list(RANGE(self.ndim))
+                p = 0
+                use_special = target.has_special
+                for i, s in enumerate(self.shape):
+                    if p == dim:
+                        axis_map[i] = p
+                        p += 1
+                        continue
+                    if p >= target.ndim + 1 and s not in (1, -1):
+                        raise TypeError(f"Unable to expand sizes {self.shape} to {target}. ")
+                    if use_special and i == self._batch_dimension:
+                        axis_map[i] = target._batch_dimension
+                        p = target._batch_dimension + 1
+                    elif use_special and i == self._channel_dimension:
+                        axis_map[i] = target._channel_dimension
+                        p = target._channel_dimension + 1
+                    elif s in (1, -1):
+                        axis_map[i] = p
+                        p += 1
+                    else:
+                        while p < target.ndim and target[p] not in (s, -1): p += 1
+                        axis_map[i] = p
+                        p += 1
+                    if p >= target.ndim + 1 and s not in (1, -1):
+                        raise TypeError(f"Unable to expand sizes {self.shape} to {target}. ")
+                axis=axis_map
+            axis = to_list(axis)
+            res = self.unsqueeze_to(target, axis=axis)
+            shape = res.shape
+            if ANY([s > 0 and x % s != 0 and x >= 0 for i, (x, s) in enumerate(zip(target, shape)) if i != dim]):
+                raise TypeError(f"Cannot expand the unsqueezed shape {shape} to {target}. Please use keyword 'axis' to manually align the dimensions, " +
+                                "use 'dim' to specify the unmatched dimension or use -1 in target size to free dimensions in the expand. ")
+            res = res.repeat(tuple(1 if i == dim else (x // s if x >= 0 and s > 0 else 1) for i, (x, s) in enumerate(zip(target, shape))))
 
         return res.as_subclass(Tensor).special_from_(target)
 
-    def unsqueeze_to(self, *target, axis: list):
+    def unsqueeze_to(self, *target, axis: list=None):
         with torch._C.DisableTorchFunction():
 
             if len(target) == 1 and not isinstance(target[0], INT): target = target[0]
             if isinstance(target, torch.Tensor): target = target.shape
             if not isinstance(target, Size): target = Size(target)
+            if self.init and self.nspecial == target.nspecial and target._batch_first != self._batch_first:
+                if self.nspace == 0 and self.ndim == 2: self = self[::-1]
+                else: raise TypeError(f"Batch and channel order not matched for {self.shape} and {target}")
 
-            new_size = list(target)
-            for i in RANGE(len(new_size)):
-                if i not in axis or self.ishape[axis.index(i)] in (1, -1):
-                    new_size[i] = 1
-            res = self.view(*new_size)
+            if axis is None:
+                axis_map = list(RANGE(self.ndim))
+                p = 0
+                for i, s in enumerate(self.shape):
+                    if i == self._batch_dimension:
+                        axis_map[i] = target._batch_dimension
+                        p = target._batch_dimension + 1
+                    elif i == self._channel_dimension:
+                        axis_map[i] = target._channel_dimension
+                        p = target._channel_dimension + 1
+                    elif s in (1, -1):
+                        axis_map[i] = p
+                        p += 1
+                    else:
+                        while p < target.ndim and target[p] not in (s, -1): p += 1
+                        axis_map[i] = p
+                        p += 1
+                    if p >= target.ndim  + 1: raise TypeError(f"Unable to expand sizes {self.shape} to {target}. ")
+                axis=axis_map
+            axis = to_list(axis)
+            for i in RANGE(len(target)):
+                if i not in axis:
+                    self = self.unsqueeze(i)
 
-        return res.as_subclass(Tensor).special_from_(target)
+        return self.as_subclass(Tensor).special_from_(target)
+
+    def unsqueeze_to_(self, *target, axis: list=None):
+        with torch._C.DisableTorchFunction():
 
-    def multiple(self, num, dim=0):
-        if isinstance(dim, list): d = dim[0]
-        elif isinstance(dim, set): d = dim.pop(); dim = {d}
-        else: d = dim
+            if len(target) == 1 and not isinstance(target[0], INT): target = target[0]
+            if isinstance(target, torch.Tensor): target = target.shape
+            if not isinstance(target, Size): target = Size(target)
+            if self.init and self.nspecial == target.nspecial and target._batch_first != self._batch_first:
+                if self.nspace == 0 and self.ndim == 2: self = self[::-1]
+                else: raise TypeError(f"Batch and channel order not matched for {self.shape} and {target}")
+
+            if axis is None:
+                axis_map = list(RANGE(self.ndim))
+                p = 0
+                for i, s in enumerate(self.shape):
+                    if i == self._batch_dimension:
+                        axis_map[i] = target._batch_dimension
+                        p = target._batch_dimension + 1
+                    elif i == self._channel_dimension:
+                        axis_map[i] = target._channel_dimension
+                        p = target._channel_dimension + 1
+                    elif s in (1, -1):
+                        axis_map[i] = p
+                        p += 1
+                    else:
+                        while p < target.ndim and target[p] not in (s, -1): p += 1
+                        axis_map[i] = p
+                        p += 1
+                    if p >= target.ndim  + 1: raise TypeError(f"Unable to expand sizes {self.shape} to {target}. ")
+                axis=axis_map
+            axis = to_list(axis)
+            for i in RANGE(len(target)):
+                if i not in axis:
+                    torch.Tensor.unsqueeze_(self, i)
+
+        self.special_from_(target)
+        return self
+
+    @alias('multiple')
+    def multiply(self, num, dim=0):
+        d = item(dim)
         return self.unsqueeze(dim).repeat((1,) * d + (num,) + (1,) * (self.ndim - d))
 
-    def sample(self, dim: INT = None, number: INT = 1, random: bool = True) -> 'Tensor':
+    @alias('ample')
+    def amplify(self, num, dim=0):
+        d = item(dim)
+        return self.multiply(num, d+1).flatten(d, d + 1).special_from_(self)
+    
+    def row(self, index):
+        dim = [d for d in RANGE(3) if d not in self._special][0]
+        return self[(slice(None),) * dim + (index,)]
+    
+    def column(self, index):
+        return self[..., index]
+
+    def repeated(self, num, dim=0):
+        d = item(dim)
+        return self.repeat((1,) * d + (num,) + (1,) * (self.ndim - d - 1))
+
+    def flip(self, dim=0):
+        d = item(dim)
+        return self[(slice(None),) * d + (arange(self.size(d)-1, -1, -1),) + (slice(None),) * (self.ndim - d - 1)]
+    
+    def with_pixelvalue(self, ind, val):
+        self[ind] = val
+        return self
+
+    def sample(self, number: INT = 1, dim: INT = None, random: bool = True):
         """
-        sample(self, dim: int = self.batch_dimension, numbder: int = 1, random: bool = True) -> Tensor
+        sample(self, numbder: int = 1, dim: int = self.batch_dimension, random: bool = True) -> Tensor
 
         Sample a few subspaces from a given dimension.
-        data.sample(2, 1, random=False) is equivalant to data[:, :, 0, ...].
+        data.sample(1, 2, random=False) is equivalant to data[:, :, :1, ...].
         """
-        if dim is None or isinstance(dim, list) and dim == []: dim = self.batch_dimension
-        if dim is None or isinstance(dim, dict) and dim == {}: dim = self.channel_dimension
-        if dim < 0: dim += self.ndim
         if dim is None: raise TypeError("Argument 'dim' needed for sampling Tensors with no special dimensions. ")
         if number < 1: raise TypeError("Argument 'number' for sampling Tensors can not be smaller than 1. ")
         sample_indices = [slice(None)] * self.dim()
         if self.shape[dim] < number: raise TypeError(f"Too many elements needed to be sampled from dimension {dim}")
         if random:
             import random
             samples = random.sample(RANGE(self.shape[dim]), k = number)
         else: samples = list(RANGE(number))
-        if len(samples) != 1:
-            sample_indices[dim] = samples
-            output_tensor = self[tuple(sample_indices)].as_subclass(Tensor).special_from_(self)
-            output_tensor.indices = samples
-            return output_tensor
-        else:
-            sample_indices[dim] = samples[0]
-            output_tensor = self[tuple(sample_indices)].as_subclass(Tensor).set_special_(special=[x - 1 if x > dim else (self.ndim-1 if x == dim else x) for x in self._special], bf=self._batch_first)
-            output_tensor.indices = samples
-            return output_tensor
+        
+        sample_indices[dim] = samples
+        output_tensor = self[tuple(sample_indices)].as_subclass(Tensor).special_from_(self)
+        output_tensor.indices = samples
+        return output_tensor
+
+        # # Deprecated codes of squeezed results for 1-sample
+        # if len(samples) != 1:
+        # else:
+        #     sample_indices[dim] = samples[0]
+        #     output_tensor = self[tuple(sample_indices)].as_subclass(Tensor).set_special_(special=[x - 1 if x > dim else (self.ndim-1 if x == dim else x) for x in self._special], bf=self._batch_first)
+        #     output_tensor.indices = samples
+        #     return output_tensor
 
     def pick(self, index: INT, dim: INT):
         """
         pick(self, dim, index) -> Tensor
 
         pick one of the item on dimension `dim` for big tensors. 
         data.pick(4, 2) is equivalent to data[:, :, 4]
         """
         if dim < 0: dim += self.ndim
         return self[(slice(None),) * dim + (index,)]
 
     def split(self, sec=1, dim=None, squeeze=False):
         """
-        pick(self, dim, index) -> Tensor
+        split(self, sec, dim) -> Tensor
 
-        pick one of the item on dimension `dim` for big tensors. 
-        data.pick(4, 2) is equivalent to data[:, :, 4]
+        split dimension `dim` to sections with each section of length `sec`. 
         """
+        if isinstance(sec, (list, set, dict)) and len(sec) == 1: dim = sec; sec = 1
         if dim is None: dim = self.channel_dimension
-        if sec == 1 or isinstance(sec, (tuple, list)) and all(x == 1 for x in sec):
+        if dim is None: raise TypeError(f"Cannot split at dimension {dim} as no such dimension found. ")
+        if sec == 1 or isinstance(sec, (tuple, list)) and ALL(x == 1 for x in sec):
             if squeeze: return tuple(x.as_subclass(Tensor).special_from_(self).squeeze(dim) for x in super().split(sec, dim))
         return tuple(x.as_subclass(Tensor).special_from_(self) for x in super().split(sec, dim))
 
-    def mvdim(self, dim1: INT, dim2: INT):
+    def movedim(self, dim1: INT, dim2: INT):
         """
-        mvdim(self, dim1, dim2) -> Tensor
+        movedim(self, dim1, dim2) -> Tensor
 
         move dim1 to dim2(specified in the targeting size)
-        data of size (2, 3, 4, 5) can be transform to (2, 4, 5, 3) by data.mvdim(1, -1) or data.mvdim(1, 3)
+        data of size (2, 3, 4, 5) can be transform to (2, 4, 5, 3) by data.movedim(1, -1) or data.movedim(1, 3)
         """
         if dim1 < 0: dim1 += self.ndim
         if dim2 < 0: dim2 += self.ndim
 
         with torch._C.DisableTorchFunction():
             if dim1 == dim2: res = self
             elif dim1 < dim2: res = self.unsqueeze(dim2+1).transpose(dim1, dim2+1).squeeze(dim1)
             else: res = self.unsqueeze(dim2).transpose(dim1+1, dim2).squeeze(dim1+1)
 
         return res.as_subclass(Tensor).set_special_(special=[dim2 if x == dim1 else (
             x if x > dim2 and x > dim1 or x < dim1 and x < dim2 
-            else (x + 1 if dim1 > dim2 else x - 1)) for x in self._special])
+            else (x + 1 if dim1 > dim2 else x - 1)) for x in self._special], bf=self._batch_first)
 
-    def mvdim_(self, dim1: INT, dim2: INT):
+    def movedim_(self, dim1: INT, dim2: INT):
         """
-        In-place operation for mvdim
+        In-place operation for movedim
         """
         if dim1 < 0: dim1 += self.ndim
         if dim2 < 0: dim2 += self.ndim
 
         with torch._C.DisableTorchFunction():
-            if dim1 == dim2: res = self
-            elif dim1 < dim2: res = self.unsqueeze_(dim2+1).transpose_(dim1, dim2+1).squeeze_(dim1)
-            else: res = self.unsqueeze_(dim2).transpose_(dim1+1, dim2).squeeze_(dim1+1)
+            if dim1 == dim2: ...
+            elif dim1 < dim2: self.unsqueeze_(dim2+1).transpose_(dim1, dim2+1).squeeze_(dim1)
+            else: self.unsqueeze_(dim2).transpose_(dim1+1, dim2).squeeze_(dim1+1)
 
-        return res.as_subclass(Tensor).special_from_(special=[dim2 if x == dim1 else (
+        self._special = [dim2 if x == dim1 else (
             x if x > dim2 and x > dim1 or x < dim1 and x < dim2 
-            else (x + 1 if dim1 > dim2 else x - 1)) for x in self._special])
+            else (x + 1 if dim1 > dim2 else x - 1)) for x in self._special]
+        if self._special[0] > self._special[1]:
+            self._special = self._special[::-1]
+            self._batch_first = not self._batch_first
+        return self
+
+    @alias("joindims")
+    def mergedims(self, *dims: INT, target: INT = None):
+        """
+        mergedims(self, *source, target) -> Tensor
 
-    def tobytes(self): return self.numpy().tobytes()
+        merge dims into one dimension: target (the last argument)
+        data of size (2, 3, 4, 5) can be transform to (24, 5) with a Cartesian of 3 x 2 x 4 by:
+            data.mergedims([1, 0, 2], target=0) / data.mergedims(1, 0, 2, target=0)
+        Note that one can only omit the target dimension if no order of dimension is changed. 
+            the automatically chosen target is the new position of the last dimension one gives. 
+            e.g. data.mergedims(1, 0, 3) result in (4, 30) and it follows a Cartesian of 2 x 3 x 5.
+        """
+        dims = list(arg_tuple(dims))
+        avouch(len(dims) >= 2, f"Please input at least two dims to be merged for method 'mergedims', not {dims}. ")
+        new_dims = []
+        cls_guess = None
+        for i, d in enumerate(dims + [target]):
+            if d is None: cls = cls_guess; new_dims.append(d); continue
+            cls = None
+            if isinstance(d, list) and len(d) == 0: ibatch = self.batch_dim if i < len(dims) else 0; d = ibatch; cls = list
+            elif isinstance(d, dict) and len(d) == 0: ichannel = self.channel_dim if i < len(dims) else (1 if self.batch_dim == 0 else 0); d = ichannel; cls = set
+            elif isinstance(d, list) and len(d) == 1: ibatch = self.batch_dim if i < len(dims) else d[0]; d = ibatch; cls = list
+            elif isinstance(d, set) and len(d) == 1: ichannel = self.channel_dim if i < len(dims) else list(d)[0]; d = ichannel; cls = set
+            if isinstance(d, INT):
+                ndim = self.ndim if i < len(dims) else self.ndim - len(dims) + 1
+                l, u = - ndim - 1, ndim
+                if not l <= d <= u:
+                    raise IndexError(f"Dimension out of range (expected to be in range of [{l}, {u}], but got {d})")
+                d += ndim if d < 0 else 0
+            else: raise TypeError(f"Invalid dimension {d} found in mergedims, it also happens when one omit 'target='. ")
+            new_dims.append(d)
+            tcls = None
+            if self.batch_dimension == d: tcls = list
+            if self.channel_dimension == d: tcls = set
+            if i < len(dims): cls_guess = cls_guess if tcls is None or cls_guess == list else tcls
+        *dims, target = new_dims
+        if target is None:
+            target = dims[-1] - SUM([1 if d < dims[-1] else 0 for d in dims[:-1]])
+            dims.sort()
+        avouch(target < self.ndim - len(dims) + 1, "Dimension out of range, please make sure that 'target' is the dimension in the resulting shape. ")
+
+        res = self.clone()
+        other_dims = [i for i in RANGE(self.ndim) if i not in dims]
+        out_dims = other_dims[:target] + dims + other_dims[target:]
+        res.permute_(out_dims)
+        res = res.flatten(target, target + len(dims) - 1)
+        if cls is not None:
+            if cls == list: res.batch_dim = target
+            elif cls == set: res.channel_dim = target
+            else: raise AssertionError(f"Invalid dimension tag of type cls: {cls}. Please contact the developer for more info (Error Code: B243). ")
+        return res
+
+    def splitdim(self, source: INT, *size: INT):
+        """
+        splitdim(self, source, *target_size) -> Tensor
+
+        split one dimension source into multiple dimensions: target
+        data of size (2, 4, 5) can be transform to (2, 2, 2, 5) with data.splitdim(1, 2, 2).
+        Note that batch representations for source and target are different
+            (splitdim([1], [2], 2) means split the batchdim at index 1 into a size of ([2], 2), which is 2x2 with batchdim at index 0).
+            One can use -1 for arbitrary size. 
+        """
+        size = bt.Size(arg_tuple(size))
+        avouch(len(size) >= 2, f"Please input an at-least-two-dim-shape to split dimension {source} into in method 'splitdim', not {size}. ")
+
+        new_size = self.shape[:source] + size + self.shape[source + 1:]
+        prod = 1
+        ni = None
+        for i, x in enumerate(size):
+            if isinstance(x, list) and len(x) == 1: x = x[0]
+            elif isinstance(x, set) and len(x) == 1: x = list(x)[0]
+            elif isinstance(x, list) and len(x) == 0: x = -1
+            elif isinstance(x, dict) and len(x) == 0: x = -1
+            if x != -1: prod *= x; continue
+            ni = i
+        if ni is not None:
+            x = self.shape[source] // prod
+            if size.batch_dimension == ni: x = [x]
+            elif size.channel_dimension == ni: x = {x}
+            new_size = new_size[:source + ni] + bt.Size(x) + new_size[source + ni + 1:]
+
+        return self.view(new_size)
+
+    def tobytes(self): return self.detach().cpu().numpy().tobytes()
 
     def cat(self, other, dim=0):
-        return torch.cat((self, other), dim=dim)
+        return cat((self, other), dim=dim)
 
     def stack(self, other, dim=0):
-        return torch.stack((self, other), dim=dim)
+        return stack((self, other), dim=dim)
+    
+    def inv(self):
+        return bt.inv(self)
+
+    def view(self, *args):
+        if len(args) == 1 and isinstance(args[0], tuple): args = args[0]
+        ibatch = ichannel = None
+        new_size = []
+        for i, x in enumerate(args):
+            if isinstance(x, list) and len(x) == 0: ibatch = i; x = -1
+            elif isinstance(x, dict) and len(x) == 0: ichannel = i; x = -1
+            elif isinstance(x, list) and len(x) == 1: ibatch = i; x = x[0]
+            elif isinstance(x, set) and len(x) == 1: ichannel = i; x = list(x)[0]
+            new_size.append(x)
+        output = super().view(*new_size).as_subclass(Tensor)
+        if ibatch is not None: output.with_batchdim(ibatch)
+        if ichannel is not None: output.with_channeldim(ichannel)
+        if isinstance(args, Size): output.special_from_(args)
+        return output
+    
+    def permute_(self, *dims):
+        dims = arg_tuple(dims)
+        avouch(len(dims) == self.ndim)
+        cur_order = list(RANGE(self.ndim))
+        for i in RANGE(len(cur_order)):
+            j = cur_order.index(dims[i])
+            cur_order[i], cur_order[j] = cur_order[j], cur_order[i]
+            self.transpose_(i, j)
+        return self
+    
+    def standard(self):
+        """
+        return a standard version of the tensor: with batch dim as the first dim, channel as the second. 
+        """
+        dim_list = list(RANGE(self.ndim))
+        order = []
+        if self._batch_dimension != self.ndim:
+            dim_list.remove(self._batch_dimension)
+            order.append(self._batch_dimension)
+        if self._channel_dimension != self.ndim:
+            dim_list.remove(self._channel_dimension)
+            order.append(self._channel_dimension)
+        return self.permute(*(order + dim_list))
+    
+    def standard_(self):
+        """
+        In-place standard of the tensor: with batch dim as the first dim, channel as the second. 
+        """
+        dim_list = list(RANGE(self.ndim))
+        order = []
+        if self._batch_dimension != self.ndim:
+            dim_list.remove(self._batch_dimension)
+            order.append(self._batch_dimension)
+        if self._channel_dimension != self.ndim:
+            dim_list.remove(self._channel_dimension)
+            order.append(self._channel_dimension)
+        self.permute_(*(order + dim_list))
+        return self
+    
+    def quantile(self, *args, **kwargs):
+        q = bt.tensor(kwargs.get('q', args[0]))
+        dim = kwargs.get('dim', args[1] if len(args) >= 2 else None)
+        if dim is None: return super().quantile(*args, **kwargs).as_subclass(Tensor)
+        if q.ndim > 0: return super().quantile(*args, **kwargs).as_subclass(Tensor).special_from_(self.unsqueeze(0))
+        return super().quantile(*args, **kwargs).as_subclass(Tensor).special_from_(self)
+    
+    ## dtypes
+    @alias("as_type")
+    def astype(self, dt):
+        """
+            numpy dtype v.s. torch dtype:
+            ==============================
+            numpy type // torch type
+            ------------------------------
+            void0, void::void // 
+            object0, object_::object // 
+            bool8, bool_::bool // torch.bool
+            byte, int8::int8 // torch.int8
+            short, int16::int16 // torch.short, torch.int16
+            int32, intc::int32 // torch.int, torch.int32
+            int0, int_, int64, intp, longlong, signedinteger::int64 // torch.long, torch.int64
+            ubyte, uint8::uint8 // torch.uint8
+            ushort, uint16::uint16 // 
+            uint32, uintc::uint32 // 
+            uint, uint0, uint64, Uint64, uintp, ulonglong::uint64 // 
+            // torch.bfloat16 # 16bit, 范围大如32bit但精度低
+            half, float16::float16 // torch.half, torch.float16
+            single, float32::float32 // torch.float, torch.float32
+            double, float64, float_, longdouble, longfloat, number::float64 // torch.double, torch.float64
+            // torch.complex32
+            csingle, complex64, singlecomplex::complex64 // torch.cfloat, torch.complex64
+            cdouble, cfloat, clongdouble, clongfloat, complex_, complex128, longcomplex::complex128 // torch.cdouble, torch.complex128
+            str0, str_, Str0::str // 
+            bytes0, bytes_, string_::bytes // 
+            datetime64::datetime64 // 
+            timedelta64::timedelta64 // 
+            # 量子计算类型
+            // torch.qint8
+            // torch.qint32
+            // torch.quint8
+            // torch.quint4x2
+        """
+        if isinstance(dt, str): return super().type(dt.replace('bt.', 'torch.')).as_subclass(self.__class__).special_from_(self)
+        if hasattr(dt, 'dtype'): dt = dt.dtype
+        if isinstance(dt, torch.dtype): return super().type(dt).as_subclass(self.__class__).special_from_(self)
+        import numpy as np
+        dt_name = np.dtype(dt).name
+        dtype_map = {'uint16': "int32", 'uint32': "int64", 'uint64': "int64"}
+        torch_dt = getattr(torch, dtype_map.get(dt_name, dt_name), None)
+        avouch(torch_dt is not None, f"Invalid dtype {dt}: {dt_name} cannot be converted into torch dtype.")
+        return super().type(torch_dt).as_subclass(self.__class__).special_from_(self)
+    
+    def type(self, dt=None):
+        if dt is None: return super().type().replace("torch.", "bt.")
+        else: return self.astype(dt)
+
+    def byte_size(self):
+        return ByteSize(self.element_size() * self.numel())
 
     @property
     def T(self: 'Tensor') -> 'Tensor':
+        output = self.clone()
+        if self.n_space == 1: output = output.unsqueeze_(-1)
         if not self.has_special: return super().T
-        s = self._special
+        s = output._special
 
         with torch._C.DisableTorchFunction():
-            permute_dim = tuple(RANGE(s[0]))[::-1] + (s[0],) + tuple(RANGE(s[0]+1, s[1]))[::-1] + (s[1],) * (s[1] != self.ndim) + tuple(RANGE(s[1]+1, self.ndim))[::-1]
+            permute_dim = tuple(RANGE(s[0]))[::-1] + (s[0],) + tuple(RANGE(s[0]+1, s[1]))[::-1] + (s[1],) * (s[1] != output.ndim) + tuple(RANGE(s[1]+1, output.ndim))[::-1]
         
-        return self.permute(*permute_dim)
+        return output.permute_(*permute_dim)
 
     def t(self) -> 'Tensor':
         return self.T
 
     def t_(self) -> 'Tensor':
         """
         t_() -> Tensor
@@ -1057,40 +1554,61 @@
             for i in RANGE(s[0] // 2):
                 self.transpose_(i, s[0] - i - 1)
             for i in RANGE((s[1] - s[0] - 1) // 2):
                 self.transpose_(s[0] + i + 1, s[1] - i - 1)
             for i in RANGE((self.ndim - s[1] - 1) // 2):
                 self.transpose_(s[1] + i + 1, self.ndim - i - 1)
         return self
+    
+    def int(self): return super().long()
+    
+    def __iter__(self):
+        for i in RANGE(self.size(0)):
+            yield self[i]
 
     def __getattr__(self, key):
         if not self.init:
             if key == '_special': return [self.ndim, self.ndim]
             elif key == '_batch_first': return True
-        try:
-            return super().__getattr__(key)
-        except:
-            raise AttributeError("{} is not a method/attribute of Tensor, the most similar name is {}".format(key, vector(dir(self)).fuzzy_search(key, 3)))
+        try: ret = super().__getattribute__(key)
+        except: raise AttributeError(f"'batorch.tensor' object has no attribute '{key}'")
+        return ret
 
     def __matmul__(self, other, **kwargs):
         if isinstance(other, torch.Tensor) and self.has_special or isinstance(other, Tensor) and other.has_special:
-            a, b = self.shape[:-2] ^ other.shape[:-2]
+            # if self.nspace == 0 and self.has_channel: self.with_channeldim(None)
+            # if other.nspace == 0 and other.has_channel: other.with_channeldim(None)
+            space1 = self.space
+            space2 = other.space
+            rem = len(space1) < 2 or len(space2) < 2
+            if len(space1) < 2: space1 += (1,)
+            if len(space2) < 2: space2 += (1,)
+            if len(space1) < 2: space1 += (1,)
+            if len(space2) < 2: space2 += (1,)
+            a, b = Size(space1[:-2]) ^ Size(space1[:-2])
+            sa = self.shape.reset_space(a)
+            sb = other.shape.reset_space(b)
             with torch._C.DisableTorchFunction():
-                res = super(torch.Tensor, self.view(a + tuple(self.shape[-2:]))).__matmul__(other.view(b + tuple(other.shape[-2:])))
-            return res.as_subclass(Tensor).special_from_(self.shape[:-2])
+                res = super(torch.Tensor, self.view(sa + space1[-2:])).__matmul__(other.view(sb + space2[-2:]))
+            if rem: res.squeeze_(-1)
+            if rem and res.size(-1) == 1: res.squeeze_(-1)
+            return res.as_subclass(Tensor).special_from_(sa)
         return super().__matmul__(other, **kwargs).as_subclass(Tensor).special_from_()
 
     def __op__(self, opname, other, **kwargs):
-        if self.has_special or isinstance(other, Tensor) and other.has_special:
-            if not isinstance(other, Tensor): other = tensor(other)
+        if not isinstance(other, torch.Tensor): other = tensor(other, device=self.device)
+        elif not isinstance(other, Tensor): other = other.as_subclass(Tensor)
+        if self.has_special and len(other.shape) > 0 or other.has_special:
             a, b = self.shape ^ other.shape
             with torch._C.DisableTorchFunction():
                 res = getattr(super(Tensor, self.view(a).as_subclass(Tensor)), opname)(other.view(b))
             return res.as_subclass(Tensor).special_from_(a)
-        return getattr(super(), opname)(other, **kwargs).as_subclass(Tensor).special_from_()
+        sp = None
+        if self.has_special: sp = self
+        return getattr(super(), opname)(other, **kwargs).as_subclass(Tensor).special_from_(sp)
 
     for op in '''
     add iadd radd
     sub isub rsub
     mul imul rmul
     div idiv rdiv
     pow ipow rpow
@@ -1102,14 +1620,38 @@
     or ior ror
     and iand rand
     xor ixor rxor
     lt le gt ge
     '''.split():
         exec(f"def __{op}__(self, *args, **kwargs): return self.__op__('__{op}__', *args, **kwargs)")
 
+    def op_(self, opname, *args, **kwargs):
+        args = [
+            other.remove_special_().unsqueeze_to_(self) if isinstance(other, Tensor) else (
+            Tensor.unsqueeze_to_(other, self) if isinstance(other, torch.Tensor) else other)
+        for other in args]
+        sp = None
+        if self.has_special: sp = self
+        getattr(torch.Tensor, opname)(self, *args, **kwargs).special_from_(sp)
+        return self
+
+    for op in '''
+    add sub mul div pow mod truediv floordiv addmm addcmul
+    '''.split():
+        exec(f"def {op}_(self, *args, **kwargs): return self.op_('{op}_', *args, **kwargs)")
+    
+    def __minmax__(self, fname, *args, **kwargs):
+        if len(args) == 1:
+            d = args[0]
+            if isinstance(d, list): args = [self.batch_dimension]
+            elif isinstance(d, (dict, set)): args = [self.channel_dimension]
+        return getattr(super(), fname)(*args, **kwargs)
+    for f in "min max median argmin argmax".split():
+        exec(f"def {f}(self, *args, **kwargs): return self.__minmax__('{f}', *args, **kwargs)")
+
     ###### old operation code ######
     #    if isinstance(other, torch.Tensor):
     #        other = Tensor(other)
     #        if self.dim() == other.dim():
     #            return super().__add__(other)
     #        elif self.dim() < other.dim():
     #            return self.expand_as(other).__add__(other)
@@ -1127,14 +1669,24 @@
     def __str__(self, *args, **kwargs):
         string = super().__str__(*args, **kwargs)
         if 'shape=' not in string:
             string = string.rstrip(')') + f', shape={self.shape})'
         return string.replace("tensor", "Tensor")
 
     def __hash__(self): return super().__hash__()
+    
+    @property
+    def grad(self):
+        g = getattr(self, '_grad_override', super().grad)
+        if not isinstance(g, torch.Tensor): return g
+        return g.as_subclass(Tensor).special_from_(self)
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
@@ -1145,47 +1697,48 @@
     @staticmethod
     def __torch_function_collect__(r, c):
         if isinstance(r, (tuple, list)):
             for x in r: Tensor.__torch_function_collect__(x, c)
         if isinstance(r, Tensor) and not r.init: c.append(r)
 
     @staticmethod
-    def __torch_function_convert_apply__(ret, apply, cls):
+    def __torch_function_convert_apply__(ret, apply, cls, force=True):
 
         with torch._C.DisableTorchFunction():
 
-            if isinstance(ret, Tensor) and not ret.init:
-                if cls != Tensor: ret = ret.as_subclass(cls)
-                apply(ret)
-                return ret
+            if isinstance(ret, Tensor):
+                if not ret.init or force:
+                    if cls != Tensor: ret = ret.as_subclass(cls)
+                    apply(ret)
+                    return ret
 
             if isinstance(ret, torch.Tensor):
                 ret = ret.as_subclass(cls)
                 return ret
 
             if isinstance(ret, (tuple, list)):
                 # Also handles things like namedtuples
                 return type(ret)(Tensor.__torch_function_convert_apply__(r, apply, cls) for r in ret)
 
-            if 'tuple_iterator' in str(type(ret)):
+            if isoftype(ret, Generator):
                 # And things iterator like Generators
                 def out():
                     for r in ret:
                         if isinstance(r, torch.Tensor):
                             r = r.as_subclass(cls)
                             apply(r)
                             yield r
                 return out()
 
             return ret
 
     @classmethod
     def __torch_function_ele_wise_func__(cls, func, types, args=(), kwargs=None):
         """
-        FOR: tensor where
+        FOR: tensor where astype type float long cuda
         __add__ __iadd__ __radd__
         __sub__ __isub__ __rsub__
         __mul__ __imul__ __rmul__
         __div__ __idiv__ __rdiv__
         __pow__ __ipow__ __rpow__
         __mod__ __imod__ __rmod__
         __truediv__ __itruediv__ __rtruediv__
@@ -1207,19 +1760,40 @@
         def apply(r):
             r.special_from_(self)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_resizing_func__(cls, func, types, args=(), kwargs=None):
-        "FOR: reshape view zeros ones rand randn"
+        "FOR: zeros ones empty rand randn"
         dims = args[1:]
-        if len(dims) == 1: dims = dims[0]
+        if len(dims) == 1 and isinstance(dims[0], tuple): dims = dims[0]
         if not isinstance(dims, Size): dims = Size(dims)
-        args = args[:1] + tuple(dims)
+        args = args[:1] + (tuple(dims),)
+
+        with torch._C.DisableTorchFunction():
+            ret = super().__torch_function__(func, types, args, kwargs)
+            if isinstance(ret, type(NotImplemented)):
+                raise NotImplementedError(f"{func} for {args} is not implemented. ")
+
+        def apply(r):
+            r.special_from_(dims)
+
+        return Tensor.__torch_function_convert_apply__(ret, apply, cls)
+
+    @classmethod
+    def __torch_function_full_func__(cls, func, types, args=(), kwargs=None):
+        "FOR: full"
+        fill = None
+        if isinstance(kwargs, dict) and 'fill_value' in kwargs: fill = kwargs['fill_value']
+        if fill: dims = args[1:]
+        else: dims, fill = args[1:]
+        if len(dims) == 1 and isinstance(dims[0], (list, tuple)): dims = dims[0]
+        if not isinstance(dims, Size): dims = Size(dims)
+        args = args[:1] + (tuple(dims), fill)
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
         def apply(r):
@@ -1281,22 +1855,22 @@
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_permute_func__(cls, func, types, args=(), kwargs=None):
         "FOR: permute"
         self = args[0]
         dims = args[1:]
-        if len(dims) == 1 and isinstance(dims[0] (list, tuple)): dims = dims[0]
+        dims = arg_tuple(dims)
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
-        d = lambda i: dims[i] if i < len(dims) else self.ndim
+        d = lambda i: dims.index(i) if i in dims else self.ndim
         def apply(r):
             r.set_special_(special=[d(self._special[0]), d(self._special[1])], bf=self._batch_first)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_matmul_func__(cls, func, types, args=(), kwargs=None):
@@ -1312,81 +1886,89 @@
             r.special_from_(self.shape[:-1] + other.shape[-1:])
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_addmm_func__(cls, func, types, args=(), kwargs=None):
         "FOR: addmm addbmm saddmm"
-        _, self, weight = args[:3]
+        _, self, other = args[:3]
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
         def apply(r):
             r.special_from_(self.shape[:-1] + other.shape[-1:])
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_reducing_func__(cls, func, types, args=(), kwargs=None):
-        "FOR: cummin cummax cumsum cumprod sum prod min max mean std argmin argmax"
+        "FOR: cummin cummax cumsum cumprod sum prod min max median mean std argmin argmax"
         func_name = str(func).split(' of ')[0].split()[-1].strip("'")
         mkwargs = kwargs if kwargs is not None else {}
         if len(args) == 1 and 'dim' not in mkwargs and func_name in ('sum', 'prod', 'mean', 'std', 'cumsum', 'cumprod'):
             self = args[0]
             s = self._special
             dims = list(RANGE(s[0])) + list(RANGE(s[0]+1, s[1])) + list(RANGE(s[1]+1, self.ndim))
             args += (dims,)
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
         def apply(r):
-            if len(args) > 1:
-                self = args[0]
-                dims = mkwargs.get('dim', args[1:])
-                if len(dims) == 1 and isinstance(dims[0], (list, tuple)): dims = dims[0]
+            self = args[0]
+            dims = mkwargs.get('dim', args[1:])
+            if mkwargs.get('keepdim', False): r.special_from_(self)
+            elif len(dims) > 0:
+                dims = arg_tuple(dims)
                 if len(dims) == 0: r.special_from_()
+                elif isinstance(dims[0], torch.Tensor): r.special_from_(self)
                 else: r.set_special_(special=[x - len([d for d in dims if 0 <= d < x or d + self.ndim < x]) if x not in dims else r.ndim for x in self._special], bf=self._batch_first)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_expanding_func__(cls, func, types, args=(), kwargs=None):
         "FOR: unsqueeze unsqueeze_ squeeze squeeze_"
         # self = args[0]
         # dims = kwget(kwargs, 'dim', args[1:])
-        # if len(dims) == 1 and isinstance(dims[0], tuple): dims = dims[0]
+        # dims = arg_tuple(dims, no_list=True)
+        # if len(dims) == 0: dims = [i for i, s in enumerate(self.shape) if s == 1]
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
         def apply(r): ...
             # a, b = self._special
             # ndim = self.ndim
             # for d in dims:
-            #     if 0 <= d <= a or d + ndim <= a: a += 1
-            #     if 0 <= d <= b or d + ndim <= b: b += 1
+            #     if 0 <= d <= a or d + ndim < a: a += 1
+            #     if 0 <= d <= b or d + ndim < b: b += 1
             #     ndim += 1
             # r.set_special_(special=[a, b], bf=self._batch_first)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_flatten_func__(cls, func, types, args=(), kwargs=None):
-        "FOR: flatten flatten_"
+        "FOR: flatten"
         dims = kwget(kwargs, 'dim', args[1:])
         if isinstance(dims, tuple) and len(dims) <= 0:
             dims = kwget(kwargs, 'start_dim', 0), kwget(kwargs, 'end_dim', -1)
+            self = args[0]
+            space_dims = [x for x in RANGE(self.ndim) if x not in self._special]
+            if len(space_dims) > 0 and space_dims[-1] - space_dims[0] == len(space_dims) - 1:
+                dims = space_dims[0], space_dims[-1]
+            args = (self,) + dims
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
         def apply(r):
@@ -1395,65 +1977,95 @@
                 dim = dims[0]
                 if dim < 0: dim += self.ndim
                 r.set_special_(special=[r.ndim if x >= dim else x for x in self._special], bf=self._batch_first)
             else:
                 dim1, dim2 = dims
                 if dim1 < 0: dim1 += self.ndim
                 if dim2 < 0: dim2 += self.ndim
-                r.set_special_(special=[r.ndim if dim1 <= x <= dim2 or x > r.ndim else x for x in self._special], bf=self._batch_first)
+                r.set_special_(special=[r.ndim if dim1 <= x <= dim2 else 
+                                        ((r.ndim if x - dim2 + dim1 > r.ndim else x - dim2 + dim1) if x > dim2 else x) 
+                                        for x in self._special], bf=self._batch_first)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_getitem_func__(cls, func, types, args=(), kwargs=None):
-        "FOR: __getitem__ __iter__"
-        if len(args) == 1: self, dims = args[0], 0
-        else: self, dims = args
+        "FOR: __getitem__" # __iter__?
+        if len(args) == 1: self, indices = args[0], 0
+        else: self, indices = args
 
         with torch._C.DisableTorchFunction():
             ret = super().__torch_function__(func, types, args, kwargs)
             if isinstance(ret, type(NotImplemented)):
                 raise NotImplementedError(f"{func} for {args} is not implemented. ")
 
             ndim = self.ndim
 
-            if not isinstance(dims, tuple): dims = (dims,)
-            types = [type(x) for x in dims]
+            if not isinstance(indices, tuple): indices = (indices,)
+            types = [type(x) for x in indices]
             if type(...) in types:
                 if types.count(type(...)) > 1:
                     raise TypeError("")
-                lp = dims[:types.index(type(...))]
-                rp = dims[types.index(type(...))+1:]
+                lp = indices[:types.index(type(...))]
+                rp = indices[types.index(type(...))+1:]
             else:
-                lp = dims
+                lp = indices
                 rp = tuple()
-            offset = ndim - len(rp)
-            isnormal = ''.join('1' if issubclass(t, (INT, slice, type(...))) else '0' for t in types)
-            if '1' in isnormal.strip('1') or '0' not in isnormal: index = -1
-            else: index = isnormal.index('0')
+            offset_rp = ndim - len(rp)
 
+            lm, li = max_argmax([x.ndim if isinstance(x, torch.Tensor) else 0 for x in lp])
+            rm, ri = max_argmax([x.ndim if isinstance(x, torch.Tensor) else 0 for x in rp])
+            ri = [offset_rp + x for x in ri]
+            if lm is not None and lm > 0: 
+                if rm is not None and rm > lm: sub_dim = rm; matched_dims = ri; offset_sub = ri[0]; is_rp = True
+                elif rm is not None and rm == lm: sub_dim = rm; matched_dims = li + ri; offset_sub = li[0]; is_rp = False
+                else: sub_dim = lm; matched_dims = li; offset_sub = li[0]; is_rp = False
+            elif rm is not None and rm > 0: sub_dim = rm; matched_dims = ri; offset_sub = ri[0]; is_rp = True
+            else: offset_sub = None; matched_dims = []; is_rp = False
+            if offset_sub is not None:
+                ref_t = rp[ri[0] - offset_rp] if is_rp else lp[li[0]]
+                sub_special = ref_t._special
+                sub_bf = ref_t._batch_first
+            else: offset_sub = 0; sub_dim = 0; sub_special = [sub_dim, sub_dim]; sub_bf = True
+            removed_dims = matched_dims + [i for i, x in enumerate(lp) if isinstance(x, INT)] + [i + offset_rp for i, x in enumerate(rp) if isinstance(x, INT)]
+    
         def apply(r):
             a, b = self._special
             rdim = r.ndim
-            offset2 = rdim - ndim + len(lp) + len(rp) - len([d for d in lp + rp if isinstance(d, slice)])
-            if a < len(lp) and not isinstance(lp[a], slice): a = None
-            elif offset <= a < ndim and not isinstance(rp[a - offset], slice): a = None
-            if b < len(lp) and not isinstance(lp[b], slice): b = None
-            elif offset <= b < ndim and not isinstance(rp[b - offset], slice): b = None
-            if a is not None and a < ndim:
-                a += offset2 if a > index else 0
-                a -= len([d for d in RANGE(len(lp)) if (0 <= d < a or d + ndim < a) and not isinstance(lp[d], slice)])
-                a -= len([d for d in RANGE(offset, ndim) if (0 <= d < a or d + ndim < a) and not isinstance(rp[d-offset], slice)])
-            elif a is not None: a = rdim
-            if b is not None and b < ndim:
-                b += offset2 if b > index else 0
-                b -= len([d for d in RANGE(len(lp)) if (0 <= d < b or d + ndim < b) and not isinstance(lp[d], slice)])
-                b -= len([d for d in RANGE(offset, ndim) if (0 <= d < b or d + ndim < b) and not isinstance(rp[d-offset], slice)])
-            elif b is not None: b = rdim
-            r.set_special_(special=[a, b], bf=self._batch_first)
+            # offset2 = rdim - ndim + len(lp) + len(rp) - len([d for d in lp + rp if isinstance(d, slice)])
+            # def notseq(x): return not isinstance(x, slice) and not (isinstance(x, bt.Tensor) and x.ndim == 1)
+            # if a < len(lp) and notseq(lp[a]): a = None
+            # elif offset <= a < ndim and notseq(rp[a - offset]): a = None
+            # if b < len(lp) and notseq(lp[b]): b = None
+            # elif offset <= b < ndim and notseq(rp[b - offset]): b = None
+            # if a < ndim:
+            #     a += offset2 if a > index else 0
+            #     a -= len([d for d in RANGE(len(lp)) if (0 <= d < a or d + ndim < a) and not isinstance(lp[d], slice)])
+            #     a -= len([d for d in RANGE(offset, ndim) if (0 <= d < a or d + ndim < a) and not isinstance(rp[d-offset], slice)])
+            # elif a is not None: a = rdim
+            # if b is not None and b < ndim:
+            #     b += offset2 if b > index else 0
+            #     b -= len([d for d in RANGE(len(lp)) if (0 <= d < b or d + ndim < b) and not isinstance(lp[d], slice)])
+            #     b -= len([d for d in RANGE(offset, ndim) if (0 <= d < b or d + ndim < b) and not isinstance(rp[d-offset], slice)])
+            # elif b is not None: b = rdim
+            if a >= ndim or a in removed_dims and not (sub_dim == 1 and len(matched_dims) == 1): a = rdim
+            else:
+                to_rm = len([1 for x in removed_dims if x < a])
+                if a > offset_sub: a += sub_dim
+                a -= to_rm
+            if b >= ndim or b in removed_dims and not (sub_dim == 1 and len(matched_dims) == 1): b = rdim
+            else:
+                to_rm = len([1 for x in removed_dims if x < b])
+                if b > offset_sub: b += sub_dim
+                b -= to_rm
+            bf = self._batch_first
+            if a == rdim: a = sub_special[sub_bf != bf] + offset_sub if sub_special[sub_bf != bf] != sub_dim else rdim
+            if b == rdim: b = sub_special[sub_bf == bf] + offset_sub if sub_special[sub_bf == bf] != sub_dim else rdim
+            if a > b: a, b = b, a; bf = not bf
+            r.set_special_(special=[a, b], bf=bf)
 
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_concatenate_func__(cls, func, types, args=(), kwargs=None):
         "FOR: cat concatenate"
         self = args[0]
@@ -1487,29 +2099,35 @@
         return Tensor.__torch_function_convert_apply__(ret, apply, cls)
 
     @classmethod
     def __torch_function_default_func__(cls, func, types, args=(), kwargs=None):
         "FOR: all the remainings"
         self = args[0]
 
-        with torch._C.DisableTorchFunction():
-            ret = super().__torch_function__(func, types, args, kwargs)
-            if isinstance(ret, type(NotImplemented)):
-                raise NotImplementedError(f"{func} for {args} is not implemented. ")
+        try:
+            with torch._C.DisableTorchFunction():
+                ret = super().__torch_function__(func, types, args, kwargs)
+                if isinstance(ret, type(NotImplemented)): return ret
+        except RuntimeError as e:
+            if kwargs is None: kwargs = {}
+            try:
+                return getattr(self.as_subclass(torch.Tensor), func.__name__)(*args[1:], **kwargs)
+            except: raise e
 
         def apply(r):
             r.special_from_(self)
 
-        return Tensor.__torch_function_convert_apply__(ret, apply, cls)
+        return Tensor.__torch_function_convert_apply__(ret, apply, cls, force=False)
 
     def __torch_function_keys__(func):
-        return func.__func__.__doc__.split('\n')[0].split(':')[-1].strip().split()
+        return func.__func__.__doc__.split('\n\n')[0].split(':')[-1].strip().split()
 
     __torch_function_map__ = {k: '__torch_function_ele_wise_func__' for k in __torch_function_keys__(__torch_function_ele_wise_func__)}
     __torch_function_map__.update({k: '__torch_function_resizing_func__' for k in __torch_function_keys__(__torch_function_resizing_func__)})
+    __torch_function_map__.update({k: '__torch_function_full_func__' for k in __torch_function_keys__(__torch_function_full_func__)})
     __torch_function_map__.update({k: '__torch_function_resizing_as_func__' for k in __torch_function_keys__(__torch_function_resizing_as_func__)})
     __torch_function_map__.update({k: '__torch_function_randint_func__' for k in __torch_function_keys__(__torch_function_randint_func__)})
     __torch_function_map__.update({k: '__torch_function_transpose_func__' for k in __torch_function_keys__(__torch_function_transpose_func__)})
     __torch_function_map__.update({k: '__torch_function_permute_func__' for k in __torch_function_keys__(__torch_function_permute_func__)})
     __torch_function_map__.update({k: '__torch_function_matmul_func__' for k in __torch_function_keys__(__torch_function_matmul_func__)})
     __torch_function_map__.update({k: '__torch_function_addmm_func__' for k in __torch_function_keys__(__torch_function_addmm_func__)})
     __torch_function_map__.update({k: '__torch_function_reducing_func__' for k in __torch_function_keys__(__torch_function_reducing_func__)})
@@ -1517,178 +2135,282 @@
     __torch_function_map__.update({k: '__torch_function_flatten_func__' for k in __torch_function_keys__(__torch_function_flatten_func__)})
     __torch_function_map__.update({k: '__torch_function_getitem_func__' for k in __torch_function_keys__(__torch_function_getitem_func__)})
     __torch_function_map__.update({k: '__torch_function_concatenate_func__' for k in __torch_function_keys__(__torch_function_concatenate_func__)})
     __torch_function_map__.update({k: '__torch_function_stack_func__' for k in __torch_function_keys__(__torch_function_stack_func__)})
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
+        try:
+            if Tensor in types and cls != Tensor: return NotImplemented
 
-        if len(args) == 0: return super().__torch_function__(func, types, args, kwargs)
+            if len(args) == 0: return super().__torch_function__(func, types, args, kwargs)
 
-        sfunc = str(func)
-        if sfunc.startswith('<attribute') or sfunc.startswith('<property'):
-            return super().__torch_function__(func, types, args, kwargs)
-
-        func_name = sfunc.split(' of ')[0].split(' at ')[0].split()[-1].strip("'").split('.')[-1]
-        if func_name in ('__get__', '__set__', '__delete__'):
-            return super().__torch_function__(func, types, args, kwargs)
+            sfunc = str(func)
+            if sfunc.startswith('<attribute') or sfunc.startswith('<property'):
+                return super().__torch_function__(func, types, args, kwargs)
 
-        self = args[0]
-        types = tuple(cls if t in [torch.nn.Parameter, tp.nn.Parameter] else t for t in types)
-        torch_func_name = Tensor.__torch_function_map__.get(func_name, None)
-        if isinstance(self, Tensor) and self.init and self.has_special: pass
-        elif torch_func_name in ('__torch_function_resizing_func__', '__torch_function_resizing_as_func__', '__torch_function_randint_func__'): pass
-        else:
-            with torch._C.DisableTorchFunction():
-                ret = super().__torch_function__(func, types, args, kwargs)
-                collection = []
-            def apply(r): r.special_from_()
-            return Tensor.__torch_function_convert_apply__(ret, apply, cls)
-
-        if torch_func_name is None: return Tensor.__torch_function_default_func__(func, types, args, kwargs)
-        else: return eval(f"Tensor.{torch_func_name}")(func, types, args, kwargs)
+            func_name = sfunc.split(' of ')[0].split(' at ')[0].split()[-1].strip("'").split('.')[-1]
+            if func_name in ('__get__', '__set__', '__delete__'):
+                return super().__torch_function__(func, types, args, kwargs)
 
+            self = args[0]
+            types = tuple(cls if t in [torch.nn.Parameter, bt.nn.Parameter] else t for t in types)
+            torch_func_name = Tensor.__torch_function_map__.get(func_name, None)
+            if isinstance(self, Tensor) and self.init and self.has_special: pass
+            elif torch_func_name in ('__torch_function_resizing_func__', '__torch_function_full_func__', '__torch_function_resizing_as_func__', '__torch_function_randint_func__'): pass
+            else:
+                with torch._C.DisableTorchFunction():
+                    ret = super().__torch_function__(func, types, args, kwargs)
+                def apply(r): r.special_from_()
+                return Tensor.__torch_function_convert_apply__(ret, apply, cls)
+
+            if torch_func_name is None: return Tensor.__torch_function_default_func__(func, types, args, kwargs)
+            else: return getattr(Tensor, torch_func_name)(func, types, args, kwargs)
+            
+        except Exception as e:
+            print(f"In function {func}:")
+            raise e#.with_traceback(None)
+
+    for f in new_dim_methods + old_dim_methods:
+        if f in locals(): locals()[f] = dim_method_wrapper(locals()[f])
+        else: exec(f"{f} = dim_method_wrapper(torch.Tensor.{f})")
 
 for func in '''
-zeros ones
+zeros ones empty
 rand randn
 '''.split():
     __all__.extend([func, func+'_like'])
-    exec(f"""
-
-def {func}(*args, **kwargs):
-
-    if len(args) == 1:
-        arg = args[0]
-        if isinstance(arg, torch.Tensor):
-            return torch.{func}_like(arg, **kwargs).as_subclass(Tensor).special_from_(arg).autodevice_()
-        elif isinstance(arg, (tuple, list)):
-            size = Size(*arg)
-            return torch.{func}(size, **kwargs).as_subclass(Tensor).special_from_(size).autodevice_()
-        else:
-            return torch.{func}(*args, **kwargs).as_subclass(Tensor).special_from_().autodevice_()
+    execblock(f"""
+    def {func}(*args, **kwargs) -> Tensor:
+        rg = kwargs.pop('requires_grad', False)
 
-    size = Size(*args)
-    return torch.{func}(size, **kwargs).as_subclass(Tensor).special_from_(size).autodevice_()
+        size= None
+        if len(args) == 1:
+            arg = args[0]
+            if isinstance(arg, torch.Tensor):
+                return torch.{func}_like(arg, **kwargs).as_subclass(Tensor).special_from_(arg).autodevice_().requires_grad_(rg)
+            elif isinstance(arg, tuple):
+                if isinstance(arg, Size): size = arg
+                else: args = arg
+        
+        if size is None: size = Size(*args)
+        return torch.{func}(size, **kwargs).as_subclass(Tensor).special_from_(size).autodevice_().requires_grad_(rg)
 
-def {func}_like(tensor, **kwargs):
-    return {func}(tensor, **kwargs)
+    def {func}_like(tensor, **kwargs) -> Tensor:
+        return {func}(tensor, **kwargs)
 """)
 
 for func in '''
-range arange
+full
 '''.split():
-    __all__.append(func)
-    exec(f"""
-def {func}(*args, **kwargs):
-    return torch.{func}(*args, **kwargs).as_subclass(Tensor).special_from_().autodevice_()
+    __all__.extend([func, func+'_like'])
+    execblock(f"""
+    def {func}(*args, **kwargs) -> Tensor:
+        rg = kwargs.pop('requires_grad', False)
+        fill = kwargs.pop('fill_value', None)
+        
+        size= None
+        if fill is None:
+            arg, fill = args
+            if isinstance(arg, torch.Tensor):
+                return torch.{func}_like(arg, fill, **kwargs).as_subclass(Tensor).special_from_(arg).autodevice_().requires_grad_(rg)
+            elif isinstance(arg, tuple):
+                if isinstance(arg, Size): size = arg
+                else: args = arg
+        
+        if size is None: size = Size(*args)
+        return torch.{func}(size, fill, **kwargs).as_subclass(Tensor).special_from_(size).autodevice_().requires_grad_(rg)
+
+    def {func}_like(tensor, **kwargs) -> Tensor:
+        return {func}(tensor, **kwargs)
 """)
 
 class _Randint:
 
     def __init__(self):
+        """Please use randint[lower, upper] to specify the range with upper end excluded. """
         self.range = (0, 2)
 
     def __getitem__(self, t):
         if len(t) == 0: t = (0, 2)
         elif len(t) == 1: t = (0, t[0])
         elif len(t) > 2: raise TypeError(f"Please use randint[lower, upper] to specify the range with upper end excluded. ")
         self.range = t
         return self
 
-    def __call__(self, *size, **kwargs):
-        return torch.randint(self.range[0], self.range[1], Size(size), **kwargs).as_subclass(Tensor).special_from_(size).autodevice_()
+    def __call__(self, *size, **kwargs) -> Tensor:
+        rg = kwargs.pop('requires_grad', False)
+        return torch.randint(self.range[0], self.range[1], Size(size), **kwargs).as_subclass(Tensor).special_from_(size).autodevice_().requires_grad_(rg)
 
 class _Randint_like:
 
     def __init__(self):
+        """Please use randint_like[lower, upper] to specify the range with upper end excluded. """
         self.range = (0, 2)
 
     def __getitem__(self, t):
         if len(t) == 0: t = (0, 2)
         elif len(t) == 1: t = (0, t[0])
         elif len(t) > 2: raise TypeError(f"Please use randint_like[lower, upper] to specify the range with upper end excluded. ")
         self.range = t
         return self
 
-    def __call__(self, data, **kwargs):
-        return torch.randint_like(data, self.range[0], self.range[1], **kwargs).as_subclass(Tensor).special_from_(data.shape).autodevice_()
+    def __call__(self, data, **kwargs) -> Tensor:
+        rg = kwargs.pop('requires_grad', False)
+        return torch.randint_like(data, self.range[0], self.range[1], **kwargs).as_subclass(Tensor).special_from_(data.shape).autodevice_().requires_grad_(rg)
 
 randint = _Randint()
 randint_like = _Randint_like()
 __all__.extend(["randint", "randint_like"])
 
-__all__.extend(["eye", "cat", "stack", "t", "unsqueeze", "tensor"])
+__all__.extend(["eye", "eye_as", "eye_like", "cat", "stack", "t", "unsqueeze", "squeeze", "tensor", "tr", "trace"])
 
-def eye(*size: tuple, **kwargs):
-    if len(size) == 1 and isinstance(size, (tuple, list)): size = size[0]
+def eye(*size: tuple, **kwargs) -> Tensor:
+    if len(size) == 1 and isinstance(size, tuple): size = size[0]
 
     size = Size(size)
     if size.nspace < 1: raise TypeError("Empty size not valid for 'eye'. ")
     if size.nspace == 1: size = size + (size.space[0],)
     if size.nspace > 2: raise TypeError("No more than 2-D is allowed for 'eye'. ")
     n = MIN(*size.space)
     s = [slice(None)] * size.ndim
     for i in RANGE(size.ndim):
         if i not in size.special:
             s[i] = torch.arange(n)
     out = zeros(size, **kwargs)
     out[tuple(s)] = 1
     return out
 
-def cat(*list_of_tensors, dim=None, **kwargs):
+@alias("eye_as")
+def eye_like(tensor: Array.Torch) -> Tensor:
+    return eye(tensor.shape)
+
+def cat(*list_of_tensors, dim=None, **kwargs) -> Tensor:
     if dim is None:
         if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], Tensor):
             dim = list_of_tensors[-1]
             list_of_tensors =list_of_tensors[:-1]
         else: dim = 0
-    if len(list_of_tensors) == 1 and isinstance(list_of_tensors[0], (tuple, list)):
-        list_of_tensors = list_of_tensors[0]
+    list_of_tensors = arg_tuple(list_of_tensors)
+    if len(list_of_tensors) == 0: return bt.tensor([])
+    pivot = list_of_tensors[_argmax([x.ndim for x in list_of_tensors])[0]]
+    list_of_tensors = [x.expand_to(pivot, dim=dim) for x in list_of_tensors if x.nele > 0]
+    avouch(ALL([SUM([a != b for a, b in zip(x.shape, pivot.shape)]) <= 1 for x in list_of_tensors]), 
+           "Tensors can only be concatenated when all of them have a same shape except for one dimension. " + 
+           f"Current: {[x.shape for x in list_of_tensors]}")
     ibatch = ichannel = None
-    if isinstance(dim, list): dim = dim[0]; ibatch = dim
-    if isinstance(dim, set): dim = dim.pop(); ichannel = dim
+    if isinstance(dim, list) and len(dim) == 1: dim = dim[0]; ibatch = dim
+    elif isinstance(dim, list) and len(dim) == 0:
+        avouch(ALL([x.has_batch for x in list_of_tensors]), "Tensors can only be concatenated along batch dimension when all of them have one. ")
+        dim = pivot.batch_dim; ibatch = dim
+    elif isinstance(dim, set) and len(dim) == 1: dim = list(dim)[0]; ichannel = dim
+    elif isinstance(dim, dict) and len(dim) == 0:
+        avouch(ALL([x.has_channel for x in list_of_tensors]), "Tensors can only be concatenated along channel dimension when all of them have one. ")
+        dim = pivot.channel_dim; ichannel = dim
+    elif isinstance(dim, INT): pass
+    else: raise TypeError(f"Not identified dimension for concatenation: {dim}.")
+    if dim < 0: dim += list_of_tensors[0].ndim
     self = [t for t in list_of_tensors if isinstance(t, Tensor)]
-    if len(self) == 0: return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_().set_special_(batch_dim=ibatch, channel_dim=ichannel)
+    if len(list_of_tensors) == 0: return torch.tensor([]).as_subclass(Tensor)
+    elif len(self) == 0: return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_().set_special_(batch_dim=ibatch, channel_dim=ichannel)
     return torch.cat(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_(self[0]).set_special_(batch_dim=ibatch, channel_dim=ichannel)
 
-def stack(*list_of_tensors, dim=None, **kwargs):
+def stack(*list_of_tensors, dim=None, **kwargs) -> Tensor:
     if dim is None:
-        if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], Tensor):
+        if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], torch.Tensor):
             dim = list_of_tensors[-1]
-            list_of_tensors =list_of_tensors[:-1]
+            list_of_tensors = list_of_tensors[:-1]
         else: dim = 0
-    if len(list_of_tensors) == 1 and isinstance(list_of_tensors[0], (tuple, list)):
-        list_of_tensors = list_of_tensors[0]
+    list_of_tensors = arg_tuple(list_of_tensors)
+    if len(list_of_tensors) == 0: return bt.tensor([])
+    pivot = list_of_tensors[_argmax([x.ndim for x in list_of_tensors])[0]]
+    if ALL([x.shape == pivot.shape for x in list_of_tensors]): pass
+    else:
+        list_of_tensors = [x.expand_to(pivot) for x in list_of_tensors if x.nele > 0]
+        avouch(ALL([x.shape == pivot.shape for x in list_of_tensors]), 
+            "Tensors can only be stacked when all of them have an exact same shape. ")
     ibatch = ichannel = None
-    if isinstance(dim, list): dim = dim[0]; ibatch = dim
-    if isinstance(dim, set): dim = dim.pop(); ichannel = dim
+    if isinstance(dim, list) and len(dim) == 1: dim = dim[0]; ibatch = dim
+    elif isinstance(dim, list) and len(dim) == 0:
+        avouch(ALL([not x.has_batch for x in list_of_tensors]), "Tensors can only be stacked along batch dimension when none of them has one. ")
+        dim = 0; ibatch = dim
+    elif isinstance(dim, set) and len(dim) == 1: dim = list(dim)[0]; ichannel = dim
+    elif isinstance(dim, dict) and len(dim) == 0:
+        avouch(ALL([not x.has_channel for x in list_of_tensors]), "Tensors can only be stacked along channel dimension when none of them has one. ")
+        dim = 1 if pivot.has_batch else 0; ichannel = dim
+    elif isinstance(dim, INT): pass
+    else: raise TypeError(f"Not identified dimension for concatenation: {dim}.")
+    if dim < 0: dim += list_of_tensors[0].ndim + 1
     self = [t for t in list_of_tensors if isinstance(t, Tensor)]
     if len(self) == 0: return torch.stack(list_of_tensors, dim, **kwargs).as_subclass(Tensor).special_from_().set_special_(batch_dim=ibatch, channel_dim=ichannel)
     return torch.stack(list_of_tensors, dim, **kwargs).as_subclass(Tensor).set_special_(special=[x + 1 if x >= dim else x for x in self[0]._special], bf=self[0]._batch_first).set_special_(batch_dim=ibatch, channel_dim=ichannel)
 
-def t(tensor: Array.Torch):
+def t(tensor: Array.Torch) -> Tensor:
     if isinstance(tensor, Tensor): return tensor.T
     else: return torch.t(tensor).as_subclass(Tensor).special_from_(tensor)
 
-def squeeze(tensor, *args, **kwargs):
+def squeeze(tensor, *args, **kwargs) -> Tensor:
     if isinstance(tensor, Tensor): return tensor.squeeze(*args, **kwargs)
     else: return torch.squeeze(tensor, *args, **kwargs).as_subclass(Tensor).special_from_(tensor)
 
-def unsqueeze(tensor, *args, **kwargs):
+def unsqueeze(tensor, *args, **kwargs) -> Tensor:
     if isinstance(tensor, Tensor): return tensor.unsqueeze(*args, **kwargs)
     else: return torch.unsqueeze(tensor, *args, **kwargs).as_subclass(Tensor).special_from_(tensor)
+    
+def diag(x) -> Tensor:
+    if not isinstance(x, Tensor): x = tensor(x)
+    if x.n_space == 1:
+        d = item([i for i in RANGE(x.n_dim) if i not in x._special])
+        n = x.size(d)
+        shape_out = x.shape[:d+1] + (n,) + x.shape[d+1:]
+        out = bt.zeros(shape_out).type(x.type())
+        out[(slice(None),)*d + (bt.arange(n), bt.arange(n)) + (slice(None),)*(x.n_dim-d-1)] = \
+            x[(slice(None),)*d + (bt.arange(n),) + (slice(None),)*(x.n_dim-d-1)]
+        return out
+    elif x.n_space == 2:
+        p, q = [i for i in RANGE(x.n_dim) if i not in x._special]
+        shape_out = x.shape[:q] + (1,) + x.shape[q+1:]
+        ind = bt.arange(x.size(p)).expand_to(shape_out, axis=p, dim=q)
+        return x.gather(q, ind).squeeze(q)
+    return torch.diag(x).as_subclass(Tensor).special_from_(x)
+
+@alias("tr")
+def trace(x) -> Tensor:
+    return diag(x).sum(-1)
+
+def tensor(data, *, device=None, requires_grad=False, **kwargs) -> Tensor:
+    batch_dim = channel_dim = None
+    for k in kwargs:
+        if 'dim' in k:
+            if k.startswith('b'): batch_dim = kwargs[k]
+            if k.startswith('c'): channel_dim = kwargs[k]
+    if device is None and _device.auto: device = _device
+    if isinstance(device, AutoDevice): device = device.device
+    if isinstance(data, (INT, FLOAT)):
+        out = torch.tensor(data, device=device, requires_grad=requires_grad).as_subclass(Tensor).special_from_()
+    elif isinstance(data, Tensor):
+        out = data.clone()
+    elif isinstance(data, torch.Tensor):
+        out = data.as_subclass(Tensor).special_from_()
+    else: out = Tensor(data, device=device, requires_grad=requires_grad)
+    if batch_dim is not None: out.batch_dim = batch_dim
+    if channel_dim is not None: out.channel_dim = channel_dim
+    return out
 
-def tensor(data, *, dtype=None, device=None, requires_grad=False, pin_memory=False):
-    if device is None and _auto_device is True:
-        device = Device
-    if isinstance(data, Tensor):
-        return data.clone()
-    if isinstance(data, torch.Tensor):
-        return data.as_subclass(Tensor).special_from_()
-    return torch.tensor(data, dtype=dtype, device=device, requires_grad=requires_grad, pin_memory=pin_memory).as_subclass(Tensor).special_from_()
+def batch_tensor(*args, **kwargs) -> Tensor:
+    if len(args) == 1 and not isinstance(args[0], (INT, FLOAT)): args = args[0]
+    if not isinstance(args, Tensor): args = tensor(list(args), **kwargs)
+    avouch(args.ndim == 1, "batorch.batch_tensor only takes 1D data. ")
+    return args.batch_dimension_(0)
+
+def channel_tensor(*args, **kwargs) -> Tensor:
+    if len(args) == 1 and not isinstance(args[0], (INT, FLOAT)): args = args[0]
+    if not isinstance(args, Tensor): args = tensor(list(args), **kwargs)
+    avouch(args.ndim == 1, "batorch.channel_tensor only takes 1D data. ")
+    return args.channel_dimension_(0)
 
 # print(torch_type_list - (torch_type_list - globals()))
 # print(torch_dtype_list - (torch_dtype_list - globals()))
 # print(torch_func_list - (torch_func_list - globals()))
 
 for key in torch_dtype_list:
     if not (key in __all__ or key in globals()):
@@ -1696,18 +2418,46 @@
         __all__.append(key)
 
 for key in torch_type_list:
     if not (key in __all__ or key in globals()):
         exec(f"{key} = torch.{key}")
         __all__.append(key)
 
-for key in dir(torch):
-    if key.startswith("_"):
-        continue
-    if inspect.isclass(eval(f"torch.{key}")):
-        continue
-    if (key in __all__ or key in globals()) and key not in {"typename"}:
-        continue
-    if key in torch_func_list:
-        # functions
-        exec(f"{key} = torch.{key}")
-        __all__.append(key)
+generating_funcs = """
+    range arange linspace
+""".split()
+
+for key in torch_func_list:
+    if key in {"typename"}: continue
+    if key in __all__: continue
+    if key in globals(): continue
+    if key in dir(torch):
+        func = key
+        __all__.append(func)
+        if func in generating_funcs:
+            doit = "ret.requires_grad_(rg)"
+        else: doit = ''
+        execblock(f"""
+        def {func}(*args, **kwargs) -> Tensor:
+            ref_shape = None
+            if len(args) > 0 and isinstance(args[0], Tensor): ref_shape = args[0].shape
+            rg = kwargs.pop('requires_grad', False)
+            ret = torch.{func}(*args, **kwargs)
+            def apply(ret):
+                with torch._C.DisableTorchFunction():
+                    if isinstance(ret, Tensor) and not ret.init or not isinstance(ret, Tensor) and isinstance(ret, torch.Tensor):
+                        ref = None
+                        if ref_shape is not None and len(ret.shape) == len(ref_shape): ref = ref_shape
+                        ret = ret.as_subclass(Tensor).autodevice_()
+                        ret = ret.as_subclass(Tensor).special_from_(ref)
+                        {doit}
+                        return ret
+
+                    if not isinstance(ret, torch.Tensor) and isoftype(ret, (tuple, list, Iterable)):
+                        # Also handles things like namedtuples
+                        return type(ret)(apply(r) for r in ret)
+
+                    return ret
+            return apply(ret)
+        """)
+
+inv = eval('inverse')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyoverload-1.1.24/pyoverload/__init__.py` & `pyoverload-1.1.26/pyoverload/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'pyoverload',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.24',
+    version = '1.1.25',
     contact = 'bertiezhou@163.com',
     keywords = ['overload'],
-    description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. "
+    description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. ",
+    requires = ['pycamia'],
+    update = '2022-07-07 21:00:45'
 ).check()
 
 from .typehint import isofsubclass, inheritable, isitertype, iterable, isarray, isdtype, isatype, isoftype, isclassmethod, typename, Type, params, Bool, Int, Float, Str, Set, List, Tuple, Dict, Class, Callable, Function, Method, Lambda, Functional, Real, real, Null, null, Sequence, sequence, Array, Iterable, Scalar, IntScalar, FloatScalar #*
 from .override import override, overload, params #*
 
 
 
 
 
 
 
+
+
+
+
+
```

### Comparing `pyoverload-1.1.24/pyoverload/override.py` & `pyoverload-1.1.26/pyoverload/override.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     override
     overload
     params
 """.split()
 
 from functools import wraps
 from .typehint import *
-from .typehint import TypeHintError, _getDeclaration
-from .utils import get_environ_globals, _get_wrapped, raw_function, decorator
+from .typehint import TypeHintError, get_declaration
+from .utils import get_environ_vars, _get_wrapped, raw_function, decorator
 
 _debug = False
 
 def set_debug_mode(m): global _debug; _debug = m
 
 def _wrap_params(f):
     if hasattr(f, '__wrapped__'):
         if '[params]' in f.__name__: return None, f
         else: return f, params(run=False)(_get_wrapped(f))
     return f, params(run=False)(f)
 
 def _collect_declarations(func, collection, place_first=False, error=''):
     f = _get_wrapped(raw_function(func))
-    toadd = '\t'.join([_getDeclaration(f)] + ([error] if error else []))
+    toadd = '\t'.join([get_declaration(f)] + ([error] if error else []))
     if place_first: collection.insert(0, toadd)
     else: collection.append(toadd)
     # if f.__doc__:
     #     lines = f.__doc__.split('\n')
     #     toadd = ''
     #     for l in lines:
     #         if not l.strip(): continue
@@ -51,16 +51,16 @@
     if fname.endswith('__0__') or fname.endswith('__default__'):
         fname = '__'.join(fname.split('__')[:-2])
         if change_name: f.__name__ = fname + '['.join(f.__name__.split('[')[1:])
     return fname
 
 @decorator
 def overload(func):
-    local_vars = get_environ_globals()
     fname = raw_function(func).__name__.split('[')[0]
+    local_vars = get_environ_vars(pivot='overload', offset=2).locals
     rawfname = _get_func_name(func, change_name = False)
     key = f"__overload_{rawfname}__"
     overrider = f"__override_{rawfname}__"
     if key in local_vars:
         local_vars[key] = local_vars[key] + 1
         new_name = f"__{fname}_overload_{local_vars[key]}"
         local_vars[new_name] = local_vars[overrider](func)
```

### Comparing `pyoverload-1.1.24/pyoverload/typehint.py` & `pyoverload-1.1.26/pyoverload/typehint.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Iterable
     Scalar
     IntScalar
     FloatScalar
 """.split()
 
 import re, sys
-from .utils import decorator, get_environ_locals, raw_function, _get_wrapped, _rawname
+from .utils import decorator, get_declaration, update_locals_by_environ, raw_function, _get_wrapped, _rawname
 
 try:
     import inspect
     have_inspect = True
 except ImportError: have_inspect = False
 
 class TypeHintError(Exception): pass
@@ -65,16 +65,16 @@
     inheritable(x) -> bool
 
     Returns whether a class type can be inherited. 
 
     Args:
         x (type): the input class name.
 
-    Example::
-
+    Example:
+    ----------
         >>> inheritable(int)
         True
         >>> inheritable(bool)
         False
     """
     if isinstance(x, Type) or callable(x): return False
     try:
@@ -87,59 +87,58 @@
     iterable(x) -> bool
 
     Returns whether an instance can be iterated. Strings are excluded. 
 
     Args:
         x (any): the input variable.
 
-    Example::
-
+    Example:
+    ----------
         >>> iterable(x for x in range(4))
         True
         >>> iterable({2, 3})
         True
         >>> iterable("12")
         False
     """
+    if equals(x, 'iterable check'): return ''
     if isinstance(x, str): return False
     if isinstance(x, type): return False
     if callable(x): return False
     return hasattr(x, '__iter__') and hasattr(x, '__len__')
 
 def isitertype(x):
     """
     isitertype(x) -> bool
 
     Returns whether a type can be iterated. Str type is excluded. 
 
     Args:
         x (type): the input variable.
 
-    Example::
-
+    Example:
+    ----------
         >>> isitertype(list)
         True
         >>> isitertype(str)
         False
     """
     if isinstance(x, str):
-        local_vars = get_environ_locals()
-        local_vars.update(locals())
-        locals().update(local_vars)
+        update_locals_by_environ()
         try: x = eval(x)
         except: return False
     if isinstance(x, Type):
         if x.itemtypes is not None: return True
         return all([isitertype(i) for i in x.types])
     if isinstance(x, type):
         return hasattr(x, '__iter__') and hasattr(x, '__len__')
     if callable(x):
         try: return equals(x('iterable check'), '')
         except Exception: return False
-    raise SystemError("Conflict between functions 'isatype' and 'isitertype', please contact the developer for more information. ")
+    raise SystemError("Conflict between functions 'isatype' and 'isitertype', please contact the developer for more information (Error Code: H121). ")
 
 def isofsubclass(x, px):
     """
     isofsubclass(x, px) -> bool
 
     Returns whether a type 'x' is a subclass of type 'px'.
 
@@ -155,16 +154,16 @@
     isarray(x) -> bool
 
     Returns whether an instance is an array. 
 
     Args:
         x (any): the input variable.
 
-    Example::
-
+    Example:
+    ----------
         >>> isarray(np.array([2, 3]))
         True
         >>> isarray(torch.tensor([2, 3]))
         True
         >>> isarray([1, 2])
         False
     """
@@ -177,16 +176,16 @@
     isdtype(x) -> bool
 
     Returns whether an instance is a data type of numpy or pytorch or tensorflow etc. . 
 
     Args:
         x (any): the input variable.
 
-    Example::
-
+    Example:
+    ----------
         >>> isdtype(np.int32)
         True
         >>> isdtype(torch.float64)
         True
         >>> isdtype(int)
         False
     """
@@ -195,23 +194,23 @@
 def isatype(x):
     """
     isatype(x) -> bool
 
     Returns whether an instance is a type. 
     
     Note:
-        Types detected includes all python classes and pyctlib.Type as well as:
+        Types detected includes all python classes, `pycamia.typehint.Type` objects and,
         1. None representing any type
         2. a list or iterable set of types like [int, float]
 
     Args:
         x (any): the input variable.
 
-    Example::
-
+    Example:
+    ----------
         >>> isatype(np.array)
         False
         >>> isatype(np.ndarray)
         True
         >>> isatype(None)
         True
         >>> isatype([int, np.ndarray])
@@ -253,34 +252,33 @@
     """
     isoftype(x, xtype) -> bool
 
     Returns whether an instance 'x' is of type 'xtype'. 
     
     Note:
         'xtype' can be provided in one of the following fashions:
-        1. a pyctlib.Type like Int, Dict[2]@{int: str} or List<<Int>>[]
+        1. a `pycamia.typehint.Type` object like Int, Dict[2]@{int: str} or List<<Int>>[]
         2. a str representing a type, either the full name of the required 
             type or a name that can be computed when the package is used.
         3. None representing any type
         4. a list or iterable set of types like [int, float]
 
     Args:
         x (any): the input variable.
         xtype (type): the type to check.
 
-    Example::
+    Example:
+    ----------
         >>> isoftype(1, None)
         True
         >>> isoftype(1., [int, 'np.ndarray'])
         False
     """
     if isinstance(xtype, str):
-        local_vars = get_environ_locals()
-        local_vars.update(locals())
-        locals().update(local_vars)
+        update_locals_by_environ()
         try: xtype = eval(xtype)
         except: return xtype in [_rawname(t) for t in type(x).__mro__]
     if xtype == type: return isatype(x)
     if xtype is None: return True
     if not iterable(xtype):
         if isinstance(xtype, Type):
             if xtype.isunion and type(x) in xtype.types: return True
@@ -312,27 +310,28 @@
 
 class _strIO:
     def __init__(self): self._str_ = ''
     def write(self, s): self._str_ += s
     def __str__(self): return self._str_
     def split(self, c=None): return self._str_.split(c)
 
-def _getDeclaration(func):
-    if have_inspect and '__file__' in func.__globals__:
-        try:
-            dec = next(l for l in inspect.getsource(func).split('\n') if l.strip() and not l.strip().startswith('@')).strip().rstrip(':')
-            return dec[dec.index('('):]
-        except OSError: pass
-    ss = _strIO()
-    oldout = sys.stdout
-    sys.stdout = ss
-    help(func)
-    sys.stdout = oldout
-    dec = [l for l in ss.split('\n') if len(l) > 0 and 'Help' not in l][0].replace("def ", '').strip().strip(':')
-    return dec[dec.index('('):]
+# def _getDeclaration(func):
+#     if have_inspect and '__file__' in func.__globals__:
+#         try:
+#             dec = next(l for l in inspect.getsource(func).split('\n') if l.strip() and not l.strip().startswith('@')).strip().rstrip(':')
+#             if '(' in dec: return '('.join([''] + dec.split('(')[1:])
+#             else: return dec
+#         except OSError: pass
+#     ss = _strIO()
+#     oldout = sys.stdout
+#     sys.stdout = ss
+#     help(func)
+#     sys.stdout = oldout
+#     dec = [l for l in ss.split('\n') if len(l) > 0 and 'Help' not in l][0].replace("def ", '').strip().strip(':')
+#     return dec[dec.index('('):]
 
 def _get_func_name(f):
     try: rawname = f.__name__
     except: rawname = ''
     if not rawname:
         try: rawname = f.__class__.__name__
         except: rawname = ''
@@ -382,15 +381,15 @@
             shape = _T[0].shape
             ext = _T[0].extendable
             itypes = _T[0].itemtypes
             inheritableT = _T[0].inheritableT
             _T = _T[0].types
         else:
             _T = Type.extractType(_T)
-            if name == None: name = cls.__name__ + '.' + '/'.join(map(typename, _T))
+            if name is None: name = cls.__name__ + '.' + '/'.join(map(typename, _T))
             inheritableT = tuple(t for t in _T if inheritable(t))
 
         self = super().__new__(cls, name, inheritableT, {})
         self.inv = inv
         self.types = _T
         self.name = name
         self.shape = shape
@@ -465,15 +464,15 @@
     def __invert__(self):
         T = Type(self)
         T.inv = not self.inv
         return T
 
     def __str__(self):
         string = f"<Type '{'*' * self.extendable}{'non-' * self.inv}{self.rawname}"
-        if self.itemtypes != None:
+        if self.itemtypes is not None:
             if isinstance(self.itemtypes, Type):
                 string += f"<{self.itemtypes.rawname}>"
             elif isinstance(self.itemtypes, type):
                 string += f"<{_rawname(self.itemtypes)}>"
             elif iterable(self.itemtypes):
                 string += f"<{'/'.join([_rawname(t).capitalize() for t in self.itemtypes])}>"
             else: string += f"<{self.itemtypes}>"
@@ -515,15 +514,15 @@
         if self.isunion: return isoftype(arg, self.types)
         if isoftype(arg, self.types):
             if len(self.shape) == 0: pass
             elif len(self.shape) == 1 and (len(arg) == self.shape[0] or self.shape[0] in (None, -1)): pass
             elif len(self.shape) > 1 and isarray(arg) and \
                 all([a==b or b in (None, -1) for a, b in zip(arg.shape, self.shape)]): pass
             else: return false
-            if self.itemtypes != None:
+            if self.itemtypes is not None:
                 if not iterable(arg): raise TypeHintError(str(arg) + " is not iterable. ")
                 if isinstance(self.itemtypes, dict):
                     if len(self.itemtypes) <= 0:
                         raise TypeHintError("Wrong item types after @, {} is not allowed. ")
                     for k, v in arg.items():
                         for ktype, vtype in self.itemtypes.items():
                             if isoftype(k, ktype) and isoftype(v, vtype): break
@@ -603,31 +602,31 @@
             import torch
             return Type(torch.Tensor)
         except ImportError: pass
 
     @property
     def TensorFlow(self):
         try:
-            ss = strIO()
+            ss = _strIO()
             olderr = sys.stderr
             sys.stderr = ss
             import tensorflow as tf
             sys.stderr = olderr
             return Type(tf.Tensor)
         except ImportError: pass
 
     @property
-    def TensorPlus(self):
+    def Batorch(self):
         try:
-            import pyctlib.torchplus as tp
-            return Type(tp.Tensor)
+            import batorch as bt
+            return Type(bt.Tensor)
         except ImportError: pass
 
 Array = ArrayType(name="Array")
-Iterable = T(Array, Sequence, set, dict, name="Iterable")
+Iterable = T(Array, Sequence, set, dict, iterable, name="Iterable")
 
 class ScalarType(Type):
     def __call__(self, x):
         if isarray(x):
             if not (len(x.shape) == 0 or all([i==1 for i in x.shape])): return False
             res = False
             for t in self.types:
@@ -643,15 +642,15 @@
     getTypes = False
     allargs = {}
     if "__type__" in kwargs: getTypes = kwargs.pop('__type__')
     if "__return__" in kwargs: allargs['return'] = kwargs.pop('__return__')
     inputargs = list(args)
     normalargs = func.__code__.co_varnames[:func.__code__.co_argcount]
     extargs = func.__code__.co_varnames[func.__code__.co_argcount:]
-    dec = _getDeclaration(func)
+    dec = get_declaration(func).split('(', 1)[-1].rstrip(')')
     eargs = ''.join(re.findall(r"[^*]\*{1} *(\w+)\b", dec))
     ekwargs = ''.join(re.findall(r"[^*]\*{2} *(\w+)\b", dec))
     lendefault = 0 if not func.__defaults__ else len(func.__defaults__)
     rg = lendefault - func.__code__.co_argcount, lendefault
     for var, idefault in zip(normalargs, range(*rg)):
         if len(inputargs) > 0:
             if var in kwargs:
@@ -687,15 +686,16 @@
     return allargs
 
 @decorator
 def params(*types, run=True, **kwtypes):
     if len(types) == 1 and len(kwtypes) == 0 and Functional(types[0]): return params()(types[0])
     @decorator
     def induced_decorator(func):
-        declaration = _getDeclaration(_get_wrapped(raw_function(func)))
+        declaration = get_declaration(_get_wrapped(raw_function(func)))
+        declaration = declaration[declaration.index('('):]
         eargs = ''
         ekwargs = ''
         depth = []
         d = 0;
         is_comma = False
         is_star = False
         args_rec = False
@@ -703,19 +703,20 @@
         for c in declaration:
             if c in '([{': d += 1
             depth.append(d)
             if c not in "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_0123456789":
                 kwargs_rec = args_rec = False
             elif kwargs_rec: ekwargs += c
             elif args_rec: eargs += c
-            if c  == '*' and d == 1:
+            if c == '*' and d == 1:
                 if is_star:
                     # **
                     kwargs_rec = True
                     ekwargs += c
+                    is_star = False
                 elif is_comma:
                     is_star = True
             elif is_star:
                 # *
                 args_rec = True
                 eargs += c
                 is_star = False
@@ -767,15 +768,16 @@
 
 @decorator
 def params_old(*types, run=True, **kwtypes):
     israw = len(kwtypes) == 0 and len(types) == 1 and \
             callable(types[0]) and not isatype(types[0])
     @decorator
     def wrap(func):
-        org_dec = _getDeclaration(func)
+        org_dec = get_declaration(func)
+        org_dec = org_dec[org_dec.index('('):]
         if isclassmethod(func): alltypes = (None,) + types
         else: alltypes = types
         if israw or (len(kwtypes) == 0 and len(types) == 0):
             annotations = {k: v.strip('\'"') if isinstance(v, str) else v for k, v in func.__annotations__.items()}
         else: annotations = getArgs(func, *alltypes, **kwtypes, __type__=True)
         def wrapper(*args, **kwargs):
             if israw or (len(kwtypes) == 0 and len(types) == 0):
@@ -818,16 +820,16 @@
                 if run:
                     retval = func(*args, **kwargs)
                     if 'return' not in _annotations or isoftype(retval, _annotations['return']): return retval
                     raise TypeHintError(_get_func_name(func) + "() returns an invalid value.")
                 else: return None
             raise TypeHintError(_get_func_name(func) + "() has argument " + arg + " of wrong type. \
 Expect type {type} but get {value}.".format(type=repr(_annotations[arg]), value=repr(_values[arg])))
-        org_dec = _getDeclaration(func)
-        dec = org_dec
+        org_dec = get_declaration(func)
+        dec = org_dec[org_dec.index('('):]
         for arg in annotations:
             if arg == 'return':
                 dec = dec[:dec.rindex(')')] + f") -> {_rawname(annotations[arg])}"
                 continue
             res = re.search(rf"\b{arg}\b", dec)
             if res:
                 idx = res.span()[0]
```

### Comparing `pyoverload-1.1.24/pyoverload.egg-info/PKG-INFO` & `pyoverload-1.1.26/pyoverload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverload
-Version: 1.1.24
+Version: 1.1.26
 Summary: 'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. 
 Home-page: https://github.com/Bertie97/PyZMyc/pyoverload
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pyoverload
         
@@ -210,15 +210,15 @@
         
         The basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, 
         
         1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. 
         2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.
         3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. 
         4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.
-        5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `torchplus` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.TorchPlus` to identify specific packages. 
+        5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `batorch` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.Batorch` to identify specific packages. 
         6. `Iterable` includes `Array`, `Sequence` and `dict`. 
         7. Three types of `Scalar`s support the array variables.
         
         All these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. 
         
         One can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned.
```

### Comparing `pyoverload-1.1.24/setup.py` & `pyoverload-1.1.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'pyoverload',
-	version = '1.1.24',
+	version = '1.1.26',
 	keywords = ['pip', 'pymyc', 'pyoverload', 'overload'],
 	description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. ",
-	long_description = '# pyoverload\n\n## Introduction\n\n[`pyoverload`](https://github.com/Bertie97/pycamia/tree/main/pyoverload) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a powerful overloading tools to provide easy overload for `python v3.6+`. `pyoverload` provide multiple usages. The simplest one, however, can be easily implemented as follows. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1)\nfunc1 1\n>>> func("1")\nfunc2 1\n```\n\n`pyoverload` has all of following appealing features:\n\n1. Support of **`Jedi` auto-completion** by keyword decorator `@overload`. This means all main-stream python IDE can hint you the overloaded functions you have defined. \n2. **Multiple usages** that are user friendly for all kinds of users, including `C/Java` language system users and those who are used to `singledispatch` based overload. Also, easy collector of ordinary python functions is also provided. \n3. Support of **all kinds of functions**, including functions, methods, class methods and static methods. One simple implementation for all.\n4. **String types** supported. This means that one can use `"numpy.ndarray"` to mark a numpy array without importing the whole package. \n5. Sufficient **built-in types are provided** for easy representations such as `List[Int]`, `Dict@{str: int}` or `List<<int>>[10]`. \n6. **Available usage listing** when no overload function matches the input arguments. \n7. **Type constraint for an ordinary function** using `@params` decorator. \n\n## Installation\n\nThis package can be installed by `pip install pyoverload` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pyoverload\n```\n\n## Usages\n\n### Usage 1: Decorator Fashion\n\nOne can use `@overload` before the functions with the same function name to build an overloaded function. When the function is called, the inputs will be handed out to the suitable implementation. \n\nThe types of the input arguments are specified by the typehints available in `python3.6+`. All known types can be added after the colon. For package classes like `np.ndarray`, please use a string to represent it. For more types, one can use types from package `types` or `pyoverload.typehint`. \n\nFor usage of `pyoverload.typehint`, please refer to section **Typehints** for more information.\n\nAll implementations of the overloaded function are referenced in the order of definition, but the implementation ends with `__default__` or `__0__` will be used when no usage is available. Note that there are **four** underlines for this notation, **two** on each side. \n\n```python\n>>> from pyoverload import *\n>>> import numpy as np\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n...\n>>> @overload\n... def func(x: str):\n... \tprint("func3", x)\n...\n>>> @overload\n... def func(x: List<<Int>>[4]):\n... \tprint("func4", x)\n...\n>>> @overload\n... def func(x: \'np.ndarray\'):\n... \tprint("func5", x)\n...\n>>> func(1)\nfunc2 1\n>>> func("1")\nfunc3 1\n>>> func([1,2,3,4])\nfunc4 [1, 2, 3, 4]\n>>> func(np.array([1,2,3,4]))\nfunc5 [1 2 3 4]\n>>> func(1.)\nfunc1 1.0\n```\n\nNote that the auto-completion by `Jedi` can only work for this usage. \n\n<img src="https://github.com/Bertie97/pycamia/raw/main/pyoverload/Jedi.jpg" alt="Jedi" style="zoom:50%;" />\n\n### Usage 2: Registering Fashion\n\nAfter using `@overload` decorator, apart from using `@overload` to decorate functions with the same name, one can also use the decorator with the function name `@{fill in the function name}` to decorate other functions with relevant names like `func1`, `func_str`, `first_func` for function `func`. However, omitting sign `_` is recommended for these functions. \n\nIn this fashion, the default function is the one decorated with `@overload` though it can still be changed by adding `__default__` or `__0__` tags in the decorated function names. All typehints are the same as the first usage. \n\nThe following example realized the first three functions in the usage 1 example in a reimplementation. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x):\n... \tprint("func1", x)\n... \n>>> @func\n... def func2(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\nNote that **usage 1** and **usage 2** can be used together though you may need to specify the default function manually like in usage 1 if needed. The last example is rewrote in a combined style. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\n### Usage 3: Collector Fashion\n\nThe last possible usage can not be used along with the previous two, or at least this is not tested by the developer and is not recommended. Another decorator `@override` is used as a collector. \n\nIn this usage, all functions should have different names and all functions with typehints should add decorator `@params` to activate the typehint regularization. Collector `@override` takes additional function list as the arguments indicating these functions should be packed into a single function. \n\nNote that the last function in the function list is the default function. \n\n```python\n>>> from pyoverload import override, params\n>>> @params\n... def func_all(x):\n... \tprint("func1", x)\n... \n>>> @params\n... def func_int(x: int):\n... \tprint("func2", x)\n... \n>>> @params\n... def func_str(x: str):\n... \tprint("func3", x)\n... \n>>> @override(func_int, func_str, func_all)\n... def func(): pass\n... \n```\n\nTheoretically, decorator `@override` can also be used in **usages 1&2**, but this is not recommended either. \n\n## Implementation List\n\nWhen an overloaded function receives arguments that are not suitable for all implementations, the error information will tell you which ones are correct. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1.)\nTraceback (most recent call last):\n  [...omitted...]\nNameError: No func() matches arguments 1.0. All available usages are:\nfunc(x:int)\nfunc(x:str)\n```\n\nThis function is available for all two Implementations but none of them takes `1.`. \n\n## Typehints\n\nDecorator `@params` enables functions to reject inputs with wrong types by raising **`TypeHintError`**. One can use it directly to decorate functions with python typehints or one can add some arguments to it. In the following example, we apply the condition that `a` is a function, `b` is an integer, `k` is a series of integers while function `test_func` needs to return an iterable type of real numbers with length `2`. \n\n```python\n>>> from pyoverload import *\n>>> @params(Func, Int, +Int, __return__ = Real[2])\n... def test_func(a, b=2, *k):\n...     print(a, b, k)\n...     return k\n...\n>>> test_func(lambda x: 1, 3, 4, 5)\n<function <lambda> at 0x7fbdb2027f70> 3 (4, 5)\n(4, 5)\n```\n\nThe basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, \n\n1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. \n2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.\n3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. \n4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.\n5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `torchplus` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.TorchPlus` to identify specific packages. \n6. `Iterable` includes `Array`, `Sequence` and `dict`. \n7. Three types of `Scalar`s support the array variables.\n\nAll these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. \n\nOne can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned. \n\nFor a `Type`, `List` for example, we can do the following operations. Except the first four, these usages are designed for iterable types only. \n\n1. `+List`: This indicates that this is an extendable argument, which means it decorates arguments after `*`. It was used to specify `*args` arguments in `@params` but currently deprecated though adding `+` would not lead to failures. \n\n2. `~List`: This invert the typehint, meaning that all non-list types. \n\n3. `List|Tuple`: This is equivalent to `Type(List, Tuple)` indicating list or tuples. \n\n4. `Type(A)&Callable`: The *and* operator. Note that both indicator should be `Type`s. \n\n   ```python\n   >>> from pyoverload import *\n   >>> class A: pass\n   ...\n   >>> class B(A): pass\n   ...\n   >>> class C(A):\n   ...     def __call__(self): pass\n   ...\n   >>> isoftype(B(), Type(A)&Callable)\n   False\n   >>> isoftype(C(), Type(A)&Callable)\n   True\n   ```\n\n5. `List[5]`: This indicates the length or shape of the variable. For other types such as `Int[5]`, this indicates an iterable of length 5 with integer elements. Note that `Array[3, 4]` represents an array with shape `3 x 4`, but this representation is not available for nested lists. Use `List[List[4]][3]` or `List<<List[4]>>[3]` instead.\n\n6. `List@[int, str]`: This only works for ordered sequence `List` and `Tuple`. It indicates that the list has 2 elements, and the first one is an integer while the second is a string. Note that this is **not** equivalent to `List[int, str]` which represents a list with elements either integer or string.\n\n7. `List@int` or `Dict@{str: int}`: For all Iterables, `A@B` indicates type `A` with all elements of type `B`. `Dict@{str:int}` represents a dictionary with string keys and integer values.  \n\n8. `List[int]`: `=List@int`. A list with integer elements. Note that one can use `List[Int|float]` to directly identify a list of elements that are either `int` or `float`. `List[int, float]` and `Dict[str: int, int:str]` are also valid for multiple element types or key-value pairs. Using list in the blankets will return to the effect of `@` operator: `List[[int, float]]=List@[int, float]`. \n\n9. `List<<int>>[10]`: `=(List@int)[10]=List[int][10]` The first one of the two types should be a `Type`. The representation refers to an integer list of length 10 which is equivalent to `List[10]@int`. The length or shape is not specified if a pair of empty blankets is given. Use `List<<Type(int, Float)>>[]` to represent multiple candidates and `Dict<<(str,int)>>[]=Dict[str:int]` to represent a dictionary. \n\n10. `len(List[10, 20])`: Function `len` returns the length of the array. `200` should be the result for the given example. \n\n## Suggestions\n\n1. The speed of type check for `pyoverload.typehint.Type` is not very fast, hence please try your best to use builtin types, types from module `types` or list of types to do the typehint. \n2. The `overload` takes extra time for delivering the arguments, hence using it for functions require fast speed is not recommended. \n3. Do use `@params` for functions not overloaded but needs typehint constraints instead of using `@overload` without actually has multiple implementations. This is because `@params` is way faster. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
+	long_description = '# pyoverload\n\n## Introduction\n\n[`pyoverload`](https://github.com/Bertie97/pycamia/tree/main/pyoverload) is a package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a powerful overloading tools to provide easy overload for `python v3.6+`. `pyoverload` provide multiple usages. The simplest one, however, can be easily implemented as follows. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1)\nfunc1 1\n>>> func("1")\nfunc2 1\n```\n\n`pyoverload` has all of following appealing features:\n\n1. Support of **`Jedi` auto-completion** by keyword decorator `@overload`. This means all main-stream python IDE can hint you the overloaded functions you have defined. \n2. **Multiple usages** that are user friendly for all kinds of users, including `C/Java` language system users and those who are used to `singledispatch` based overload. Also, easy collector of ordinary python functions is also provided. \n3. Support of **all kinds of functions**, including functions, methods, class methods and static methods. One simple implementation for all.\n4. **String types** supported. This means that one can use `"numpy.ndarray"` to mark a numpy array without importing the whole package. \n5. Sufficient **built-in types are provided** for easy representations such as `List[Int]`, `Dict@{str: int}` or `List<<int>>[10]`. \n6. **Available usage listing** when no overload function matches the input arguments. \n7. **Type constraint for an ordinary function** using `@params` decorator. \n\n## Installation\n\nThis package can be installed by `pip install pyoverload` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pyoverload\n```\n\n## Usages\n\n### Usage 1: Decorator Fashion\n\nOne can use `@overload` before the functions with the same function name to build an overloaded function. When the function is called, the inputs will be handed out to the suitable implementation. \n\nThe types of the input arguments are specified by the typehints available in `python3.6+`. All known types can be added after the colon. For package classes like `np.ndarray`, please use a string to represent it. For more types, one can use types from package `types` or `pyoverload.typehint`. \n\nFor usage of `pyoverload.typehint`, please refer to section **Typehints** for more information.\n\nAll implementations of the overloaded function are referenced in the order of definition, but the implementation ends with `__default__` or `__0__` will be used when no usage is available. Note that there are **four** underlines for this notation, **two** on each side. \n\n```python\n>>> from pyoverload import *\n>>> import numpy as np\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n...\n>>> @overload\n... def func(x: str):\n... \tprint("func3", x)\n...\n>>> @overload\n... def func(x: List<<Int>>[4]):\n... \tprint("func4", x)\n...\n>>> @overload\n... def func(x: \'np.ndarray\'):\n... \tprint("func5", x)\n...\n>>> func(1)\nfunc2 1\n>>> func("1")\nfunc3 1\n>>> func([1,2,3,4])\nfunc4 [1, 2, 3, 4]\n>>> func(np.array([1,2,3,4]))\nfunc5 [1 2 3 4]\n>>> func(1.)\nfunc1 1.0\n```\n\nNote that the auto-completion by `Jedi` can only work for this usage. \n\n<img src="https://github.com/Bertie97/pycamia/raw/main/pyoverload/Jedi.jpg" alt="Jedi" style="zoom:50%;" />\n\n### Usage 2: Registering Fashion\n\nAfter using `@overload` decorator, apart from using `@overload` to decorate functions with the same name, one can also use the decorator with the function name `@{fill in the function name}` to decorate other functions with relevant names like `func1`, `func_str`, `first_func` for function `func`. However, omitting sign `_` is recommended for these functions. \n\nIn this fashion, the default function is the one decorated with `@overload` though it can still be changed by adding `__default__` or `__0__` tags in the decorated function names. All typehints are the same as the first usage. \n\nThe following example realized the first three functions in the usage 1 example in a reimplementation. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x):\n... \tprint("func1", x)\n... \n>>> @func\n... def func2(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\nNote that **usage 1** and **usage 2** can be used together though you may need to specify the default function manually like in usage 1 if needed. The last example is rewrote in a combined style. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func__default__(x):\n... \tprint("func1", x)\n...\n>>> @overload\n... def func(x: int):\n... \tprint("func2", x)\n... \n>>> @func\n... def _(x: str):\n... \tprint("func3", x)\n... \n```\n\n### Usage 3: Collector Fashion\n\nThe last possible usage can not be used along with the previous two, or at least this is not tested by the developer and is not recommended. Another decorator `@override` is used as a collector. \n\nIn this usage, all functions should have different names and all functions with typehints should add decorator `@params` to activate the typehint regularization. Collector `@override` takes additional function list as the arguments indicating these functions should be packed into a single function. \n\nNote that the last function in the function list is the default function. \n\n```python\n>>> from pyoverload import override, params\n>>> @params\n... def func_all(x):\n... \tprint("func1", x)\n... \n>>> @params\n... def func_int(x: int):\n... \tprint("func2", x)\n... \n>>> @params\n... def func_str(x: str):\n... \tprint("func3", x)\n... \n>>> @override(func_int, func_str, func_all)\n... def func(): pass\n... \n```\n\nTheoretically, decorator `@override` can also be used in **usages 1&2**, but this is not recommended either. \n\n## Implementation List\n\nWhen an overloaded function receives arguments that are not suitable for all implementations, the error information will tell you which ones are correct. \n\n```python\n>>> from pyoverload import overload\n>>> @overload\n... def func(x: int):\n...     print("func1", x)\n...\n>>> @overload\n... def func(x: str):\n...     print("func2", x)\n...\n>>> func(1.)\nTraceback (most recent call last):\n  [...omitted...]\nNameError: No func() matches arguments 1.0. All available usages are:\nfunc(x:int)\nfunc(x:str)\n```\n\nThis function is available for all two Implementations but none of them takes `1.`. \n\n## Typehints\n\nDecorator `@params` enables functions to reject inputs with wrong types by raising **`TypeHintError`**. One can use it directly to decorate functions with python typehints or one can add some arguments to it. In the following example, we apply the condition that `a` is a function, `b` is an integer, `k` is a series of integers while function `test_func` needs to return an iterable type of real numbers with length `2`. \n\n```python\n>>> from pyoverload import *\n>>> @params(Func, Int, +Int, __return__ = Real[2])\n... def test_func(a, b=2, *k):\n...     print(a, b, k)\n...     return k\n...\n>>> test_func(lambda x: 1, 3, 4, 5)\n<function <lambda> at 0x7fbdb2027f70> 3 (4, 5)\n(4, 5)\n```\n\nThe basic types in `pyoverload.typehint` are `Bool`, `Int`, `Float`, `Str`, `Set`, `List`, `Tuple`, `Dict`, `Callable`, `Function`, `Method`, `Lambda`, `Functional`, `Real`, `Null`, `Sequence`, `Array`, `Iterable`, `Scalar`, `IntScalar`, `FloatScalar`. Among which, \n\n1. `callable` contains all callable objects including callable classes while `Func` consists all kinds of actual functions. `Function`, however, only refer to explicitly defined functions, and `Method` and `Lambda` refer to the class methods and anonymous functions respectively. These three types are all contained in type `Functional`. \n2. `Real` is a `pyoverload.typehint.Type` while `real`, a list `[int, float]`, is not.\n3. `null` is the type of element `None` while `Null` is the `pyoverload.typehint.Type` form of it. \n4. `sequence` is `[tuple, list, set]`, while `Sequence` is the `pyoverload.typehint.Type` form.\n5. `Array` is the type of package based tensors. Only the tensors of `numpy`, `torch`, `tensorflow` and `batorch` are currently supported. Use `Array.Numpy`, `Array.Torch`, `Array.Tensorflow` and `Array.Batorch` to identify specific packages. \n6. `Iterable` includes `Array`, `Sequence` and `dict`. \n7. Three types of `Scalar`s support the array variables.\n\nAll these types are subclasses of `type` and instances of `pyoverload.typehint.Type` which will be abbreviated as `Type` in the following introduction. \n\nOne can use `Type(int)` to convert a python type like `int` to a `Type` or use `Type(int, float)` to combine multiple existing types. Recurrence is also acceptable, `Type(Type(int, float), Type(str))` is equivalent to `Type(int, float, str)`. It will be better if a keyword `name` is also assigned. \n\nFor a `Type`, `List` for example, we can do the following operations. Except the first four, these usages are designed for iterable types only. \n\n1. `+List`: This indicates that this is an extendable argument, which means it decorates arguments after `*`. It was used to specify `*args` arguments in `@params` but currently deprecated though adding `+` would not lead to failures. \n\n2. `~List`: This invert the typehint, meaning that all non-list types. \n\n3. `List|Tuple`: This is equivalent to `Type(List, Tuple)` indicating list or tuples. \n\n4. `Type(A)&Callable`: The *and* operator. Note that both indicator should be `Type`s. \n\n   ```python\n   >>> from pyoverload import *\n   >>> class A: pass\n   ...\n   >>> class B(A): pass\n   ...\n   >>> class C(A):\n   ...     def __call__(self): pass\n   ...\n   >>> isoftype(B(), Type(A)&Callable)\n   False\n   >>> isoftype(C(), Type(A)&Callable)\n   True\n   ```\n\n5. `List[5]`: This indicates the length or shape of the variable. For other types such as `Int[5]`, this indicates an iterable of length 5 with integer elements. Note that `Array[3, 4]` represents an array with shape `3 x 4`, but this representation is not available for nested lists. Use `List[List[4]][3]` or `List<<List[4]>>[3]` instead.\n\n6. `List@[int, str]`: This only works for ordered sequence `List` and `Tuple`. It indicates that the list has 2 elements, and the first one is an integer while the second is a string. Note that this is **not** equivalent to `List[int, str]` which represents a list with elements either integer or string.\n\n7. `List@int` or `Dict@{str: int}`: For all Iterables, `A@B` indicates type `A` with all elements of type `B`. `Dict@{str:int}` represents a dictionary with string keys and integer values.  \n\n8. `List[int]`: `=List@int`. A list with integer elements. Note that one can use `List[Int|float]` to directly identify a list of elements that are either `int` or `float`. `List[int, float]` and `Dict[str: int, int:str]` are also valid for multiple element types or key-value pairs. Using list in the blankets will return to the effect of `@` operator: `List[[int, float]]=List@[int, float]`. \n\n9. `List<<int>>[10]`: `=(List@int)[10]=List[int][10]` The first one of the two types should be a `Type`. The representation refers to an integer list of length 10 which is equivalent to `List[10]@int`. The length or shape is not specified if a pair of empty blankets is given. Use `List<<Type(int, Float)>>[]` to represent multiple candidates and `Dict<<(str,int)>>[]=Dict[str:int]` to represent a dictionary. \n\n10. `len(List[10, 20])`: Function `len` returns the length of the array. `200` should be the result for the given example. \n\n## Suggestions\n\n1. The speed of type check for `pyoverload.typehint.Type` is not very fast, hence please try your best to use builtin types, types from module `types` or list of types to do the typehint. \n2. The `overload` takes extra time for delivering the arguments, hence using it for functions require fast speed is not recommended. \n3. Do use `@params` for functions not overloaded but needs typehint constraints instead of using `@overload` without actually has multiple implementations. This is because `@params` is way faster. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/pyoverload',
 	author = 'Yuncheng Zhou',
 	author_email = 'bertiezhou@163.com',
 	packages = find_packages(),
 	include_package_data = True,
 	platforms = 'any',
-	install_requires = []
+	install_requires = ['pycamia']
 )
```

