# Comparing `tmp/fastervit-0.9.0.tar.gz` & `tmp/fastervit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-pdkhyeni/fastervit-0.9.0.tar", last modified: Sat Jul  1 03:59:10 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-zaj7smev/fastervit-0.9.1.tar", last modified: Wed Jul  5 05:28:12 2023, max compression
```

## Comparing `fastervit-0.9.0.tar` & `fastervit-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-01 03:20:05.000000 fastervit-0.9.0/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-01 03:20:05.000000 fastervit-0.9.0/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)    10793 2023-07-01 03:59:10.000000 fastervit-0.9.0/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     9843 2023-07-01 03:36:57.000000 fastervit-0.9.0/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    42354 2023-07-01 03:28:20.000000 fastervit-0.9.0/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    44191 2023-07-01 03:29:51.000000 fastervit-0.9.0/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/train.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/utils/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4288 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/checkpoint.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/datasets.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    10793 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      854 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-01 03:59:10.000000 fastervit-0.9.0/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-01 03:37:49.000000 fastervit-0.9.0/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-05 05:27:14.000000 fastervit-0.9.1/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-05 05:27:14.000000 fastervit-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11887 2023-07-05 05:28:12.000000 fastervit-0.9.1/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10937 2023-07-05 05:27:14.000000 fastervit-0.9.1/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    48432 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    50190 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/train.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/utils/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/utils/datasets.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11887 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-05 05:28:12.000000 fastervit-0.9.1/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-05 05:27:14.000000 fastervit-0.9.1/setup.py
```

### Comparing `fastervit-0.9.0/LICENSE` & `fastervit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/PKG-INFO` & `fastervit-0.9.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: fastervit
-Version: 0.9.0
-Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
-Home-page: https://github.com/NVlabs/FasterViT
-Author: Ali Hatamizadeh
-Author-email: ahatamiz123@gmail.com
-License: NVIDIA Source Code License-NC
-Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FasterViT: Fast Vision Transformers with Hierarchical Attention
 
 Official PyTorch implementation of [**FasterViT: Fast Vision Transformers with Hierarchical Attention**](https://arxiv.org/abs/2306.06189).
 
 [Ali Hatamizadeh](https://research.nvidia.com/person/ali-hatamizadeh),
 [Greg Heinrich](https://developer.nvidia.com/blog/author/gheinrich/),
 [Hongxu (Danny) Yin](https://scholar.princeton.edu/hongxu),
@@ -34,77 +12,101 @@
 
 For business inquiries, please visit our website and submit the form: [NVIDIA Research Licensing](https://www.nvidia.com/en-us/research/inquiries/)
 
 
 --- 
 
 FasterViT achieves a new SOTA Pareto-front in
-terms of accuracy vs. image throughput (no extra training data !)
+terms of accuracy vs. image throughput without extra training data !
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
 We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
 ![teaser](./fastervit/assets/hierarchial_attn.png)
 
-## 💥 News 💥
-
-- **[06.30.2023]** 🔥🔥 We have further improved the [Any-resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
-- **[06.29.2023]** 🔥 Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
-- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
-- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
-
 ## Quick Start
 
-The FasterViT can be conveniently installed by:
+We can import pre-trained FasterViT models with **1 line of code**. First, FasterViT can be simply installed by:
 
 ```bash
 pip install fastervit
 ```
 
-A FasterViT model with default hyper-parameters can be created as in the following:
+A pretrained FasterViT model with default hyper-parameters can be created as in the following:
 
 ```python
 >>> from fastervit import create_model
 
 # Define fastervit-0 model with 224 x 224 resolution
->>> model = create_model('faster_vit_0_224')
+
+>>> model = create_model('faster_vit_0_224', 
+                          pretrained=True,
+                          model_path="/tmp/faster_vit_0.pth.tar")
+```
+
+We can adjust where to download the above FasterViT-0 model by passing `model_path`.
+
+We can also simply test the model by passing a dummy input image. The output is the logits:
+
+```python
+>>> import torch
+
+>>> image = torch.rand(1, 3, 224, 224)
+>>> output = model(image) # torch.Size([1, 1000])
 ```
 
-We can also use the any-resolution FasterViT model to accommodate arbitrary image resolutions. In the following, we define an any-resolution FasterViT-1
+We can also use the any-resolution FasterViT model to accommodate arbitrary image resolutions. In the following, we define an any-resolution FasterViT-0
 model with input resolution of 576 x 960, window sizes of 12 and 6 in 3rd and 4th stages, carrier token size of 2 and embedding dimension of
 128:
 
 ```python
 >>> from fastervit import create_model
 
-# Define any-resolution FasterViT-1 model with 576 x 960 resolution
->>> model = create_model('faster_vit_1_any_res', 
+# Define any-resolution FasterViT-0 model with 576 x 960 resolution
+>>> model = create_model('faster_vit_0_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
-                          dim=128)
+                          dim=64,
+                          pretrained=True)
 ```
+Note that the above model is intiliazed from the original ImageNet pre-trained FasterViT with original resolution of 224 x 224. As a result, missing keys and mis-matches could be expected since we are addign new layers (e.g. addition of new carrier tokens, etc.) 
+
+We can simply test the model by passing a dummy input image. The output is the logits:
+
+```python
+>>> import torch
+
+>>> image = torch.rand(1, 3, 576, 960)
+>>> output = model(image) # torch.Size([1, 1000])
+```
+
+## 💥 News 💥
+
+- **[07.04.2023]** 🔥🔥 ImageNet pretrained FasterViT models can now be imported with **1 line of code**. Please install the latest FasterViT pip package to use this functionality (also supports Any-resolution FasterViT models).
+- **[06.30.2023]** 🔥 We have further improved the [TensorRT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
+- **[06.29.2023]** Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
+- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
+- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
+
 
 ## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
 - [x] Add capablity to initialize any-resolution FasterViT from ImageNet-pretrained weights. 
-- [ ] Update training scripts to support model.compile
-- [ ] Add isotropic FasterViT
 - [ ] ImageNet-21K pre-trained models
-- [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
 - [ ] Segmentation code + models
 
 --- 
 
 ## Results + Pretrained Models
```

### Comparing `fastervit-0.9.0/fastervit/assets/hierarchial_attn.png` & `fastervit-0.9.1/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/models/faster_vit.py` & `fastervit-0.9.1/fastervit/models/faster_vit.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import torch
 import torch.nn as nn
 from timm.models.registry import register_model
 from timm.models.layers import trunc_normal_, DropPath, LayerNorm2d
 from .registry import register_pip_model
 import numpy as np
+from pathlib import Path
 
 
 def _cfg(url='', **kwargs):
     return {'url': url,
             'num_classes': 1000,
             'input_size': (3, 224, 224),
             'pool_size': None,
@@ -27,39 +28,39 @@
             'mean': (0.485, 0.456, 0.406),
             'std': (0.229, 0.224, 0.225),
             **kwargs
             }
 
 
 default_cfgs = {
-    'faster_vit_0_224': _cfg(url='',
+    'faster_vit_0_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_0_224_1k.pth.tar',
                              crop_pct=0.875,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_1_224': _cfg(url='',
+    'faster_vit_1_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_1_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_2_224': _cfg(url='',
+    'faster_vit_2_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_2_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_3_224': _cfg(url='',
+    'faster_vit_3_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_3_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_4_224': _cfg(url='',
+    'faster_vit_4_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_4_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_5_224': _cfg(url='',
+    'faster_vit_5_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_5_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
-    'faster_vit_6_224': _cfg(url='',
+    'faster_vit_6_224': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_6_224_1k.pth.tar',
                              crop_pct=1.0,
                              input_size=(3, 224, 224),
                              crop_mode='center'),
 }
 
 
 def window_partition(x, window_size):
@@ -87,14 +88,115 @@
     bs = ct.shape[0]
     N = ct.shape[2]
     ct = ct.view(bs, H // window_size, window_size, W // window_size, window_size, N)
     ct = ct.permute(0, 1, 3, 2, 4, 5)
     return ct
 
 
+def _load_state_dict(module, state_dict, strict=False, logger=None):
+    """Load state_dict to a module.
+
+    This method is modified from :meth:`torch.nn.Module.load_state_dict`.
+    Default value for ``strict`` is set to ``False`` and the message for
+    param mismatch will be shown even if strict is False.
+
+    Args:
+        module (Module): Module that receives the state_dict.
+        state_dict (OrderedDict): Weights.
+        strict (bool): whether to strictly enforce that the keys
+            in :attr:`state_dict` match the keys returned by this module's
+            :meth:`~torch.nn.Module.state_dict` function. Default: ``False``.
+        logger (:obj:`logging.Logger`, optional): Logger to log the error
+            message. If not specified, print function will be used.
+    """
+    unexpected_keys = []
+    all_missing_keys = []
+    err_msg = []
+
+    metadata = getattr(state_dict, '_metadata', None)
+    state_dict = state_dict.copy()
+    if metadata is not None:
+        state_dict._metadata = metadata
+    
+    def load(module, prefix=''):
+        local_metadata = {} if metadata is None else metadata.get(
+            prefix[:-1], {})
+        module._load_from_state_dict(state_dict, prefix, local_metadata, True,
+                                     all_missing_keys, unexpected_keys,
+                                     err_msg)
+        for name, child in module._modules.items():
+            if child is not None:
+                load(child, prefix + name + '.')
+
+    load(module)
+    load = None
+    missing_keys = [
+        key for key in all_missing_keys if 'num_batches_tracked' not in key
+    ]
+
+    if unexpected_keys:
+        err_msg.append('unexpected key in source '
+                       f'state_dict: {", ".join(unexpected_keys)}\n')
+    if missing_keys:
+        err_msg.append(
+            f'missing keys in source state_dict: {", ".join(missing_keys)}\n')
+
+    
+    if len(err_msg) > 0:
+        err_msg.insert(
+            0, 'The model and loaded state dict do not match exactly\n')
+        err_msg = '\n'.join(err_msg)
+        if strict:
+            raise RuntimeError(err_msg)
+        elif logger is not None:
+            logger.warning(err_msg)
+        else:
+            print(err_msg)
+
+
+def _load_checkpoint(model,
+                    filename,
+                    map_location='cpu',
+                    strict=False,
+                    logger=None):
+    """Load checkpoint from a file or URI.
+
+    Args:
+        model (Module): Module to load checkpoint.
+        filename (str): Accept local filepath, URL, ``torchvision://xxx``,
+            ``open-mmlab://xxx``. Please refer to ``docs/model_zoo.md`` for
+            details.
+        map_location (str): Same as :func:`torch.load`.
+        strict (bool): Whether to allow different params for the model and
+            checkpoint.
+        logger (:mod:`logging.Logger` or None): The logger for error message.
+
+    Returns:
+        dict or OrderedDict: The loaded checkpoint.
+    """
+    checkpoint = torch.load(filename, map_location=map_location)
+    if not isinstance(checkpoint, dict):
+        raise RuntimeError(
+            f'No state_dict found in checkpoint file {filename}')
+    if 'state_dict' in checkpoint:
+        state_dict = checkpoint['state_dict']
+    elif 'model' in checkpoint:
+        state_dict = checkpoint['model']
+    else:
+        state_dict = checkpoint
+    if list(state_dict.keys())[0].startswith('module.'):
+        state_dict = {k[7:]: v for k, v in state_dict.items()}
+
+    if sorted(list(state_dict.keys()))[0].startswith('encoder'):
+        state_dict = {k.replace('encoder.', ''): v for k, v in state_dict.items() if k.startswith('encoder.')}
+
+    _load_state_dict(model, state_dict, strict, logger)
+    return checkpoint
+
+
 class PosEmbMLPSwinv2D(nn.Module):
     def __init__(self,
                  window_size,
                  pretrained_window_size,
                  num_heads, seq_length,
                  ct_correct=False,
                  no_log=False):
@@ -836,41 +938,52 @@
         x = torch.flatten(x, 1)
         return x
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.head(x)
         return x
+    
+    def _load_state_dict(self, 
+                         pretrained, 
+                         strict: bool = False):
+        _load_checkpoint(self, 
+                         pretrained, 
+                         strict=strict)
 
 
 @register_pip_model
 @register_model
 def faster_vit_0_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [2, 3, 6, 5])
     num_heads = kwargs.pop("num_heads", [2, 4, 8, 16])
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 64)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_0.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_0_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_1_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [1, 3, 8, 5])
@@ -878,27 +991,31 @@
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 80)
     in_dim = kwargs.pop("in_dim", 32)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_1.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_1_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_2_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 8, 5])
@@ -906,27 +1023,31 @@
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 96)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_2.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_3_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -935,14 +1056,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 128)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_3.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -950,15 +1072,18 @@
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_3_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_4_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -967,14 +1092,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 196)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_4.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -983,15 +1109,18 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_4_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_5_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -1000,14 +1129,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_5.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -1016,15 +1146,18 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_5_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_6_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 16, 8])
@@ -1033,14 +1166,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.5)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_6.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -1049,9 +1183,12 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_6_224']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
```

### Comparing `fastervit-0.9.0/fastervit/models/faster_vit_any_res.py` & `fastervit-0.9.1/fastervit/models/faster_vit_any_res.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 import torch
 import torch.nn as nn
 from timm.models.registry import register_model
 from timm.models.layers import trunc_normal_, DropPath, LayerNorm2d
 from .registry import register_pip_model
 import numpy as np
-from utils.checkpoint import load_checkpoint
+from pathlib import Path
+
+
 
 def _cfg(url='', **kwargs):
     return {'url': url,
             'num_classes': 1000,
             'input_size': (3, 224, 224),
             'pool_size': None,
             'crop_pct': 0.875,
@@ -27,39 +29,39 @@
             'mean': (0.485, 0.456, 0.406),
             'std': (0.229, 0.224, 0.225),
             **kwargs
             }
 
 
 default_cfgs = {
-    'faster_vit_0_any_res': _cfg(url='',
+    'faster_vit_0_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_0_224_1k.pth.tar',
                                  crop_pct=0.875,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_1_any_res': _cfg(url='',
+    'faster_vit_1_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_1_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_2_any_res': _cfg(url='',
+    'faster_vit_2_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_2_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_3_any_res': _cfg(url='',
+    'faster_vit_3_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_3_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_4_any_res': _cfg(url='',
+    'faster_vit_4_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_4_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_5_any_res': _cfg(url='',
+    'faster_vit_5_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_5_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
-    'faster_vit_6_any_res': _cfg(url='',
+    'faster_vit_6_any_res': _cfg(url='https://huggingface.co/ahatamiz/FasterViT/resolve/main/fastervit_6_224_1k.pth.tar',
                                  crop_pct=1.0,
                                  input_size=(3, 224, 224),
                                  crop_mode='center'),
 }
 
 
 def window_partition(x, window_size):
@@ -86,14 +88,116 @@
 def ct_window(ct, W, H, window_size):
     bs = ct.shape[0]
     N = ct.shape[2]
     ct = ct.view(bs, H // window_size, window_size, W // window_size, window_size, N)
     ct = ct.permute(0, 1, 3, 2, 4, 5)
     return ct
 
+
+def _load_state_dict(module, state_dict, strict=False, logger=None):
+    """Load state_dict to a module.
+
+    This method is modified from :meth:`torch.nn.Module.load_state_dict`.
+    Default value for ``strict`` is set to ``False`` and the message for
+    param mismatch will be shown even if strict is False.
+
+    Args:
+        module (Module): Module that receives the state_dict.
+        state_dict (OrderedDict): Weights.
+        strict (bool): whether to strictly enforce that the keys
+            in :attr:`state_dict` match the keys returned by this module's
+            :meth:`~torch.nn.Module.state_dict` function. Default: ``False``.
+        logger (:obj:`logging.Logger`, optional): Logger to log the error
+            message. If not specified, print function will be used.
+    """
+    unexpected_keys = []
+    all_missing_keys = []
+    err_msg = []
+
+    metadata = getattr(state_dict, '_metadata', None)
+    state_dict = state_dict.copy()
+    if metadata is not None:
+        state_dict._metadata = metadata
+    
+    def load(module, prefix=''):
+        local_metadata = {} if metadata is None else metadata.get(
+            prefix[:-1], {})
+        module._load_from_state_dict(state_dict, prefix, local_metadata, True,
+                                     all_missing_keys, unexpected_keys,
+                                     err_msg)
+        for name, child in module._modules.items():
+            if child is not None:
+                load(child, prefix + name + '.')
+
+    load(module)
+    load = None
+    missing_keys = [
+        key for key in all_missing_keys if 'num_batches_tracked' not in key
+    ]
+
+    if unexpected_keys:
+        err_msg.append('unexpected key in source '
+                       f'state_dict: {", ".join(unexpected_keys)}\n')
+    if missing_keys:
+        err_msg.append(
+            f'missing keys in source state_dict: {", ".join(missing_keys)}\n')
+
+    
+    if len(err_msg) > 0:
+        err_msg.insert(
+            0, 'The model and loaded state dict do not match exactly\n')
+        err_msg = '\n'.join(err_msg)
+        if strict:
+            raise RuntimeError(err_msg)
+        elif logger is not None:
+            logger.warning(err_msg)
+        else:
+            print(err_msg)
+
+
+def _load_checkpoint(model,
+                    filename,
+                    map_location='cpu',
+                    strict=False,
+                    logger=None):
+    """Load checkpoint from a file or URI.
+
+    Args:
+        model (Module): Module to load checkpoint.
+        filename (str): Accept local filepath, URL, ``torchvision://xxx``,
+            ``open-mmlab://xxx``. Please refer to ``docs/model_zoo.md`` for
+            details.
+        map_location (str): Same as :func:`torch.load`.
+        strict (bool): Whether to allow different params for the model and
+            checkpoint.
+        logger (:mod:`logging.Logger` or None): The logger for error message.
+
+    Returns:
+        dict or OrderedDict: The loaded checkpoint.
+    """
+    checkpoint = torch.load(filename, map_location=map_location)
+    if not isinstance(checkpoint, dict):
+        raise RuntimeError(
+            f'No state_dict found in checkpoint file {filename}')
+    if 'state_dict' in checkpoint:
+        state_dict = checkpoint['state_dict']
+    elif 'model' in checkpoint:
+        state_dict = checkpoint['model']
+    else:
+        state_dict = checkpoint
+    if list(state_dict.keys())[0].startswith('module.'):
+        state_dict = {k[7:]: v for k, v in state_dict.items()}
+
+    if sorted(list(state_dict.keys()))[0].startswith('encoder'):
+        state_dict = {k.replace('encoder.', ''): v for k, v in state_dict.items() if k.startswith('encoder.')}
+
+    _load_state_dict(model, state_dict, strict, logger)
+    return checkpoint
+
+
 class PosEmbMLPSwinv2D(nn.Module):
     def __init__(self,
                  window_size,
                  pretrained_window_size,
                  num_heads, seq_length,
                  ct_correct=False,
                  no_log=False):
@@ -863,42 +967,52 @@
         x = torch.flatten(x, 1)
         return x
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.head(x)
         return x
-    def load_state_dict(self, pretrained, strict: bool = False):
-        load_checkpoint(self, pretrained, strict=strict)
+    
+    def _load_state_dict(self, 
+                         pretrained, 
+                         strict: bool = False):
+        _load_checkpoint(self, 
+                         pretrained, 
+                         strict=strict)
+
 
 @register_pip_model
 @register_model
 def faster_vit_0_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [2, 3, 6, 5])
     num_heads = kwargs.pop("num_heads", [2, 4, 8, 16])
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 64)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_0.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_0_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_1_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [1, 3, 8, 5])
@@ -906,27 +1020,31 @@
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 80)
     in_dim = kwargs.pop("in_dim", 32)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_1.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_1_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_2_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 8, 5])
@@ -934,27 +1052,31 @@
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 96)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [541, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_2.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_3_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -963,14 +1085,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 128)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_3.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -978,15 +1101,18 @@
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_3_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_4_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -995,14 +1121,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 196)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_4.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -1011,15 +1138,18 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_4_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_5_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -1028,14 +1158,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_5.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -1044,15 +1175,18 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_5_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_6_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 16, 8])
@@ -1061,14 +1195,15 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.5)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
+    model_path = kwargs.pop("model_path", "/tmp/faster_vit_6.pth.tar")
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
@@ -1077,9 +1212,12 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_6_any_res']
     if pretrained:
