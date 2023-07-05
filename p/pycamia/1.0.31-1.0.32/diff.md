# Comparing `tmp/pycamia-1.0.31.tar.gz` & `tmp/pycamia-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycamia-1.0.31.tar", last modified: Fri Sep  9 13:35:11 2022, max compression
+gzip compressed data, was "pycamia-1.0.32.tar", last modified: Wed Jul  5 06:46:34 2023, max compression
```

## Comparing `pycamia-1.0.31.tar` & `pycamia-1.0.32.tar`

### file list

```diff
@@ -1,26 +1,93 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 13:35:11.717849 pycamia-1.0.31/
--rw-r--r--   0 admin      (501) staff       (20)     8214 2022-09-09 13:35:11.717568 pycamia-1.0.31/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     7041 2022-09-09 13:35:11.000000 pycamia-1.0.31/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 13:35:11.716530 pycamia-1.0.31/pycamia/
--rw-r--r--   0 admin      (501) staff       (20)     1845 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3453 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/decorators.py
--rw-r--r--   0 admin      (501) staff       (20)     9387 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/environment.py
--rw-r--r--   0 admin      (501) staff       (20)     4242 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/exception.py
--rw-r--r--   0 admin      (501) staff       (20)      683 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/functions.py
--rw-r--r--   0 admin      (501) staff       (20)     3814 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/inout.py
--rw-r--r--   0 admin      (501) staff       (20)     7258 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/listop.py
--rw-r--r--   0 admin      (501) staff       (20)     6398 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/logging.py
--rw-r--r--   0 admin      (501) staff       (20)     7135 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/manager.py
--rw-r--r--   0 admin      (501) staff       (20)     5867 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/math.py
--rw-r--r--   0 admin      (501) staff       (20)     1061 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/more.py
--rw-r--r--   0 admin      (501) staff       (20)     1091 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/numpyop.py
--rw-r--r--   0 admin      (501) staff       (20)     9106 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/strop.py
--rw-r--r--   0 admin      (501) staff       (20)    20522 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/system.py
--rw-r--r--   0 admin      (501) staff       (20)     8215 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia/timing.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-09-09 13:35:11.716985 pycamia-1.0.31/pycamia.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     8214 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      426 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2022-09-09 13:35:11.000000 pycamia-1.0.31/pycamia.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-09-09 13:35:11.717901 pycamia-1.0.31/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     7719 2022-09-09 13:35:11.000000 pycamia-1.0.31/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.452977 pycamia-1.0.32/
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 06:46:34.452731 pycamia-1.0.32/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     7041 2023-07-05 06:46:34.000000 pycamia-1.0.32/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.439838 pycamia-1.0.32/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.440875 pycamia-1.0.32/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.444072 pycamia-1.0.32/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.445581 pycamia-1.0.32/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 06:46:33.000000 pycamia-1.0.32/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.447677 pycamia-1.0.32/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2336 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/metrics.py
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 06:46:31.000000 pycamia-1.0.32/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.451195 pycamia-1.0.32/pycamia/
+-rw-r--r--   0 admin      (501) staff       (20)     1944 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3453 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/decorators.py
+-rw-r--r--   0 admin      (501) staff       (20)     9424 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/environment.py
+-rw-r--r--   0 admin      (501) staff       (20)     4260 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)      683 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/functions.py
+-rw-r--r--   0 admin      (501) staff       (20)     3814 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/inout.py
+-rw-r--r--   0 admin      (501) staff       (20)    15299 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/listop.py
+-rw-r--r--   0 admin      (501) staff       (20)     6550 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/logging.py
+-rw-r--r--   0 admin      (501) staff       (20)     7135 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     5867 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/math.py
+-rw-r--r--   0 admin      (501) staff       (20)     1061 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/more.py
+-rw-r--r--   0 admin      (501) staff       (20)     1091 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/numpyop.py
+-rw-r--r--   0 admin      (501) staff       (20)     9791 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/strop.py
+-rw-r--r--   0 admin      (501) staff       (20)    21362 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/system.py
+-rw-r--r--   0 admin      (501) staff       (20)    12327 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia/timing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.451893 pycamia-1.0.32/pycamia.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     2048 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       39 2023-07-05 06:46:34.000000 pycamia-1.0.32/pycamia.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 06:46:34.452477 pycamia-1.0.32/pyoverload/
+-rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 06:46:33.000000 pycamia-1.0.32/pyoverload/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 06:46:33.000000 pycamia-1.0.32/pyoverload/override.py
+-rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 06:46:33.000000 pycamia-1.0.32/pyoverload/typehint.py
+-rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 06:46:33.000000 pycamia-1.0.32/pyoverload/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 06:46:34.453031 pycamia-1.0.32/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     7719 2023-07-05 06:46:34.000000 pycamia-1.0.32/setup.py
```

### Comparing `pycamia-1.0.31/PKG-INFO` & `pycamia-1.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.31
+Version: 1.0.32
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.31/README.md` & `pycamia-1.0.32/README.md`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/__init__.py` & `pycamia-1.0.32/pycamia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,33 @@
 ).check()
 
 from .environment import get_environ_vars, get_environ_globals, get_environ_locals, update_locals_by_environ, get_args_expression, get_declaration, EnvironVars #*
 from .exception import touch, touch_func, crashed, avouch, Error, void #*
 from .functions import empty_function, const_function, identity_function #*
 from .inout import no_out, no_print, SPrint, StrIO #*
 from .manager import info_manager, Hyper, hypers, Version #*
-from .timing import time_this, Timer, Jump, scope, jump, Workflow, periodic, periodic_run, periodic_call #*
+from .timing import time_this, Timer, Jump, scope, jump, Workflow, periodic, periodic_run, periodic_call, run_later #*
 from .decorators import alias, restore_type_wrapper #*
-from .listop import prod, cartesian_prod, argmin, argmax, min_argmin, max_argmax, flatten_list, item, to_list, to_tuple, to_set, map_ele, sublist, arg_tuple, count, unique #*
-from .strop import is_digits, is_alphas, is_snakename, get_digits, get_alphas, get_snakename, get_snakenames, str_len, str_slice, find_all, sorted_dict_repr, enclosed_object, tokenize, dict_parse, no_indent #*
-from .system import path, Path, path_list, PathList, set_black_list, get_black_list, curdir, pardir, homedir, rootdir, pwd, ls, cp, copy, is_valid_command, Shell, execblock, ByteSize #*
+from .listop import prod, cartesian_prod, argmin, argmax, min_argmin, max_argmax, kth_biggest, kth_smallest, median, flatten_list, item, to_list, to_tuple, to_set, map_ele, sublist, arg_tuple, arg_extract, count, unique, iterate #*
+from .strop import is_digits, is_alphas, is_snakename, get_digits, get_alphas, get_snakename, get_snakenames, str_len, str_slice, find_all, sorted_dict_repr, enclosed_object, tokenize, dict_parse, no_indent, columns #*
+from .system import path, Path, path_list, PathList, set_black_list, get_black_list, curdir, pardir, homedir, rootdir, pwd, ls, cp, copy, mv, move, rename, is_valid_command, Shell, execblock, ByteSize #*
 from .logging import logging, start_logging #*
 from .math import GCD, isint, rational #*
 from . import system as pth
 
 
 
 
 
 
 
+
+
+
+
```

