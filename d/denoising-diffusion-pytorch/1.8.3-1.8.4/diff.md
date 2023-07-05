# Comparing `tmp/denoising-diffusion-pytorch-1.8.3.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.3.tar", last modified: Thu Jun 22 15:50:42 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.4.tar", last modified: Wed Jul  5 18:31:54 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.3.tar` & `denoising-diffusion-pytorch-1.8.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36175 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36837 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.3/LICENSE` & `denoising-diffusion-pytorch-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/PKG-INFO` & `denoising-diffusion-pytorch-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.3
+Version: 1.8.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.3/README.md` & `denoising-diffusion-pytorch-1.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 ### 1D Sequence
 
 By popular request, a 1D Unet + Gaussian Diffusion implementation.
 
 ```python
 import torch
-from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D, Dataset1D
 
 model = Unet1D(
     dim = 64,
     dim_mults = (1, 2, 4, 8),
     channels = 32
 )
 
@@ -123,22 +123,24 @@
     model,
     seq_length = 128,
     timesteps = 1000,
     objective = 'pred_v'
 )
 
 training_seq = torch.rand(64, 32, 128) # features are normalized from 0 to 1
+dataset = Dataset1D(training_seq)  # this is just an example, but you can formulate your own Dataset and pass it into the `Trainer1D` below
+
 loss = diffusion(training_seq)
 loss.backward()
 
 # Or using trainer
 
 trainer = Trainer1D(
     diffusion,
-    dataset = training_seq,
+    dataset = dataset,
     train_batch_size = 32,
     train_lr = 8e-5,
     train_num_steps = 700000,         # total training steps
     gradient_accumulate_every = 2,    # gradient accumulation steps
     ema_decay = 0.995,                # exponential moving average decay
     amp = True,                       # turn on mixed precision
 )
```

#### html2text {}

```diff
@@ -32,21 +32,23 @@
 () ``` Samples and model checkpoints will be logged to `./results` periodically
 ## Multi-GPU Training The `Trainer` class is now equipped with ð¤
 Accelerator. You can easily do multi-gpu training in two steps using their
 `accelerate` CLI At the project root directory, where the training script is,
 run ```python $ accelerate config ``` Then, in the same directory ```python $
 accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
 request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
-from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
-model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
-GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000, objective =
-'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are normalized
-from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or using trainer
-trainer = Trainer1D( diffusion, dataset = training_seq, train_batch_size = 32,
-train_lr = 8e-5, train_num_steps = 700000, # total training steps
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D,
+Dataset1D model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 )
+diffusion = GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000,
+objective = 'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are
+normalized from 0 to 1 dataset = Dataset1D(training_seq) # this is just an
+example, but you can formulate your own Dataset and pass it into the
+`Trainer1D` below loss = diffusion(training_seq) loss.backward() # Or using
+trainer trainer = Trainer1D( diffusion, dataset = dataset, train_batch_size =
+32, train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
 trainer.train() # after a lot of training sampled_seq = diffusion.sample
 (batch_size = 4) sampled_seq.shape # (4, 32, 128) ``` `Trainer1D` does not
 evaluate the generated samples in any way since the type of data is not known.
 You could consider adding a suitable metric to the training loop yourself after
 doing an editable install of this package `pip install -e .`. ## Citations
