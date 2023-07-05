# Comparing `tmp/so_vits_svc_fork_mandarin-1.0.2.tar.gz` & `tmp/so_vits_svc_fork_mandarin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork_mandarin-1.0.2.tar", max compression
+gzip compressed data, was "so_vits_svc_fork_mandarin-1.0.3.tar", max compression
```

## Comparing `so_vits_svc_fork_mandarin-1.0.2.tar` & `so_vits_svc_fork_mandarin-1.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12686 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.2/LICENSE
--rw-r--r--   0        0        0     3290 2023-07-05 17:55:19.954951 so_vits_svc_fork_mandarin-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    29696 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.2/README.md
--rw-r--r--   0        0        0       75 2023-07-05 17:04:13.034805 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    25864 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1441 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     5055 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2962 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2691 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7506 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    31789 2023-07-05 17:54:29.286294 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      902 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    25441 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9690 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1215 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    17171 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4752 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1509 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       79 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11929 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      355 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      333 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      430 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     9198 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     5021 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5781 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4536 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1438 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1463 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5958 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14887 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8411 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2129 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1774 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1933 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     3070 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2796 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4824 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4591 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     3041 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     2284 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      131 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21930 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    16095 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    31274 1970-01-01 00:00:00.000000 so_vits_svc_fork_mandarin-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    12686 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3290 2023-07-05 18:11:46.948006 so_vits_svc_fork_mandarin-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    29696 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.3/README.md
+-rw-r--r--   0        0        0       75 2023-07-05 17:04:13.034805 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    25864 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1441 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     5055 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2962 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2691 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7506 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    31931 2023-07-05 18:10:14.908293 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      902 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9690 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1215 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    17171 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4752 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1509 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       79 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11929 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      355 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      333 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      430 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     9198 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     5021 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5781 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4536 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1438 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1463 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5958 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14887 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8411 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2129 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1774 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1933 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     3070 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2796 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4824 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4591 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     3041 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2284 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      131 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21930 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    16095 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    31274 1970-01-01 00:00:00.000000 so_vits_svc_fork_mandarin-1.0.3/PKG-INFO
```

### Comparing `so_vits_svc_fork_mandarin-1.0.2/LICENSE` & `so_vits_svc_fork_mandarin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/pyproject.toml` & `so_vits_svc_fork_mandarin-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork-mandarin"
-version = "1.0.2"
+version = "1.0.3"
 description = "A mandarin translation version of a fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/weihaozhaung/so-vits-svc-fork-mandarin"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork_mandarin-1.0.2/README.md` & `so_vits_svc_fork_mandarin-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
                     key="model_path",
                     default_text=model_candidates[-1].absolute().as_posix()
                     if model_candidates
                     else "",
                     enable_events=True,
                 ),
                 sg.FileBrowse(
+                    button_text="瀏覽",
                     initial_folder=Path("./logs/44k/").absolute
                     if Path("./logs/44k/").exists()
                     else Path(".").absolute().as_posix(),
                     key="model_path_browse",
                     file_types=(
                         ("PyTorch", "G_*.pth G_*.pt"),
                         ("Pytorch", "*.pth *.pt"),
@@ -210,14 +211,15 @@
                     key="config_path",
                     default_text=Path("./configs/44k/config.json").absolute().as_posix()
                     if Path("./configs/44k/config.json").exists()
                     else "",
                     enable_events=True,
                 ),
                 sg.FileBrowse(
+                    button_text="瀏覽",
                     initial_folder=Path("./configs/44k/").as_posix()
                     if Path("./configs/44k/").exists()
                     else Path(".").absolute().as_posix(),
                     key="config_path_browse",
                     file_types=(("JSON", "*.json"),),
                 ),
             ],
@@ -228,14 +230,15 @@
                     key="cluster_model_path",
                     default_text=Path("./logs/44k/kmeans.pt").absolute().as_posix()
                     if Path("./logs/44k/kmeans.pt").exists()
                     else "",
                     enable_events=True,
                 ),
                 sg.FileBrowse(
+                    button_text="瀏覽",
                     initial_folder="./logs/44k/"
                     if Path("./logs/44k/").exists()
                     else ".",
                     key="cluster_model_path_browse",
                     file_types=(("PyTorch", "*.pt"), ("Pickle", "*.pt *.pth *.pkl")),
                 ),
             ],
@@ -334,15 +337,15 @@
                     key="max_chunk_seconds",
                     resolution=1.0,
                 ),
             ],
             [
                 sg.Checkbox(
                     key="absolute_thresh",
-                    text="Absolute threshold (ignored (True) in realtime inference)",
+                    text="固定閾值（在即時變聲時此選項會被忽略並設為True）",
                 )
             ],
         ],
         "檔案": [
             [
                 sg.Text("要換聲音的檔案路徑"),
                 sg.Push(),
```

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork_mandarin-1.0.3/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork_mandarin-1.0.2/PKG-INFO` & `so_vits_svc_fork_mandarin-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork-mandarin
-Version: 1.0.2
+Version: 1.0.3
 Summary: A mandarin translation version of a fork of so-vits-svc.
 Home-page: https://github.com/weihaozhaung/so-vits-svc-fork-mandarin
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork-mandarin Version: 1.0.2 Summary: A
+Metadata-Version: 2.1 Name: so-vits-svc-fork-mandarin Version: 1.0.3 Summary: A
 mandarin translation version of a fork of so-vits-svc. Home-page: https://
 github.com/weihaozhaung/so-vits-svc-fork-mandarin License: MIT Author: 34j
 Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