### Comparing `pycamia-1.0.31/pycamia/decorators.py` & `pycamia-1.0.32/pycamia/decorators.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/environment.py` & `pycamia-1.0.32/pycamia/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     update_locals_by_environ
     get_args_expression
     get_declaration
     EnvironVars
 """.split()
 
 import os, sys
+from .strop import tokenize
 
 try:
     import ctypes
 except ModuleNotFoundError:
     ctypes = None
 else:
     if hasattr(ctypes, "pythonapi") and \
@@ -175,16 +176,16 @@
         with open(client_frame.f_code.co_filename) as fp:
             for _ in range(client_frame.f_lineno-1): fp.readline()
             l = fp.readline()
             if func_name not in l:
                 raise TypeError(f"Cannot find function name `{func_name}` in {client_frame.f_code.co_filename} line {client_frame.f_lineno}:\n\t{l}" +
                     "Problem occurs in code stack, please contact the developer for further information (Error Code: E002). ")
             exp = l.split(func_name)[-1].split(';')[0].strip()
-            if exp.startswith('('): exp = exp[1:]
-            if exp.endswith(')'): exp = exp[:-1]
+            if not exp.startswith('('): exp = f"({exp})"
+            exp = tokenize(exp, sep=['(', ')'])[1]
             return exp
     else: return "<unreachable arg expression>"
 
 def get_declaration(func, func_name = None):
     func_code = func.__code__
     if func_name is None: func_name = func.__name__
     if os.path.exists(func_code.co_filename):
```

### Comparing `pycamia-1.0.31/pycamia/exception.py` & `pycamia-1.0.32/pycamia/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     avouch
     Error
     void
 """.split()
 
 from .environment import get_args_expression, get_environ_vars, update_locals_by_environ
 from .functions import const_function
-from .strop import is_snakename
+from .strop import is_snakename, tokenize
 
 def touch(v, default=None, error_type=Exception):
     """
     Touch a function or an expression `v`, see if it causes exception in `error_type`. 
     If not, output the result, otherwise, output `default`. 
     
     Params:
@@ -86,15 +86,15 @@
     
     Inputs:
         v[bool]: the expression to be validated.
         txt[str]: the assertion message when the test fails.
     """
     if not v:
         if not txt:
