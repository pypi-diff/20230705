# Comparing `tmp/block-recurrent-transformer-pytorch-0.4.2.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.4.2.tar", last modified: Thu Apr 20 21:41:43 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.4.3.tar", last modified: Wed Jul  5 20:32:02 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.4.2.tar` & `block-recurrent-transformer-pytorch-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:41:43.079678 block-recurrent-transformer-pytorch-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 21:41:30.000000 block-recurrent-transformer-pytorch-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 21:41:43.079678 block-recurrent-transformer-pytorch-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-20 21:41:30.000000 block-recurrent-transformer-pytorch-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:41:43.079678 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 21:41:30.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37294 2023-04-20 21:41:30.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:41:43.079678 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 21:41:43.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 21:41:43.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:41:43.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 21:41:43.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 21:41:43.000000 block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:41:43.079678 block-recurrent-transformer-pytorch-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 21:41:30.000000 block-recurrent-transformer-pytorch-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:02.759544 block-recurrent-transformer-pytorch-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 20:31:53.000000 block-recurrent-transformer-pytorch-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 20:32:02.759544 block-recurrent-transformer-pytorch-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-05 20:31:53.000000 block-recurrent-transformer-pytorch-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:02.759544 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-05 20:31:53.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37274 2023-07-05 20:31:53.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:02.759544 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 20:32:02.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 20:32:02.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:32:02.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 20:32:02.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 20:32:02.000000 block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:32:02.759544 block-recurrent-transformer-pytorch-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-05 20:31:53.000000 block-recurrent-transformer-pytorch-0.4.3/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.4.2/LICENSE` & `block-recurrent-transformer-pytorch-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.4.2/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.4.2/README.md` & `block-recurrent-transformer-pytorch-0.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Block Recurrent Transformer - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2203.07852">Block Recurrent Transformer</a> - Pytorch. The highlight of the paper is its reported ability to remember something up to 60k tokens ago.
 
 This design is SOTA for recurrent transformers line of research, afaict.
 
-It will also include <a href="https://arxiv.org/abs/2205.14135">flash attention</a> as well as <a href="https://arxiv.org/abs/2203.08913">KNN attention layers</a>
+It will also include <a href="https://arxiv.org/abs/2205.14135">flash attention</a> as well as routed memories of up to 250k tokens using ideas from <a href="https://github.com/lucidrains/CoLT5-attention">this paper</a>
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability.ai</a> for the generous sponsorship to work and open source cutting edge artificial intelligence research
 
 ## Install
 
@@ -66,15 +66,15 @@
 - [x] make sure attention allow for single head key / values too
 - [x] run a few experiments of fixed gating in regular transformers - does not work
 - [x] integrate <a href="https://github.com/hazyresearch/flash-attention">flash attention</a>
 - [x] cache attention mask + rotary embeddings
 - [x] add <a href="https://github.com/lucidrains/compressive-transformer-pytorch">compressed memories</a>
 
 - [ ] revisit <a href="https://github.com/lucidrains/memformer">memformer</a>
-- [ ] add ability to gate in memorizing transformers knn attention layers
+- [ ] try routing long distance memories of up to 250k using coordinate descent (Wright et al.)
 
 ## Citations
 
 ```bibtex
 @article{Hutchins2022BlockRecurrentT,
     title   = {Block-Recurrent Transformers},
     author  = {DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam Neyshabur},
@@ -107,9 +107,16 @@
     title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
     author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
     booktitle = {Advances in Neural Information Processing Systems},
     year    = {2022}
 }
 ```
 
+```bibtex
+@inproceedings{Ainslie2023CoLT5FL,
+    title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
+    author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
+    year    = {2023}
+}
+```
 
 *Memory is Attention through Time* - Alex Graves
```

#### html2text {}

```diff
@@ -1,51 +1,57 @@
 [./block-recurrent-transformer.png] ## Block Recurrent Transformer - Pytorch
 Implementation of Block_Recurrent_Transformer - Pytorch. The highlight of the
 paper is its reported ability to remember something up to 60k tokens ago. This
 design is SOTA for recurrent transformers line of research, afaict. It will
