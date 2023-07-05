# Comparing `tmp/SwissArmyTransformer-0.3.7.tar.gz` & `tmp/SwissArmyTransformer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-txtcgohx/SwissArmyTransformer-0.3.7.tar", last modified: Thu Jun  1 06:56:48 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-br8z1pgj/SwissArmyTransformer-0.4.0.tar", last modified: Wed Jul  5 09:26:21 2023, max compression
```

## Comparing `SwissArmyTransformer-0.3.7.tar` & `SwissArmyTransformer-0.4.0.tar`

### file list

```diff
@@ -1,149 +1,176 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.7/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4203 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       84 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       83 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24867 2023-05-27 05:04:41.000000 SwissArmyTransformer-0.3.7/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.7/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.7/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/samplers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.7/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4025 2023-05-27 05:35:24.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.7/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.3.7/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13873 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/lora.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13473 2023-06-01 06:34:25.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/lora2.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12358 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.7/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13912 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.3.7/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5402 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27066 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2216 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.3.7/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-05-16 05:12:03.000000 SwissArmyTransformer-0.3.7/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/mappings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.7/sat/ops/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/ops/local_attention_function.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.7/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/quantization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.7/sat/quantization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.7/sat/quantization/kernels.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.7/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.7/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.321936 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.321936 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.309936 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.325935 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23052 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.7/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.7/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.7/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7072 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-06-01 06:38:59.000000 SwissArmyTransformer-0.3.7/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.7/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/tests/test_nested_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.3.7/tests/test_speed.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.7/tests/test_train.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.3.7/tests/test_train_dp.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/tests/test_train_nested.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.874483 SwissArmyTransformer-0.4.0/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.4.0/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      191 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.846483 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4934 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       90 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       89 2023-06-28 07:19:19.000000 SwissArmyTransformer-0.4.0/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    25363 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15565 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2676 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.4.0/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/data_utils/samplers.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7129 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/webds.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9777 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4025 2023-05-27 05:35:24.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.4.0/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.4.0/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/attention/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      110 2023-06-06 14:36:22.000000 SwissArmyTransformer-0.4.0/sat/model/attention/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3654 2023-06-07 06:54:10.000000 SwissArmyTransformer-0.4.0/sat/model/attention/memory_efficient_attention.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12760 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1731 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13473 2023-06-01 06:34:25.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/lora2.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      391 2023-06-06 14:36:32.000000 SwissArmyTransformer-0.4.0/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/normalization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       24 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/normalization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      610 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/normalization/rms.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      676 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1923 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     6378 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/chatglm2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12890 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.4.0/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13903 2023-06-06 13:57:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4614 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/llama_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.4.0/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5402 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2713 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings_original.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    28857 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2217 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.4.0/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    18083 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/mappings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1243 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/operation.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3924 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1233 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.842483 SwissArmyTransformer-0.4.0/sat/ops/csrc/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      947 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5595 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_apply.cuh
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7076 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      336 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/compat.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     6388 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/type_shim.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10712 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/fused_ema_adam.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      578 2023-06-07 05:52:48.000000 SwissArmyTransformer-0.4.0/sat/ops/memory_efficient_attention.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1982 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    28554 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/builder.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      957 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/fused_ema_adam.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-06-05 05:26:26.000000 SwissArmyTransformer-0.4.0/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/quantization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.0/sat/quantization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.0/sat/quantization/kernels.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6754 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3081 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.4.0/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.842483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.866483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23899 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.4.0/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11576 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.4.0/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9348 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-07-05 09:26:21.874483 SwissArmyTransformer-0.4.0/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-07-05 09:23:25.000000 SwissArmyTransformer-0.4.0/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.0/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3104 2023-06-07 06:54:04.000000 SwissArmyTransformer-0.4.0/tests/test_mea.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      913 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/tests/test_model_parallel.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.4.0/tests/test_speed.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.0/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.4.0/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.7/LICENSE` & `SwissArmyTransformer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/PKG-INFO` & `SwissArmyTransformer-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.7
+Version: 0.4.0
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.7/README.md` & `SwissArmyTransformer-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.7
+Version: 0.4.0
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 sat/helpers.py
 sat/transformer_defaults.py
 sat/data_utils/__init__.py
 sat/data_utils/configure_data.py
 sat/data_utils/datasets.py
 sat/data_utils/hf_dataset.py
 sat/data_utils/samplers.py
+sat/data_utils/webds.py
 sat/generation/__init__.py
 sat/generation/autoregressive_sampling.py
 sat/generation/cuda2d_sampling.py
 sat/generation/magnify.py
 sat/generation/utils.py
 sat/generation/sampling_strategies/__init__.py
 sat/generation/sampling_strategies/base_strategy.py
@@ -29,54 +30,72 @@
 sat/model/__init__.py
 sat/model/base_model.py
 sat/model/cached_autoregressive_model.py
 sat/model/encoder_decoder_model.py
 sat/model/mixins.py
 sat/model/registry.py
 sat/model/transformer.py
+sat/model/attention/__init__.py
+sat/model/attention/memory_efficient_attention.py
 sat/model/finetune/__init__.py
 sat/model/finetune/adapter.py
 sat/model/finetune/ffadd.py
 sat/model/finetune/lora.py
 sat/model/finetune/lora2.py
 sat/model/finetune/mlp_head.py
 sat/model/finetune/prompt_tuning.py
+sat/model/normalization/__init__.py
+sat/model/normalization/rms.py
 sat/model/official/__init__.py
 sat/model/official/bert_model.py
 sat/model/official/cait_model.py
+sat/model/official/chatglm2_model.py
 sat/model/official/chatglm_model.py
 sat/model/official/clip_model.py
 sat/model/official/cuda2d_model.py
 sat/model/official/distill_model.py
 sat/model/official/dpr_model.py
 sat/model/official/eva2_model.py
 sat/model/official/glm130B_model.py
 sat/model/official/glm_model.py
 sat/model/official/gpt2_model.py
 sat/model/official/gptneo_model.py
+sat/model/official/llama_model.py
 sat/model/official/mae_model.py
 sat/model/official/roberta_model.py
 sat/model/official/t5_model.py
 sat/model/official/vit_model.py
 sat/model/official/yolos_model.py
 sat/model/position_embedding/__init__.py
 sat/model/position_embedding/rotary_embeddings.py
+sat/model/position_embedding/rotary_embeddings_original.py
 sat/model/position_embedding/sincos2d.py
 sat/model/position_embedding/vision_rotary_embeddings.py
 sat/mpu/__init__.py
 sat/mpu/cross_entropy.py
 sat/mpu/data.py
 sat/mpu/initialize.py
 sat/mpu/layers.py
 sat/mpu/mappings.py
+sat/mpu/operation.py
 sat/mpu/utils.py
 sat/ops/__init__.py
+sat/ops/fused_ema_adam.py
 sat/ops/layernorm.py
 sat/ops/local_attention_function.py
+sat/ops/memory_efficient_attention.py
 sat/ops/scaled_mask_softmax.py
+sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
+sat/ops/csrc/adam/multi_tensor_apply.cuh
+sat/ops/csrc/adam/multi_tensor_ema_adam.cu
+sat/ops/csrc/includes/compat.h
+sat/ops/csrc/includes/type_shim.h
+sat/ops/ops_builder/__init__.py
+sat/ops/ops_builder/builder.py
+sat/ops/ops_builder/fused_ema_adam.py
 sat/quantization/__init__.py
 sat/quantization/kernels.py
 sat/resources/__init__.py
 sat/resources/download.py
 sat/resources/urls.py
 sat/tokenization/__init__.py
 sat/tokenization/hf_tokenizer.py