-            expr = get_args_expression().split(',')[0].strip()
+            expr = tokenize(get_args_expression(), sep=',')[0].strip()
             if (expr is not None):
                 txt = f"Failure in assertion '{expr}'"
         txt = ' '.join(txt.split())
         raise AssertionError(txt)
 
 def crashed(func):
     """
```

### Comparing `pycamia-1.0.31/pycamia/functions.py` & `pycamia-1.0.32/pycamia/functions.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/inout.py` & `pycamia-1.0.32/pycamia/inout.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/logging.py` & `pycamia-1.0.32/pycamia/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         self.file_path = log_path
         self.file_dir = log_dir
         self.vars = _vars
         self.fp = None
         self.is_fplinestart = True
         self.exc_remove = exc_remove
         self.line_width = line_width
+        self.start_time = datetime.now()
 
     def __enter__(self):
         if self.file_path is not None and not self.file_path: return
         if self.file_dir is not None and not self.file_dir: return
         if self.vars is None: self.vars = get_environ_vars()
         vars = self.vars
         if self.file_path is None:
@@ -122,19 +123,20 @@
             exc_string = "Traceback (most recent call last): \n"
             for item in tb.StackSummary.from_list(tb.extract_tb(traceback)).format(): exc_string += str(item)
             exc_string += exc_type.__name__ + ': ' + str(exc_value) + '\n'
             self.fp_print(exc_string)
             self.fp.close()
             if self.exc_remove:
                 log_file = Path(self.file_path)
-                log_file.remove()
+                if "KeyboardInterrupt: " in exc_string: log_file.rename(log_file^"interrupted")
+                else: log_file.remove()
                 er_file = log_file.with_name("error_msgs")
                 if er_file.exists(): mode = 'a'
                 else: mode = 'w'
-                with er_file.open(mode) as fp: fp.write(('\n' if mode == 'a' else '') + '[' + str(datetime.now()) + ']: ' + exc_string)
+                with er_file.open(mode) as fp: fp.write(('\n' if mode == 'a' else '') + f"[{self.start_time} - {datetime.now()}]: {exc_string}")
         self.fp = None
         builtins.print = builtin_print
         
     def print(self, *values, sep=' ', end='\n', **kwargs):
         builtin_print(self.fp_print(*values, sep=sep, end=end, **kwargs), end='')
 
     def fp_print(self, *values, sep=' ', end='\n', **kwargs):
```

### Comparing `pycamia-1.0.31/pycamia/manager.py` & `pycamia-1.0.32/pycamia/manager.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/math.py` & `pycamia-1.0.32/pycamia/math.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/more.py` & `pycamia-1.0.32/pycamia/more.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/numpyop.py` & `pycamia-1.0.32/pycamia/numpyop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.31/pycamia/strop.py` & `pycamia-1.0.32/pycamia/strop.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     str_slice
     find_all
     sorted_dict_repr
     enclosed_object
     tokenize
     dict_parse
     no_indent
+    columns
 """.split()
 
-import re
-from .environment import get_environ_vars
+import re, math
 
 def is_digits(str_:str):
     """
     Return whether `str_` characters are all digits. 
     
     Example:
     ----------
@@ -90,16 +90,24 @@
     
     Example:
     ----------
     >>> print(repr(get_snakename("abc2_x")), repr(get_snakename("1bc")), repr(get_snakename("x_ y:")))
     'abc2_x' 'bc' 'x_y'
     """
     past_prefix = False
-    def past(): get_environ_vars()['past_prefix'] = True
-    return ''.join(x for x in str(str_) if ((65 <= ord(x) <= 90 or 97 <= ord(x) <= 122) and past() is None) or (48 <= ord(x) <= 57 or ord(x) == 95) and past_prefix)
+    result = ""
+    for x in str(str_):
+        if (65 <= ord(x) <= 90 or 97 <= ord(x) <= 122):
+            result += x
+            past_prefix = True
+        elif (48 <= ord(x) <= 57 or ord(x) == 95) and past_prefix:
+            result += x
+        else:
+            continue
+    return result
 
 def get_snakenames(str_:str):
     """
     Return all alphabets/digits/underlines (snakename) words in `str_`. 
     
     Example:
     ----------
@@ -286,7 +294,25 @@
     lines = str(str_).split('\n')
     for l in lines:
         indent = re.search(r'^([ \t]*)[^ \t]', l)
         if indent is None: continue
         n_indent = len(indent.group(1))
         if min_indent is None or n_indent < min_indent: min_indent = n_indent
     return '\n'.join([l[min_indent:] for l in lines])
+
+def columns(*strs, line_width = 100):
+    strs = list(strs)
+    n = len(strs)
+    col_width = line_width // n
+    lines = []
+    for s in strs:
+        column = []
+        for l in str(s).split('\n'):
+            if len(l) > col_width:
+                for p in range(math.ceil(len(l) / col_width)):
+                    column.append(l[p*col_width:(p+1)*col_width])
+            else: column.append(l)
+        lines.append(column)
+    output = ""
+    for i in range(max(len(c) for c in lines)):
+        output += '|'.join((c[i] + ' ' * (col_width - len(c[i]))) if i < len(c) else ' ' * col_width for c in lines) + '\n'
+    return output
```

### Comparing `pycamia-1.0.31/pycamia/system.py` & `pycamia-1.0.32/pycamia/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     path_list PathList
     set_black_list
     get_black_list
     curdir
     pardir
     homedir
     rootdir
-    pwd ls cp copy
+    pwd ls
+    cp copy
+    mv move
+    rename
     is_valid_command
     Shell
     execblock
     ByteSize
 """.split()
 
 import os, re, math
@@ -379,14 +382,15 @@
     
     @alias("delete", "del", "rm")
     def remove(self, verbose=True):
         if self.is_dir():
             if verbose and self.ls():
                 print(f"You want to delete directory: {self}")
                 if 'y' not in input("Do you want to continue? [Y/n]: ").lower(): return
+            for f in self: f.remove(verbose=verbose)
             os.rmdir(self._abs)
         else: os.remove(self._abs)
         
     def rename(self, new_name):
         old_wd = os.path.abspath(os.curdir)
         os.chdir(self.parent._abs)
         os.rename(self.filename, (new_name - self.parent) if isinstance(new_name, Path) else new_name)
@@ -398,14 +402,20 @@
             cmd = command.format(self, file=self, path=self)
             old_wd = os.path.abspath(os.curdir)
             os.chdir(self.ref)
             os.system(cmd)
             os.chdir(old_wd)
         except Exception as e:
             print(f"Command error in {cmd}:", e)