-also include flash_attention as well as KNN_attention_layers ## Appreciation -
-Stability.ai for the generous sponsorship to work and open source cutting edge
-artificial intelligence research ## Install ```bash $ pip install block-
-recurrent-transformer-pytorch ``` ## Usage ```python import torch from
-block_recurrent_transformer_pytorch import BlockRecurrentTransformer model =
-BlockRecurrentTransformer( num_tokens = 20000, # vocab size dim = 512, # model
-dimensions depth = 6, # depth dim_head = 64, # attention head dimensions heads
-= 8, # number of attention heads max_seq_len = 1024, # the total receptive
-field of the transformer, in the paper this was 2 * block size block_width =
-512, # block size - total receptive field is max_seq_len, 2 * block size in
-paper. the block furthest forwards becomes the new cached xl memories, which is
-a block size of 1 (please open an issue if i am wrong) num_state_vectors = 512,
-# number of state vectors, i believe this was a single block size in the paper,
-but can be any amount recurrent_layers = (4,), # where to place the recurrent
-layer(s) for states with fixed simple gating use_compressed_mem = False, #
-whether to use compressed memories of a single block width, from https://
-arxiv.org/abs/1911.05507 compressed_mem_factor = 4, # compression factor of
-compressed memories use_flash_attn = True # use flash attention, if on pytorch
-2.0 ) seq = torch.randint(0, 2000, (1, 1024)) out, mems1, states1 = model(seq)
-out, mems2, states2 = model(seq, xl_memories = mems1, states = states1) out,
-mems3, states3 = model(seq, xl_memories = mems2, states = states2) ``` ## Test
-on Enwik8 First `pip install -r requirements.txt`, then ```bash $ python
-train.py ``` ## Todo - [x] use dynamic positional bias - [x] add enhanced
-recurrence - [x] setup local attention blocks, as in the paper - [x] wrapper
-transformer class for training - [x] take care of generation with recurrence in
-`RecurrentTrainWrapper` - [x] add ability to dropout to entire memories and
-states during each segment step during trainng - [x] test full system on enwik8
-locally and ablate states and memories and see effects first hand - [x] make
-sure attention allow for single head key / values too - [x] run a few
-experiments of fixed gating in regular transformers - does not work - [x]
-integrate flash_attention - [x] cache attention mask + rotary embeddings - [x]
-add compressed_memories - [ ] revisit memformer - [ ] add ability to gate in
-memorizing transformers knn attention layers ## Citations ```bibtex @article
+also include flash_attention as well as routed memories of up to 250k tokens
+using ideas from this_paper ## Appreciation - Stability.ai for the generous
+sponsorship to work and open source cutting edge artificial intelligence
+research ## Install ```bash $ pip install block-recurrent-transformer-pytorch
+``` ## Usage ```python import torch from block_recurrent_transformer_pytorch
+import BlockRecurrentTransformer model = BlockRecurrentTransformer( num_tokens
+= 20000, # vocab size dim = 512, # model dimensions depth = 6, # depth dim_head
+= 64, # attention head dimensions heads = 8, # number of attention heads
+max_seq_len = 1024, # the total receptive field of the transformer, in the
+paper this was 2 * block size block_width = 512, # block size - total receptive
+field is max_seq_len, 2 * block size in paper. the block furthest forwards
+becomes the new cached xl memories, which is a block size of 1 (please open an
+issue if i am wrong) num_state_vectors = 512, # number of state vectors, i
+believe this was a single block size in the paper, but can be any amount
+recurrent_layers = (4,), # where to place the recurrent layer(s) for states
+with fixed simple gating use_compressed_mem = False, # whether to use
+compressed memories of a single block width, from https://arxiv.org/abs/
+1911.05507 compressed_mem_factor = 4, # compression factor of compressed
+memories use_flash_attn = True # use flash attention, if on pytorch 2.0 ) seq =
+torch.randint(0, 2000, (1, 1024)) out, mems1, states1 = model(seq) out, mems2,
+states2 = model(seq, xl_memories = mems1, states = states1) out, mems3, states3
+= model(seq, xl_memories = mems2, states = states2) ``` ## Test on Enwik8 First
+`pip install -r requirements.txt`, then ```bash $ python train.py ``` ## Todo -
+[x] use dynamic positional bias - [x] add enhanced recurrence - [x] setup local
+attention blocks, as in the paper - [x] wrapper transformer class for training
+- [x] take care of generation with recurrence in `RecurrentTrainWrapper` - [x]
+add ability to dropout to entire memories and states during each segment step
+during trainng - [x] test full system on enwik8 locally and ablate states and
+memories and see effects first hand - [x] make sure attention allow for single
+head key / values too - [x] run a few experiments of fixed gating in regular
+transformers - does not work - [x] integrate flash_attention - [x] cache
+attention mask + rotary embeddings - [x] add compressed_memories - [ ] revisit
+memformer - [ ] try routing long distance memories of up to 250k using
+coordinate descent (Wright et al.) ## Citations ```bibtex @article
 {Hutchins2022BlockRecurrentT, title = {Block-Recurrent Transformers}, author =
 {DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam
 Neyshabur}, journal = {ArXiv}, year = {2022}, volume = {abs/2203.07852} } ```
 ```bibtex @article{Shazeer2019FastTD, title = {Fast Transformer Decoding: One
 Write-Head is All You Need}, author = {Noam M. Shazeer}, journal = {ArXiv},
 year = {2019}, volume = {abs/1911.02150} } ``` ```bibtex @inproceedings
 {Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
 and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
 and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex
 @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
 Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
 Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` *Memory is Attention through Time* - Alex Graves
+} ``` ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-
+Range Transformers with Conditional Computation}, author = {Joshua Ainslie and
+Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
+Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
+and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` *Memory is Attention
+through Time* - Alex Graves
```

### Comparing `block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,14 @@
         assert start_len < self.max_seq_len
         assert length <= (self.max_seq_len + 1)
         assert start_len < length
 
         output = prime
 
         memories = []
-        states = []
 
         for ind in range(length - start_len):
 
             logits, next_memories, next_states = self.forward(
                 output,
                 xl_memories = xl_memories,
                 states = states
```

### Comparing `block-recurrent-transformer-pytorch-0.4.2/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.4.2/setup.py` & `block-recurrent-transformer-pytorch-0.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.2',
+  version = '0.4.3',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