@@ -112,12 +131,14 @@
 sat/training/deepspeed_zero2.json
 sat/training/learning_rates.py
 sat/training/model_io.py
 sat/training/utils.py
 tests/test_base_model.py
 tests/test_inference.py
 tests/test_list_info.py
+tests/test_mea.py
+tests/test_model_parallel.py
 tests/test_nested_model.py
 tests/test_speed.py
 tests/test_train.py
 tests/test_train_dp.py
 tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.7/sat/arguments.py` & `SwissArmyTransformer-0.4.0/sat/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
                        help='num of transformer attention heads')
     group.add_argument('--vocab-size', type=int, default=100,
                        help='vocab size for tokenization. the size of word_embeddings.')
     group.add_argument('--max-sequence-length', type=int, default=512,
                        help='maximum number of position embeddings to use')
     
     # ---------------  Optional hyper-parameters --------------- 
+    # for developers:
+    #   if you want to add more optional arch hyper-parameters, please also add them in model_io.py, base_model.py, and of course, transformer.py and anywhere in use.
 
     group.add_argument('--layernorm-order', type=str, default='pre',
                        help='choose from "pre", "post", "sandwich".',
                        choices=['post', # In the original Transformer.
                                 'pre', # Used by most current frameworks.
                                 'sandwich' # More stable.
                                 ])
@@ -63,14 +65,17 @@
                        help='size of the model parallel. only use if you are an expert.')
 
     group.add_argument('--skip-init', action='store_true',
                        help='skip model initialization')
     
     group.add_argument('--use-gpu-initialization', action='store_true', 
                        help='initialize model on gpu')
+
+    group.add_argument('--num-multi-query-heads', type=int, default=0, 
+                       help='use multi-query attention, num of kv groups. 0 means multi-head attention.')
     
     # ---------------  Inessential hyper-parameters --------------- 
 
     # Dropout and eps hyper-parameters
     group.add_argument('--layernorm-epsilon', type=float, default=1e-5,
                        help='layer norm epsilon')
     group.add_argument('--hidden-dropout', type=float, default=0.1,
@@ -225,14 +230,16 @@
     # Efficiency.
     group.add_argument('--num-workers', type=int, default=1,
                        help="""Number of workers to use for dataloading""")
     # Sometimes, num-workders > 1 and cpu_offload (zero-stage 2) will make the validation dataloader hang.
     # I have no idea on the reason, and just set the default num-workers to 1.
     group.add_argument('--block-size', type=int, default=10000,
                        help="""Size of block to reduce memory in dataset, ignore it for most users.""")
+    group.add_argument('--prefetch-factor', type=int, default=4, 
+                       help='prefetching number of batches.')
 
     return parser
 
 
 def add_text_generate_args(parser):
     """Text generate arguments."""
```

### Comparing `SwissArmyTransformer-0.3.7/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.4.0/sat/data_utils/configure_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         args.test_last_shape = [1] * world_size
         args.test_drop_number = 0
         return torch.utils.data.DataLoader(
             dataset,
             batch_size=batch_size//world_size,
             num_workers=args.num_workers,
             pin_memory=True,
-            collate_fn=collate_fn
+            collate_fn=collate_fn,
+            prefetch_factor=args.prefetch_factor,
             )
 
     sampler = torch.utils.data.SequentialSampler(dataset)
     # drop_last = distributed
     drop_last = False # TODO will always drop last to keep the consistency.
     # or, how to avg in eval last batch?
 
@@ -85,28 +86,30 @@
     elif split=='test':
         args.test_last_shape = last_shape
         args.test_drop_number = drop_number
     data_loader = torch.utils.data.DataLoader(dataset,
                                               batch_sampler=batch_sampler,
                                               num_workers=args.num_workers,
                                               pin_memory=True,
-                                              collate_fn=collate_fn)
+                                              collate_fn=collate_fn,
+                                              prefetch_factor=args.prefetch_factor,
+                                              )
     return data_loader
 
 
 def make_dataset_full(path, split, args, create_dataset_function, 
         dataset_weights=None, random_mapping=True, is_train_data=False, **kwargs):
     """function to create datasets+tokenizers for common options"""
     print_all('make dataset ' + str(path), level='DEBUG')
     assert isinstance(path, list)
 
     if args.iterable_dataset: # cannot indexed
         # the random mapping is flexible and efficient, but sometimes we have pratical issue
         # For instance, someone just gives you a iterable dataset, e.g. webdataset
-        from .datasets import ConfiguredResampledShards, DataPipeline
+        from .webds import ConfiguredResampledShards, DataPipeline
         valid_types = (ConfiguredResampledShards, DataPipeline)
         
         assert split[0] == 1, 'Iterable dataset cannot auto split.'
         assert dataset_weights is None
         for p in path:
             ds = []
             for p in path:
@@ -129,17 +132,17 @@
                 ds = RandomDataset(ds, scale=args.epochs, seed=args.seed)
             else:
                 world_size = torch.distributed.get_world_size(
                     group=mpu.get_data_parallel_group())
                 if is_train_data:
                 # only train-dataset will set this to True,
                 # so we enlarge it to make sure that the data is sufficient.