+            
+    def move_to(self, path):
+        move(self, path)
+
+    def copy_to(self, path):
+        copy(self, path)
 
     def open(self, mode='r+'):
         if 'w' not in mode and not self.exists(): raise FileNotFoundError(f"Cannot find file {self._abs}. ")
         elif not self.parent.exists(): raise FileNotFoundError(f"Cannot find file folder {self.parent._abs}. ")
         avouch(self.is_file() or self.is_filepath() and 'w' in mode, "Only files can be opened as python stream. ")
         return open(self._abs, mode)
 
@@ -463,14 +473,35 @@
     avouch(isinstance(dst, str))
     src = Path(src)
     dst = Path(dst)
     src = Path(src, ref=src.parent)
     dst = dst - src.parent
     opt = '-r' if src.is_dir() else ''
     src.command(f"cp {opt} {{path}} {dst}")
+
+@alias('mv')
+def move(src, dst):
+    avouch(isinstance(src, str))
+    avouch(isinstance(dst, str))
+    src = Path(src)
+    dst = Path(dst)
+    src = Path(src, ref=src.parent)
+    dst = dst - src.parent
+    src.command(f"mv {{path}} {dst}")
+    
+def rename(src, dst):
+    avouch(isinstance(src, str))
+    avouch(isinstance(dst, str))
+    src = Path(src)
+    dst = Path(dst)
+    src = Path(src, ref=src.parent)
+    if dst.parent == curdir:
+        dst = dst.filename
+    else: dst = dst - src.parent
+    src.command(f"mv {{path}} {dst}")
     
 def is_valid_command(cmd, error_name='command not found'):
     p = Popen(cmd, shell=True, stdout=PIPE, stderr=PIPE)
     try: stdout, stderr = p.communicate(timeout=0.05)
     except: stderr = b''
     return bytes(error_name, 'utf8') not in stderr
     
@@ -547,15 +578,17 @@
     ...
     >>> A().additional_method(3)
     25
     """
     code = no_indent(code)
     vars = get_environ_vars()
     loc_vars = {}
-    exec(code, vars.globals, loc_vars)
+    try: exec(code, vars.globals, loc_vars)
+    except Exception as e:
+        raise NameError(f"Error ({e}) in block execution: \n{code}")
     vars.update(loc_vars)
 
 ByteSize_class = {}
 def ByteSize(x):
     T = type(x)
     if T in ByteSize_class: return ByteSize_class[T](x)
     class ByteSizeClass(T):
```

### Comparing `pycamia-1.0.31/pycamia/timing.py` & `pycamia-1.0.32/pyoverload/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,274 +1,237 @@
 
-from .manager import info_manager
+from pycamia import info_manager
 
 __info__ = info_manager(
-    project = "PyCAMIA",
-    package = "<main>",
-    author = "Yuncheng Zhou",
-    create = "2021-12",
-    fileinfo = "File to record time."
+    project = "PyZMyc",
+    package = "pyoverload",
+    fileinfo = "Useful tools for decorators."
 )
 
 __all__ = """
