# Comparing `tmp/tfswin-3.3.3.tar.gz` & `tmp/tfswin-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfswin-3.3.3.tar", last modified: Mon Feb 13 14:50:45 2023, max compression
+gzip compressed data, was "tfswin-3.4.0.tar", last modified: Wed Jul  5 21:15:00 2023, max compression
```

## Comparing `tfswin-3.3.3.tar` & `tfswin-3.4.0.tar`

### file list

```diff
@@ -1,39 +1,28 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-13 14:50:45.984104 tfswin-3.3.3/
--rw-r--r--   0 alex       (501) staff       (20)     1070 2021-01-02 15:55:39.000000 tfswin-3.3.3/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       33 2021-11-19 08:13:39.000000 tfswin-3.3.3/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     8571 2023-02-13 14:50:45.984452 tfswin-3.3.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     6431 2023-01-17 08:02:26.000000 tfswin-3.3.3/README.md
--rw-r--r--   0 alex       (501) staff       (20)       47 2022-12-11 13:14:49.000000 tfswin-3.3.3/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)       91 2023-02-13 14:50:45.985254 tfswin-3.3.3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1205 2023-02-13 14:50:21.000000 tfswin-3.3.3/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-13 14:50:45.969859 tfswin-3.3.3/tfswin/
--rw-r--r--   0 alex       (501) staff       (20)      532 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1633 2022-12-11 13:14:49.000000 tfswin-3.3.3/tfswin/ape.py
--rw-r--r--   0 alex       (501) staff       (20)     5305 2023-02-13 14:50:21.000000 tfswin-3.3.3/tfswin/basic.py
--rw-r--r--   0 alex       (501) staff       (20)     1505 2022-12-11 13:14:49.000000 tfswin-3.3.3/tfswin/drop.py
--rw-r--r--   0 alex       (501) staff       (20)     1508 2023-01-31 10:49:15.000000 tfswin-3.3.3/tfswin/embed.py
--rw-r--r--   0 alex       (501) staff       (20)     2614 2022-12-11 13:14:49.000000 tfswin-3.3.3/tfswin/merge.py
--rw-r--r--   0 alex       (501) staff       (20)     1637 2022-12-11 13:14:49.000000 tfswin-3.3.3/tfswin/mlp.py
--rw-r--r--   0 alex       (501) staff       (20)    16525 2023-02-10 10:06:04.000000 tfswin-3.3.3/tfswin/model.py
--rw-r--r--   0 alex       (501) staff       (20)     1315 2023-01-04 20:05:22.000000 tfswin-3.3.3/tfswin/norm.py
--rw-r--r--   0 alex       (501) staff       (20)      384 2022-09-12 20:57:18.000000 tfswin-3.3.3/tfswin/prep.py
--rw-r--r--   0 alex       (501) staff       (20)     3920 2023-02-10 10:06:04.000000 tfswin-3.3.3/tfswin/swin.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-13 14:50:45.983104 tfswin-3.3.3/tfswin/tests/
--rw-r--r--   0 alex       (501) staff       (20)      875 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/tests/test_ape.py
--rw-r--r--   0 alex       (501) staff       (20)     1303 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)      811 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/tests/test_drop.py
--rw-r--r--   0 alex       (501) staff       (20)      920 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/tests/test_embed.py
--rw-r--r--   0 alex       (501) staff       (20)      843 2022-09-12 17:30:34.000000 tfswin-3.3.3/tfswin/tests/test_merge.py
--rw-r--r--   0 alex       (501) staff       (20)      824 2022-05-26 19:17:56.000000 tfswin-3.3.3/tfswin/tests/test_mlp.py
--rw-r--r--   0 alex       (501) staff       (20)     5199 2023-01-16 14:07:50.000000 tfswin-3.3.3/tfswin/tests/test_model.py
--rw-r--r--   0 alex       (501) staff       (20)     1200 2022-12-28 19:38:20.000000 tfswin-3.3.3/tfswin/tests/test_norm.py
--rw-r--r--   0 alex       (501) staff       (20)     3446 2023-01-16 10:51:38.000000 tfswin-3.3.3/tfswin/tests/test_swin.py
--rw-r--r--   0 alex       (501) staff       (20)     3116 2023-01-17 08:02:26.000000 tfswin-3.3.3/tfswin/tests/test_winatt.py
--rw-r--r--   0 alex       (501) staff       (20)     7125 2023-01-31 10:49:15.000000 tfswin-3.3.3/tfswin/winatt.py
--rw-r--r--   0 alex       (501) staff       (20)     3542 2023-01-04 20:05:22.000000 tfswin-3.3.3/tfswin/window.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-02-13 14:50:45.972651 tfswin-3.3.3/tfswin.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     8571 2023-02-13 14:50:45.000000 tfswin-3.3.3/tfswin.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      683 2023-02-13 14:50:45.000000 tfswin-3.3.3/tfswin.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-02-13 14:50:45.000000 tfswin-3.3.3/tfswin.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       47 2023-02-13 14:50:45.000000 tfswin-3.3.3/tfswin.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        7 2023-02-13 14:50:45.000000 tfswin-3.3.3/tfswin.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-05 21:15:00.175626 tfswin-3.4.0/
+-rw-r--r--   0 alex       (501) staff       (20)     1070 2021-01-02 15:55:39.000000 tfswin-3.4.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       33 2021-11-19 08:13:39.000000 tfswin-3.4.0/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     7259 2023-07-05 21:15:00.175757 tfswin-3.4.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     6431 2023-01-17 08:02:26.000000 tfswin-3.4.0/README.md
+-rw-r--r--   0 alex       (501) staff       (20)       47 2023-07-05 21:14:40.000000 tfswin-3.4.0/requirements.txt
+-rw-r--r--   0 alex       (501) staff       (20)       91 2023-07-05 21:15:00.176187 tfswin-3.4.0/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1205 2023-07-05 21:14:40.000000 tfswin-3.4.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-05 21:15:00.173592 tfswin-3.4.0/tfswin/
+-rw-r--r--   0 alex       (501) staff       (20)      532 2022-05-26 19:17:56.000000 tfswin-3.4.0/tfswin/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1617 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/ape.py
+-rw-r--r--   0 alex       (501) staff       (20)     5289 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/basic.py
+-rw-r--r--   0 alex       (501) staff       (20)     1493 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/drop.py
+-rw-r--r--   0 alex       (501) staff       (20)     1492 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/embed.py
+-rw-r--r--   0 alex       (501) staff       (20)     2598 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/merge.py
+-rw-r--r--   0 alex       (501) staff       (20)     1621 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/mlp.py
+-rw-r--r--   0 alex       (501) staff       (20)    16533 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/model.py
+-rw-r--r--   0 alex       (501) staff       (20)     1295 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/norm.py
+-rw-r--r--   0 alex       (501) staff       (20)      384 2022-09-12 20:57:18.000000 tfswin-3.4.0/tfswin/prep.py
+-rw-r--r--   0 alex       (501) staff       (20)     3904 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/swin.py
+-rw-r--r--   0 alex       (501) staff       (20)     7109 2023-07-05 21:14:40.000000 tfswin-3.4.0/tfswin/winatt.py
+-rw-r--r--   0 alex       (501) staff       (20)     3542 2023-01-04 20:05:22.000000 tfswin-3.4.0/tfswin/window.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-05 21:15:00.175375 tfswin-3.4.0/tfswin.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     7259 2023-07-05 21:15:00.000000 tfswin-3.4.0/tfswin.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      419 2023-07-05 21:15:00.000000 tfswin-3.4.0/tfswin.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-05 21:15:00.000000 tfswin-3.4.0/tfswin.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       47 2023-07-05 21:15:00.000000 tfswin-3.4.0/tfswin.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        7 2023-07-05 21:15:00.000000 tfswin-3.4.0/tfswin.egg-info/top_level.txt
```

### Comparing `tfswin-3.3.3/LICENSE` & `tfswin-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfswin-3.3.3/README.md` & `tfswin-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tfswin-3.3.3/setup.py` & `tfswin-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tfswin',
-    version='3.3.3',
+    version='3.4.0',
     description='Keras (TensorFlow v2) reimplementation of Swin Transformer V1 & V2 models.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/shkarupa-alex/tfswin',
     author='Shkarupa Alex',
     author_email='shkarupa.alex@gmail.com',
     license='MIT',