-                    scale = max(200, 1 + (args.train_iters * args.batch_size * world_size) // len(ds))
+                    scale = max(200, 1 + (args.train_iters * args.batch_size * args.gradient_accumulation_steps * world_size) // len(ds))
                 else:
-                    scale = max(200, 1 + ((1 + args.train_iters // args.eval_interval) * args.eval_iters * args.eval_batch_size * world_size) // len(ds))
+                    scale = max(200, 1 + ((1 + args.train_iters // args.eval_interval) * args.eval_iters * args.eval_batch_size * args.gradient_accumulation_steps * world_size) // len(ds))
                 ds = RandomMappingDataset(ds, scale=scale)
         return ds 
     else:
         # must first split datasets, then reweight/concat, finally random-mapping.
         # this order avoids overlapping.
         train_ds, valid_ds, test_ds = [], [], []
         for p in path:
```

### Comparing `SwissArmyTransformer-0.3.7/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.4.0/sat/data_utils/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,30 +80,11 @@
     def __len__(self):
         return len(self.items)
     
     def __getitem__(self, index):
         return self.process_fn(self.items[index])
 
 try:
-    import webdataset as wds
-    from webdataset import ResampledShards, DataPipeline, tarfile_to_samples
-    from webdataset.utils import pytorch_worker_seed
-    def worker_seed_sat(group=None, seed=0):
-        return pytorch_worker_seed(group=group) + seed * 23
-    
-    class ConfiguredResampledShards(ResampledShards):
-        def __init__(self, urls, seed, nshards=sys.maxsize, deterministic=True):
-            from sat.mpu import get_data_parallel_group
-            worker_seed_sat_this = partial(worker_seed_sat, group=get_data_parallel_group(), seed=seed)
-            super().__init__(urls, nshards, worker_seed_sat_this, deterministic)
-
-    class SimpleDistributedWebDataset(DataPipeline):
-        def __init__(self, path, process_fn, seed, *, shuffle_buffer=1000):
-            super().__init__(
-                ConfiguredResampledShards(path, seed), # Lots of shards are recommended, or not evenly
-                tarfile_to_samples(),
-                wds.shuffle(shuffle_buffer), # set shuffle_buffer = 1 to disable it, TODO model-parallel with different due to shuffle
-                process_fn
-            )
+    from .webds import SimpleDistributedWebDataset, MetaDistributedWebDataset
         
 except ModuleNotFoundError: # webdataset not install, use pip to install
     pass
```

### Comparing `SwissArmyTransformer-0.3.7/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.4.0/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.4.0/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.4.0/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/magnify.py` & `SwissArmyTransformer-0.4.0/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/base_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/generation/utils.py` & `SwissArmyTransformer-0.4.0/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/helpers.py` & `SwissArmyTransformer-0.4.0/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/base_model.py` & `SwissArmyTransformer-0.4.0/sat/model/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sat.model.registry import model_registry, MetaModel
 
 from sat.model.transformer import BaseTransformer, standard_attention
 from sat.arguments import update_args_with_file, overwrite_args_by_dict
 from sat.training.model_io import load_checkpoint
 from sat.helpers import print_rank0
 
-from sat.transformer_defaults import HOOKS_DEFAULT
+from sat.transformer_defaults import HOOKS_DEFAULT, ARGS_DEFAULT
 from sat.resources import auto_create
 
 def non_conflict(func):
     '''mark a hook function as non-conflict,
     so that it can be compatible with any already defined hooks.
     e.g. PrefixTuningMixin.attention_fn
     '''
@@ -81,33 +81,24 @@
         if transformer is not None:
             self.transformer = transformer
         else:
             # check if model-only mode
             from sat.arguments import _simple_init
             success = _simple_init(model_parallel_size=args.model_parallel_size)
 
+            args_dict = {k: (getattr(args, v[0]) if hasattr(args, v[0]) else v[1]) for k, v in ARGS_DEFAULT.items()}
+
             self.transformer = BaseTransformer(
                 num_layers=args.num_layers,
                 vocab_size=args.vocab_size,
                 hidden_size=args.hidden_size,
                 num_attention_heads=args.num_attention_heads,
                 max_sequence_length=args.max_sequence_length,
                 layernorm_order=args.layernorm_order,
-                embedding_dropout_prob=args.hidden_dropout if hasattr(args, 'hidden_dropout') else 0,
-                attention_dropout_prob=args.attention_dropout if hasattr(args, 'attention_dropout') else 0,
-                output_dropout_prob=args.hidden_dropout if hasattr(args, 'hidden_dropout') else 0,
-                inner_hidden_size=args.inner_hidden_size if hasattr(args, 'inner_hidden_size') else None,
-                hidden_size_per_attention_head=args.hidden_size_per_attention_head if hasattr(args, 'hidden_size_per_attention_head') else None,
-                checkpoint_activations=args.checkpoint_activations if hasattr(args, 'checkpoint_activations') else False,
-                checkpoint_num_layers=args.checkpoint_num_layers if hasattr(args, 'checkpoint_num_layers') else 1,
-                is_decoder=args.is_decoder if hasattr(args, 'is_decoder') else False,
-                cross_attn_hidden_size=args.cross_attn_hidden_size if hasattr(args, 'cross_attn_hidden_size') else None,
-                use_final_layernorm=args.use_final_layernorm if hasattr(args, 'use_final_layernorm') else True,
-                layernorm_epsilon=args.layernorm_epsilon if hasattr(args, 'layernorm_epsilon') else 1e-5,
-                use_bias=args.use_bias if hasattr(args, 'use_bias') else True,
+                **args_dict,
                 hooks=self.hooks,
                 params_dtype=params_dtype,
                 skip_init=args.skip_init,
                 device=torch.cuda.current_device() if hasattr(args, 'use_gpu_initialization') and args.use_gpu_initialization else torch.device('cpu'),
                 **kwargs
             )
 
@@ -238,15 +229,15 @@
             Returns:
                 args: the parsed args.
         '''
         parser = cls.list_avail_args(print=False)
         # use parser to parse kwargs
         args = parser.parse_args([])
         for k, v in kwargs.items():
-            if hasattr(args, k) or k in ['fp16']: # optional args
+            if hasattr(args, k) or k in ['fp16']: # non-arch args but affect building models
                 setattr(args, k, v)
             else:
                 print_rank0(f'warning: Unknown arg {k} for class {cls.__name__}.', level='DEBUG')
                 setattr(args, k, v)
         return args
 
 class AutoModel():
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.4.0/sat/model/cached_autoregressive_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 import os
 import sys
 import math
 import random
 import torch
 
 from .base_model import BaseModel, BaseMixin, non_conflict
-from sat.model.transformer import standard_attention, split_tensor_along_last_dim
+from sat.transformer_defaults import attention_fn_default
 
 class CachedAutoregressiveMixin(BaseMixin):
     def __init__(self):
         super().__init__()     
            
     @non_conflict
-    def attention_fn(self, q, k, v, mask, dropout_fn, mems=None, cross_attention=False, old_impl=standard_attention,
+    def attention_fn(self, q, k, v, mask, dropout_fn, mems=None, cross_attention=False, old_impl=attention_fn_default,
                      **kw_args):
         if not cross_attention:
             mem = mems[kw_args['layer_id']] if mems is not None else None # 2, batch, head, seqlen, hidden_size
             b, nh, seq_len, hidden_size = k.shape
 
             cache_kv = torch.stack((k, v)).permute(1, 3, 0, 2, 4).detach().contiguous().view(b, seq_len, nh * hidden_size * 2)
             kw_args['output_this_layer']['mem_kv'] = cache_kv
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.4.0/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/lora2.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/lora2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.4.0/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/__init__.py` & `SwissArmyTransformer-0.4.0/sat/model/official/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 from .clip_model import CLIP
 from .gptneo_model import GPTNeoModel
 from .dpr_model import DPRQuestionEncoder
 from .dpr_model import DPRContextEncoder
 from .dpr_model import DPRReader
 from .gpt2_model import GPT2Model
 from .chatglm_model import ChatGLMModel
-from .eva2_model import EVA2Model
+from .eva2_model import EVA2Model
+from .llama_model import LLaMAModel
+from .chatglm2_model import ChatGLM2Model
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/bert_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,9 +41,9 @@
         self.add_mixin("bert-final", BertFinalMixin(args.vocab_size, args.hidden_size))
         self.add_mixin("bert-type", BertTypeMixin(args.num_types, args.hidden_size))
         
 
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('BERT', 'BERT Configurations')
-        group.add_argument('--num-types', type=int)
+        group.add_argument('--num-types', type=int, default=2, help='Number of token types')
         return super().add_model_specific_args(parser)
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/chatglm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,25 @@
             hidden_states = attention_input * alpha + attention_output
         else:
             hidden_states = hidden_states + attention_output
 
         
         mlp_input = self.post_attention_layernorm(hidden_states)
 
+        if self.is_decoder:
+            encoder_outputs = kw_args['encoder_outputs']
+            if encoder_outputs is not None:
+                assert 'cross_attention_mask' in kw_args
+                # Cross attention
+                attention_output = self.cross_attention(mlp_input, **kw_args)
+                # Residual connection.
+                hidden_states = mlp_input + attention_output
+                # Layer norm post the cross attention
+                mlp_input = self.post_cross_attention_layernorm(hidden_states)
+
         # MLP.
         mlp_output = self.mlp(mlp_input, **kw_args)
 
         # Fourth LayerNorm
         if self.layernorm_order == 'sandwich':
             mlp_output = self.fourth_layernorm(mlp_output)
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/glm130B_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,21 +148,21 @@
 class SelfAttentionWithFP32SoftmaxMixin(BaseMixin):
     def __init__(self, hidden_size, num_attention_heads, model_parallel_size):
         super().__init__()
         self.hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
         self.hidden_size_per_partition = divide(hidden_size, model_parallel_size)
         self.scale_mask_softmax = None
 
-        from sat.ops.scaled_mask_softmax import FusedScaleMaskSoftmax, AttnMaskType
+        from sat.ops.scaled_mask_softmax import FusedScaleMaskSoftmax
 
         if FusedScaleMaskSoftmax is not None:
             self.scale_mask_softmax = FusedScaleMaskSoftmax(
                 input_in_fp16=True,
                 input_in_bf16=False,
-                attn_mask_type=AttnMaskType.padding,
+                attn_mask_type=1, # AttnMaskType.padding,
                 scaled_masked_softmax_fusion=True,
                 mask_func=self.attention_mask_func,
                 softmax_in_fp32=True,
                 scale=1,
             )
 
     @staticmethod
```

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.4.0/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.4.0/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.4.0/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/registry.py` & `SwissArmyTransformer-0.4.0/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/model/transformer.py` & `SwissArmyTransformer-0.4.0/sat/model/transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,41 +30,50 @@
 
 from sat.transformer_defaults import HOOKS_DEFAULT, standard_attention, split_tensor_along_last_dim
 
 
 class SelfAttention(torch.nn.Module):
     def __init__(self, hidden_size, num_attention_heads,
                  attention_dropout_prob, output_dropout_prob,
-                 init_method, layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True,
+                 init_method, layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True, qkv_bias=False, num_multi_query_heads=0,
                  hooks={}, transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
         super(SelfAttention, self).__init__()
         # Set output layer initialization if not provided.
         if output_layer_init_method is None:
             output_layer_init_method = init_method
         self.hooks = hooks
         self.layer_id = layer_id
         # Per attention head and per partition values.
         world_size = get_model_parallel_world_size()
         self.hidden_size = hidden_size
+        self.num_attention_heads = num_attention_heads
+        self.num_multi_query_heads = num_multi_query_heads
         if hidden_size_per_attention_head is None:
             self.hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
         else:
             self.hidden_size_per_attention_head = hidden_size_per_attention_head
         self.num_attention_heads_per_partition = divide(num_attention_heads, world_size)
+        self.num_multi_query_heads_per_partition = divide(num_multi_query_heads, world_size)
         self.inner_hidden_size = num_attention_heads * self.hidden_size_per_attention_head
         self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
 
         # Strided linear layer.
+        if num_multi_query_heads == 0:
+            qkv_size = 3 * self.inner_hidden_size
+            self.stride = 3
+        else: # multi-query 
+            qkv_size = self.inner_hidden_size + self.hidden_size_per_attention_head * self.num_multi_query_heads_per_partition * 2 
+            self.stride = [self.num_attention_heads_per_partition, self.num_multi_query_heads_per_partition, self.num_multi_query_heads_per_partition]
         self.query_key_value = ColumnParallelLinear(
             hidden_size,
-            3 * self.inner_hidden_size,
-            stride=3,
+            qkv_size,
+            stride=self.stride,
             gather_output=False,
             init_method=init_method,
-            bias=bias,
+            bias=bias or qkv_bias,
             params_dtype=params_dtype,
             module=self,
             name="query_key_value",
             skip_init=skip_init,
             device=device
         )
         self.attention_dropout = torch.nn.Dropout(attention_dropout_prob)
@@ -87,41 +96,46 @@
         assert transformer_pointer is not None
 
     def _transpose_for_scores(self, tensor):
         """Transpose a 3D tensor [b, s, np*hn] into a 4D tensor with
         size [b, np, s, hn].
         """
         new_tensor_shape = tensor.size()[:-1] + \
-                           (self.num_attention_heads_per_partition,
+                           (-1, # flexible for multi-query
                             self.hidden_size_per_attention_head)
         tensor = tensor.view(*new_tensor_shape)
         return tensor.permute(0, 2, 1, 3)
 
     def forward(self, hidden_states, mask, *args, **kw_args):
         if 'attention_forward' in self.hooks:
             return self.hooks['attention_forward'](hidden_states, mask, **kw_args)
         else:
             return HOOKS_DEFAULT['attention_forward'](self, hidden_states, mask, **kw_args)
 
+    def repartition(self):
+        world_size = get_model_parallel_world_size()
+        self.num_attention_heads_per_partition = divide(self.num_attention_heads, world_size)
+        self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
 
 class CrossAttention(torch.nn.Module):
     """Parallel cross-attention layer for Transformer"""
 
     def __init__(self, hidden_size, num_attention_heads, attention_dropout_prob, output_dropout_prob, init_method,
                  layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True, hooks={},
                  cross_attn_hidden_size=None, transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
         super().__init__()
         # Set output layer initialization if not provided.
         if output_layer_init_method is None:
             output_layer_init_method = init_method
         self.hooks = hooks
         self.layer_id = layer_id
+        self.num_attention_heads = num_attention_heads
+        self.hidden_size = hidden_size
         # Per attention head and per partition values.
         world_size = get_model_parallel_world_size()
-        self.hidden_size = hidden_size
         if hidden_size_per_attention_head is None:
             self.hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
         else:
             self.hidden_size_per_attention_head = hidden_size_per_attention_head
         self.num_attention_heads_per_partition = divide(num_attention_heads, world_size)
         self.inner_hidden_size = num_attention_heads * self.hidden_size_per_attention_head
         self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
@@ -165,15 +179,20 @@
 
     def forward(self, hidden_states, cross_attention_mask, encoder_outputs, **kw_args):
         # hidden_states: [b, s, h]
         if 'cross_attention_forward' in self.hooks:
             return self.hooks['cross_attention_forward'](hidden_states, cross_attention_mask, encoder_outputs, **kw_args)
         else:
             return HOOKS_DEFAULT['cross_attention_forward'](self, hidden_states, cross_attention_mask, encoder_outputs, **kw_args)
-
+    
+    def repartition(self):
+        world_size = get_model_parallel_world_size()
+        self.num_attention_heads_per_partition = divide(self.num_attention_heads, world_size)
+        self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
+    
 
 class MLP(torch.nn.Module):
     def __init__(self, hidden_size, output_dropout_prob, init_method, inner_hidden_size=None,
                  output_layer_init_method=None, layer_id=None, hooks={}, bias=True, activation_func=gelu, transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
         super(MLP, self).__init__()
         self.layer_id = layer_id
         self.activation_func = activation_func
@@ -241,14 +260,16 @@
             hidden_size_per_attention_head=None,
             output_layer_init_method=None,
             layernorm_order='pre',
             layernorm=LayerNorm,
             is_decoder=False,
             cross_attn_hidden_size=None,
             use_bias=True,
+            use_qkv_bias=False,
+            num_multi_query_heads=0,
             activation_func=gelu,
             hooks={},
             transformer_pointer=None,
             params_dtype=torch.float,
             skip_init=False,
             device=torch.device('cpu')
     ):
@@ -273,14 +294,16 @@
             attention_dropout_prob,
             output_dropout_prob,
             init_method,
             layer_id,
             hidden_size_per_attention_head=hidden_size_per_attention_head,
             output_layer_init_method=output_layer_init_method,
             bias=use_bias,
+            qkv_bias=use_qkv_bias,
+            num_multi_query_heads=num_multi_query_heads,
             hooks=hooks,
             transformer_pointer=transformer_pointer,
             params_dtype=params_dtype,
             skip_init=skip_init,
             device=device
         )
 
@@ -347,14 +370,16 @@
                  inner_hidden_size=None,
                  hidden_size_per_attention_head=None,
                  layernorm_order='pre',
                  parallel_output=True,
                  is_decoder=False,
                  cross_attn_hidden_size=None,
                  use_bias=True,
+                 use_qkv_bias=False,
+                 num_multi_query_heads=0,
                  activation_func=gelu,
                  layernorm=LayerNorm,
                  init_method=None,
                  use_final_layernorm=True,
                  hooks={},
                  params_dtype=torch.float,
                  skip_init=False,
@@ -366,14 +391,16 @@
         self.inner_hidden_size = inner_hidden_size
         self.hidden_size_per_attention_head = hidden_size_per_attention_head
         self.is_decoder = is_decoder
         self.cross_attn_hidden_size = cross_attn_hidden_size
         if not is_decoder and cross_attn_hidden_size is not None:
             print('warning: cross_attn_hidden_size is set but is_decoder is False')
         self.use_bias = use_bias
+        self.use_qkv_bias = use_qkv_bias
+        self.num_multi_query_heads = num_multi_query_heads
         self.use_final_layernorm = use_final_layernorm
         self.layernorm_epsilon = layernorm_epsilon
         self.parallel_output = parallel_output
         self.checkpoint_activations = checkpoint_activations
         self.checkpoint_num_layers = checkpoint_num_layers
         self.max_sequence_length = max_sequence_length
         self.layernorm_order = layernorm_order
@@ -411,14 +438,16 @@
                 hidden_size_per_attention_head=hidden_size_per_attention_head,
                 output_layer_init_method=self.output_layer_init_method,
                 is_decoder=self.is_decoder,
                 cross_attn_hidden_size=cross_attn_hidden_size,
                 layernorm_order=layernorm_order,
                 layernorm=layernorm,
                 use_bias=use_bias,
+                use_qkv_bias=use_qkv_bias,
+                num_multi_query_heads=num_multi_query_heads,
                 activation_func=activation_func,
                 hooks=self.hooks,
                 transformer_pointer=self,
                 params_dtype=params_dtype,
                 skip_init=skip_init,
                 device=device
             )
@@ -562,15 +591,15 @@
                         layer_id=torch.tensor(i),
                         **kw_args,
                         position_ids=position_ids,
                         **output_cross_layer,
                         output_this_layer=output_this_layer_obj, output_cross_layer=output_cross_layer_obj
                     )
                 else:
-                    layer_ret = layer(*args, layer_id=torch.tensor(i), **kw_args, **output_cross_layer,
+                    layer_ret = layer(*args, layer_id=torch.tensor(i), **kw_args, position_ids=position_ids, **output_cross_layer,
                         output_this_layer=output_this_layer_obj, output_cross_layer=output_cross_layer_obj)
                 if isinstance(layer_ret, tuple):
                     layer_ret = layer_ret[0] # for legacy API
                 hidden_states, output_this_layer, output_cross_layer = layer_ret, output_this_layer_obj, output_cross_layer_obj
 
                 if output_hidden_states:
                     output_this_layer['hidden_states'] = hidden_states
```

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/__init__.py` & `SwissArmyTransformer-0.4.0/sat/mpu/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,24 @@
 from .initialize import get_model_parallel_rank
 from .initialize import get_model_parallel_src_rank
 from .initialize import get_model_parallel_world_size
 from .initialize import initialize_model_parallel
 from .initialize import model_parallel_is_initialized
 
 from .layers import ColumnParallelLinear
-from .layers import ParallelEmbedding
 from .layers import RowParallelLinear
 from .layers import VocabParallelEmbedding
 
 from .mappings import copy_to_model_parallel_region
 from .mappings import gather_from_model_parallel_region
 from .mappings import reduce_from_model_parallel_region
 from .mappings import scatter_to_model_parallel_region
 
+from .operation import mp_split_model
+
 try:
     import torch
     assert torch.cuda.is_available() # or set get_cuda_rng_tracker to None
     from deepspeed.runtime.activation_checkpointing.checkpointing import checkpoint, get_cuda_rng_tracker, model_parallel_cuda_manual_seed
 except Exception as e:
     from sat.helpers import print_rank0
     print_rank0(str(e), level="DEBUG")
```

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.4.0/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/data.py` & `SwissArmyTransformer-0.4.0/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/initialize.py` & `SwissArmyTransformer-0.4.0/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/layers.py` & `SwissArmyTransformer-0.4.0/sat/mpu/layers.py`

 * *Files 14% similar despite different names*

```diff
@@ -125,14 +125,28 @@
                                       self.norm_type, self.scale_grad_by_freq,
                                       self.sparse)
         # Mask the output embedding.
         output_parallel[input_mask, :] = 0.0
         # Reduce across all the model parallel GPUs.
         output = reduce_from_model_parallel_region(output_parallel)
         return output
+    
+    def repartition(self):
+        assert self.num_embeddings_per_partition == self.num_embeddings
+        self.vocab_start_index, self.vocab_end_index = \
+            VocabUtility.vocab_range_from_global_vocab_size(
+                self.num_embeddings, get_model_parallel_rank(),
+                get_model_parallel_world_size())
+        self.num_embeddings_per_partition = self.vocab_end_index - \
+                                            self.vocab_start_index
+        self.original_weight = self.weight
+        self.weight = torch.nn.Parameter(torch.clone(
+            self.weight[self.vocab_start_index:self.vocab_end_index],
+            ).detach())
+        del self.original_weight
 
 
 class ParallelEmbedding(torch.nn.Module):
     """Embedding parallelized in the embedding dimension.
 
     This is mainly adapted from torch.nn.Embedding and all the default
     values are kept.
@@ -191,25 +205,27 @@
         output_size: second dimension of matrix A.
         bias: If true, add bias
         gather_output: If true, call all-gether on output and make Y avaiable
                        to all GPUs, otherwise, every GPU will have its output
                        which is Y_i = XA_i
         init_method: method to initialize weights. Note that bias is always set
                      to zero.
-        stride: For the strided linear layers.
+        stride: For the strided linear layers. Seems like only used in initialization, 
+                     but it is homogenerous, so always 1 is okay. # TODO check this conclusion
         keep_master_weight_for_test: This was added for testing and should be
                                      set to False. It returns the master weights
                                      used for initialization.
     """
     def __init__(self, input_size, output_size, bias=True, gather_output=True,
                  init_method=unscaled_init_method(0.02), stride=1,
                  keep_master_weight_for_test=False, params_dtype=torch.float, module=None, name=None, skip_init=False, device=torch.device('cpu')):
         super(ColumnParallelLinear, self).__init__()
 
         # Keep input parameters
+        self.stride = stride
         self.input_size = input_size
         self.output_size = output_size
         self.gather_output = gather_output
         # Divide the weight matrix along the last dimension.
         world_size = get_model_parallel_world_size()
         self.output_size_per_partition = divide(output_size, world_size)
 
@@ -230,27 +246,71 @@
             self.register_parameter('bias', None)
 
         # Initialize weight.
         if not skip_init:
             self.master_weight = _initialize_affine_weight(
                 self.weight, self.output_size, self.input_size,
                 self.output_size_per_partition, 0, init_method,
-                stride=stride, return_master_weight=keep_master_weight_for_test, module=module, name=name)
+                stride=1, return_master_weight=keep_master_weight_for_test, module=module, name=name)
 
     def forward(self, input_):
-        # Set up backprop all-reduce.
+        # Set up backprop all-reduce, and don't change the input.
         input_parallel = copy_to_model_parallel_region(input_)
         # Matrix multiply.
+        # input_parallel: [seq_len, input_size]
+        # weight: [output_size // mp_size, input_size]
+        # bias: [output_size // mp_size]
         output_parallel = F.linear(input_parallel, self.weight, self.bias)
         if self.gather_output:
             # All-gather across the partitions.
             output = gather_from_model_parallel_region(output_parallel)
         else:
             output = output_parallel
         return output
+    
+    def repartition(self):
+        assert self.output_size_per_partition == self.output_size
+        self.output_size_per_partition = divide(self.output_size, get_model_parallel_world_size())
+        mp_rank = get_model_parallel_rank()
+        mp_size = get_model_parallel_world_size()
+        self.original_weight = self.weight
+        # weight is arranged as [stride0...stride1...stride2] * [input_size], extract non-contiguous parts
+        strides = [1]*self.stride if isinstance(self.stride, int) else self.stride # int means equal number of qkv, or ratios
+        assert self.weight.shape[0] % sum(strides) == 0, 'cannot divide weight evenly'
+        factor = self.weight.shape[0] // sum(strides)
+        # decompose weight according to strides
+        strided_weights, _acm = [], 0
+        for i in range(len(strides)):
+            strided_weights.append(self.weight[_acm:_acm+factor*strides[i], :].detach())
+            _acm += factor*strides[i]
+        new_weight = torch.cat([
+            strided_weight[
+                (strided_weight.shape[0]//mp_size)*mp_rank:
+                (strided_weight.shape[0]//mp_size)*(mp_rank+1)
+                ]
+            for strided_weight in strided_weights
+        ], dim=0).contiguous().view(self.output_size_per_partition, self.input_size)
+        self.weight = torch.nn.Parameter(new_weight)
+        del self.original_weight
+        if self.bias is not None:
+            self.original_bias = self.bias
+            # decompose bias according to strides
+            strided_biases, _acm = [], 0
+            for i in range(len(strides)):
+                strided_biases.append(self.bias[_acm:_acm+factor*strides[i]].detach())
+                _acm += factor*strides[i]
+            new_bias = torch.cat([
+                strided_bias[
+                    (strided_bias.shape[0]//mp_size)*mp_rank:
+                    (strided_bias.shape[0]//mp_size)*(mp_rank+1)
+                    ]
+                for strided_bias in strided_biases
+            ], dim=0).contiguous().view(self.output_size_per_partition)
+            self.bias = torch.nn.Parameter(new_bias)
+            del self.original_bias
 
 
 class RowParallelLinear(torch.nn.Module):
     """Linear layer with row parallelism.
 
     The linear layer is defined as Y = XA + b. A is parallelized along
     its first dimension and X along its second dimension as:
@@ -307,22 +367,34 @@
         if not skip_init:
             self.master_weight = _initialize_affine_weight(
                 self.weight, self.output_size, self.input_size,
                 self.input_size_per_partition, 1, init_method,
                 stride=stride, return_master_weight=keep_master_weight_for_test, module=module, name=name)
 
     def forward(self, input_):
-        # Set up backprop all-reduce.
+        # Split the input vector along the last dimension.
         if self.input_is_parallel:
             input_parallel = input_
         else:
             input_parallel = scatter_to_model_parallel_region(input_)
         # Matrix multiply.
+        # input_parallel: [seq_len, input_size // mp_size]
+        # weight: [output_size, input_size // mp_size]
         output_parallel = F.linear(input_parallel, self.weight)
         # All-reduce across all the partitions.
         output_ = reduce_from_model_parallel_region(output_parallel)
         if self.bias is not None:
             output = output_ + self.bias
         else:
             output = output_
         return output
 
+    def repartition(self):
+        assert self.input_size_per_partition == self.input_size
+        self.input_size_per_partition = divide(self.input_size, get_model_parallel_world_size())
+        mp_rank = get_model_parallel_rank()
+        self.original_weight = self.weight
+        self.weight = torch.nn.Parameter(torch.clone(
+            self.weight[:, mp_rank*self.input_size_per_partition
+                            :(mp_rank+1)*self.input_size_per_partition],
+            ).detach())
+        del self.original_weight
```

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/mappings.py` & `SwissArmyTransformer-0.4.0/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/mpu/utils.py` & `SwissArmyTransformer-0.4.0/sat/mpu/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,22 +33,30 @@
 
 def split_tensor_along_last_dim(tensor, num_partitions,
                                 contiguous_split_chunks=False):
     """Split a tensor along its last dimension.
     Arguments:
         tensor: input tensor.
         num_partitions: number of partitions to split the tensor
+            or a list of strides (ratios) for each partition.
         contiguous_split_chunks: If True, make each chunk contiguous
                                  in memory.
     """
     # Get the size and dimension.
     last_dim = tensor.dim() - 1
-    last_dim_size = divide(tensor.size()[last_dim], num_partitions)
+    if isinstance(num_partitions, int):
+        last_dim_size = divide(tensor.size()[last_dim], num_partitions)
     # Split.
-    tensor_list = torch.split(tensor, last_dim_size, dim=last_dim)
+        tensor_list = torch.split(tensor, last_dim_size, dim=last_dim)
+    elif isinstance(num_partitions, (list, tuple)):
+        factor = tensor.size()[last_dim] // sum(num_partitions)
+        tensor_list = torch.split(tensor, [factor * x for x in num_partitions],
+                                  dim=last_dim)
+    else:
+        raise ValueError('num_partitions must be either int or list/tuple.')
     # Note: torch.split does not create contiguous tensors by default.
     if contiguous_split_chunks:
         return tuple(chunk.contiguous() for chunk in tensor_list)
 
     return tensor_list
```

### Comparing `SwissArmyTransformer-0.3.7/sat/ops/layernorm.py` & `SwissArmyTransformer-0.4.0/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.4.0/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/quantization/kernels.py` & `SwissArmyTransformer-0.4.0/sat/quantization/kernels.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/resources/urls.py` & `SwissArmyTransformer-0.4.0/sat/resources/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,18 @@
     'vit-base-patch16-224-in21k': 'https://cloud.tsinghua.edu.cn/f/fdf40233d9034b6a8bdc/?dl=1',
     'deit-tiny': 'https://cloud.tsinghua.edu.cn/f/b759657cb80e4bc69303/?dl=1',
     'deit-small': 'https://cloud.tsinghua.edu.cn/f/51498210e2c943dbbef1/?dl=1',
     'deit-base': 'https://cloud.tsinghua.edu.cn/f/9a26fd1aee7146e1a848/?dl=1',
     'cait-s24-224': 'https://cloud.tsinghua.edu.cn/f/bdfb12396000468b8bb9/?dl=1',
     'gpt2': 'https://cloud.tsinghua.edu.cn/f/4448cff2f1644bd88fa9/?dl=1',
     'chatglm-6b': 'https://cloud.tsinghua.edu.cn/f/26587ca6dd6f45f1ae85/?dl=1',
+    'chatglm2-6b': 'r2://chatglm2-6b.zip',
     'eva02_L_pt_m38m_p14': 'https://cloud.tsinghua.edu.cn/f/98feef10af4f4ff79764/?dl=1',
+    'llama-7b': 'https://cloud.tsinghua.edu.cn/f/8b5c193342c842988357/?dl=1',
+    'llama-13b': 'https://cloud.tsinghua.edu.cn/f/8a9bc9a95d8d40d9a971/?dl=1',
     # CLIP
     'clip': 'https://cloud.tsinghua.edu.cn/f/bd29f0537f9949e6a4fb/?dl=1', # vit-base-patch32
     'clip-vit-base-patch16': 'https://lfs.aminer.cn/misc/clip/clip-vit-base-patch16.zip',
     'clip-vit-large-patch14': 'https://lfs.aminer.cn/misc/clip/clip-vit-large-patch14.zip',
     'yolos-tiny': 'https://cloud.tsinghua.edu.cn/f/8ee048b6a1f1403d9253/?dl=1',
     'mae-vit-base': 'https://cloud.tsinghua.edu.cn/f/5ab3543f0e1d4507ad8c/?dl=1',
     'cogview-base': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
```

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.4.0/sat/training/deepspeed_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,31 @@
 
     param_groups = get_optimizer_param_groups(model)
 
     if args.train_data is not None:
         if args.deepspeed:
             from packaging import version
             print_rank0("DeepSpeed is enabled.", level='DEBUG')
+            # checking optimizer
+            optimizer_name = args.deepspeed_config.get('optimizer',{}).get('type', '')
+            if optimizer_name.startswith('sat.'):
+                from importlib import import_module
+                from functools import partial
+                # split and import 
+                optimizer_callable = getattr(import_module(optimizer_name.rsplit('.', maxsplit=1)[0]), optimizer_name.split('.')[-1])
+                optimizer_callable = partial(optimizer_callable, **args.deepspeed_config.get('optimizer', {}).get('params', {}))
+                print_rank0(f'Using optimizer {optimizer_name} from sat.')
+                del args.deepspeed_config['optimizer']
+            else:
+                optimizer_callable = None
+                
             model, optimizer, _, _ = deepspeed.initialize(
                 model=model,
                 model_parameters=param_groups,
+                optimizer=optimizer_callable,
                 args=args,
                 mpu=mpu,
                 dist_init_required=False,
                 config_params=args.deepspeed_config
                     if version.parse(deepspeed.version) < version.parse("0.9.0")
                     else None
             )
@@ -464,15 +478,15 @@
                 else:
                     # metrics_gathered = None
                     metrics_gathered = [torch.zeros_like(metrics[name], dtype=metrics[name].dtype, device=metrics[name].device) for _ in range(args.world_size)]
                 # torch.distributed.gather(metrics[name], metrics_gathered, 0)
                 torch.distributed.all_gather(metrics_gathered, metrics[name])
 
                 if rank==0:
-                    gathered_len = len(metrics_gathered) if not is_last else len(metrics_gathered) - drop_number
+                    gathered_len = len(metrics_gathered) if not is_last else len(metrics_gathered) - drop_number * args.model_parallel_size
                     for i in range(gathered_len):
                         if is_scalar[name] or not is_last:
                             metrics_total[name].append(metrics_gathered[i].data.cpu())
                         else:
                             metrics_total[name].append(metrics_gathered[i][:last_shape[i]].data.cpu())
     # Move model back to the train mode.
     model.train()
```

### Comparing `SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/training/learning_rates.py` & `SwissArmyTransformer-0.4.0/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/training/model_io.py` & `SwissArmyTransformer-0.4.0/sat/training/model_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import sys
 import math
 import random
 import torch
 import numpy as np
 import json
 import argparse
-
 from sat import mpu
 from sat.helpers import print_rank0, print_all
 
 def get_checkpoint_name(checkpoints_path, iteration, release=False, zero=False):
     if release:
         d = 'release'
     else:
@@ -47,89 +46,120 @@
                     print(e)
     ret = {}
     for k in vars(parser.parse_args([])).keys():
         if hasattr(args, k):
             ret[k] = getattr(args, k)
     return ret
 
+def extract_model_specific_args_to_dump(args, model):
+    module = model.module if hasattr(model, 'module') else model
+    # model_class
+    to_dump = {'model_class': type(module).__name__} 
+    # tokenizer_type
+    if hasattr(args, 'tokenizer_type') and args.tokenizer_type != 'fake':
+        to_dump['tokenizer_type'] = args.tokenizer_type 
+    # architecture related args
+    arch_args_list = ['num_layers', 'hidden_size', 'num_attention_heads', 'vocab_size',
+        'layernorm_order', 'model_parallel_size', 'max_sequence_length',
+        ]
+    for name in arch_args_list: 
+        if hasattr(args, name) and getattr(args, name) is not None:
+            to_dump[name] = getattr(args, name)
+
+    # optional architecture related args, only save if not default
+    # optional means might be changed when loading 
+    optional_arch_args_list = [
+        ('is_decoder', False), 
+        ('cross_attn_hidden_size', None), 
+        ('use_bias', True),
+        ('use_qkv_bias', False),
+        ('inner_hidden_size', None),
+        ('hidden_size_per_attention_head', None),
+        ('use_final_layernorm', True),
+        ('layernorm_epsilon', 1e-5),
+        ('num_multi_query_heads', 0)
+    ]
+    if hasattr(module, 'transformer'):
+        for name, default in optional_arch_args_list:
+            if module.transformer.__dict__[name] != default:
+                to_dump[name] = module.transformer.__dict__[name]
+
+    # model specific args
+    model_specific_args = extract_model_specific_args_from_model(args, module)
+    to_dump.update(model_specific_args)
+    return to_dump
+
+
+def update_ema_parameters_to_model(optimizer):
+    """update ema parameters"""
+    import deepspeed
+    from deepspeed import comm as dist
+    from deepspeed.runtime.utils import all_gather_dp_groups
+    for i, (bit16_partitions, fp32_partition) in enumerate(
+                zip(optimizer.parallel_partitioned_bit16_groups, optimizer.single_partition_of_fp32_groups)):
+            ema_optimizer= optimizer.optimizer
+            state = ema_optimizer.state[fp32_partition]
+            partition_id = dist.get_rank(group=optimizer.real_dp_process_group[i])
+            bit16_partitions[partition_id].data.copy_(state['shadow'].data)
+    
+    all_gather_dp_groups(partitioned_param_groups=optimizer.parallel_partitioned_bit16_groups,
+                             dp_process_group=optimizer.real_dp_process_group,
+                             start_alignment_factor=optimizer.nccl_start_alignment_factor,
+                             allgather_bucket_size=optimizer.allgather_bucket_size)
+
 def save_checkpoint(iteration, model, optimizer,
                     lr_scheduler, args):
     """Save a model checkpoint."""
     if hasattr(args, 'deepspeed') and args.deepspeed:
         if mpu.get_data_parallel_rank() == 0:
             print_rank0('Saving Model...')
             save_ds_checkpoint(iteration, model, lr_scheduler, args)
+        if optimizer.optimizer.__class__.__name__ ==  "FusedEmaAdam" :
+            update_ema_parameters_to_model(optimizer)
+            if mpu.get_data_parallel_rank() == 0:
+                print_rank0('Saving Ema Model...')
+                save_ds_checkpoint(iteration, model, lr_scheduler, args, True)
     elif args.mode == 'inference':
         os.makedirs(os.path.join(args.save, str(iteration)), exist_ok=True)
         torch.save({'module': model.state_dict()}, os.path.join(args.save, str(iteration), 'mp_rank_00_model_states.pt'))
     else:
         raise ValueError("training without deepspeed is not supported.")
     # Wait so everyone is done (necessary)
     torch.distributed.barrier()
     # And update the latest iteration
     if torch.distributed.get_rank() == 0:
         tracker_filename = get_checkpoint_tracker_filename(args.save)
         with open(tracker_filename, 'w') as f:
             f.write(str(iteration))
         # save model_config.json for from_pretrained().
         with open(os.path.join(args.save, 'model_config.json'), 'w') as f:
-            module = model.module if hasattr(model, 'module') else model
-            # model_class
-            to_dump = {'model_class': type(module).__name__} 
-            # tokenizer_type
-            if args.tokenizer_type != 'fake':
-                to_dump['tokenizer_type'] = args.tokenizer_type 
-            # architecture related args
-            arch_args_list = ['num_layers', 'hidden_size', 'num_attention_heads', 'vocab_size',
-             'layernorm_order', 'model_parallel_size', 'max_sequence_length',
-             ]
-            for name in arch_args_list: 
-                if hasattr(args, name) and getattr(args, name) is not None:
-                    to_dump[name] = getattr(args, name)
-
-            # optional architecture related args, only save if not default
-            # optional means might be changed when loading 
-            optional_arch_args_list = [
-                ('is_decoder', False), 
-                ('cross_attn_hidden_size', None), 
-                ('use_bias', True),
-                ('inner_hidden_size', None),
-                ('hidden_size_per_attention_head', None),
-                ('use_final_layernorm', True),
-                ('layernorm_epsilon', 1e-5),
-            ]
-            if hasattr(module, 'transformer'):
-                for name, default in optional_arch_args_list:
-                    if module.transformer.__dict__[name] != default:
-                        to_dump[name] = module.transformer.__dict__[name]
-
-            # model specific args
-            model_specific_args = extract_model_specific_args_from_model(args, module)
-            to_dump.update(model_specific_args)
-
+            to_dump = extract_model_specific_args_to_dump(args, model)
             json.dump(to_dump, f, indent=4)
 
     # Wait so everyone is done (not necessary)
     torch.distributed.barrier()
 
 
-def save_ds_checkpoint(iteration, model, lr_scheduler, args):
+def save_ds_checkpoint(iteration, model, lr_scheduler, args, use_ema = False):
     """Save a model checkpoint."""
 
     sd = {}
     sd['iteration'] = iteration
     if lr_scheduler is not None:
         sd['client_lr_scheduler'] = lr_scheduler.state_dict()
     # rng states.
     if not args.no_save_rng:
         sd['random_rng_state'] = random.getstate()
         sd['np_rng_state'] = np.random.get_state()
         sd['torch_rng_state'] = torch.get_rng_state()
         sd['cuda_rng_state'] = torch.cuda.get_rng_state()
-    save_ds_checkpoint_no_optim(model, args.save, str(iteration), client_state=sd)
+    if not use_ema:
+        save_ds_checkpoint_no_optim(model, args.save, str(iteration), client_state=sd)
+    else:
+        save_ds_checkpoint_no_optim(model, args.save, str(iteration)+'-ema', client_state=sd)
 
 
 def save_ds_checkpoint_no_optim(model, save_dir, tag=None, client_state={}, save_latest=True):
     os.makedirs(save_dir, exist_ok=True)
     # Ensure tag is a string
     tag = str(tag)
     # Real save via deepspeed
@@ -212,19 +242,21 @@
     if len(missing_keys) > 0:
         if args.mode == 'inference':
             if 'force_inference' in args and args.force_inference:
                 print_rank0(f'Warning: Missing keys for inference: {missing_keys}.')
             else:
                 raise ValueError(f'Missing keys for inference: {missing_keys}.\nIf you still want to inference anyway, pass --force_inference to args.')
         else: # new params
-            assert all(name.find('mixins')>=0 for name in missing_keys), missing_keys
+            assert all(name.find('mixins')>=0 or name.find('cross_attention')>=0 for name in missing_keys), missing_keys
             assert args.mode == 'finetune'
             # list all mixin names
             mixin_names = []
             for key_name in missing_keys:
+                if key_name.find('mixins') < 0:
+                    continue
                 parts = key_name.split('.')
                 mixin_name = parts[parts.index('mixins')+1]
                 if mixin_name not in mixin_names:
                     mixin_names.append(mixin_name)
             module.reinit(mixin_names) # initialize mixins
 
     # Do not need this any more, because we create optimizer after load now.
```

### Comparing `SwissArmyTransformer-0.3.7/sat/training/utils.py` & `SwissArmyTransformer-0.4.0/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/sat/transformer_defaults.py` & `SwissArmyTransformer-0.4.0/sat/transformer_defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -39,24 +39,49 @@
                 attention_probs = attention_dropout(attention_probs)
         else:
             attention_probs = attention_dropout(attention_probs)
 
     context_layer = torch.matmul(attention_probs, value_layer)
     return context_layer
 
+def attention_fn_default(query_layer, key_layer, value_layer, attention_mask,
+                       attention_dropout=None, log_attention_weights=None, scaling_attention_score=True, **kwargs):
+    # expand head dim to query dim, if necessary
+    # only useful for multi-query attention
+    batch_size, num_query_heads = query_layer.shape[:2] # [b, np, s, hn]
+    num_kv_heads = key_layer.shape[1] # [b, np, s, hn]
+    key_layer = key_layer.unsqueeze(2).expand(-1, -1, num_query_heads//num_kv_heads, -1, -1).contiguous().view(batch_size, num_query_heads, *key_layer.shape[2:])
+    value_layer = value_layer.unsqueeze(2).expand(-1, -1, num_query_heads//num_kv_heads, -1, -1).contiguous().view(batch_size, num_query_heads, *value_layer.shape[2:])
+
+    if int(torch.__version__.split('.')[0]) >= 2:
+        assert scaling_attention_score == True
+        dropout_p = 0. if attention_dropout is None or not attention_dropout.training else attention_dropout.p
+        attention_mask = (attention_mask >= 0.5).bool()
+        return torch.nn.functional.scaled_dot_product_attention(
+            query_layer, key_layer, value_layer, 
+            attention_mask,
+            dropout_p
+        )
+    else:
+        return standard_attention(
+            query_layer, key_layer, value_layer, attention_mask,
+            attention_dropout=attention_dropout, log_attention_weights=log_attention_weights,
+            scaling_attention_score=scaling_attention_score, **kwargs
+        )
+
 def attention_forward_default(self, hidden_states, mask, **kw_args):
     self = self.transformer.layers[kw_args['layer_id']].attention
-    attention_fn = standard_attention
+    attention_fn = attention_fn_default
     if 'attention_fn' in self.hooks:
         attention_fn = self.hooks['attention_fn']
 
     mixed_raw_layer = self.query_key_value(hidden_states)
     (mixed_query_layer,
         mixed_key_layer,
-        mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
+        mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, self.stride)
 
     dropout_fn = self.attention_dropout if self.training else None
 
     query_layer = self._transpose_for_scores(mixed_query_layer)
     key_layer = self._transpose_for_scores(mixed_key_layer)
     value_layer = self._transpose_for_scores(mixed_value_layer)
 
@@ -162,16 +187,33 @@
         output = mlp_input + mlp_output
     else:
         output = hidden_states + mlp_output
 
     return output
 
 HOOKS_DEFAULT = {
-    'attention_fn': standard_attention,
+    'attention_fn': attention_fn_default,
     'attention_forward': attention_forward_default,
     'cross_attention_forward': cross_attention_forward_default,
     'mlp_forward': mlp_forward_default,
     'word_embedding_forward': word_embedding_forward_default,
     'position_embedding_forward': position_embedding_forward_default,
     'final_forward': final_forward_default,
     'layer_forward': layer_forward_default
 }
+
+ARGS_DEFAULT = {
+    'embedding_dropout_prob': ('hidden_dropout', 0),
+    'attention_dropout_prob': ('attention_dropout', 0),
+    'output_dropout_prob': ('hidden_dropout', 0),
+    'inner_hidden_size': ('inner_hidden_size', None),
+    'hidden_size_per_attention_head': ('hidden_size_per_attention_head', None),
+    'checkpoint_activations': ('checkpoint_activations', False),
+    'checkpoint_num_layers': ('checkpoint_num_layers', 1),
+    'is_decoder': ('is_decoder', False),
+    'cross_attn_hidden_size': ('cross_attn_hidden_size', None),
+    'use_final_layernorm': ('use_final_layernorm', True),
+    'layernorm_epsilon': ('layernorm_epsilon', 1e-5),
+    'use_bias': ('use_bias', True),
+    'use_qkv_bias': ('use_qkv_bias', False),
+    'num_multi_query_heads': ('num_multi_query_heads', 0)
+}
```

### Comparing `SwissArmyTransformer-0.3.7/setup.py` & `SwissArmyTransformer-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.3.7',
+    version='0.4.0',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.3.7/tests/test_base_model.py` & `SwissArmyTransformer-0.4.0/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_inference.py` & `SwissArmyTransformer-0.4.0/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_nested_model.py` & `SwissArmyTransformer-0.4.0/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_speed.py` & `SwissArmyTransformer-0.4.0/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_train.py` & `SwissArmyTransformer-0.4.0/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_train_dp.py` & `SwissArmyTransformer-0.4.0/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.7/tests/test_train_nested.py` & `SwissArmyTransformer-0.4.0/tests/test_train_nested.py`

 * *Files identical despite different names*

