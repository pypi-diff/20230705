# Comparing `tmp/so-vits-svc-fork-mandarin-0.0.0.tar.gz` & `tmp/so_vits_svc_fork_mandarin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so-vits-svc-fork-mandarin-0.0.0.tar", last modified: Wed Jul  5 16:48:01 2023, max compression
+gzip compressed data, was "so_vits_svc_fork_mandarin-1.0.1.tar", max compression
```

## Comparing `so-vits-svc-fork-mandarin-0.0.0.tar` & `so_vits_svc_fork_mandarin-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.894713 so-vits-svc-fork-mandarin-0.0.0/
--rw-rw-rw-   0        0        0    12686 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      127 2023-07-05 16:48:01.894713 so-vits-svc-fork-mandarin-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    29387 2023-07-05 16:21:43.000000 so-vits-svc-fork-mandarin-0.0.0/README.md
--rw-rw-rw-   0        0        0     3229 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 16:48:01.894713 so-vits-svc-fork-mandarin-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-07-05 16:47:49.000000 so-vits-svc-fork-mandarin-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.841355 so-vits-svc-fork-mandarin-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.853427 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/
--rw-rw-rw-   0        0        0       75 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/__init__.py
--rw-rw-rw-   0        0        0    25864 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.855427 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/cluster/
--rw-rw-rw-   0        0        0     1441 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/cluster/__init__.py
--rw-rw-rw-   0        0        0     5055 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-rw-rw-   0        0        0     2962 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/dataset.py
--rw-rw-rw-   0        0        0     7506 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/f0.py
--rw-rw-rw-   0        0        0    31751 2023-07-05 16:06:08.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/gui.py
--rw-rw-rw-   0        0        0      902 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/hparams.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.858487 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/
--rw-rw-rw-   0        0        0        0 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/__init__.py
--rw-rw-rw-   0        0        0    25441 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/core.py
--rw-rw-rw-   0        0        0     9690 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/main.py
--rw-rw-rw-   0        0        0     1215 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.867550 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/
--rw-rw-rw-   0        0        0        0 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/__init__.py
--rw-rw-rw-   0        0        0    17171 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/attentions.py
--rw-rw-rw-   0        0        0     4752 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/commons.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.869552 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/
--rw-rw-rw-   0        0        0        0 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/f0.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.871552 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/
--rw-rw-rw-   0        0        0       79 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-rw-rw-   0        0        0    11929 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-rw-rw-   0        0        0      355 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.877622 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/
--rw-rw-rw-   0        0        0      333 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-rw-rw-   0        0        0    12853 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-rw-rw-   0        0        0      430 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-rw-rw-   0        0        0     4853 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-rw-rw-   0        0        0     9198 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-rw-rw-   0        0        0     5021 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-rw-rw-   0        0        0     5781 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/descriminators.py
--rw-rw-rw-   0        0        0     4536 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/encoders.py
--rw-rw-rw-   0        0        0     1438 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/flows.py
--rw-rw-rw-   0        0        0     1463 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/losses.py
--rw-rw-rw-   0        0        0     5958 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/mel_processing.py
--rw-rw-rw-   0        0        0    14887 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/modules.py
--rw-rw-rw-   0        0        0     8411 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/synthesizers.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.884623 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-rw-rw-   0        0        0     2796 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-rw-rw-   0        0        0     4824 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-rw-rw-   0        0        0     4591 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-rw-rw-   0        0        0     3041 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-rw-rw-   0        0        0     2284 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-rw-rw-   0        0        0      131 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-rw-rw-   0        0        0    21930 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/train.py
--rw-rw-rw-   0        0        0    16095 2023-07-05 15:08:45.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:48:01.893713 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork_mandarin.egg-info/
--rw-rw-rw-   0        0        0      127 2023-07-05 16:48:01.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork_mandarin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2023-07-05 16:48:01.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork_mandarin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 16:48:01.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork_mandarin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 16:48:01.000000 so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork_mandarin.egg-info/top_level.txt
+-rw-r--r--   0        0        0    12686 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3290 2023-07-05 17:21:25.480614 so_vits_svc_fork_mandarin-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    29696 2023-07-05 17:04:13.026630 so_vits_svc_fork_mandarin-1.0.1/README.md
+-rw-r--r--   0        0        0       75 2023-07-05 17:04:13.034805 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    25864 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1441 2023-07-05 17:04:13.035793 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     5055 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2962 2023-07-05 17:04:13.036804 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2691 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7506 2023-07-05 17:04:13.037914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    31775 2023-07-05 17:14:28.940182 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      902 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.038914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9690 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1215 2023-07-05 17:04:13.039914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    17171 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4752 2023-07-05 17:04:13.040914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1509 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       79 2023-07-05 17:04:13.041914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11929 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      355 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      333 2023-07-05 17:04:13.042914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      430 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4853 2023-07-05 17:04:13.043914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     9198 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     5021 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5781 2023-07-05 17:04:13.044914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4536 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1438 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1463 2023-07-05 17:04:13.045914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5958 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14887 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8411 2023-07-05 17:04:13.046914 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2129 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1774 2023-07-05 17:04:13.048018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1933 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     3070 2023-07-05 17:04:13.049018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2796 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4824 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4591 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     3041 2023-07-05 17:04:13.050018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2284 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      131 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:04:13.051018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21930 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    16095 2023-07-05 17:04:13.052018 so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    31274 1970-01-01 00:00:00.000000 so_vits_svc_fork_mandarin-1.0.1/PKG-INFO
```

### Comparing `so-vits-svc-fork-mandarin-0.0.0/LICENSE` & `so_vits_svc_fork_mandarin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/README.md` & `so_vits_svc_fork_mandarin-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-# SoftVC VITS Singing Voice Conversion Fork
-
-[简体中文](README_zh_CN.md)
-
-<p align="center">
-  <a href="https://github.com/34j/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
-    <img src="https://img.shields.io/github/actions/workflow/status/34j/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
-  </a>
-  <a href="https://so-vits-svc-fork.readthedocs.io">
-    <img src="https://img.shields.io/readthedocs/so-vits-svc-fork.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
-  </a>
-  <a href="https://codecov.io/gh/34j/so-vits-svc-fork">
-    <img src="https://img.shields.io/codecov/c/github/34j/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
-  </a>
-</p>
-<p align="center">
-  <a href="https://python-poetry.org/">
-    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
-  </a>
-  <a href="https://github.com/ambv/black">
-    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
-  </a>
-  <a href="https://github.com/pre-commit/pre-commit">
-    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
-  </a>
-</p>
-<p align="center">
-  <a href="https://pypi.org/project/so-vits-svc-fork/">
-    <img src="https://img.shields.io/pypi/v/so-vits-svc-fork.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
-  </a>
-  <img src="https://img.shields.io/pypi/pyversions/so-vits-svc-fork.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
-  <img src="https://img.shields.io/pypi/l/so-vits-svc-fork.svg?style=flat-square" alt="License">
-</p>
-
-A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with **realtime support** and **greatly improved interface**. Based on branch `4.0` (v1) (or `4.1`) and the models are compatible.
-
-## Features not available in the original repo
-
-- **Realtime voice conversion** (enhanced in v1.1.0)
-- Integrates [`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion)
-- Fixed misuse of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original repository.[^c]
-- More accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/).
-- GUI and unified CLI available
-- ~2x faster training
-- Ready to use just by installing with `pip`.
-- Automatically download pretrained models. No need to install `fairseq`.
-- Code completely formatted with black, isort, autoflake etc.
-
-[^c]: [#206](https://github.com/34j/so-vits-svc-fork/issues/206)
-
-## Installation
-
-### One click easy installation
-
-<a href="https://github.com/34j/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
-  <img src="https://img.shields.io/badge/.bat-download-blue?style=flat-square&logo=windows" alt="Download .bat">
-</a>
-
-This BAT file will automatically perform the steps described below.
-
-### Manual installation
-
-<details>
-  <summary>Creating a virtual environment</summary>
-
-Windows:
-
-```shell
-py -3.10 -m venv venv
-venv\Scripts\activate
-```
-
-Linux/MacOS:
-
-```shell
-python3.10 -m venv venv
-source venv/bin/activate
-```
-
-Anaconda:
-
-```shell
-conda create -n so-vits-svc-fork python=3.10 pip
-conda activate so-vits-svc-fork
-```
-
-Installing without creating a virtual environment may cause a `PermissionError` if Python is installed in Program Files, etc.
-
-</details>
-
-Install this via pip (or your favourite package manager that uses pip):
-
-```shell
-python -m pip install -U pip setuptools wheel
-pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118
-pip install -U so-vits-svc-fork
-```
-
-<details>
-  <summary>Notes</summary>
-
-- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118`. MPS is probably supported.
-- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url https://download.pytorch.org/whl/rocm5.4.2`. AMD GPUs are not supported on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)).
-  </details>
-
-### Update
-
-Please update this package regularly to get the latest features and bug fixes.
-
-```shell
-pip install -U so-vits-svc-fork
-```
-
-## Usage
-
-### Inference
-
-#### GUI
-
-![GUI](https://raw.githubusercontent.com/34j/so-vits-svc-fork/main/docs/_static/gui.png)
-
-GUI launches with the following command:
-
-```shell
-svcg
-```
-
-#### CLI
-
-- Realtime (from microphone)
-
-```shell
-svc vc
-```
-
-- File
-
-```shell
-svc infer source.wav
-```
-
-Pretrained models are available on [Hugging Face](https://huggingface.co/models?search=so-vits-svc) or [CIVITAI](https://civitai.com/?query=so-vits-svc).
-
-#### Notes
-
-- If using WSL, please note that WSL requires additional setup to handle audio and the GUI will not work without finding an audio device.
-- In real-time inference, if there is noise on the inputs, the HuBERT model will react to those as well. Consider using realtime noise reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this case.
-- Models other than for 4.0v1 or this repository are not supported.
-- GPU inference requires at least 4 GB of VRAM. If it does not work, try CPU inference as it is fast enough. [^r-inference]
-
-[^r-inference]: [#469](https://github.com/voicepaw/so-vits-svc-fork/issues/469)
-
-### Training
-
-#### Before training
-
-- If your dataset has BGM, please remove the BGM using software such as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1]
-- If your dataset is a long audio file with a single speaker, use `svc pre-split` to split the dataset into multiple files (using `librosa`).
-- If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
-- To manually classify audio files, `svc pre-classify` is available. Up and down arrow keys can be used to change the playback speed.
-
-[^1]: https://ytpmv.info/how-to-use-uvr/
-
-#### Cloud
-
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
-[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
-[![Paperspace Referral](<https://img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p]
-
-If you do not have access to a GPU with more than 10 GB of VRAM, the free plan of Google Colab is recommended for light users and the Pro/Growth plan of Paperspace is recommended for heavy users. Conversely, if you have access to a high-end GPU, the use of cloud services is not recommended.
-
-[^p]: If you register a referral code and then add a payment method, you may save about $5 on your first month's monthly billing. Note that both referral rewards are Paperspace credits and not cash. It was a tough decision but inserted because debugging and training the initial model requires a large amount of computing power and the developer is a student.
-
-#### Local
-
-Place your dataset like `dataset_raw/{speaker_id}/**/{wav_file}.{any_format}` (subfolders and non-ASCII filenames are acceptable) and run:
-
-```shell
-svc pre-resample
-svc pre-config
-svc pre-hubert
-svc train -t
-```
-
-#### Notes
-
-- Dataset audio duration per file should be <~ 10s.
-- Need at least 4GB of VRAM. [^r-training]
-- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
-- To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
-- To use `ContentVec` correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may take slightly longer because some weights are reset due to reusing legacy initial generator weights.
-- To use `MS-iSTFT Decoder`, replace `svc pre-config` with `svc pre-config -t quickvc`.
-- Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
-- If you have trained on a large, copyright-free dataset, consider releasing it as an initial model.
-- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or [Discussions](https://github.com/34j/so-vits-svc-fork/discussions).
-
-[^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456)
-
-### Further help
-
-For more details, run `svc -h` or `svc <subcommand> -h`.
-
-```shell
-> svc -h
-Usage: svc [OPTIONS] COMMAND [ARGS]...
-
-  so-vits-svc allows any folder structure for training data.
-  However, the following folder structure is recommended.
-      When training: dataset_raw/{speaker_name}/**/{wav_name}.{any_format}
-      When inference: configs/44k/config.json, logs/44k/G_XXXX.pth
-  If the folder structure is followed, you DO NOT NEED TO SPECIFY model path, config path, etc.
-  (The latest model will be automatically loaded.)
-  To train a model, run pre-resample, pre-config, pre-hubert, train.
-  To infer a model, run infer.
-
-Options:
-  -h, --help  Show this message and exit.
-
-Commands:
-  clean          Clean up files, only useful if you are using the default file structure
-  infer          Inference
-  onnx           Export model to onnx (currently not working)
-  pre-classify   Classify multiple audio files into multiple files
-  pre-config     Preprocessing part 2: config
-  pre-hubert     Preprocessing part 3: hubert If the HuBERT model is not found, it will be...
-  pre-resample   Preprocessing part 1: resample
-  pre-sd         Speech diarization using pyannote.audio
-  pre-split      Split audio files into multiple files
-  train          Train model If D_0.pth or G_0.pth not found, automatically download from hub.
-  train-cluster  Train k-means clustering
-  vc             Realtime inference from microphone
-```
-
-#### External Links
-
-[Video Tutorial](https://www.youtube.com/watch?v=tZn0lcGO5OQ)
-
-## Contributors ✨
-
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-
-<!-- prettier-ignore-start -->
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/34j"><img src="https://avatars.githubusercontent.com/u/55338215?v=4?s=80" width="80px;" alt="34j"/><br /><sub><b>34j</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Code">💻</a> <a href="#ideas-34j" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Documentation">📖</a> <a href="#example-34j" title="Examples">💡</a> <a href="#infra-34j" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-34j" title="Maintenance">🚧</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/pulls?q=is%3Apr+reviewed-by%3A34j" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Tests">⚠️</a> <a href="#tutorial-34j" title="Tutorials">✅</a> <a href="#promotion-34j" title="Promotion">📣</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3A34j" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GarrettConway"><img src="https://avatars.githubusercontent.com/u/22782004?v=4?s=80" width="80px;" alt="GarrettConway"/><br /><sub><b>GarrettConway</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=GarrettConway" title="Code">💻</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AGarrettConway" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=GarrettConway" title="Documentation">📖</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/pulls?q=is%3Apr+reviewed-by%3AGarrettConway" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BlueAmulet"><img src="https://avatars.githubusercontent.com/u/43395286?v=4?s=80" width="80px;" alt="BlueAmulet"/><br /><sub><b>BlueAmulet</b></sub></a><br /><a href="#ideas-BlueAmulet" title="Ideas, Planning, & Feedback">🤔</a> <a href="#question-BlueAmulet" title="Answering Questions">💬</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=BlueAmulet" title="Code">💻</a> <a href="#maintenance-BlueAmulet" title="Maintenance">🚧</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ThrowawayAccount01"><img src="https://avatars.githubusercontent.com/u/125531852?v=4?s=80" width="80px;" alt="ThrowawayAccount01"/><br /><sub><b>ThrowawayAccount01</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AThrowawayAccount01" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MashiroSA"><img src="https://avatars.githubusercontent.com/u/40637516?v=4?s=80" width="80px;" alt="緋"/><br /><sub><b>緋</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=MashiroSA" title="Documentation">📖</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AMashiroSA" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Lordmau5"><img src="https://avatars.githubusercontent.com/u/1345036?v=4?s=80" width="80px;" alt="Lordmau5"/><br /><sub><b>Lordmau5</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ALordmau5" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Lordmau5" title="Code">💻</a> <a href="#ideas-Lordmau5" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-Lordmau5" title="Maintenance">🚧</a> <a href="#question-Lordmau5" title="Answering Questions">💬</a> <a href="#userTesting-Lordmau5" title="User Testing">📓</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DL909"><img src="https://avatars.githubusercontent.com/u/71912115?v=4?s=80" width="80px;" alt="DL909"/><br /><sub><b>DL909</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADL909" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Satisfy256"><img src="https://avatars.githubusercontent.com/u/101394399?v=4?s=80" width="80px;" alt="Satisfy256"/><br /><sub><b>Satisfy256</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ASatisfy256" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pierluigizagaria"><img src="https://avatars.githubusercontent.com/u/57801386?v=4?s=80" width="80px;" alt="Pierluigi Zagaria"/><br /><sub><b>Pierluigi Zagaria</b></sub></a><br /><a href="#userTesting-pierluigizagaria" title="User Testing">📓</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruckusmattster"><img src="https://avatars.githubusercontent.com/u/77196088?v=4?s=80" width="80px;" alt="ruckusmattster"/><br /><sub><b>ruckusmattster</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aruckusmattster" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Desuka-art"><img src="https://avatars.githubusercontent.com/u/111822082?v=4?s=80" width="80px;" alt="Desuka-art"/><br /><sub><b>Desuka-art</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADesuka-art" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/heyfixit"><img src="https://avatars.githubusercontent.com/u/41658450?v=4?s=80" width="80px;" alt="heyfixit"/><br /><sub><b>heyfixit</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=heyfixit" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://www.youtube.com/c/NerdyRodent"><img src="https://avatars.githubusercontent.com/u/74688049?v=4?s=80" width="80px;" alt="Nerdy Rodent"/><br /><sub><b>Nerdy Rodent</b></sub></a><br /><a href="#video-nerdyrodent" title="Videos">📹</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/xieyumc"><img src="https://avatars.githubusercontent.com/u/47858007?v=4?s=80" width="80px;" alt="谢宇"/><br /><sub><b>谢宇</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=xieyumc" title="Documentation">📖</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ColdCawfee"><img src="https://avatars.githubusercontent.com/u/79474598?v=4?s=80" width="80px;" alt="ColdCawfee"/><br /><sub><b>ColdCawfee</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AColdCawfee" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sbersier"><img src="https://avatars.githubusercontent.com/u/34165937?v=4?s=80" width="80px;" alt="sbersier"/><br /><sub><b>sbersier</b></sub></a><br /><a href="#ideas-sbersier" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-sbersier" title="User Testing">📓</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Asbersier" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Meldoner"><img src="https://avatars.githubusercontent.com/u/43951115?v=4?s=80" width="80px;" alt="Meldoner"/><br /><sub><b>Meldoner</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AMeldoner" title="Bug reports">🐛</a> <a href="#ideas-Meldoner" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Meldoner" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mmodeusher"><img src="https://avatars.githubusercontent.com/u/46575920?v=4?s=80" width="80px;" alt="mmodeusher"/><br /><sub><b>mmodeusher</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Ammodeusher" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AlonDan"><img src="https://avatars.githubusercontent.com/u/21152334?v=4?s=80" width="80px;" alt="AlonDan"/><br /><sub><b>AlonDan</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AAlonDan" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Likkkez"><img src="https://avatars.githubusercontent.com/u/44336181?v=4?s=80" width="80px;" alt="Likkkez"/><br /><sub><b>Likkkez</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ALikkkez" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DuctTapeGames"><img src="https://avatars.githubusercontent.com/u/84365142?v=4?s=80" width="80px;" alt="Duct Tape Games"/><br /><sub><b>Duct Tape Games</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADuctTapeGames" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://tec.hxlxz.com/"><img src="https://avatars.githubusercontent.com/u/6624983?v=4?s=80" width="80px;" alt="Xianglong He"/><br /><sub><b>Xianglong He</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Ahxl9654" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/75aosu"><img src="https://avatars.githubusercontent.com/u/79185331?v=4?s=80" width="80px;" alt="75aosu"/><br /><sub><b>75aosu</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3A75aosu" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tonyco82"><img src="https://avatars.githubusercontent.com/u/56610534?v=4?s=80" width="80px;" alt="tonyco82"/><br /><sub><b>tonyco82</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Atonyco82" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yxlllc"><img src="https://avatars.githubusercontent.com/u/33565655?v=4?s=80" width="80px;" alt="yxlllc"/><br /><sub><b>yxlllc</b></sub></a><br /><a href="#ideas-yxlllc" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=yxlllc" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/outhipped"><img src="https://avatars.githubusercontent.com/u/116147475?v=4?s=80" width="80px;" alt="outhipped"/><br /><sub><b>outhipped</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aouthipped" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/escoolioinglesias"><img src="https://avatars.githubusercontent.com/u/73505402?v=4?s=80" width="80px;" alt="escoolioinglesias"/><br /><sub><b>escoolioinglesias</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aescoolioinglesias" title="Bug reports">🐛</a> <a href="#userTesting-escoolioinglesias" title="User Testing">📓</a> <a href="#video-escoolioinglesias" title="Videos">📹</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Blacksingh"><img src="https://avatars.githubusercontent.com/u/130872856?v=4?s=80" width="80px;" alt="Blacksingh"/><br /><sub><b>Blacksingh</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ABlacksingh" title="Bug reports">🐛</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="http://tybantarnusa.com"><img src="https://avatars.githubusercontent.com/u/9532857?v=4?s=80" width="80px;" alt="Mgs. M. Thoyib Antarnusa"/><br /><sub><b>Mgs. M. Thoyib Antarnusa</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Atybantarnusa" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ZeroHackz"><img src="https://avatars.githubusercontent.com/u/15729496?v=4?s=80" width="80px;" alt="Exosfeer"/><br /><sub><b>Exosfeer</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AZeroHackz" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=ZeroHackz" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/guranon"><img src="https://avatars.githubusercontent.com/u/130421189?v=4?s=80" width="80px;" alt="guranon"/><br /><sub><b>guranon</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aguranon" title="Bug reports">🐛</a> <a href="#ideas-guranon" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=guranon" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexanderkoumis"><img src="https://avatars.githubusercontent.com/u/5108856?v=4?s=80" width="80px;" alt="Alexander Koumis"/><br /><sub><b>Alexander Koumis</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=alexanderkoumis" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://www.meimadix.com"><img src="https://avatars.githubusercontent.com/u/653972?v=4?s=80" width="80px;" alt="Roee Shenberg"/><br /><sub><b>Roee Shenberg</b></sub></a><br /><a href="#userTesting-shenberg" title="User Testing">📓</a> <a href="#ideas-shenberg" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=shenberg" title="Code">💻</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-<!-- prettier-ignore-end -->
-
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+# SoftVC VITS Singing Voice Conversion Fork
+
+[简体中文](README_zh_CN.md)
+
+<p align="center">
+  <a href="https://github.com/34j/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/34j/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://so-vits-svc-fork.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/so-vits-svc-fork.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/34j/so-vits-svc-fork">
+    <img src="https://img.shields.io/codecov/c/github/34j/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/so-vits-svc-fork/">
+    <img src="https://img.shields.io/pypi/v/so-vits-svc-fork.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/so-vits-svc-fork.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/so-vits-svc-fork.svg?style=flat-square" alt="License">
+</p>
+
+A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with **realtime support** and **greatly improved interface**. Based on branch `4.0` (v1) (or `4.1`) and the models are compatible.
+
+## Features not available in the original repo
+
+- **Realtime voice conversion** (enhanced in v1.1.0)
+- Integrates [`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion)
+- Fixed misuse of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original repository.[^c]
+- More accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/).
+- GUI and unified CLI available
+- ~2x faster training
+- Ready to use just by installing with `pip`.
+- Automatically download pretrained models. No need to install `fairseq`.
+- Code completely formatted with black, isort, autoflake etc.
+
+[^c]: [#206](https://github.com/34j/so-vits-svc-fork/issues/206)
+
+## Installation
+
+### One click easy installation
+
+<a href="https://github.com/34j/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
+  <img src="https://img.shields.io/badge/.bat-download-blue?style=flat-square&logo=windows" alt="Download .bat">
+</a>
+
+This BAT file will automatically perform the steps described below.
+
+### Manual installation
+
+<details>
+  <summary>Creating a virtual environment</summary>
+
+Windows:
+
+```shell
+py -3.10 -m venv venv
+venv\Scripts\activate
+```
+
+Linux/MacOS:
+
+```shell
+python3.10 -m venv venv
+source venv/bin/activate
+```
+
+Anaconda:
+
+```shell
+conda create -n so-vits-svc-fork python=3.10 pip
+conda activate so-vits-svc-fork
+```
+
+Installing without creating a virtual environment may cause a `PermissionError` if Python is installed in Program Files, etc.
+
+</details>
+
+Install this via pip (or your favourite package manager that uses pip):
+
+```shell
+python -m pip install -U pip setuptools wheel
+pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118
+pip install -U so-vits-svc-fork
+```
+
+<details>
+  <summary>Notes</summary>
+
+- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118`. MPS is probably supported.
+- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url https://download.pytorch.org/whl/rocm5.4.2`. AMD GPUs are not supported on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)).
+  </details>
+
+### Update
+
+Please update this package regularly to get the latest features and bug fixes.
+
+```shell
+pip install -U so-vits-svc-fork
+```
+
+## Usage
+
+### Inference
+
+#### GUI
+
+![GUI](https://raw.githubusercontent.com/34j/so-vits-svc-fork/main/docs/_static/gui.png)
+
+GUI launches with the following command:
+
+```shell
+svcg
+```
+
+#### CLI
+
+- Realtime (from microphone)
+
+```shell
+svc vc
+```
+
+- File
+
+```shell
+svc infer source.wav
+```
+
+Pretrained models are available on [Hugging Face](https://huggingface.co/models?search=so-vits-svc) or [CIVITAI](https://civitai.com/?query=so-vits-svc).
+
+#### Notes
+
+- If using WSL, please note that WSL requires additional setup to handle audio and the GUI will not work without finding an audio device.
+- In real-time inference, if there is noise on the inputs, the HuBERT model will react to those as well. Consider using realtime noise reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this case.
+- Models other than for 4.0v1 or this repository are not supported.
+- GPU inference requires at least 4 GB of VRAM. If it does not work, try CPU inference as it is fast enough. [^r-inference]
+
+[^r-inference]: [#469](https://github.com/voicepaw/so-vits-svc-fork/issues/469)
+
+### Training
+
+#### Before training
+
+- If your dataset has BGM, please remove the BGM using software such as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1]
+- If your dataset is a long audio file with a single speaker, use `svc pre-split` to split the dataset into multiple files (using `librosa`).
+- If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
+- To manually classify audio files, `svc pre-classify` is available. Up and down arrow keys can be used to change the playback speed.
+
+[^1]: https://ytpmv.info/how-to-use-uvr/
+
+#### Cloud
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
+[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
+[![Paperspace Referral](<https://img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p]
+
+If you do not have access to a GPU with more than 10 GB of VRAM, the free plan of Google Colab is recommended for light users and the Pro/Growth plan of Paperspace is recommended for heavy users. Conversely, if you have access to a high-end GPU, the use of cloud services is not recommended.
+
+[^p]: If you register a referral code and then add a payment method, you may save about $5 on your first month's monthly billing. Note that both referral rewards are Paperspace credits and not cash. It was a tough decision but inserted because debugging and training the initial model requires a large amount of computing power and the developer is a student.
+
+#### Local
+
+Place your dataset like `dataset_raw/{speaker_id}/**/{wav_file}.{any_format}` (subfolders and non-ASCII filenames are acceptable) and run:
+
+```shell
+svc pre-resample
+svc pre-config
+svc pre-hubert
+svc train -t
+```
+
+#### Notes
+
+- Dataset audio duration per file should be <~ 10s.
+- Need at least 4GB of VRAM. [^r-training]
+- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
+- To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
+- To use `ContentVec` correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may take slightly longer because some weights are reset due to reusing legacy initial generator weights.
+- To use `MS-iSTFT Decoder`, replace `svc pre-config` with `svc pre-config -t quickvc`.
+- Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
+- If you have trained on a large, copyright-free dataset, consider releasing it as an initial model.
+- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or [Discussions](https://github.com/34j/so-vits-svc-fork/discussions).
+
+[^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456)
+
+### Further help
+
+For more details, run `svc -h` or `svc <subcommand> -h`.
+
+```shell
+> svc -h
+Usage: svc [OPTIONS] COMMAND [ARGS]...
+
+  so-vits-svc allows any folder structure for training data.
+  However, the following folder structure is recommended.
+      When training: dataset_raw/{speaker_name}/**/{wav_name}.{any_format}
+      When inference: configs/44k/config.json, logs/44k/G_XXXX.pth
+  If the folder structure is followed, you DO NOT NEED TO SPECIFY model path, config path, etc.
+  (The latest model will be automatically loaded.)
+  To train a model, run pre-resample, pre-config, pre-hubert, train.
+  To infer a model, run infer.
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  clean          Clean up files, only useful if you are using the default file structure
+  infer          Inference
+  onnx           Export model to onnx (currently not working)
+  pre-classify   Classify multiple audio files into multiple files
+  pre-config     Preprocessing part 2: config
+  pre-hubert     Preprocessing part 3: hubert If the HuBERT model is not found, it will be...
+  pre-resample   Preprocessing part 1: resample
+  pre-sd         Speech diarization using pyannote.audio
+  pre-split      Split audio files into multiple files
+  train          Train model If D_0.pth or G_0.pth not found, automatically download from hub.
+  train-cluster  Train k-means clustering
+  vc             Realtime inference from microphone
+```
+
+#### External Links
+
+[Video Tutorial](https://www.youtube.com/watch?v=tZn0lcGO5OQ)
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/34j"><img src="https://avatars.githubusercontent.com/u/55338215?v=4?s=80" width="80px;" alt="34j"/><br /><sub><b>34j</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Code">💻</a> <a href="#ideas-34j" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Documentation">📖</a> <a href="#example-34j" title="Examples">💡</a> <a href="#infra-34j" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-34j" title="Maintenance">🚧</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/pulls?q=is%3Apr+reviewed-by%3A34j" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=34j" title="Tests">⚠️</a> <a href="#tutorial-34j" title="Tutorials">✅</a> <a href="#promotion-34j" title="Promotion">📣</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3A34j" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GarrettConway"><img src="https://avatars.githubusercontent.com/u/22782004?v=4?s=80" width="80px;" alt="GarrettConway"/><br /><sub><b>GarrettConway</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=GarrettConway" title="Code">💻</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AGarrettConway" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=GarrettConway" title="Documentation">📖</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/pulls?q=is%3Apr+reviewed-by%3AGarrettConway" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BlueAmulet"><img src="https://avatars.githubusercontent.com/u/43395286?v=4?s=80" width="80px;" alt="BlueAmulet"/><br /><sub><b>BlueAmulet</b></sub></a><br /><a href="#ideas-BlueAmulet" title="Ideas, Planning, & Feedback">🤔</a> <a href="#question-BlueAmulet" title="Answering Questions">💬</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=BlueAmulet" title="Code">💻</a> <a href="#maintenance-BlueAmulet" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ThrowawayAccount01"><img src="https://avatars.githubusercontent.com/u/125531852?v=4?s=80" width="80px;" alt="ThrowawayAccount01"/><br /><sub><b>ThrowawayAccount01</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AThrowawayAccount01" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MashiroSA"><img src="https://avatars.githubusercontent.com/u/40637516?v=4?s=80" width="80px;" alt="緋"/><br /><sub><b>緋</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=MashiroSA" title="Documentation">📖</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AMashiroSA" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Lordmau5"><img src="https://avatars.githubusercontent.com/u/1345036?v=4?s=80" width="80px;" alt="Lordmau5"/><br /><sub><b>Lordmau5</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ALordmau5" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Lordmau5" title="Code">💻</a> <a href="#ideas-Lordmau5" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-Lordmau5" title="Maintenance">🚧</a> <a href="#question-Lordmau5" title="Answering Questions">💬</a> <a href="#userTesting-Lordmau5" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DL909"><img src="https://avatars.githubusercontent.com/u/71912115?v=4?s=80" width="80px;" alt="DL909"/><br /><sub><b>DL909</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADL909" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Satisfy256"><img src="https://avatars.githubusercontent.com/u/101394399?v=4?s=80" width="80px;" alt="Satisfy256"/><br /><sub><b>Satisfy256</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ASatisfy256" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pierluigizagaria"><img src="https://avatars.githubusercontent.com/u/57801386?v=4?s=80" width="80px;" alt="Pierluigi Zagaria"/><br /><sub><b>Pierluigi Zagaria</b></sub></a><br /><a href="#userTesting-pierluigizagaria" title="User Testing">📓</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ruckusmattster"><img src="https://avatars.githubusercontent.com/u/77196088?v=4?s=80" width="80px;" alt="ruckusmattster"/><br /><sub><b>ruckusmattster</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aruckusmattster" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Desuka-art"><img src="https://avatars.githubusercontent.com/u/111822082?v=4?s=80" width="80px;" alt="Desuka-art"/><br /><sub><b>Desuka-art</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADesuka-art" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/heyfixit"><img src="https://avatars.githubusercontent.com/u/41658450?v=4?s=80" width="80px;" alt="heyfixit"/><br /><sub><b>heyfixit</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=heyfixit" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.youtube.com/c/NerdyRodent"><img src="https://avatars.githubusercontent.com/u/74688049?v=4?s=80" width="80px;" alt="Nerdy Rodent"/><br /><sub><b>Nerdy Rodent</b></sub></a><br /><a href="#video-nerdyrodent" title="Videos">📹</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/xieyumc"><img src="https://avatars.githubusercontent.com/u/47858007?v=4?s=80" width="80px;" alt="谢宇"/><br /><sub><b>谢宇</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=xieyumc" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ColdCawfee"><img src="https://avatars.githubusercontent.com/u/79474598?v=4?s=80" width="80px;" alt="ColdCawfee"/><br /><sub><b>ColdCawfee</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AColdCawfee" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sbersier"><img src="https://avatars.githubusercontent.com/u/34165937?v=4?s=80" width="80px;" alt="sbersier"/><br /><sub><b>sbersier</b></sub></a><br /><a href="#ideas-sbersier" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-sbersier" title="User Testing">📓</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Asbersier" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Meldoner"><img src="https://avatars.githubusercontent.com/u/43951115?v=4?s=80" width="80px;" alt="Meldoner"/><br /><sub><b>Meldoner</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AMeldoner" title="Bug reports">🐛</a> <a href="#ideas-Meldoner" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Meldoner" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mmodeusher"><img src="https://avatars.githubusercontent.com/u/46575920?v=4?s=80" width="80px;" alt="mmodeusher"/><br /><sub><b>mmodeusher</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Ammodeusher" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AlonDan"><img src="https://avatars.githubusercontent.com/u/21152334?v=4?s=80" width="80px;" alt="AlonDan"/><br /><sub><b>AlonDan</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AAlonDan" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Likkkez"><img src="https://avatars.githubusercontent.com/u/44336181?v=4?s=80" width="80px;" alt="Likkkez"/><br /><sub><b>Likkkez</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ALikkkez" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/DuctTapeGames"><img src="https://avatars.githubusercontent.com/u/84365142?v=4?s=80" width="80px;" alt="Duct Tape Games"/><br /><sub><b>Duct Tape Games</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ADuctTapeGames" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://tec.hxlxz.com/"><img src="https://avatars.githubusercontent.com/u/6624983?v=4?s=80" width="80px;" alt="Xianglong He"/><br /><sub><b>Xianglong He</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Ahxl9654" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/75aosu"><img src="https://avatars.githubusercontent.com/u/79185331?v=4?s=80" width="80px;" alt="75aosu"/><br /><sub><b>75aosu</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3A75aosu" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tonyco82"><img src="https://avatars.githubusercontent.com/u/56610534?v=4?s=80" width="80px;" alt="tonyco82"/><br /><sub><b>tonyco82</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Atonyco82" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yxlllc"><img src="https://avatars.githubusercontent.com/u/33565655?v=4?s=80" width="80px;" alt="yxlllc"/><br /><sub><b>yxlllc</b></sub></a><br /><a href="#ideas-yxlllc" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=yxlllc" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/outhipped"><img src="https://avatars.githubusercontent.com/u/116147475?v=4?s=80" width="80px;" alt="outhipped"/><br /><sub><b>outhipped</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aouthipped" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/escoolioinglesias"><img src="https://avatars.githubusercontent.com/u/73505402?v=4?s=80" width="80px;" alt="escoolioinglesias"/><br /><sub><b>escoolioinglesias</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aescoolioinglesias" title="Bug reports">🐛</a> <a href="#userTesting-escoolioinglesias" title="User Testing">📓</a> <a href="#video-escoolioinglesias" title="Videos">📹</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Blacksingh"><img src="https://avatars.githubusercontent.com/u/130872856?v=4?s=80" width="80px;" alt="Blacksingh"/><br /><sub><b>Blacksingh</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3ABlacksingh" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://tybantarnusa.com"><img src="https://avatars.githubusercontent.com/u/9532857?v=4?s=80" width="80px;" alt="Mgs. M. Thoyib Antarnusa"/><br /><sub><b>Mgs. M. Thoyib Antarnusa</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Atybantarnusa" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ZeroHackz"><img src="https://avatars.githubusercontent.com/u/15729496?v=4?s=80" width="80px;" alt="Exosfeer"/><br /><sub><b>Exosfeer</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AZeroHackz" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=ZeroHackz" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/guranon"><img src="https://avatars.githubusercontent.com/u/130421189?v=4?s=80" width="80px;" alt="guranon"/><br /><sub><b>guranon</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aguranon" title="Bug reports">🐛</a> <a href="#ideas-guranon" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=guranon" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexanderkoumis"><img src="https://avatars.githubusercontent.com/u/5108856?v=4?s=80" width="80px;" alt="Alexander Koumis"/><br /><sub><b>Alexander Koumis</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=alexanderkoumis" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.meimadix.com"><img src="https://avatars.githubusercontent.com/u/653972?v=4?s=80" width="80px;" alt="Roee Shenberg"/><br /><sub><b>Roee Shenberg</b></sub></a><br /><a href="#userTesting-shenberg" title="User Testing">📓</a> <a href="#ideas-shenberg" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=shenberg" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `so-vits-svc-fork-mandarin-0.0.0/pyproject.toml` & `so_vits_svc_fork_mandarin-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
-name = "so-vits-svc-fork"
-version = "4.1.1"
-description = "A fork of so-vits-svc."
+name = "so-vits-svc-fork-mandarin"
+version = "1.0.1"
+description = "A mandarin translation version of a fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/34j/so-vits-svc-fork"
+repository = "https://github.com/weihaozhaung/so-vits-svc-fork-mandarin"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
```

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         },
     )
     sg.theme("Very Dark")
 
     model_candidates = list(sorted(Path("./logs/44k/").glob("G_*.pth")))
 
     frame_contents = {
-        "Paths": [
+        "模型設定": [
             [
                 sg.Text("聲音模型"),
                 sg.Push(),
                 sg.InputText(
                     key="model_path",
                     default_text=model_candidates[-1].absolute().as_posix()
                     if model_candidates
@@ -473,15 +473,15 @@
                                 "    情況二：麥克風輸入音量過低（降低靜音閾值）\n"
                             )
                         ]
                     ],
                 ),
             ],
         ],
-        "Presets": [
+        "預設": [
             [
                 sg.Text("預設參數"),
                 sg.Push(),
                 sg.Combo(
                     key="presets",
                     values=list(load_presets().keys()),
                     size=(40, 1),
@@ -525,24 +525,24 @@
             sg.Button("暫停變聲器", key="stop_vc"),
             sg.Push(),
             # sg.Button("ONNX Export", key="onnx_export"),
         ],
     ]
     column1 = sg.Column(
         [
-            frames["Paths"],
-            frames["Common"],
+            frames["模型設定"],
+            frames["一般設定"],
         ],
         vertical_alignment="top",
     )
     column2 = sg.Column(
         [
-            frames["File"],
-            frames["Realtime"],
-            frames["Presets"],
+            frames["檔案"],
+            frames["即時變聲"],
+            frames["預設"],
         ]
         + bottoms
     )
     # columns
     layout = [[column1, column2]]
     # get screen size
     screen_width, screen_height = sg.Window.get_screen_size()
```

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so-vits-svc-fork-mandarin-0.0.0/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork_mandarin-1.0.1/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