```

### Comparing `tfswin-3.3.3/tfswin/__init__.py` & `tfswin-3.4.0/tfswin/__init__.py`

 * *Files identical despite different names*

### Comparing `tfswin-3.3.3/tfswin/ape.py` & `tfswin-3.4.0/tfswin/ape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from keras import initializers, layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 
 
 @register_keras_serializable(package='TFSwin')
 class AbsoluteEmbedding(layers.Layer):
     def __init__(self, pretrain_size, **kwargs):
         super().__init__(**kwargs)
         self.input_spec = layers.InputSpec(ndim=4)
```

### Comparing `tfswin-3.3.3/tfswin/basic.py` & `tfswin-3.4.0/tfswin/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
 from keras import layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 from tfswin.swin import SwinBlock
 from tfswin.window import window_partition
 
 
 @register_keras_serializable(package='TFSwin')
 class BasicLayer(layers.Layer):
     def __init__(self, depth, num_heads, window_size, mlp_ratio=4., qkv_bias=True, qk_scale=None,
```

### Comparing `tfswin-3.3.3/tfswin/drop.py` & `tfswin-3.4.0/tfswin/drop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from keras import backend, layers
-from keras.utils.control_flow_util import smart_cond
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.control_flow_util import smart_cond
+from keras.src.utils.tf_utils import shape_type_conversion
 
 
 @register_keras_serializable(package='TFSwin')
 class DropPath(layers.Layer):
     def __init__(self, rate, **kwargs):
         super().__init__(**kwargs)
         self.input_spec = layers.InputSpec(min_ndim=1)
```

### Comparing `tfswin-3.3.3/tfswin/embed.py` & `tfswin-3.4.0/tfswin/embed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from keras import layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 from tfswin.norm import LayerNorm
 
 
 @register_keras_serializable(package='TFSwin')
 class PatchEmbedding(layers.Layer):
     def __init__(self, patch_size, embed_dim, normalize, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `tfswin-3.3.3/tfswin/merge.py` & `tfswin-3.4.0/tfswin/merge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import numpy as np
 import tensorflow as tf
 from keras import layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 from tfswin.norm import LayerNorm
 
 
 @register_keras_serializable(package='TFSwin')
 class PatchMerging(layers.Layer):
     def __init__(self, swin_v2=False, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `tfswin-3.3.3/tfswin/mlp.py` & `tfswin-3.4.0/tfswin/mlp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from keras import activations, layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 
 
 @register_keras_serializable(package='TFSwin')
 class MLP(layers.Layer):
     def __init__(self, ratio, dropout, **kwargs):
         super().__init__(**kwargs)
         self.input_spec = layers.InputSpec(ndim=4)
```

### Comparing `tfswin-3.3.3/tfswin/model.py` & `tfswin-3.4.0/tfswin/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
 from keras import backend, layers, models
-from keras.applications import imagenet_utils
-from keras.utils import conv_utils, data_utils, layer_utils
+from keras.src.applications import imagenet_utils
+from keras.src.utils import conv_utils, data_utils, layer_utils
 from tfswin.ape import AbsoluteEmbedding
 from tfswin.basic import BasicLayer
 from tfswin.embed import PatchEmbedding
 from tfswin.merge import PatchMerging
 from tfswin.norm import LayerNorm
 
 BASE_URL = 'https://github.com/shkarupa-alex/tfswin/releases/download/{}/swin{}_{}.h5'
```

### Comparing `tfswin-3.3.3/tfswin/norm.py` & `tfswin-3.4.0/tfswin/norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from keras import layers
-from keras.saving.object_registration import register_keras_serializable
+from keras.saving import register_keras_serializable
 
 
 @register_keras_serializable(package='TFSwin')
 class LayerNorm(layers.LayerNormalization):
     # Overload to use fused implementation
 
     def __init__(self, epsilon=1.001e-5, **kwargs):
```

### Comparing `tfswin-3.3.3/tfswin/swin.py` & `tfswin-3.4.0/tfswin/swin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from keras import layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 from tfswin.drop import DropPath
 from tfswin.mlp import MLP
 from tfswin.norm import LayerNorm
 from tfswin.winatt import WindowAttention
 
 
 @register_keras_serializable(package='TFSwin')
```

### Comparing `tfswin-3.3.3/tfswin/winatt.py` & `tfswin-3.4.0/tfswin/winatt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
 from keras import initializers, layers
-from keras.saving.object_registration import register_keras_serializable
-from keras.utils.tf_utils import shape_type_conversion
+from keras.saving import register_keras_serializable
+from keras.src.utils.tf_utils import shape_type_conversion
 from tfswin.window import window_partition_fused, window_reverse_fused
 
 
 @register_keras_serializable(package='TFSwin')
 class WindowAttention(layers.Layer):
     def __init__(self, num_heads, qkv_bias=True, qk_scale=None, attn_drop=0., proj_drop=0.,
                  window_pretrain=0, swin_v2=False, **kwargs):
```

### Comparing `tfswin-3.3.3/tfswin/window.py` & `tfswin-3.4.0/tfswin/window.py`

 * *Files identical despite different names*