-    time_this
-    Timer
-    Jump
-    scope
-    jump
-    Workflow
-    periodic
-    periodic_run
-    periodic_call
+    raw_function
+    return_type_wrapper
+    decorator
 """.split()
 
-import time
+import os, sys
 from functools import wraps
-from threading import Timer as tTimer
 
-from .environment import get_environ_vars
+try:
+    import ctypes
+except ModuleNotFoundError:
+    ctypes = None
+else:
+    if hasattr(ctypes, "pythonapi") and \
+       hasattr(ctypes.pythonapi, "PyFrame_LocalsToFast"): pass
+    else: ctypes = None
+
+def raw_function(func):
+    if hasattr(func, "__func__"):
+        return func.__func__
+    return func
+
+def _get_wrapped(f):
+    while hasattr(f, '__wrapped__'): f = f.__wrapped__
+    return f
 
-def time_this(func):
-    """
-    A function wrapper of function `func` that outputs the time used to run it. 
-
-    Example:
-    ----------
-    @timethis
-    >>> def func_to_run(*args):
-    ...     # inside codes
-    ... 
-    >>> func_to_run(*input_args)
-    # some outputs
-    [func_to_run takes 0.001s]
-    """
-    @wraps(func)
+def decorator(wrapper_func):
+    if not callable(wrapper_func): raise TypeError("@decorator wrapping a non-wrapper")
     def wrapper(*args, **kwargs):
-        start = time.time()
-        result = func(*args, **kwargs)
-        end = time.time()
-        if hasattr(getattr(func, '__wrapped__', func), '__name__'):
-            print("[%s takes %lfs]"%(func.__name__, end-start))
+        if not kwargs and len(args) == 1:
+            func = args[0]
+            raw_func = raw_function(func)
+            if callable(raw_func):
+                func_name = f"{raw_func.__name__}[{wrapper_func.__qualname__.split('.')[0]}]"
+                wrapped_func = wraps(raw_func)(wrapper_func(raw_func))
+                wrapped_func.__name__ = func_name
+                wrapped_func.__doc__ = raw_func.__doc__
+                # return wrapped_func
+                if 'staticmethod' in str(type(func)): trans = staticmethod
+                elif 'classmethod' in str(type(func)): trans = classmethod
+                else: trans = lambda x: x
+                return trans(wrapped_func)
+        return decorator(wrapper_func(*args, **kwargs))
+    return wraps(wrapper_func)(wrapper)
+
+def _mid(x): return x[1] if len(x) > 1 else x[0]
+def _rawname(s): return _mid(str(s).split("'"))
+
+stack_error = lambda x, ext: TypeError(f"Unexpected function stack for {x}, please contact the developer for further information (Error Code: E001*). {ext}")
+
+# def _get_frames():
+#     frames = []
+#     frame = sys._getframe()
+#     fname = frame.f_back.f_code.co_name
+#     while frame is not None:
+#         frame_file = _rawname(frame)
+#         if frame_file.startswith('<') and frame_file.endswith('>') and frame_file != '<stdin>':
+#             frame = frame.f_back
+#             continue
+#         frames.append(frame)
+#         if len(frames) >= 4: return frames[2:]
+#         frame = frame.f_back
+#     raise stack_error(fname)
+
+# def get_environ_locals():
+#     _, client_frame = _get_frames()
+#     return client_frame.f_locals
+
+# def get_environ_globals():
+#     _, client_frame = _get_frames()
+#     return client_frame.f_globals
+
+def _get_frames(i = [2, 3], key=''):
+    """
+    Get frames in stack. 
+    By default: it gets frame of the function calling get_environ (function frame) and the frame calling this function (client frame). 
+    Returns: function frame, client frame
+    """
+    frames = []
+    frame = sys._getframe()
+    fname = frame.f_back
+    if isinstance(i, int): i = [i]
+    if i is not None:
+        if len(i) == 0: raise IndexError("Invalid index for _get_frames")
+        max_i = max(i)
+    while frame is not None:
+        frame_file = frame.f_code.co_filename
+        if frame_file.startswith('<') and frame_file.endswith('>') and frame_file != '<stdin>':
+            frame = frame.f_back
+            continue
+        if i is None:
+            if frame.f_code.co_name == key: frames.append(frame)
         else:
-            print("[%s takes %lfs]"%(func.__class__.__name__, end-start))
-        return result
-    return wrapper
-
-class Timer(object):
-    """
-    An environment that outputs the time used to run codes within. 
+            frames.append(frame)
+            if len(frames) >= max_i + 1:
+                domain = [frames[j] for j in i]
+                if key != '': domain = [f for f in domain if f.f_code.co_name == key]
+                return domain if len(domain) > 1 else domain[0]
+        frame = frame.f_back
+    if i is not None or len(frames) == 0:
+        try: f_all = _get_frames(-1)
+        except: raise stack_error(fname, f"\n_get_frames({i}) got stack: \n" + '\n'.join(map(str, frames)))
+        raise stack_error(fname, "\nComplete stack: \n" + '\n'.join(map(str, f_all)) + f"\n_get_frames({i}) got stack: \n" + '\n'.join(map(str, frames)))
+    return frames
 
-    Example:
-    ----------
-    >>> with Timer("test"):
-    ...     # inside codes
-    ... 
-    # some outputs
-    [test takes 0.001s]
-    """
-    def __init__(self, name='', timing=True):
-        if not timing: name = ''
-        self.name = name
-        self.nround = 0
-        self.prevrecord = None
-    @property
-    def recorded_time(self): return self.prevrecord
-    def __enter__(self):
-        self.start = time.time()
-        self.prevtime = self.start
-        return self
-    def round(self, name = ''):
-        self.nround += 1
-        self.end = time.time()
-        if self.name:
-            if not name: name = "%s(round%d)"%(self.name, self.nround)
-            self.prevrecord = self.end - self.prevtime
-            print(f"[{name} takes {self.prevrecord}s]")
-        self.prevtime = self.end
-    def exit(self): raise RuntimeError("JUMP")
-    def __exit__(self, exc_type, exc_value, traceback):
-        if exc_type == RuntimeError and str(exc_value) == "JUMP": return True
-        if self.name:
-            self.prevrecord = time.time() - self.start
-            print(f"[{self.name}{'' if self.nround == 0 else '(all)'} takes {self.prevrecord}s]")
-
-class Jump(object):
-    """
-    Creates a Jump RuntimeError, designed for instance `jump`. 
-    """
-    def __init__(self, jump=None): self.jump = True if jump is None else jump
-    def __enter__(self):
-        def dojump(): raise RuntimeError("JUMP")
-        if self.jump: dojump()
-        else: return dojump
-    def __exit__(self, *args): pass
-    def __call__(self, condition): return Jump(condition)
-    
-def scope(name, timing=True):
-    """
-    An allias of timer to better organize the codes. 
+class EnvironVars():
     
-    Inputs:
-        name (str): the name of the scope, used to display. 
-        timing (bool): whether to show the time span or not. 
-
-    Example:
-    ----------
-    >>> with scope("test"):
-    ...     # inside codes
-    ... 
-    # some outputs
-    [scope test takes 0.001s]
-    """
-    return Timer("scope " + str(name), timing)
+    def __init__(self, frame): self.frame = frame
 
-jump = Jump()
-"""
-The jumper, one can use it along with `scope`(or `Timer`) to jump a chunk of codes. 
-
-Example:
-----------
->>> with scope("test"), jump:
-...     # inside codes
-... 
-# nothing, the inside codes do not run
->>> with scope("test"), jump as stop:
-...     print('a')
-...     stop()
-...     print('b')
-... 
-a
-"""
-
-class Workflow:
-    """
-    A structure to create a series of workflow. 
+    def get(self, name, default=None):
+        res = self.frame.f_locals.get(name, self.frame.f_globals.get(name, default))
+        if res is None: raise AttributeError(f"No variable {name} found in the environment. ")
+        return res
+
+    def set(self, name, value, in_dict=None):
+        if not in_dict: in_dict = 'local'
+        if in_dict.lower().startswith('loc'): self.frame.f_locals[name] = value
+        else: self.frame.f_globals[name] = value
+        if ctypes is not None:
+            ctypes.pythonapi.PyFrame_LocalsToFast(ctypes.py_object(self.frame), ctypes.c_int(0))
     