```

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     return d() if callable(d) else d
 
 def cast_tuple(t, length = 1):
     if isinstance(t, tuple):
         return t
     return ((t,) * length)
 
+def divisible_by(numer, denom):
+    return (numer % denom) == 0
+
 def identity(t, *args, **kwargs):
     return t
 
 def cycle(dl):
     while True:
         for data in dl:
             yield data
@@ -121,15 +124,15 @@
 
 class RandomOrLearnedSinusoidalPosEmb(nn.Module):
     """ following @crowsonkb 's lead with random (learned optional) sinusoidal pos emb """
     """ https://github.com/crowsonkb/v-diffusion-jax/blob/master/diffusion/models/danbooru_128.py#L8 """
 
     def __init__(self, dim, is_random = False):
         super().__init__()
-        assert (dim % 2) == 0
+        assert divisible_by(dim, 2)
         half_dim = dim // 2
         self.weights = nn.Parameter(torch.randn(half_dim), requires_grad = not is_random)
 
     def forward(self, x):
         x = rearrange(x, 'b -> b 1')
         freqs = x * rearrange(self.weights, 'd -> 1 d') * 2 * math.pi
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
@@ -351,15 +354,21 @@
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
+    @property
+    def downsample_factor(self):
+        return 2 ** (len(self.downs) - 1)
+
     def forward(self, x, time, x_self_cond = None):
+        assert all([divisible_by(d, self.downsample_factor) for d in x.shape[-2:]]), f'your input dimensions {x.shape[-2:]} need to be divisible by {self.downsample_factor}, given the unet'
+
         if self.self_condition:
             x_self_cond = default(x_self_cond, lambda: torch.zeros_like(x))
             x = torch.cat((x_self_cond, x), dim = 1)
 
         x = self.init_conv(x)
         r = x.clone()
 
@@ -864,30 +873,30 @@
         self.channels = diffusion_model.channels
 
         # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
-        if save_best_and_latest_only:
-            assert calculate_fid, "`calculate_fid` must be True to provide a means for model evaluation for `save_best_and_latest_only`."
-            self.best_fid = 1e10 # infinite
-        self.save_best_and_latest_only = save_best_and_latest_only
 
         self.batch_size = train_batch_size
         self.gradient_accumulate_every = gradient_accumulate_every
+        assert (train_batch_size * gradient_accumulate_every) >= 16, f'your effective batch size (train_batch_size x gradient_accumulate_every) should be at least 16 or above'
 
         self.train_num_steps = train_num_steps
         self.image_size = diffusion_model.image_size
 
         self.max_grad_norm = max_grad_norm
 
         # dataset and dataloader
 
         self.ds = Dataset(folder, self.image_size, augment_horizontal_flip = augment_horizontal_flip, convert_image_to = convert_image_to)
+
+        assert len(self.ds) >= 100, 'you should have at least 100 images in your folder. at least 10k images recommended'
+
         dl = DataLoader(self.ds, batch_size = train_batch_size, shuffle = True, pin_memory = True, num_workers = cpu_count())
 
         dl = self.accelerator.prepare(dl)
         self.dl = cycle(dl)
 
         # optimizer
 
@@ -928,14 +937,20 @@
                 accelerator=self.accelerator,
                 stats_dir=results_folder,
                 device=self.device,
                 num_fid_samples=num_fid_samples,
                 inception_block_idx=inception_block_idx
             )
 
+        if save_best_and_latest_only:
+            assert calculate_fid, "`calculate_fid` must be True to provide a means for model evaluation for `save_best_and_latest_only`."
+            self.best_fid = 1e10 # infinite
+
+        self.save_best_and_latest_only = save_best_and_latest_only
+
     @property
     def device(self):
         return self.accelerator.device
 
     def save(self, milestone):
         if not self.accelerator.is_local_main_process:
             return
@@ -1001,15 +1016,15 @@
 
                 accelerator.wait_for_everyone()
 
                 self.step += 1
                 if accelerator.is_main_process:
                     self.ema.update()
 
-                    if self.step != 0 and self.step % self.save_and_sample_every == 0:
+                    if self.step != 0 and divisible_by(self.step, self.save_and_sample_every):
                         self.ema.ema_model.eval()
 
                         with torch.inference_mode():
                             milestone = self.step // self.save_and_sample_every
                             batches = num_to_groups(self.num_samples, self.batch_size)
                             all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
```

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.3
+Version: 1.8.4
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.3/setup.py` & `denoising-diffusion-pytorch-1.8.4/setup.py`

 * *Files identical despite different names*

