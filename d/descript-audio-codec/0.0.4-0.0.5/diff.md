# Comparing `tmp/descript-audio-codec-0.0.4.tar.gz` & `tmp/descript-audio-codec-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descript-audio-codec-0.0.4.tar", last modified: Wed Jun 21 17:49:04 2023, max compression
+gzip compressed data, was "descript-audio-codec-0.0.5.tar", last modified: Wed Jul  5 15:59:29 2023, max compression
```

## Comparing `descript-audio-codec-0.0.4.tar` & `descript-audio-codec-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/LICENSE
--rw-r--r--   0 ishaan    (1016) research  (1001)     6260 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)     5503 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/README.md
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/
--rw-r--r--   0 ishaan    (1016) research  (1001)      237 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.4/dac/__main__.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/compare/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/compare/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/compare/encodec.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/model/
--rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/base.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.4/dac/model/dac.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/discriminator.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/nn/
--rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/layers.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/loss.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.4/dac/nn/quantize.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/utils/
--rw-r--r--   0 ishaan    (1016) research  (1001)     2580 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     5891 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/decode.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     6357 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/encode.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/
--rw-r--r--   0 ishaan    (1016) research  (1001)     6260 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/SOURCES.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/dependency_links.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/requires.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/top_level.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/setup.cfg
--rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/setup.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/tests/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/tests/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2232 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/tests/test_cli.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/tests/test_train.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/LICENSE
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6342 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5585 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/README.md
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/
+-rw-r--r--   0 ishaan    (1016) research  (1001)      237 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.5/dac/__main__.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/compare/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/compare/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/compare/encodec.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/model/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/base.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.5/dac/model/dac.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/discriminator.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/dac/nn/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/layers.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/loss.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.5/dac/nn/quantize.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/dac/utils/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2783 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5901 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/decode.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6367 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/encode.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6342 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/requires.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/top_level.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/setup.cfg
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/setup.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/tests/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/tests/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2241 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/tests/test_cli.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/tests/test_train.py
```

### Comparing `descript-audio-codec-0.0.4/LICENSE` & `descript-audio-codec-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/PKG-INFO` & `descript-audio-codec-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.4
+Version: 0.0.5
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -49,20 +49,21 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+We release weights for models that can natively support 16 kHz, 24kHz, and 44.1kHz sampling rates.
 Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
 ```bash
 python3 -m dac download # downloads the default 44kHz variant
 python3 -m dac download --model_type 44khz # downloads the 44kHz variant
 python3 -m dac download --model_type 24khz # downloads the 24kHz variant
+python3 -m dac download --model_type 16khz # downloads the 16kHz variant
 ```
 We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
```

### Comparing `descript-audio-codec-0.0.4/README.md` & `descript-audio-codec-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,21 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+We release weights for models that can natively support 16 kHz, 24kHz, and 44.1kHz sampling rates.
 Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
 ```bash
 python3 -m dac download # downloads the default 44kHz variant
 python3 -m dac download --model_type 44khz # downloads the 44kHz variant
 python3 -m dac download --model_type 24khz # downloads the 24kHz variant
+python3 -m dac download --model_type 16khz # downloads the 16kHz variant
 ```
 We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