-        model.load_state_dict(pretrained)
+        if not Path(model_path).is_file():
+            url = model.default_cfg['url']
+            torch.hub.download_url_to_file(url=url, dst=model_path)
+        model._load_state_dict(model_path)
     return model
```

### Comparing `fastervit-0.9.0/fastervit/models/registry.py` & `fastervit-0.9.1/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/cosine_lr.py` & `fastervit-0.9.1/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/multistep_lr.py` & `fastervit-0.9.1/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/plateau_lr.py` & `fastervit-0.9.1/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/poly_lr.py` & `fastervit-0.9.1/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/scheduler.py` & `fastervit-0.9.1/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.9.1/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/step_lr.py` & `fastervit-0.9.1/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/scheduler/tanh_lr.py` & `fastervit-0.9.1/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/tensorboard.py` & `fastervit-0.9.1/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/train.py` & `fastervit-0.9.1/fastervit/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 This script was started from an early version of the PyTorch ImageNet example
 (https://github.com/pytorch/examples/tree/master/imagenet)
 
 NVIDIA CUDA specific speedups adopted from NVIDIA Apex examplesf
 (https://github.com/NVIDIA/apex/tree/master/examples/imagenet)
 
-Hacked together by / Copyright 2020 Ross Wightman (https://github.com/rwightman)
+Hacked together by / Copyright 2023 Ross Wightman (https://github.com/rwightman)
 """
 import argparse
 import time
 import yaml
 import os
 import logging
 from collections import OrderedDict
@@ -36,15 +36,14 @@
 from timm.optim import create_optimizer_v2, optimizer_kwargs
 from timm.scheduler import *
 from timm.utils import ApexScaler, NativeScaler
 from scheduler.scheduler_factory import create_scheduler
 import shutil
 from utils.datasets import imagenet_lmdb_dataset
 from tensorboard import TensorboardLogger
-from ptflops import get_model_complexity_info
 from models.faster_vit import *
 from models.faster_vit_any_res import *
 
 try:
     from apex import amp
     from apex.parallel import DistributedDataParallel as ApexDDP
     from apex.parallel import convert_syncbn_model
@@ -434,20 +433,15 @@
         global_pool=args.gp,
         bn_momentum=args.bn_momentum,
         bn_eps=args.bn_eps,
         scriptable=args.torchscript,
         checkpoint_path=args.initial_checkpoint,
         attn_drop_rate=args.attn_drop_rate,
         drop_rate=args.drop_rate)
-        # drop_path_rate=args.drop_path)
-
-    macs, params = get_model_complexity_info(model, tuple([3, args.input_size[1], args.input_size[2]]),
-                                                as_strings=False, print_per_layer_stat=False, verbose=False)
-    print(f"Model stats: macs: {macs / 1e9}, and params (M): {params / 1e6}")
-
+    
     if args.bfloat:
         args.dtype = torch.bfloat16
     else:
         args.dtype = torch.float16
 
     if args.num_classes is None:
         assert hasattr(model, 'num_classes'), 'Model must have `num_classes` attr if not set on cmd line/config.'
```

### Comparing `fastervit-0.9.0/fastervit/utils/datasets.py` & `fastervit-0.9.1/fastervit/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit/validate.py` & `fastervit-0.9.1/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.0/fastervit.egg-info/PKG-INFO` & `fastervit-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.9.0
+Version: 0.9.1
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -34,77 +34,101 @@
 
 For business inquiries, please visit our website and submit the form: [NVIDIA Research Licensing](https://www.nvidia.com/en-us/research/inquiries/)
 
 
 --- 
 
 FasterViT achieves a new SOTA Pareto-front in
-terms of accuracy vs. image throughput (no extra training data !)
+terms of accuracy vs. image throughput without extra training data !
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
 We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
 ![teaser](./fastervit/assets/hierarchial_attn.png)
 
-## 💥 News 💥
-
-- **[06.30.2023]** 🔥🔥 We have further improved the [Any-resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
-- **[06.29.2023]** 🔥 Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
-- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
-- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
-
 ## Quick Start
 
-The FasterViT can be conveniently installed by:
+We can import pre-trained FasterViT models with **1 line of code**. First, FasterViT can be simply installed by:
 
 ```bash
 pip install fastervit
 ```
 
-A FasterViT model with default hyper-parameters can be created as in the following:
+A pretrained FasterViT model with default hyper-parameters can be created as in the following:
 
 ```python
 >>> from fastervit import create_model
 
 # Define fastervit-0 model with 224 x 224 resolution
->>> model = create_model('faster_vit_0_224')
+
+>>> model = create_model('faster_vit_0_224', 
+                          pretrained=True,
+                          model_path="/tmp/faster_vit_0.pth.tar")
+```
+
+We can adjust where to download the above FasterViT-0 model by passing `model_path`.
+
+We can also simply test the model by passing a dummy input image. The output is the logits:
+
+```python
+>>> import torch
+
+>>> image = torch.rand(1, 3, 224, 224)
+>>> output = model(image) # torch.Size([1, 1000])
 ```
 
-We can also use the any-resolution FasterViT model to accommodate arbitrary image resolutions. In the following, we define an any-resolution FasterViT-1
+We can also use the any-resolution FasterViT model to accommodate arbitrary image resolutions. In the following, we define an any-resolution FasterViT-0
 model with input resolution of 576 x 960, window sizes of 12 and 6 in 3rd and 4th stages, carrier token size of 2 and embedding dimension of
 128:
 
 ```python
 >>> from fastervit import create_model
 
-# Define any-resolution FasterViT-1 model with 576 x 960 resolution
->>> model = create_model('faster_vit_1_any_res', 
+# Define any-resolution FasterViT-0 model with 576 x 960 resolution
+>>> model = create_model('faster_vit_0_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
-                          dim=128)
+                          dim=64,
+                          pretrained=True)
 ```
+Note that the above model is intiliazed from the original ImageNet pre-trained FasterViT with original resolution of 224 x 224. As a result, missing keys and mis-matches could be expected since we are addign new layers (e.g. addition of new carrier tokens, etc.) 
+
+We can simply test the model by passing a dummy input image. The output is the logits:
+
+```python
+>>> import torch
+
+>>> image = torch.rand(1, 3, 576, 960)
+>>> output = model(image) # torch.Size([1, 1000])
+```
+
+## 💥 News 💥
+
+- **[07.04.2023]** 🔥🔥 ImageNet pretrained FasterViT models can now be imported with **1 line of code**. Please install the latest FasterViT pip package to use this functionality (also supports Any-resolution FasterViT models).
+- **[06.30.2023]** 🔥 We have further improved the [TensorRT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
+- **[06.29.2023]** Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
+- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
+- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
+
 
 ## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
 - [x] Add capablity to initialize any-resolution FasterViT from ImageNet-pretrained weights. 
-- [ ] Update training scripts to support model.compile
-- [ ] Add isotropic FasterViT
 - [ ] ImageNet-21K pre-trained models
-- [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
 - [ ] Segmentation code + models
 
 --- 
 
 ## Results + Pretrained Models
```

### Comparing `fastervit-0.9.0/fastervit.egg-info/SOURCES.txt` & `fastervit-0.9.1/fastervit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 fastervit/scheduler/plateau_lr.py
 fastervit/scheduler/poly_lr.py
 fastervit/scheduler/scheduler.py
 fastervit/scheduler/scheduler_factory.py
 fastervit/scheduler/step_lr.py
 fastervit/scheduler/tanh_lr.py
 fastervit/utils/__init__.py
-fastervit/utils/checkpoint.py
 fastervit/utils/datasets.py
```

### Comparing `fastervit-0.9.0/setup.py` & `fastervit-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.9.0',
+    version='0.9.1',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