-    Note:
-        Remember to manually add `, {workflow_name}.jump` after `with` so that 
-        we can control it. See the example. 
+    def update(self, dic, in_dict=None):
+        for k, v in dic.items():
+            if not in_dict: in_dict = 'local'
+            if in_dict.lower().startswith('loc'): self.frame.f_locals[k] = v
+            else: self.frame.f_globals[k] = v
+        if ctypes is not None:
+            ctypes.pythonapi.PyFrame_LocalsToFast(ctypes.py_object(self.frame), ctypes.c_int(0))
+        
+    def __contains__(self, key): return key in self.frame.f_locals or key in self.frame.f_globals
+    def __getitem__(self, key): return self.get(key)
+    def __setitem__(self, key, value): return self.set(key, value)
+    def __getattr__(self, key):
+        if key in self.__dict__: return super().__getattr__(key)
+        return self.get(key)
+    def __setattr__(self, key, value):
+        if key == 'frame': return super().__setattr__(key, value)
+        return self.set(key, value)
     
-    Args:
-        *args: the list of scope names to run. 
-
-    Example:
-    ----------
-    >>> run = Workflow("read data", "run method", "visualization")
-    ... with run("read data"), run.jump:
-    ...     print(1, end='')
-    ... with run("pre-processing"), run.jump:
-    ...     print(2, end='')
-    ... with run("run method"), run.jump:
-    ...     print(3, end='')
-    ... with run("visualization"), run.jump:
-    ...     print(4, end='')
-    ... 
-    1[read data takes 0.000022s]
-    3[run method takes 0.000008s]
-    4[visualization takes 0.000006s]
-    """
-    def __init__(self, *args, verbose=True): self.workflow = args; self.verbose=verbose
-    def __call__(self, *keys):
-        if len(keys) == 1 and isinstance(keys[0], (list, tuple)): keys = keys[0]
-        self.keys=keys
-        return Timer(','.join(keys), timing=self.verbose)
-    def __getattr__(self, *k): return self(*k)
-    def __getitem__(self, *k): return self(*k)
     @property
-    def j(self): return self.jump
-    @property
-    def jump(self):
-        if len(self.keys) > 1: raise TypeError("Trying to use workflow.jump for section with multiple keys, please use 'jump_or' or 'jump_and' instead. ")
-        return Jump(self.keys[0] not in self.workflow)
+    def locals(self): return self.frame.f_locals
+    
     @property
-    def jump_and(self): return Jump(any(k not in self.workflow for k in self.keys))
+    def globals(self): return self.frame.f_globals
+    
     @property
-    def jump_or(self): return Jump(all(k not in self.workflow for k in self.keys))
-
-class TimerCtrl(tTimer):
-    """
-    Creates a Time Handler, designed for function `periodic`. 
-    """
-
-    def __init__(self, seconds, function):
-        tTimer.__init__(self, seconds, function)
-        self.isCanceled = False
-        self.seconds = seconds
-        self.function = function
-        self.funcname = function.__name__
-        self.startTime = time.time()
-
-    def cancel(self):
-        tTimer.cancel(self)
-        self.isCanceled = True
-
-    def is_canceled(self): return self.isCanceled
-
-    def setFunctionName(self, funcname): self.funcname = funcname
-
+    def all(self):
+        all = self.frame.f_globals.copy()
+        all.update(self.frame.f_locals)
+        return all
+    
+def get_environ_vars(offset=0, pivot=''):
+    client_frame = _get_frames(3) # offset of frame
+    if pivot: client_frame = _get_frames(None, key=pivot)
+    if isinstance(client_frame, list): client_frame = client_frame[-1]
+    for _ in range(offset):
+        client_frame = client_frame.f_back
+    return EnvironVars(client_frame)
+
+def update_locals_by_environ():
+    module_frame, client_frame = _get_frames()
+    vars_set = client_frame.f_locals.copy()
+    vars_set.update(module_frame.f_locals)
+    module_frame.f_locals.update(vars_set)
+
+class StrIO:
+    def __init__(self, file_name = os.path.abspath('.null')):
+        self._str_ = None
+        self._file_ = open(file_name, 'w+')
+        self.file_name = file_name
+        self.fileno = self._file_.fileno
+    def write(self, s): self._file_.write(s)
     def __str__(self):
-        return "%5.3fs to run next "%(self.seconds + self.startTime -
-                                      time.time()) + self.funcname
-
-class STOP:
-    def __init__(self): self.stopped = False; self.index = 0
-    def __bool__(self): return self.stopped
-    def set_index(self, index): self.index = index
-    def stop(self): self.stopped = True
-    def resume(self): self.stopped = False
-
-def periodic(period, maxiter=float('Inf'), wait_return=False):
-    """
-    A function wrapper to repeatedly run the wrapped function `period`.
-    The return of function being False means the periodic process should stop.
+        if self._str_ is not None: return self._str_
+        self._file_.seek(0)
+        self._str_ = self._file_.read()
+        self.close()
+        return self._str_
+    def split(self, c=None): return str(self).split(c)
+    def string(self): return str(self)
+    def close(self):
+        self._file_.close()
+        if self.file_name == os.path.abspath('.null'):
+            os.remove(self.file_name)
+            self._file_ = None
     