```

### Comparing `descript-audio-codec-0.0.4/dac/__main__.py` & `descript-audio-codec-0.0.5/dac/__main__.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/compare/encodec.py` & `descript-audio-codec-0.0.5/dac/compare/encodec.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/model/base.py` & `descript-audio-codec-0.0.5/dac/model/base.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/model/dac.py` & `descript-audio-codec-0.0.5/dac/model/dac.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/model/discriminator.py` & `descript-audio-codec-0.0.5/dac/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/nn/layers.py` & `descript-audio-codec-0.0.5/dac/nn/layers.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/nn/loss.py` & `descript-audio-codec-0.0.5/dac/nn/loss.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/nn/quantize.py` & `descript-audio-codec-0.0.5/dac/nn/quantize.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/dac/utils/__init__.py` & `descript-audio-codec-0.0.5/dac/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,52 +7,58 @@
 
 DAC = dac.model.DAC
 Accelerator = ml.Accelerator
 
 __MODEL_LATEST_TAGS__ = {
     "44khz": "0.0.1",
     "24khz": "0.0.4",
+    "16khz": "0.0.5",
 }
 
 __MODEL_URLS__ = {
     (
         "44khz",
         "0.0.1",
     ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.1/weights.pth",
     (
         "24khz",
         "0.0.4",
     ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.4/weights_24khz.pth",
+    (
+        "16khz",
+        "0.0.5",
+    ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.5/weights_16khz.pth",
 }
 
 
 @argbind.bind(group="download", positional=True, without_prefix=True)
 def ensure_default_model(tag: str = "latest", model_type: str = "44khz"):
     """
     Function that downloads the weights file from URL if a local cache is not found.
 
     Parameters
     ----------
     tag : str
         The tag of the model to download. Defaults to "latest".
     model_type : str
-        The type of model to download. Must be one of "44khz" or "24khz". Defaults to "44khz".
+        The type of model to download. Must be one of "44khz", "24khz", or "16khz". Defaults to "44khz".
 
     Returns
     -------
     Path
         Directory path required to load model via audiotools.
     """
     model_type = model_type.lower()
     tag = tag.lower()
 
     assert model_type in [
         "44khz",
         "24khz",
-    ], "model_type must be one of '44khz' or '24khz'"
+        "16khz",
+    ], "model_type must be one of '44khz', '24khz', or '16khz'"
 
     if tag == "latest":
         tag = __MODEL_LATEST_TAGS__[model_type]
 
     download_link = __MODEL_URLS__.get((model_type, tag), None)
 
     if download_link is None:
```

### Comparing `descript-audio-codec-0.0.4/dac/utils/decode.py` & `descript-audio-codec-0.0.5/dac/utils/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     model_tag : str, optional
         Tag of the model to use, by default "latest". Ignored if `weights_path` is specified.
     preserve_sample_rate : bool, optional
         If True, return audio will have the same sample rate as the original
     device : str, optional
         Device to use, by default "cuda". If "cpu", the model will be loaded on the CPU.
     model_type : str, optional
-        The type of model to download. Must be one of "44khz" or "24khz". Defaults to "44khz". Ignored if `weights_path` is specified.
+        The type of model to download. Must be one of "44khz", "24khz", or "16khz". Defaults to "44khz". Ignored if `weights_path` is specified.
     """
     generator = load_model(
         tag=model_tag,
         load_path=weights_path,
         model_type=model_type,
     )
     generator.to(device)
```

### Comparing `descript-audio-codec-0.0.4/dac/utils/encode.py` & `descript-audio-codec-0.0.5/dac/utils/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     model_tag : str, optional
         Tag of the model to use, by default "latest". Ignored if `weights_path` is specified.
     n_quantizers : int, optional
         Number of quantizers to use, by default None. If not specified, all the quantizers will be used and the model will compress at maximum bitrate.
     device : str, optional
         Device to use, by default "cuda"
     model_type : str, optional
-        The type of model to download. Must be one of "44khz" or "24khz". Defaults to "44khz". Ignored if `weights_path` is specified.
+        The type of model to download. Must be one of "44khz", "24khz", or "16khz". Defaults to "44khz". Ignored if `weights_path` is specified.
     """
     generator = load_model(
         tag=model_tag,
         load_path=weights_path,
         model_type=model_type,
     )
     generator.to(device)
```

### Comparing `descript-audio-codec-0.0.4/descript_audio_codec.egg-info/PKG-INFO` & `descript-audio-codec-0.0.5/descript_audio_codec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.4
+Version: 0.0.5
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -49,20 +49,21 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+We release weights for models that can natively support 16 kHz, 24kHz, and 44.1kHz sampling rates.
 Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
 ```bash
 python3 -m dac download # downloads the default 44kHz variant
 python3 -m dac download --model_type 44khz # downloads the 44kHz variant
 python3 -m dac download --model_type 24khz # downloads the 24kHz variant
+python3 -m dac download --model_type 16khz # downloads the 16kHz variant
 ```
 We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
```

### Comparing `descript-audio-codec-0.0.4/descript_audio_codec.egg-info/SOURCES.txt` & `descript-audio-codec-0.0.5/descript_audio_codec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.4/setup.py` & `descript-audio-codec-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="descript-audio-codec",
-    version="0.0.4",
+    version="0.0.5",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Topic :: Artistic Software",
         "Topic :: Multimedia",
         "Topic :: Multimedia :: Sound/Audio",
```

### Comparing `descript-audio-codec-0.0.4/tests/test_cli.py` & `descript-audio-codec-0.0.5/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def teardown_module(module):
     repo_root = Path(__file__).parent.parent
     subprocess.check_output(["rm", "-rf", f"{repo_root}/tests/assets"])
 
 
-@pytest.mark.parametrize("model_type", ["44khz", "24khz"])
+@pytest.mark.parametrize("model_type", ["44khz", "24khz", "16khz"])
 def test_reconstruction(model_type):
     # Test encoding
     input_dir = Path(__file__).parent / "assets" / "input"
     output_dir = input_dir.parent / model_type / "encoded_output"
     args = {
         "input": str(input_dir),
         "output": str(output_dir),
```

### Comparing `descript-audio-codec-0.0.4/tests/test_train.py` & `descript-audio-codec-0.0.5/tests/test_train.py`

 * *Files identical despite different names*