-    Args:
-        maxiter (int): the number of iterations. 
-        wait_return (bool): If True, the next iteration starts when the current is over, the gap is period.
-            If False, the next iteration starts right after 'period' seconds.
-        Note: if wait_return is False, function should accept a timer controler timer as the first argument just like 'self'.
-
-    Example:
-    ----------
-    >>> i = 1
-    ... @periodic(1)
-    ... def func(timer):
-    ...     print(i)
-    ...     i+= 1
-    ...     timer.stop()
-    ...     timer.resume()
-    ... 
-    1
-    2
-    3
-    [Output every 1s, and GO ON...]
-    """
-    def wrap(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            global count, stopped
-            if 'count' not in globals(): count = 1
-            if 'stopped' not in globals(): stopped = STOP()
-            if stopped: return
-            timer_ctrl = TimerCtrl(period, lambda : wrapper(*args, **kwargs))
-            timer_ctrl.setFunctionName(func.__name__)
-            if not wait_return:
-                timer_ctrl.start()
-                stopped.set_index(count)
-                ret = func(stopped, *args, **kwargs)
-                count += 1
-                if count >= maxiter: return ret
-                return ret
-            else:
-                ret = func(*args, **kwargs)
-                count += 1
-                if count >= maxiter: return
-                if ret == False: return
-                timer_ctrl.start()
-        return wrapper
-    return wrap
-
-def periodic_run(period, maxiter=float('Inf')):
-    return periodic(period, maxiter=maxiter, wait_return=True)
-
-def periodic_call(period, maxiter=float('Inf')):
-    return periodic(period, maxiter=maxiter, wait_return=False)
+def get_args_expression():
+    module_frame, client_frame = _get_frames()
+    func_name = module_frame.f_code.co_name
+    if os.path.exists(client_frame.f_code.co_filename):
+        with open(client_frame.f_code.co_filename) as fp:
+            for _ in range(client_frame.f_lineno-1): fp.readline()
+            l = fp.readline()
+            if func_name not in l:
+                raise TypeError(f"Cannot find function name `{func_name}` in {client_frame.f_code.co_filename} line {client_frame.f_lineno}:\n\t{l}. \n" +
+                    "Problem occurs in code stack, please contact the developer for further information (Error Code: E002*). ")
+            exp = l.split(func_name)[-1].split(';')[0].strip()
+            if exp.startswith('('): exp = exp[1:]
+            if exp.endswith(')'): exp = exp[:-1]
+            return exp
+    else: return "<unreachable arg expression>"
+
+def get_declaration(func):
+    func_code = func.__code__
+    func_name = func.__name__
+    if os.path.exists(func_code.co_filename):
+        with open(func_code.co_filename) as fp:
+            for _ in range(func_code.co_firstlineno - 1): fp.readline()
+            i = func_code.co_firstlineno
+            while True:
+                l = fp.readline()
+                if func_name not in l:
+                    if not l.strip() or l.strip().startswith('@') or l.strip().startswith('#'): i += 1; continue
+                    raise TypeError(f"Cannot find function name `{func_name}` in {func_code.co_filename} line {i}:\n\t{l}. \n" +
+                        "Problem occurs in code stack, please contact the developer for further information (Error Code: E003*). ")
+                dec_line = l
+                break
+    else:
+        ss = StrIO()
+        oldout = sys.stdout
+        sys.stdout = ss
+        help(func)
+        sys.stdout = oldout
+        dec_line = [l for l in ss.split('\n') if len(l) > 0 and 'Help' not in l][0]
+    if not dec_line: return "<unreachable declaration>"
+    dec = dec_line.strip().split(' ', 1)[-1].rstrip(':')
+    return dec
```

### Comparing `pycamia-1.0.31/pycamia.egg-info/PKG-INFO` & `pycamia-1.0.32/pycamia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.31
+Version: 1.0.32
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.31/setup.py` & `pycamia-1.0.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'pycamia',
-	version = '1.0.31',
+	version = '1.0.32',
 	keywords = ['pip', 'pymyc', 'pycamia', 'environment', 'path', 'touch'],
 	description = 'The main package and a background support of project PyCAMIA. ',
 	long_description = '# pycamia\n\n## Introduction\n\n[`pycamia`](https://github.com/Bertie97/pycamia/tree/main/pycamia) is the base package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a collection of different useful tools necessary in python programming. `pycamia` was designed for `python v3.6+`. It is consist of the following sub-packages. \n\n1. **environment** is a package containing functions to inspect the context. e.g. get the local variables in the context that calls a function. \n2. **strop** is a collection of advanced functions for strings. e.g. tokenize a string by spliting outside brackets OR find all indices for matched sub-strings.\n3. **listop** is a collection of advanced functions for lists. e.g. flatten a nested list.\n4. **manager** is a package to manage file and package infos. e.g. easily check the dependencies OR easy update the version. \n5. **functions** is a package of special (and commonly trivial) functions. e.g. empty functions. \n6. **exceptions** is a package to handle exceptions. e.g. touch a function and suppress the error OR assert with comment OR quickly create an Error.\n7. **inout** is a package to extend the input/output. e.g. printing to a string OR suppressing the console output. \n8. **timing** is a package to time the executions. e.g. use `with` structure to record time spent for a set of commands. \n9. **more** is a collection of uncategorized functions, one need to import them from `pycamia.more`.\n\n## Installation\n\nThis package can be installed by `pip install pycamia` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pycamia\n```\n\n## Package `environment`\n\nThis package fetches the surrounding environment of the call. It is likely that no more functions would be added to it. If there\'s any suggestion, please contact the developer. \n1. Use `v = get_environ_locals()` or `v = get_environ_globals()` to get the dictionary of local or global variables in the parent environment. If the result is out of expectations, please contact the developer. \n2. Use `v[\'name\']` to read variable `name` and `v[\'name\'] = value` to add variable to the environment. \n\n## Package `strop`\n\nThis package cope with str objects. \n1. Use `str_len` to find the ASCII length for a string, with a length `2` for wide characters.\n2. Use `str_slice` to slice a string by given indices.\n3. Use `find_all` to obtain all the indices of a given string. `str_slice(s, find_all(s, k))` is equivalent to `s.split(k)`. \n4. Use `sorted_dict_repr` to create a repr string for a dictionary with ordered key.\n5. Use `enclosed_object` to find the first object enclosed by brackets. \n6. Use `tokenize` to split a string without breaking enclosed objects. This is useful in breaking text of dictionary structures or arguments. e.g. one can use `tokenize(args, sep=[\',\', \'=\'])[::2]` to find the argument names if `args` is a string in the format `key1=value1, key2 = value2, ...`.\n\n## Package `listop`\n\nThis package cope with list objects. More useful functions will be added to it in the future. \n1. Use `argmin(list, domain)` to find the indices for the minimal value in list. The function only search in the indices `domain`. A list is output as there may be multiple entries. \n2. Use `argmax` to find the indices for the maximal value, similar to `argmin`. \n3. Use `flatten_list` to unwrap the list elements to create a list with no element in type `list`. \n4. Use `prod` to obtain the product of all numbers in the list. \n5. Use `item` to fetch the only element in the list. An error will be raised if there isn\'t any or are more than 1 elements. \n\n## Package `manager`\n\nThis package manages the info of packages and files. One can use it to organize the project. \n1. Use `__info__ = info_manager(project="PyCAMIA", ...)` to list the properties at the front of files. This serve as a brief introduction to readers.\n2. Use `info_manager` at the beginning of `__init__.py`, `pack.py` uses it to create the portrait of a package. \n3. Use `__info__.check_requires()` to automatically check if the dependencies in attribute `requires` exist or not. This is commonly used in `__init__.py`. One can use `__info__ = info_manager(...).check()` to perform an in-place check.\n4. Use `with __info__:` before importing required dependencies as well to perform a double check. \n\n## Package `functions`\n\nThis package contains simple functions. It is the simplest package in the project so far. \n1. Use `empty_function` for a function that does nothing. One can put any argument to the function but nothing would happen. \n2. Use `const_function(a)` for a function that accepts any argument but does nothing and always return `a`.\n\n## Package `exceptions`\n\nThis package handles exceptions. \n1. Use `touch(function)` to try a function and suppress the error in the mean time. e.g. `touch(lambda: 1/a)` returns `None` to tell you that an exception occurs when `a=0`, but returns `1` when `a=1`. \n2. Use `crashed(function)` to check whether a function fails or not. \n3. Use `avouch(bool_to_be_tested, assertion_text)` to avouch that the given expression is true and output your designed `assertion_text` when the test fails. \n4. Use `Error("name")` to creat a new error type. It is the same as creating an Error tag by `class nameError(Exception): pass`.\n\n## Package `inout`\n\nThis package manipulates the input/output. Currently, it only deal with print. Shell handler or other inout functions will be added here in the future. \n1. Use `with no_print:` to suppress the console output. Although not recommended, one can use `with no_print as out_stream:` and `output = str(out_stream)` inside the `with` structure to fetch the output. \n2. Use `sprint = SPrint()` to create a function `sprint` that collects the printed text. Use `out = sprint()` or `sprint.text` to get the results.\n\n## Package `timing`\n\nThis package use the time spent of commands to perform useful inspection or organization of the codes.\n1. Use `@time_this` to time a function.\n2. Use `with Timer("name"):` to time a series of commands.\n3. Use `with scope("name"):` to nest a series of commands. It is an alias of `Timer`. \n4. Use `with scope("name"), jump:` to jump a series of commands. \n5. Use `with scope("name"), Jump(False):` to disable the jump.\n6. Use `wf = Workflow("step1", "step2")` and `with wf("step1(2)"), wf.jump:` before commands of "step1(2)" to create a workflow. One can change the arguments in the init function to decide which steps to run. \n7. Use `@periodic(seconds, max_repeat)` to run a function repeatedly. \n\n## Package `more`\n\nCurrently, only `once` is contained in the `more` package. \nAdding it in a function to check if the function is run once or not. \n\n## Waiting to Be Imroved\n\n1. More functions will be added in the future, including path handler, tools for shell and so on. \n2. Contact us to make suggestions. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/pycamia',
 	author = 'Yuncheng Zhou',
```

