# Comparing `tmp/vllm-0.1.1.tar.gz` & `tmp/vllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm-0.1.1.tar", last modified: Thu Jun 22 07:39:10 2023, max compression
+gzip compressed data, was "vllm-0.1.2.tar", last modified: Wed Jul  5 04:52:32 2023, max compression
```

## Comparing `vllm-0.1.1.tar` & `vllm-0.1.2.tar`

### file list

```diff
@@ -1,94 +1,103 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.312857 vllm-0.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-05-19 19:30:16.000000 vllm-0.1.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-06-06 03:07:23.000000 vllm-0.1.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2023-06-22 07:39:10.310857 vllm-0.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4257 2023-06-21 15:58:37.000000 vllm-0.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.779801 vllm-0.1.1/csrc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-04-02 07:37:46.000000 vllm-0.1.1/csrc/activation.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/activation_kernels.cu
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.839808 vllm-0.1.1/csrc/attention/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-06-03 11:19:52.000000 vllm-0.1.1/csrc/attention/attention_dtypes.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1721 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_generic.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19900 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1850 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_utils.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10962 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_bfloat16.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10793 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_float16.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_float32.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/attention.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/cache.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14699 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/cache_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2023-03-31 16:51:49.000000 vllm-0.1.1/csrc/layernorm.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/layernorm_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/pos_encoding.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2901 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/pos_encoding_kernels.cu
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1592 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/reduction_utils.cuh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2023-06-06 03:07:24.000000 vllm-0.1.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-24 04:45:48.000000 vllm-0.1.1/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-22 07:39:10.314858 vllm-0.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6082 2023-06-21 15:58:37.000000 vllm-0.1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.903815 vllm-0.1.1/vllm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1831 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/block.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8486 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.976822 vllm-0.1.1/vllm/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10341 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/block_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      896 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/policy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2023-06-21 15:58:37.000000 vllm-0.1.1/vllm/core/scheduler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.033828 vllm-0.1.1/vllm/engine/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/engine/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6546 2023-06-18 13:35:33.000000 vllm-0.1.1/vllm/engine/arg_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8927 2023-06-22 07:23:09.000000 vllm-0.1.1/vllm/engine/async_llm_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/engine/llm_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4233 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/engine/ray_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-06-21 15:58:37.000000 vllm-0.1.1/vllm/engine/tokenizer_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.060831 vllm-0.1.1/vllm/entrypoints/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2970 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5726 2023-06-22 07:23:09.000000 vllm-0.1.1/vllm/entrypoints/llm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.086834 vllm-0.1.1/vllm/entrypoints/openai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12233 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3895 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/protocol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.131839 vllm-0.1.1/vllm/model_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2194 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/input_metadata.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.173843 vllm-0.1.1/vllm/model_executor/layers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/activation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9322 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/attention.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/layernorm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16062 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/sampler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1836 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/model_loader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.216848 vllm-0.1.1/vllm/model_executor/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12118 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/gpt2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10979 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/gpt_neox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11763 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/llama.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12958 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/opt.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.234849 vllm-0.1.1/vllm/model_executor/parallel_utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22861 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/parallel_state.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.278854 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18207 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8586 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2460 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/weight_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4093 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/outputs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/sampling_params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7767 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/sequence.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      730 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.300856 vllm-0.1.1/vllm/worker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/worker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-06-18 08:57:00.000000 vllm-0.1.1/vllm/worker/cache_engine.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12283 2023-06-18 08:56:51.000000 vllm-0.1.1/vllm/worker/worker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.943819 vllm-0.1.1/vllm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2290 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.593359 vllm-0.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-05-19 19:30:16.000000 vllm-0.1.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-06-06 03:07:23.000000 vllm-0.1.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-07-05 04:52:32.590359 vllm-0.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4794 2023-07-05 04:42:28.000000 vllm-0.1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.035305 vllm-0.1.2/csrc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-04-02 07:37:46.000000 vllm-0.1.2/csrc/activation.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/activation_kernels.cu
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.104312 vllm-0.1.2/csrc/attention/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-06-03 11:19:52.000000 vllm-0.1.2/csrc/attention/attention_dtypes.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1721 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/attention_generic.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20688 2023-07-05 04:42:28.000000 vllm-0.1.2/csrc/attention/attention_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1850 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/attention_utils.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10962 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_bfloat16.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10793 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_float16.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/attention/dtype_float32.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      595 2023-07-03 20:41:37.000000 vllm-0.1.2/csrc/attention.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-05-19 19:30:17.000000 vllm-0.1.2/csrc/cache.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14699 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/cache_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2023-03-31 16:51:49.000000 vllm-0.1.2/csrc/layernorm.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/layernorm_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-05-19 19:30:17.000000 vllm-0.1.2/csrc/pos_encoding.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2901 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/pos_encoding_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1592 2023-06-18 04:39:39.000000 vllm-0.1.2/csrc/reduction_utils.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2023-06-06 03:07:24.000000 vllm-0.1.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-07-05 04:42:28.000000 vllm-0.1.2/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-05 04:52:32.594359 vllm-0.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6038 2023-06-29 15:14:11.000000 vllm-0.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.173318 vllm-0.1.2/vllm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1852 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/block.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9369 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.239325 vllm-0.1.2/vllm/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10443 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/core/block_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      896 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/core/policy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18979 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/core/scheduler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.276328 vllm-0.1.2/vllm/engine/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/engine/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8079 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/engine/arg_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9653 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/engine/async_llm_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14359 2023-07-03 21:53:08.000000 vllm-0.1.2/vllm/engine/llm_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/engine/ray_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.298330 vllm-0.1.2/vllm/entrypoints/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/entrypoints/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2983 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6279 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/llm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.320332 vllm-0.1.2/vllm/entrypoints/openai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/entrypoints/openai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22383 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/entrypoints/openai/api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5299 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/entrypoints/openai/protocol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1615 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.360336 vllm-0.1.2/vllm/model_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      246 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2023-07-03 20:41:37.000000 vllm-0.1.2/vllm/model_executor/input_metadata.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.399340 vllm-0.1.2/vllm/model_executor/layers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/model_executor/layers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1164 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/layers/activation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15036 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/layers/attention.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-06-18 04:39:39.000000 vllm-0.1.2/vllm/model_executor/layers/layernorm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16825 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/layers/sampler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/model_loader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.465346 vllm-0.1.2/vllm/model_executor/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12489 2023-07-03 21:53:08.000000 vllm-0.1.2/vllm/model_executor/models/bloom.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/gpt2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14532 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/gpt_bigcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11460 2023-07-03 20:41:37.000000 vllm-0.1.2/vllm/model_executor/models/gpt_neox.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12189 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/llama.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/model_executor/models/mpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13635 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/models/opt.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.481348 vllm-0.1.2/vllm/model_executor/parallel_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22861 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/parallel_state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.522352 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18207 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8586 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/random.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2460 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/model_executor/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4472 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/model_executor/weight_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4139 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/outputs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6702 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/sampling_params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9648 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/sequence.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.543354 vllm-0.1.2/vllm/transformers_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 15:14:11.000000 vllm-0.1.2/vllm/transformers_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.558355 vllm-0.1.2/vllm/transformers_utils/configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/configs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2261 2023-07-05 04:42:28.000000 vllm-0.1.2/vllm/transformers_utils/configs/mpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3907 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/transformers_utils/tokenizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      893 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.580358 vllm-0.1.2/vllm/worker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:40.000000 vllm-0.1.2/vllm/worker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5980 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/worker/cache_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2023-07-03 19:04:57.000000 vllm-0.1.2/vllm/worker/worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:52:32.209322 vllm-0.1.2/vllm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2561 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      120 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-05 04:52:31.000000 vllm-0.1.2/vllm.egg-info/top_level.txt
```

### Comparing `vllm-0.1.1/LICENSE` & `vllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/PKG-INFO` & `vllm-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
@@ -31,41 +31,44 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
-
-- [2023/06] We officially released vLLM! vLLM has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid April. Check out our [blog post](https://vllm.ai).
+- [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
+- [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
 vLLM is fast with:
 
 - State-of-the-art serving throughput
 - Efficient management of attention key and value memory with **PagedAttention**
-- Dynamic batching of incoming requests
+- Continuous batching of incoming requests
 - Optimized CUDA kernels
 
 vLLM is flexible and easy to use with:
 
 - Seamless integration with popular HuggingFace models
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
-- GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
+- GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
 - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
 ```
```

#### html2text {}

```diff
@@ -1,46 +1,53 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.1 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.2 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] We officially released vLLM! vLLM has
-powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid
-April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
-to-use library for LLM inference and serving. vLLM is fast with: - State-of-
-the-art serving throughput - Efficient management of attention key and value
-memory with **PagedAttention** - Dynamic batching of incoming requests -
-Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
-integration with popular HuggingFace models - High-throughput serving with
-various decoding algorithms, including *parallel sampling*, *beam search*, and
-more - Tensor parallelism support for distributed inference - Streaming outputs
-- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
-models, including the following architectures: - GPT-2 (`gpt2`, `gpt2-xl`,
-etc.) - GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`,
-`stabilityai/stablelm-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`,
-`young-geng/koala`, `openlm-research/open_llama_13b`, etc.) - OPT (`facebook/
-opt-66b`, `facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from
-source](https://vllm.readthedocs.io/en/latest/getting_started/
-installation.html#build-from-source): ```bash pip install vllm ``` ## Getting
-Started Visit our [documentation](https://vllm.readthedocs.io/en/latest/) to
-get started. - [Installation](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html) - [Quickstart](https://vllm.readthedocs.io/
-en/latest/getting_started/quickstart.html) - [Supported Models](https://
-vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
-outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
-Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
-our [blog post](https://vllm.ai).
+--- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
+Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
+master/llm/vllm) to start the vLLM demo, and the [blog post](https://
+blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
+) for the story behind vLLM development on the clouds. - [2023/06] We
+officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
+and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
+post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
+inference and serving. vLLM is fast with: - State-of-the-art serving throughput
+- Efficient management of attention key and value memory with
+**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
+kernels vLLM is flexible and easy to use with: - Seamless integration with
+popular HuggingFace models - High-throughput serving with various decoding
+algorithms, including *parallel sampling*, *beam search*, and more - Tensor
+parallelism support for distributed inference - Streaming outputs - OpenAI-
+compatible API server vLLM seamlessly supports many Huggingface models,
+including the following architectures: - BLOOM (`bigscience/bloom`,
+`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
+(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+(`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
+tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
+`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
+mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
+Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
+getting_started/installation.html#build-from-source): ```bash pip install vllm
+``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
+en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
+latest/getting_started/installation.html) - [Quickstart](https://
+vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
+Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
+Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
+Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
+details, check out our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.1/README.md` & `vllm-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,41 +13,44 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
-
-- [2023/06] We officially released vLLM! vLLM has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid April. Check out our [blog post](https://vllm.ai).
+- [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
+- [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
 vLLM is fast with:
 
 - State-of-the-art serving throughput
 - Efficient management of attention key and value memory with **PagedAttention**
-- Dynamic batching of incoming requests
+- Continuous batching of incoming requests
 - Optimized CUDA kernels
 
 vLLM is flexible and easy to use with:
 
 - Seamless integration with popular HuggingFace models
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
-- GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
+- GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
 - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
 ```
```

#### html2text {}

```diff
@@ -1,36 +1,43 @@
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] We officially released vLLM! vLLM has
-powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid
-April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
-to-use library for LLM inference and serving. vLLM is fast with: - State-of-
-the-art serving throughput - Efficient management of attention key and value
-memory with **PagedAttention** - Dynamic batching of incoming requests -
-Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
-integration with popular HuggingFace models - High-throughput serving with
-various decoding algorithms, including *parallel sampling*, *beam search*, and
-more - Tensor parallelism support for distributed inference - Streaming outputs
-- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
-models, including the following architectures: - GPT-2 (`gpt2`, `gpt2-xl`,
-etc.) - GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`,
-`stabilityai/stablelm-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`,
-`young-geng/koala`, `openlm-research/open_llama_13b`, etc.) - OPT (`facebook/
-opt-66b`, `facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from
-source](https://vllm.readthedocs.io/en/latest/getting_started/
-installation.html#build-from-source): ```bash pip install vllm ``` ## Getting
-Started Visit our [documentation](https://vllm.readthedocs.io/en/latest/) to
-get started. - [Installation](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html) - [Quickstart](https://vllm.readthedocs.io/
-en/latest/getting_started/quickstart.html) - [Supported Models](https://
-vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
-outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
-Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
-our [blog post](https://vllm.ai).
+--- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
+Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
+master/llm/vllm) to start the vLLM demo, and the [blog post](https://
+blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
+) for the story behind vLLM development on the clouds. - [2023/06] We
+officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
+and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
+post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
+inference and serving. vLLM is fast with: - State-of-the-art serving throughput
+- Efficient management of attention key and value memory with
+**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
+kernels vLLM is flexible and easy to use with: - Seamless integration with
+popular HuggingFace models - High-throughput serving with various decoding
+algorithms, including *parallel sampling*, *beam search*, and more - Tensor
+parallelism support for distributed inference - Streaming outputs - OpenAI-
+compatible API server vLLM seamlessly supports many Huggingface models,
+including the following architectures: - BLOOM (`bigscience/bloom`,
+`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
+(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+(`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
+tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
+`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
+mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
+Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
+getting_started/installation.html#build-from-source): ```bash pip install vllm
+``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
+en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
+latest/getting_started/installation.html) - [Quickstart](https://
+vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
+Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
+Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
+Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
+details, check out our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.1/csrc/activation_kernels.cu` & `vllm-0.1.2/csrc/activation_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention/attention_generic.cuh` & `vllm-0.1.2/csrc/attention/attention_generic.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention/attention_kernels.cu` & `vllm-0.1.2/csrc/attention/attention_kernels.cu`

 * *Files 3% similar despite different names*

```diff
@@ -76,25 +76,27 @@
   const scalar_t* __restrict__ q,         // [num_seqs, num_heads, head_size]
   const scalar_t* __restrict__ k_cache,   // [num_blocks, num_heads, head_size/x, block_size, x]
   const scalar_t* __restrict__ v_cache,   // [num_blocks, num_heads, head_size, block_size]
   const float scale,
   const int* __restrict__ block_tables,   // [num_seqs, max_num_blocks_per_seq]
   const int* __restrict__ context_lens,   // [num_seqs]
   const int max_num_blocks_per_seq,
+  const float* __restrict__ alibi_slopes, // [num_heads]
   const int q_stride) {
   constexpr int THREAD_GROUP_SIZE = MAX(WARP_SIZE / BLOCK_SIZE, 1);
   constexpr int NUM_TOKENS_PER_THREAD_GROUP = (BLOCK_SIZE + WARP_SIZE - 1) / WARP_SIZE;
   constexpr int NUM_WARPS = NUM_THREADS / WARP_SIZE;
   const int thread_idx = threadIdx.x;
   const int warp_idx = thread_idx / WARP_SIZE;
   const int lane = thread_idx % WARP_SIZE;
 
   const int head_idx = blockIdx.x;
   const int num_heads = gridDim.x;
   const int seq_idx = blockIdx.y;
+  const float alibi_slope = alibi_slopes == nullptr ? 0.f : alibi_slopes[head_idx];
 
   // A vector type to store a part of a key or a query.
   // The vector size is configured in such a way that the threads in a thread group
   // fetch or compute 16 bytes at a time.
   // For example, if the size of a thread group is 4 and the data type is half,
   // then the vector size is 16 / (4 * sizeof(half)) == 2.
   constexpr int VEC_SIZE = MAX(16 / (THREAD_GROUP_SIZE * sizeof(scalar_t)), 1);
@@ -163,20 +165,22 @@
         const int offset1 = (vec_idx * VEC_SIZE) / x;
         const int offset2 = (vec_idx * VEC_SIZE) % x;
         k_vecs[j] = *reinterpret_cast<const K_vec*>(k_ptr + offset1 * BLOCK_SIZE * x + offset2);
       }
 
       // Compute dot product.
       // This includes a reduction across the threads in the same thread group.
-      const float qk = scale * Qk_dot<scalar_t, THREAD_GROUP_SIZE>::dot(q_vecs, k_vecs);
-      const bool mask = token_idx >= context_len;
-    
+      float qk = scale * Qk_dot<scalar_t, THREAD_GROUP_SIZE>::dot(q_vecs, k_vecs);
+      // Add the ALiBi bias if slopes are given.
+      qk += (alibi_slope != 0) ? alibi_slope * (token_idx - context_len) : 0;
+
       if (thread_group_offset == 0) {
         // Store the partial reductions to shared memory.
         // NOTE(woosuk): It is required to zero out the masked logits.
+        const bool mask = token_idx >= context_len;
         logits[token_idx] = mask ? 0.f : qk;
         // Update the max value.
         qk_max = mask ? qk_max : fmaxf(qk_max, qk);
       }
     }
   }
 
@@ -324,14 +328,15 @@
     query_ptr,                                                                                \
     key_cache_ptr,                                                                            \
     value_cache_ptr,                                                                          \
     scale,                                                                                    \
     block_tables_ptr,                                                                         \
     context_lens_ptr,                                                                         \
     max_num_blocks_per_seq,                                                                   \
+    alibi_slopes_ptr,                                                                         \
     query_stride);
 
 // TODO(woosuk): Tune NUM_THREADS.
 template<
   typename T,
   int BLOCK_SIZE,
   int NUM_THREADS = 128>
@@ -339,24 +344,30 @@
   torch::Tensor& out,
   torch::Tensor& query,
   torch::Tensor& key_cache,
   torch::Tensor& value_cache,
   float scale,
   torch::Tensor& block_tables,
   torch::Tensor& context_lens,
-  int max_context_len) {
+  int max_context_len,
+  const c10::optional<torch::Tensor>& alibi_slopes) {
   int num_seqs = query.size(0);
   int num_heads = query.size(1);
   int head_size = query.size(2);
   int max_num_blocks_per_seq = block_tables.size(1);
   int query_stride = query.stride(0);
 
   int thread_group_size = MAX(WARP_SIZE / BLOCK_SIZE, 1);
   assert(head_size % thread_group_size == 0);
 
+  // NOTE: alibi_slopes is optional.
+  const float* alibi_slopes_ptr = alibi_slopes ?
+    reinterpret_cast<const float*>(alibi_slopes.value().data_ptr())
+    : nullptr;
+
   T* out_ptr = reinterpret_cast<T*>(out.data_ptr());
   T* query_ptr = reinterpret_cast<T*>(query.data_ptr());
   T* key_cache_ptr = reinterpret_cast<T*>(key_cache.data_ptr());
   T* value_cache_ptr = reinterpret_cast<T*>(value_cache.data_ptr());
   int* block_tables_ptr = block_tables.data_ptr<int>();
   int* context_lens_ptr = context_lens.data_ptr<int>();
 
@@ -380,14 +391,17 @@
       break;
     case 80:
       LAUNCH_ATTENTION_KERNEL(T, 80, BLOCK_SIZE, NUM_THREADS);
       break;
     case 96:
       LAUNCH_ATTENTION_KERNEL(T, 96, BLOCK_SIZE, NUM_THREADS);
       break;
+    case 112:
+      LAUNCH_ATTENTION_KERNEL(T, 112, BLOCK_SIZE, NUM_THREADS);
+      break;
     case 128:
       LAUNCH_ATTENTION_KERNEL(T, 128, BLOCK_SIZE, NUM_THREADS);
       break;
     // case 160:
     //   LAUNCH_ATTENTION_KERNEL(T, 160, BLOCK_SIZE, NUM_THREADS);
     //   break;
     // case 192:
@@ -407,15 +421,16 @@
     out,                                                            \
     query,                                                          \
     key_cache,                                                      \
     value_cache,                                                    \
     scale,                                                          \
     block_tables,                                                   \
     context_lens,                                                   \
-    max_context_len);
+    max_context_len,                                                \
+    alibi_slopes);
 
 // NOTE(woosuk): To reduce the compilation time, we omitted block sizes
 // 1, 2, 4, 64, 128, 256.
 #define CALL_KERNEL_LAUNCHER_BLOCK_SIZE(T)                          \
   switch (block_size) {                                             \
     /* case 1:                         */                           \
     /*   CALL_KERNEL_LAUNCHER(T, 1);   */                           \
@@ -454,15 +469,16 @@
   torch::Tensor& query,           // [num_seqs, num_heads, head_size]
   torch::Tensor& key_cache,       // [num_blocks, num_heads, head_size/x, block_size, x]
   torch::Tensor& value_cache,     // [num_blocks, num_heads, head_size, block_size]
   float scale,
   torch::Tensor& block_tables,    // [num_seqs, max_num_blocks_per_seq]
   torch::Tensor& context_lens,    // [num_seqs]
   int block_size,
-  int max_context_len) {
+  int max_context_len,
+  const c10::optional<torch::Tensor>& alibi_slopes) {
   if (query.dtype() == at::ScalarType::Float) {
     CALL_KERNEL_LAUNCHER_BLOCK_SIZE(float);
   } else if (query.dtype() == at::ScalarType::Half) {
     CALL_KERNEL_LAUNCHER_BLOCK_SIZE(uint16_t);
   } else if (query.dtype() == at::ScalarType::BFloat16) {
     CALL_KERNEL_LAUNCHER_BLOCK_SIZE(__nv_bfloat16);
   } else {
```

### Comparing `vllm-0.1.1/csrc/attention/attention_utils.cuh` & `vllm-0.1.2/csrc/attention/attention_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention/dtype_bfloat16.cuh` & `vllm-0.1.2/csrc/attention/dtype_bfloat16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention/dtype_float16.cuh` & `vllm-0.1.2/csrc/attention/dtype_float16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention/dtype_float32.cuh` & `vllm-0.1.2/csrc/attention/dtype_float32.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/attention.cpp` & `vllm-0.1.2/csrc/attention.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #include <torch/extension.h>
+#include <c10/util/Optional.h>
 
 void single_query_cached_kv_attention(
   torch::Tensor& out,
   torch::Tensor& query,
   torch::Tensor& key_cache,
   torch::Tensor& value_cache,
   float scale,
   torch::Tensor& block_tables,
   torch::Tensor& context_lens,
   int block_size,
-  int max_context_len);
+  int max_context_len,
+  const c10::optional<torch::Tensor>& alibi_slopes);
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
   m.def(
     "single_query_cached_kv_attention",
     &single_query_cached_kv_attention,
     "Compute the attention between an input query and the cached key/value tensors");
 }
```

### Comparing `vllm-0.1.1/csrc/cache.cpp` & `vllm-0.1.2/csrc/cache.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/cache_kernels.cu` & `vllm-0.1.2/csrc/cache_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/layernorm_kernels.cu` & `vllm-0.1.2/csrc/layernorm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/pos_encoding_kernels.cu` & `vllm-0.1.2/csrc/pos_encoding_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/csrc/reduction_utils.cuh` & `vllm-0.1.2/csrc/reduction_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/setup.py` & `vllm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 # TODO(woosuk): Should we use -O3?
 NVCC_FLAGS = ["-O2", "-std=c++17"]
 
 ABI = 1 if torch._C._GLIBCXX_USE_CXX11_ABI else 0
 CXX_FLAGS += [f"-D_GLIBCXX_USE_CXX11_ABI={ABI}"]
 NVCC_FLAGS += [f"-D_GLIBCXX_USE_CXX11_ABI={ABI}"]
 
-if not torch.cuda.is_available():
+if CUDA_HOME is None:
     raise RuntimeError(
-        f"Cannot find CUDA at CUDA_HOME: {CUDA_HOME}. "
-        "CUDA must be available in order to build the package.")
+        f"Cannot find CUDA_HOME. CUDA must be available in order to build the package.")
 
 
 def get_nvcc_cuda_version(cuda_dir: str) -> Version:
     """Get the CUDA version from nvcc.
 
     Adapted from https://github.com/NVIDIA/apex/blob/8b7a1ff183741dd8f9b87e7bafd04cfde99cea28/setup.py
     """
```

### Comparing `vllm-0.1.1/vllm/__init__.py` & `vllm-0.1.2/vllm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""vLLM: a high-throughput and memory-efficient inference engine for LLMs"""
+
 from vllm.engine.arg_utils import AsyncEngineArgs, EngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.ray_utils import initialize_cluster
 from vllm.entrypoints.llm import LLM
 from vllm.outputs import CompletionOutput, RequestOutput
 from vllm.sampling_params import SamplingParams
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __all__ = [
     "LLM",
     "SamplingParams",
     "RequestOutput",
     "CompletionOutput",
     "LLMEngine",
```

### Comparing `vllm-0.1.1/vllm/block.py` & `vllm-0.1.2/vllm/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         return self.block_size - self.num_tokens
 
     def is_full(self) -> bool:
         return self.num_tokens == self.block_size
 
     def append_tokens(self, token_ids: List[int]) -> None:
         assert len(token_ids) <= self.get_num_empty_slots()
-        self.token_ids[self.num_tokens:self.num_tokens + len(token_ids)] = token_ids
+        curr_idx = self.num_tokens
+        self.token_ids[curr_idx:curr_idx + len(token_ids)] = token_ids
         self.num_tokens += len(token_ids)
 
     def get_token_ids(self) -> List[int]:
         return self.token_ids[:self.num_tokens]
 
     def get_last_token_id(self) -> int:
         assert self.num_tokens > 0
```

### Comparing `vllm-0.1.1/vllm/config.py` & `vllm-0.1.2/vllm/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 from typing import Optional
 
 import torch
-from transformers import AutoConfig, PretrainedConfig
+from transformers import PretrainedConfig
 
 from vllm.logger import init_logger
+from vllm.transformers_utils.config import get_config
 from vllm.utils import get_cpu_memory
 
 logger = init_logger(__name__)
 
-_GiB = 1 << 30
+_GB = 1 << 30
 
 
 class ModelConfig:
     """Configuration for the model.
 
     Args:
         model: Name or path of the huggingface model to use.
+        tokenizer: Name or path of the huggingface tokenizer to use.
+        tokenizer_mode: Tokenizer mode. "auto" will use the fast tokenizer if
+            available, and "slow" will always use the slow tokenizer.
         download_dir: Directory to download and load the weights, default to the
             default cache directory of huggingface.
         use_np_weights: Save a numpy copy of model weights for faster loading.
             This can increase the disk usage by up to 2x.
         use_dummy_weights: Use dummy values for model weights (for profiling).
         dtype: Data type for model weights and activations. The "auto" option
             will use FP16 precision for FP32 and FP16 models, and BF16 precision
             for BF16 models.
         seed: Random seed for reproducibility.
     """
 
     def __init__(
         self,
         model: str,
+        tokenizer: str,
+        tokenizer_mode: str,
         download_dir: Optional[str],
         use_np_weights: bool,
         use_dummy_weights: bool,
         dtype: str,
         seed: int,
     ) -> None:
         self.model = model
+        self.tokenizer = tokenizer
+        self.tokenizer_mode = tokenizer_mode
         self.download_dir = download_dir
         self.use_np_weights = use_np_weights
         self.use_dummy_weights = use_dummy_weights
         self.seed = seed
 
-        self.hf_config: PretrainedConfig = AutoConfig.from_pretrained(model)
+        self.hf_config = get_config(model)
         self.dtype = _get_and_verify_dtype(self.hf_config, dtype)
+        self._verify_tokenizer_mode()
+
+    def _verify_tokenizer_mode(self) -> None:
+        tokenizer_mode = self.tokenizer_mode.lower()
+        if tokenizer_mode not in ["auto", "slow"]:
+            raise ValueError(
+                f"Unknown tokenizer mode: {self.tokenizer_mode}. Must be "
+                "either 'auto' or 'slow'.")
+        self.tokenizer_mode = tokenizer_mode
 
     def verify_with_parallel_config(
         self,
         parallel_config: "ParallelConfig",
     ) -> None:
         total_num_attention_heads = self.hf_config.num_attention_heads
         tensor_parallel_size = parallel_config.tensor_parallel_size
@@ -86,23 +103,24 @@
 
     Args:
         block_size: Size of a cache block in number of tokens.
         gpu_memory_utilization: Fraction of GPU memory to use for the
             vLLM execution.
         swap_space: Size of the CPU swap space per GPU (in GiB).
     """
+
     def __init__(
         self,
         block_size: int,
         gpu_memory_utilization: float,
         swap_space: int,
     ) -> None:
         self.block_size = block_size
         self.gpu_memory_utilization = gpu_memory_utilization
-        self.swap_space_bytes = swap_space * _GiB
+        self.swap_space_bytes = swap_space * _GB
         self._verify_args()
 
         # Will be set after profiling.
         self.num_gpu_blocks = None
         self.num_cpu_blocks = None
 
     def _verify_args(self) -> None:
@@ -117,34 +135,34 @@
     ) -> None:
         total_cpu_memory = get_cpu_memory()
         # FIXME(woosuk): Here, it is assumed that the GPUs in a tensor parallel
         # group are in the same node. However, the GPUs may span multiple nodes.
         num_gpus_per_node = parallel_config.tensor_parallel_size
         cpu_memory_usage = self.swap_space_bytes * num_gpus_per_node
 
-        msg = (
-            f"{cpu_memory_usage / _GiB:.2f} GiB out of "
-            f"the {total_cpu_memory / _GiB:.2f} GiB total CPU memory is "
-            "allocated for the swap space.")
+        msg = (f"{cpu_memory_usage / _GB:.2f} GiB out of "
+               f"the {total_cpu_memory / _GB:.2f} GiB total CPU memory is "
+               "allocated for the swap space.")
         if cpu_memory_usage > 0.7 * total_cpu_memory:
             raise ValueError("Too large swap space. " + msg)
         elif cpu_memory_usage > 0.4 * total_cpu_memory:
-            logger.warn("Possibly too large swap space. " + msg)
+            logger.warning("Possibly too large swap space. " + msg)
 
 
 class ParallelConfig:
     """Configuration for the distributed execution.
 
     Args:
         pipeline_parallel_size: Number of pipeline parallel groups.
         tensor_parallel_size: Number of tensor parallel groups.
         worker_use_ray: Whether to use Ray for model workers. Will be set to
             True if either pipeline_parallel_size or tensor_parallel_size is
             greater than 1.
     """
+
     def __init__(
         self,
         pipeline_parallel_size: int,
         tensor_parallel_size: int,
         worker_use_ray: bool,
     ) -> None:
         self.pipeline_parallel_size = pipeline_parallel_size
@@ -166,22 +184,23 @@
     """Scheduler configuration.
 
     Args:
         max_num_batched_tokens: Maximum number of tokens to be processed in
             a single iteration.
         max_num_seqs: Maximum number of sequences to be processed in a single
             iteration.
+        max_seq_len: Maximum length of a sequence (including prompt
+            and generated text).
     """
-    def __init__(
-        self,
-        max_num_batched_tokens: int,
-        max_num_seqs: int,
-    ) -> None:
+
+    def __init__(self, max_num_batched_tokens: int, max_num_seqs: int,
+                 max_seq_len: int) -> None:
         self.max_num_batched_tokens = max_num_batched_tokens
         self.max_num_seqs = max_num_seqs
+        self.max_seq_len = max_seq_len
 
 
 _STR_DTYPE_TO_TORCH_DTYPE = {
     "half": torch.float16,
     "float16": torch.float16,
     "float": torch.float32,
     "float32": torch.float32,
@@ -217,15 +236,15 @@
             # Upcasting to float32 is allowed.
             pass
         elif config_dtype == torch.float32:
             # Downcasting from float32 to float16 or bfloat16 is allowed.
             pass
         else:
             # Casting between float16 and bfloat16 is allowed with a warning.
-            logger.warn(f"Casting {config_dtype} to {torch_dtype}.")
+            logger.warning(f"Casting {config_dtype} to {torch_dtype}.")
 
     # Check if the GPU supports the dtype.
     if torch_dtype == torch.bfloat16:
         compute_capability = torch.cuda.get_device_capability()
         if compute_capability[0] < 8:
             gpu_name = torch.cuda.get_device_name()
             raise ValueError(
```

### Comparing `vllm-0.1.1/vllm/core/block_manager.py` & `vllm-0.1.2/vllm/core/block_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
         self.device = device
         self.block_size = block_size
         self.num_blocks = num_blocks
 
         # Initialize the free blocks.
         self.free_blocks: List[PhysicalTokenBlock] = []
         for i in range(num_blocks):
-            block = PhysicalTokenBlock(
-                device=device, block_number=i, block_size=block_size)
+            block = PhysicalTokenBlock(device=device,
+                                       block_number=i,
+                                       block_size=block_size)
             self.free_blocks.append(block)
 
     def allocate(self) -> PhysicalTokenBlock:
         if not self.free_blocks:
             raise ValueError("Out of memory! No free blocks are available.")
         block = self.free_blocks.pop()
         block.ref_count = 1
@@ -80,18 +81,20 @@
     def can_allocate(self, seq_group: SequenceGroup) -> bool:
         # FIXME(woosuk): Here we assume that all sequences in the group share
         # the same prompt. This may not be true for preempted sequences.
         seq = seq_group.get_seqs()[0]
         num_required_blocks = len(seq.logical_token_blocks)
         num_free_gpu_blocks = self.gpu_allocator.get_num_free_blocks()
         # Use watermark to avoid frequent cache eviction.
-        return num_free_gpu_blocks - num_required_blocks >= self.watermark_blocks
+        return (num_free_gpu_blocks - num_required_blocks >=
+                self.watermark_blocks)
 
     def allocate(self, seq_group: SequenceGroup) -> None:
-        # NOTE: Here we assume that all sequences in the group have the same prompt.
+        # NOTE: Here we assume that all sequences in the group have the same
+        # prompt.
         seq = seq_group.get_seqs()[0]
 
         # Allocate new physical token blocks that will store the prompt tokens.
         block_table: BlockTable = []
         for _ in range(len(seq.logical_token_blocks)):
             block = self.gpu_allocator.allocate()
             # Set the reference counts of the token blocks.
@@ -139,15 +142,16 @@
         # NOTE: fork does not allocate a new physical block.
         # Thus, it is always safe from OOM.
         src_block_table = self.block_tables[parent_seq.seq_id]
         self.block_tables[child_seq.seq_id] = src_block_table.copy()
         for block in src_block_table:
             block.ref_count += 1
 
-    def _get_physical_blocks(self, seq_group: SequenceGroup) -> List[PhysicalTokenBlock]:
+    def _get_physical_blocks(
+            self, seq_group: SequenceGroup) -> List[PhysicalTokenBlock]:
         # NOTE: Here, we assume that the physical blocks are only shared by
         # the sequences in the same group.
         blocks: Set[PhysicalTokenBlock] = set()
         for seq in seq_group.get_seqs():
             if seq.is_finished():
                 continue
             block_table = self.block_tables[seq.seq_id]
```

### Comparing `vllm-0.1.1/vllm/core/policy.py` & `vllm-0.1.2/vllm/core/policy.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/core/scheduler.py` & `vllm-0.1.2/vllm/core/scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         self.blocks_to_swap_in = blocks_to_swap_in
         self.blocks_to_swap_out = blocks_to_swap_out
         self.blocks_to_copy = blocks_to_copy
         # Swap in and swap out should never happen at the same time.
         assert not (blocks_to_swap_in and blocks_to_swap_out)
 
     def is_empty(self) -> bool:
-        return (not self.blocks_to_swap_in
-                and not self.blocks_to_swap_out
+        return (not self.blocks_to_swap_in and not self.blocks_to_swap_out
                 and not self.blocks_to_copy)
 
 
 class Scheduler:
 
     def __init__(
         self,
@@ -57,15 +56,15 @@
         log_stats: bool,
     ) -> None:
         self.scheduler_config = scheduler_config
         self.cache_config = cache_config
         self.log_stats = log_stats
 
         # Instantiate the scheduling policy.
-        self.policy = PolicyFactory.get_policy(policy_name='fcfs')
+        self.policy = PolicyFactory.get_policy(policy_name="fcfs")
         # Create the block space manager.
         self.block_manager = BlockSpaceManager(
             block_size=self.cache_config.block_size,
             num_gpu_blocks=self.cache_config.num_gpu_blocks,
             num_cpu_blocks=self.cache_config.num_cpu_blocks,
         )
 
@@ -98,19 +97,21 @@
 
     def has_unfinished_seqs(self) -> bool:
         return self.waiting or self.running or self.swapped
 
     def get_num_unfinished_seq_groups(self) -> int:
         return len(self.waiting) + len(self.running) + len(self.swapped)
 
-    def _schedule(self) -> Tuple[SchedulerOutputs, List[str]]:
+    def _schedule(
+            self) -> Tuple[SchedulerOutputs, List[str], List[SequenceGroup]]:
         # Blocks that need to be swaped or copied before model execution.
         blocks_to_swap_in: Dict[int, int] = {}
         blocks_to_swap_out: Dict[int, int] = {}
         blocks_to_copy: Dict[int, List[int]] = {}
+        ignored_seq_groups: List[SequenceGroup] = []
 
         # Fix the current time.
         now = time.time()
 
         # NOTE(woosuk): We prioritize the sequence groups in the RUNNING state
         # in order to minimize the preemption overheads.
         # Preemption happens only when there is no available slot to keep all
@@ -152,27 +153,29 @@
             # If the sequence group cannot be swapped in, stop.
             if not self.block_manager.can_swap_in(seq_group):
                 break
 
             # The total number of sequences in the RUNNING state should not
             # exceed the maximum number of sequences.
             num_new_seqs = seq_group.num_seqs(status=SequenceStatus.SWAPPED)
-            num_curr_seqs = len(self.running)
-            if num_curr_seqs + num_new_seqs > self.scheduler_config.max_num_seqs:
+            num_curr_seqs = sum(
+                seq_group.num_seqs(status=SequenceStatus.RUNNING)
+                for seq_group in self.running)
+            if (num_curr_seqs + num_new_seqs >
+                    self.scheduler_config.max_num_seqs):
                 break
 
             seq_group = self.swapped.pop(0)
             self._swap_in(seq_group, blocks_to_swap_in)
             self._append_slot(seq_group, blocks_to_copy)
             self.running.append(seq_group)
 
         num_batched_tokens = sum(
             seq_group.num_seqs(status=SequenceStatus.RUNNING)
-            for seq_group in self.running
-        )
+            for seq_group in self.running)
 
         # Join waiting sequences if possible.
         prompt_group_ids: List[str] = []
         # NOTE(woosuk): The sequence groups in the SWAPPED state are strictly
         # prioritized over the sequence groups in the WAITING state.
         # This is because we want to bound the amount of CPU memory taken by
         # the swapped sequence groups.
@@ -181,90 +184,109 @@
             # sequence groups are added to the front and the new sequence groups
             # are added to the back.
             while self.waiting:
                 seq_group = self.waiting[0]
                 # If the sequence group has been preempted in this step, stop.
                 if seq_group in preempted:
                     break
+
+                num_prompt_tokens = seq_group.get_seqs()[0].get_len()
+                if num_prompt_tokens >= self.scheduler_config.max_seq_len:
+                    logger.warning(
+                        f"Input prompt ({num_prompt_tokens} tokens) is too long"
+                        " and exceeds limit of "
+                        f"{self.scheduler_config.max_seq_len}")
+                    for seq in seq_group.get_seqs():
+                        seq.status = SequenceStatus.FINISHED_IGNORED
+                    ignored_seq_groups.append(seq_group)
+                    self.waiting.pop(0)
+                    break
+
                 # If the sequence group cannot be allocated, stop.
                 if not self.block_manager.can_allocate(seq_group):
                     break
 
                 # If the number of batched tokens exceeds the limit, stop.
-                num_prompt_tokens = seq_group.get_seqs()[0].get_len()
-                if (num_batched_tokens + num_prompt_tokens
-                    > self.scheduler_config.max_num_batched_tokens):
+                if (num_batched_tokens + num_prompt_tokens >
+                        self.scheduler_config.max_num_batched_tokens):
                     break
 
                 # The total number of sequences in the RUNNING state should not
                 # exceed the maximum number of sequences.
-                num_new_seqs = seq_group.num_seqs(status=SequenceStatus.WAITING)
-                num_curr_seqs = len(self.running)
-                if num_curr_seqs + num_new_seqs > self.scheduler_config.max_num_seqs:
+                num_new_seqs = seq_group.num_seqs(
+                    status=SequenceStatus.WAITING)
+                num_curr_seqs = sum(
+                    seq_group.num_seqs(status=SequenceStatus.RUNNING)
+                    for seq_group in self.running)
+                if (num_curr_seqs + num_new_seqs >
+                        self.scheduler_config.max_num_seqs):
                     break
 
                 seq_group = self.waiting.pop(0)
                 self._allocate(seq_group)
                 self.running.append(seq_group)
                 num_batched_tokens += num_prompt_tokens
                 prompt_group_ids.append(seq_group.request_id)
 
         scheduler_outputs = SchedulerOutputs(
             blocks_to_swap_in=blocks_to_swap_in,
             blocks_to_swap_out=blocks_to_swap_out,
             blocks_to_copy=blocks_to_copy,
         )
         if not self.log_stats:
-            return scheduler_outputs, prompt_group_ids
+            return scheduler_outputs, prompt_group_ids, ignored_seq_groups
 
         # TODO(woosuk): Move the below code to the engine.
         now = time.time()
         if num_batched_tokens > 0:
             self.num_input_tokens.append((now, num_batched_tokens))
         elapsed_time = now - self.last_logging_time
         if elapsed_time > _LOGGING_INTERVAL_SEC:
             self.last_logging_time = now
-            self.num_input_tokens = [
-                (t, n) for t, n in self.num_input_tokens
-                if now - t < _LOGGING_INTERVAL_SEC
-            ]
+            self.num_input_tokens = [(t, n) for t, n in self.num_input_tokens
+                                     if now - t < _LOGGING_INTERVAL_SEC]
             if len(self.num_input_tokens) > 1:
-                total_num_tokens = sum(n for _, n in self.num_input_tokens[:-1])
+                total_num_tokens = sum(n
+                                       for _, n in self.num_input_tokens[:-1])
                 window = now - self.num_input_tokens[0][0]
                 avg_throughput = total_num_tokens / window
             else:
                 avg_throughput = 0.0
 
             total_num_gpu_blocks = self.cache_config.num_gpu_blocks
             num_free_gpu_blocks = self.block_manager.get_num_free_gpu_blocks()
             num_used_gpu_blocks = total_num_gpu_blocks - num_free_gpu_blocks
             gpu_cache_usage = num_used_gpu_blocks / total_num_gpu_blocks
 
             total_num_cpu_blocks = self.cache_config.num_cpu_blocks
             if total_num_cpu_blocks > 0:
-                num_free_cpu_blocks = self.block_manager.get_num_free_cpu_blocks()
+                num_free_cpu_blocks = (
+                    self.block_manager.get_num_free_cpu_blocks())
                 num_used_cpu_blocks = total_num_cpu_blocks - num_free_cpu_blocks
                 cpu_cache_usage = num_used_cpu_blocks / total_num_cpu_blocks
             else:
                 cpu_cache_usage = 0.0
 
-            logger.info(
-                f"Throughput: {avg_throughput:.1f} tokens/s, "
-                f"Running: {len(self.running)} reqs, "
-                f"Swapped: {len(self.swapped)} reqs, "
-                f"Pending: {len(self.waiting)} reqs, "
-                f"GPU KV cache usage: {gpu_cache_usage * 100:.1f}%, "
-                f"CPU KV cache usage: {cpu_cache_usage * 100:.1f}%")
-        return scheduler_outputs, prompt_group_ids
-
-    def schedule(self) -> Tuple[List[SequenceGroupMetadata], SchedulerOutputs]:
+            logger.info(f"Throughput: {avg_throughput:.1f} tokens/s, "
+                        f"Running: {len(self.running)} reqs, "
+                        f"Swapped: {len(self.swapped)} reqs, "
+                        f"Pending: {len(self.waiting)} reqs, "
+                        f"GPU KV cache usage: {gpu_cache_usage * 100:.1f}%, "
+                        f"CPU KV cache usage: {cpu_cache_usage * 100:.1f}%")
+        return scheduler_outputs, prompt_group_ids, ignored_seq_groups
+
+    def schedule(
+        self
+    ) -> Tuple[List[SequenceGroupMetadata], SchedulerOutputs,
+               List[SequenceGroup]]:
         # Schedule sequence groups.
         # This function call changes the internal states of the scheduler
         # such as self.running, self.swapped, and self.waiting.
-        scheduler_outputs, prompt_group_ids = self._schedule()
+        (scheduler_outputs, prompt_group_ids,
+         ignored_seq_groups) = self._schedule()
 
         # Create input data structures.
         seq_group_metadata_list: List[SequenceGroupMetadata] = []
         for seq_group in self.running:
             is_prompt = seq_group.request_id in prompt_group_ids
 
             seq_data: Dict[int, List[SequenceData]] = {}
@@ -278,28 +300,28 @@
                 request_id=seq_group.request_id,
                 is_prompt=is_prompt,
                 seq_data=seq_data,
                 sampling_params=seq_group.sampling_params,
                 block_tables=block_tables,
             )
             seq_group_metadata_list.append(seq_group_metadata)
-        return seq_group_metadata_list, scheduler_outputs
+        return seq_group_metadata_list, scheduler_outputs, ignored_seq_groups
 
     def update(
         self,
         seq_outputs: Dict[int, SequenceOutputs],
     ) -> List[SequenceGroup]:
         # Update the running sequences and free blocks.
         for seq_group in self.running:
             # Process beam search results before processing the new tokens.
             for seq in seq_group.get_seqs(status=SequenceStatus.RUNNING):
                 output = seq_outputs[seq.seq_id]
                 if seq.seq_id != output.parent_seq_id:
-                    # The sequence is a fork of the parent sequence (beam search).
-                    # Free the current sequence.
+                    # The sequence is a fork of the parent sequence (beam
+                    # search). Free the current sequence.
                     self.block_manager.free(seq)
                     # Fork the parent sequence.
                     parent_seq = seq_group.find(output.parent_seq_id)
                     parent_seq.fork(seq)
                     self.block_manager.fork(parent_seq, seq)
 
             # Process the new tokens.
@@ -364,15 +386,15 @@
             else:
                 preemption_mode = PreemptionMode.SWAP
         if preemption_mode == PreemptionMode.RECOMPUTE:
             self._preempt_by_recompute(seq_group)
         elif preemption_mode == PreemptionMode.SWAP:
             self._preempt_by_swap(seq_group, blocks_to_swap_out)
         else:
-            assert False, 'Invalid preemption mode.'
+            assert False, "Invalid preemption mode."
 
     def _preempt_by_recompute(
         self,
         seq_group: SequenceGroup,
     ) -> None:
         seqs = seq_group.get_seqs(status=SequenceStatus.RUNNING)
         assert len(seqs) == 1
```

### Comparing `vllm-0.1.1/vllm/engine/arg_utils.py` & `vllm-0.1.2/vllm/engine/arg_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,129 +7,172 @@
                          SchedulerConfig)
 
 
 @dataclass
 class EngineArgs:
     """Arguments for vLLM engine."""
     model: str
+    tokenizer: Optional[str] = None
+    tokenizer_mode: str = 'auto'
     download_dir: Optional[str] = None
     use_np_weights: bool = False
     use_dummy_weights: bool = False
-    dtype: str = "auto"
+    dtype: str = 'auto'
     seed: int = 0
     worker_use_ray: bool = False
     pipeline_parallel_size: int = 1
     tensor_parallel_size: int = 1
     block_size: int = 16
     swap_space: int = 4  # GiB
     gpu_memory_utilization: float = 0.90
     max_num_batched_tokens: int = 2560
     max_num_seqs: int = 256
     disable_log_stats: bool = False
 
     def __post_init__(self):
+        if self.tokenizer is None:
+            self.tokenizer = self.model
         self.max_num_seqs = min(self.max_num_seqs, self.max_num_batched_tokens)
 
     @staticmethod
     def add_cli_args(
-        parser: argparse.ArgumentParser,
-    ) -> argparse.ArgumentParser:
+            parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
         """Shared CLI arguments for vLLM engine."""
         # Model arguments
-        parser.add_argument('--model', type=str, default='facebook/opt-125m',
-                            help='name or path of the huggingface model to use')
-        parser.add_argument('--download-dir', type=str,
+        parser.add_argument(
+            '--model',
+            type=str,
+            default='facebook/opt-125m',
+            help='name or path of the huggingface model to use')
+        parser.add_argument(
+            '--tokenizer',
+            type=str,
+            default=EngineArgs.tokenizer,
+            help='name or path of the huggingface tokenizer to use')
+        parser.add_argument('--tokenizer-mode',
+                            type=str,
+                            default=EngineArgs.tokenizer_mode,
+                            choices=['auto', 'slow'],
+                            help='tokenizer mode. "auto" will use the fast '
+                            'tokenizer if available, and "slow" will '
+                            'always use the slow tokenizer.')
+        parser.add_argument('--download-dir',
+                            type=str,
                             default=EngineArgs.download_dir,
                             help='directory to download and load the weights, '
-                                 'default to the default cache dir of '
-                                 'huggingface')
-        parser.add_argument('--use-np-weights', action='store_true',
+                            'default to the default cache dir of '
+                            'huggingface')
+        parser.add_argument('--use-np-weights',
+                            action='store_true',
                             help='save a numpy copy of model weights for '
-                                 'faster loading. This can increase the disk '
-                                 'usage by up to 2x.')
-        parser.add_argument('--use-dummy-weights', action='store_true',
+                            'faster loading. This can increase the disk '
+                            'usage by up to 2x.')
+        parser.add_argument('--use-dummy-weights',
+                            action='store_true',
                             help='use dummy values for model weights')
         # TODO(woosuk): Support FP32.
-        parser.add_argument('--dtype', type=str, default=EngineArgs.dtype,
-                            choices=['auto', 'half', 'bfloat16', 'float'],
-                            help='data type for model weights and activations. '
-                                 'The "auto" option will use FP16 precision '
-                                 'for FP32 and FP16 models, and BF16 precision '
-                                 'for BF16 models.')
+        parser.add_argument(
+            '--dtype',
+            type=str,
+            default=EngineArgs.dtype,
+            choices=['auto', 'half', 'bfloat16', 'float'],
+            help='data type for model weights and activations. '
+            'The "auto" option will use FP16 precision '
+            'for FP32 and FP16 models, and BF16 precision '
+            'for BF16 models.')
         # Parallel arguments
-        parser.add_argument('--worker-use-ray', action='store_true',
+        parser.add_argument('--worker-use-ray',
+                            action='store_true',
                             help='use Ray for distributed serving, will be '
-                                 'automatically set when using more than 1 GPU')
-        parser.add_argument('--pipeline-parallel-size', '-pp', type=int,
+                            'automatically set when using more than 1 GPU')
+        parser.add_argument('--pipeline-parallel-size',
+                            '-pp',
+                            type=int,
                             default=EngineArgs.pipeline_parallel_size,
                             help='number of pipeline stages')
-        parser.add_argument('--tensor-parallel-size', '-tp', type=int,
+        parser.add_argument('--tensor-parallel-size',
+                            '-tp',
+                            type=int,
                             default=EngineArgs.tensor_parallel_size,
                             help='number of tensor parallel replicas')
         # KV cache arguments
-        parser.add_argument('--block-size', type=int,
+        parser.add_argument('--block-size',
+                            type=int,
                             default=EngineArgs.block_size,
                             choices=[8, 16, 32],
                             help='token block size')
         # TODO(woosuk): Support fine-grained seeds (e.g., seed per request).
-        parser.add_argument('--seed', type=int, default=EngineArgs.seed,
+        parser.add_argument('--seed',
+                            type=int,
+                            default=EngineArgs.seed,
                             help='random seed')
-        parser.add_argument('--swap-space', type=int,
+        parser.add_argument('--swap-space',
+                            type=int,
                             default=EngineArgs.swap_space,
                             help='CPU swap space size (GiB) per GPU')
-        parser.add_argument('--gpu-memory-utilization', type=float,
+        parser.add_argument('--gpu-memory-utilization',
+                            type=float,
                             default=EngineArgs.gpu_memory_utilization,
                             help='the percentage of GPU memory to be used for'
-                                 'the model executor')
-        parser.add_argument('--max-num-batched-tokens', type=int,
+                            'the model executor')
+        parser.add_argument('--max-num-batched-tokens',
+                            type=int,
                             default=EngineArgs.max_num_batched_tokens,
                             help='maximum number of batched tokens per '
-                                 'iteration')
-        parser.add_argument('--max-num-seqs', type=int,
+                            'iteration')
+        parser.add_argument('--max-num-seqs',
+                            type=int,
                             default=EngineArgs.max_num_seqs,
                             help='maximum number of sequences per iteration')
-        parser.add_argument('--disable-log-stats', action='store_true',
+        parser.add_argument('--disable-log-stats',
+                            action='store_true',
                             help='disable logging statistics')
         return parser
 
     @classmethod
-    def from_cli_args(cls, args: argparse.Namespace) -> "EngineArgs":
+    def from_cli_args(cls, args: argparse.Namespace) -> 'EngineArgs':
         # Get the list of attributes of this dataclass.
         attrs = [attr.name for attr in dataclasses.fields(cls)]
         # Set the attributes from the parsed arguments.
         engine_args = cls(**{attr: getattr(args, attr) for attr in attrs})
         return engine_args
 
     def create_engine_configs(
         self,
     ) -> Tuple[ModelConfig, CacheConfig, ParallelConfig, SchedulerConfig]:
         # Initialize the configs.
-        model_config = ModelConfig(
-            self.model, self.download_dir, self.use_np_weights,
-            self.use_dummy_weights, self.dtype, self.seed)
-        cache_config = CacheConfig(self.block_size, self.gpu_memory_utilization,
+        model_config = ModelConfig(self.model, self.tokenizer,
+                                   self.tokenizer_mode, self.download_dir,
+                                   self.use_np_weights, self.use_dummy_weights,
+                                   self.dtype, self.seed)
+        cache_config = CacheConfig(self.block_size,
+                                   self.gpu_memory_utilization,
                                    self.swap_space)
         parallel_config = ParallelConfig(self.pipeline_parallel_size,
                                          self.tensor_parallel_size,
                                          self.worker_use_ray)
+        model_max_len = getattr(model_config.hf_config,
+                                'max_position_embeddings', float('inf'))
+        max_seq_len = min(self.max_num_batched_tokens, model_max_len)
         scheduler_config = SchedulerConfig(self.max_num_batched_tokens,
-                                           self.max_num_seqs)
+                                           self.max_num_seqs, max_seq_len)
         return model_config, cache_config, parallel_config, scheduler_config
 
 
 @dataclass
 class AsyncEngineArgs(EngineArgs):
     """Arguments for asynchronous vLLM engine."""
     engine_use_ray: bool = False
     disable_log_requests: bool = False
 
     @staticmethod
     def add_cli_args(
-        parser: argparse.ArgumentParser,
-    ) -> argparse.ArgumentParser:
+            parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
         parser = EngineArgs.add_cli_args(parser)
-        parser.add_argument('--engine-use-ray', action='store_true',
+        parser.add_argument('--engine-use-ray',
+                            action='store_true',
                             help='use Ray to start the LLM engine in a '
-                                 'separate process as the server process.')
-        parser.add_argument('--disable-log-requests', action='store_true',
+                            'separate process as the server process.')
+        parser.add_argument('--disable-log-requests',
+                            action='store_true',
                             help='disable logging requests')
         return parser
```

### Comparing `vllm-0.1.1/vllm/engine/async_llm_engine.py` & `vllm-0.1.2/vllm/engine/async_llm_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import time
 from typing import Dict, List, Optional
 
+from vllm.config import ModelConfig
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.ray_utils import initialize_cluster, ray
 from vllm.logger import init_logger
 from vllm.outputs import RequestOutput
 from vllm.sampling_params import SamplingParams
 
 logger = init_logger(__name__)
 
-TIMEOUT_TO_PREVENT_DEADLOCK = 1 # seconds
+TIMEOUT_TO_PREVENT_DEADLOCK = 1  # seconds
 
 
 class AsyncLLMEngine:
     """An asynchronous wrapper for LLMEngine.
 
     This class is used to wrap the LLMEngine class to make it asynchronous. It
     uses asyncio to create a background loop that keeps processing incoming
@@ -31,16 +32,21 @@
             `parallel_config.worker_use_ray`.
         engine_use_ray: Whether to make LLMEngine a Ray actor. If so, the
             async frontend will be executed in a separate process as the
             model workers.
         log_requests: Whether to log the requests.
         *args, *kwargs: Arguments for LLMEngine.
     """
-    def __init__(self, worker_use_ray: bool, engine_use_ray: bool,
-                 log_requests: bool = True, *args, **kwargs) -> None:
+
+    def __init__(self,
+                 worker_use_ray: bool,
+                 engine_use_ray: bool,
+                 *args,
+                 log_requests: bool = True,
+                 **kwargs) -> None:
         self.worker_use_ray = worker_use_ray
         self.engine_use_ray = engine_use_ray
         self.log_requests = log_requests
         if not self.engine_use_ray:
             engine_class = LLMEngine
         elif self.worker_use_ray:
             engine_class = ray.remote(num_cpus=0)(LLMEngine).remote
@@ -72,20 +78,19 @@
         # Notify the waiting coroutines that there are new outputs ready.
         for request_output in request_outputs:
             request_id = request_output.request_id
             self.request_outputs[request_id] = request_output
             self.request_events[request_id].set()
 
     async def generate(
-        self,
-        prompt: Optional[str],
-        sampling_params: SamplingParams,
-        request_id: str,
-        prompt_token_ids: Optional[List[int]] = None
-    ) -> RequestOutput:
+            self,
+            prompt: Optional[str],
+            sampling_params: SamplingParams,
+            request_id: str,
+            prompt_token_ids: Optional[List[int]] = None) -> RequestOutput:
         """Generate outputs for a request.
 
         Generate outputs for a request. This method is a coroutine. It adds the
         request into the waiting queue of the LLMEngine and streams the outputs
         from the LLMEngine to the caller.
 
         Args:
@@ -113,34 +118,41 @@
                         f"prompt: {prompt!r}, "
                         f"sampling params: {sampling_params}, "
                         f"prompt token ids: {prompt_token_ids}.")
 
         # Add the request into the vLLM engine's waiting queue.
         if self.engine_use_ray:
             await self.engine.add_request.remote(
-                request_id, prompt, sampling_params,
+                request_id,
+                prompt,
+                sampling_params,
                 prompt_token_ids=prompt_token_ids,
                 arrival_time=arrival_time)
         else:
-            self.engine.add_request(
-                request_id, prompt, sampling_params,
-                prompt_token_ids=prompt_token_ids,
-                arrival_time=arrival_time)
+            self.engine.add_request(request_id,
+                                    prompt,
+                                    sampling_params,
+                                    prompt_token_ids=prompt_token_ids,
+                                    arrival_time=arrival_time)
 
         # The vLLM engine does not have a background loop that keeps
         # processing incoming requests. Therefore, we need to keep kicking
         # the engine to process the requests.
         while True:
             if request_id not in self.request_events:
                 # The request has been aborted.
                 return
 
             # Kick the engine if the engine is not running.
             if not self.is_engine_running:
-                await self.engine_step(request_id)
+                try:
+                    await self.engine_step(request_id)
+                except RuntimeError as e:
+                    await self.abort(request_id)
+                    raise e
 
             # Wait for new output. The group_event will be set in engine_step
             # when there is new output available for the sequence group.
             # Added a timeout to prevent deadlock.
             try:
                 await asyncio.wait_for(request_event.wait(),
                                        timeout=TIMEOUT_TO_PREVENT_DEADLOCK)
@@ -195,24 +207,33 @@
 
         # To prevent deadlock when a request is aborted while the engine is
         # running.
         if self.kicking_request_id == request_id:
             self.is_engine_running = False
             self.kicking_request_id = None
 
+    async def get_model_config(self) -> ModelConfig:
+        """Get the model configuration of the vLLM engine."""
+        if self.engine_use_ray:
+            return await self.engine.get_model_config.remote()
+        else:
+            return self.engine.get_model_config()
+
     @classmethod
-    def from_engine_args(cls, engine_args: AsyncEngineArgs) -> "AsyncLLMEngine":
+    def from_engine_args(cls,
+                         engine_args: AsyncEngineArgs) -> "AsyncLLMEngine":
         """Creates an async LLM engine from the engine arguments."""
         # Create the engine configs.
         engine_configs = engine_args.create_engine_configs()
         parallel_config = engine_configs[2]
         # Initialize the cluster.
         distributed_init_method, devices = initialize_cluster(
             parallel_config, engine_args.engine_use_ray)
         # Create the async LLM engine.
         engine = cls(engine_args.worker_use_ray,
                      engine_args.engine_use_ray,
-                     not engine_args.disable_log_requests,
                      *engine_configs,
-                     distributed_init_method, devices,
+                     distributed_init_method,
+                     devices,
+                     log_requests=not engine_args.disable_log_requests,
                      log_stats=not engine_args.disable_log_stats)
         return engine
```

### Comparing `vllm-0.1.1/vllm/engine/llm_engine.py` & `vllm-0.1.2/vllm/engine/llm_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from typing import Any, List, Optional
 
 from vllm.config import (CacheConfig, ModelConfig, ParallelConfig,
                          SchedulerConfig)
 from vllm.core.scheduler import Scheduler
 from vllm.engine.arg_utils import EngineArgs
 from vllm.engine.ray_utils import DeviceID, initialize_cluster, ray
-from vllm.engine.tokenizer_utils import detokenize_incrementally, get_tokenizer
 from vllm.logger import init_logger
 from vllm.outputs import RequestOutput
 from vllm.sampling_params import SamplingParams
 from vllm.sequence import Sequence, SequenceGroup, SequenceStatus
+from vllm.transformers_utils.tokenizer import (detokenize_incrementally,
+                                               get_tokenizer)
 from vllm.utils import Counter
 from vllm.worker.worker import Worker
 
 logger = init_logger(__name__)
 
 
 class LLMEngine:
@@ -55,31 +56,33 @@
         distributed_init_method: str,
         stage_devices: List[List[DeviceID]],
         log_stats: bool,
     ) -> None:
         logger.info(
             "Initializing an LLM engine with config: "
             f"model={model_config.model!r}, "
+            f"tokenizer={model_config.tokenizer!r}, "
+            f"tokenizer_mode={model_config.tokenizer_mode}, "
             f"dtype={model_config.dtype}, "
             f"use_dummy_weights={model_config.use_dummy_weights}, "
             f"download_dir={model_config.download_dir!r}, "
             f"use_np_weights={model_config.use_np_weights}, "
             f"tensor_parallel_size={parallel_config.tensor_parallel_size}, "
-            f"seed={model_config.seed})"
-        )
+            f"seed={model_config.seed})")
         # TODO(woosuk): Print more configs in debug mode.
 
         self.model_config = model_config
         self.cache_config = cache_config
         self.parallel_config = parallel_config
         self.scheduler_config = scheduler_config
         self.log_stats = log_stats
         self._verify_args()
 
-        self.tokenizer = get_tokenizer(model_config.model)
+        self.tokenizer = get_tokenizer(
+            model_config.tokenizer, tokenizer_mode=model_config.tokenizer_mode)
         self.seq_counter = Counter()
 
         # Create the parallel GPU workers.
         self.workers: List[Worker] = []
         assert len(stage_devices) == 1, "Only support one stage for now."
         for rank, node_resource, _ in stage_devices[0]:
             worker_cls = Worker
@@ -121,18 +124,18 @@
 
         # Since we use a shared centralized controller, we take the minimum
         # number of blocks across all workers to make sure all the memory
         # operators can be applied to all workers.
         num_gpu_blocks = min(b[0] for b in num_blocks)
         num_cpu_blocks = min(b[1] for b in num_blocks)
         # FIXME(woosuk): Change to debug log.
-        logger.info(f'# GPU blocks: {num_gpu_blocks}, '
-                    f'# CPU blocks: {num_cpu_blocks}')
+        logger.info(f"# GPU blocks: {num_gpu_blocks}, "
+                    f"# CPU blocks: {num_cpu_blocks}")
 
-        if num_gpu_blocks <= 0 or num_cpu_blocks <= 0:
+        if num_gpu_blocks <= 0:
             raise ValueError("No available memory for the cache blocks. "
                              "Try increasing `gpu_memory_utilization` when "
                              "initializing the engine.")
 
         self.cache_config.num_gpu_blocks = num_gpu_blocks
         self.cache_config.num_cpu_blocks = num_cpu_blocks
 
@@ -144,15 +147,17 @@
         """Creates an LLM engine from the engine arguments."""
         # Create the engine configs.
         engine_configs = engine_args.create_engine_configs()
         parallel_config = engine_configs[2]
         # Initialize the cluster.
         distributed_init_method, devices = initialize_cluster(parallel_config)
         # Create the LLM engine.
-        engine = cls(*engine_configs, distributed_init_method, devices,
+        engine = cls(*engine_configs,
+                     distributed_init_method,
+                     devices,
                      log_stats=not engine_args.disable_log_stats)
         return engine
 
     def add_request(
         self,
         request_id: str,
         prompt: Optional[str],
@@ -201,14 +206,18 @@
         """Aborts a request with the given ID.
 
         Args:
             request_id: The ID of the request to abort.
         """
         self.scheduler.abort_seq_group(request_id)
 
+    def get_model_config(self) -> ModelConfig:
+        """Gets the model configuration."""
+        return self.model_config
+
     def get_num_unfinished_requests(self) -> int:
         """Gets the number of unfinished requests."""
         return self.scheduler.get_num_unfinished_seq_groups()
 
     def has_unfinished_requests(self) -> bool:
         """Returns True if there are unfinished requests."""
         return self.scheduler.has_unfinished_seqs()
@@ -218,16 +227,18 @@
 
         This function performs one decoding iteration of the engine. It first
         schedules the sequences to be executed in the next iteration and the
         token blocks to be swapped in/out/copy. Then, it executes the model
         and updates the scheduler with the model outputs. Finally, it decodes
         the sequences and returns the newly generated results.
         """
-        seq_group_metadata_list, scheduler_outputs = self.scheduler.schedule()
-        if (not seq_group_metadata_list) and scheduler_outputs.is_empty():
+        (seq_group_metadata_list, scheduler_outputs,
+         ignored_seq_groups) = self.scheduler.schedule()
+        if ((not seq_group_metadata_list) and scheduler_outputs.is_empty()
+                and (not ignored_seq_groups)):
             # Nothing to do.
             return []
 
         # Execute the model.
         output = self._run_workers(
             "execute_model",
             seq_group_metadata_list=seq_group_metadata_list,
@@ -243,15 +254,15 @@
         # Stop the sequences that meet the stopping criteria.
         self._stop_sequences(seq_groups)
         # Free the finished sequence groups.
         self.scheduler.free_finished_seq_groups()
 
         # Create the outputs.
         request_outputs: List[RequestOutput] = []
-        for seq_group in seq_groups:
+        for seq_group in seq_groups + ignored_seq_groups:
             request_output = RequestOutput.from_seq_group(seq_group)
             request_outputs.append(request_output)
         return request_outputs
 
     def _decode_sequences(self, seq_groups: List[SequenceGroup]) -> None:
         """Decodes the sequence outputs."""
         for seq_group in seq_groups:
@@ -273,38 +284,44 @@
                 # Check if the sequence has generated a stop string.
                 stopped = False
                 for stop_str in sampling_params.stop:
                     if seq.output_text.endswith(stop_str):
                         # Truncate the output text so that the stop string is
                         # not included in the output.
                         seq.output_text = seq.output_text[:-len(stop_str)]
-                        self.scheduler.free_seq(seq,
-                                                SequenceStatus.FINISHED_STOPPED)
+                        self.scheduler.free_seq(
+                            seq, SequenceStatus.FINISHED_STOPPED)
                         stopped = True
                         break
                 if stopped:
                     continue
 
+                # Check if the sequence has reached max_seq_len.
+                if (seq.get_len() >=
+                        self.scheduler.scheduler_config.max_seq_len):
+                    self.scheduler.free_seq(
+                        seq, SequenceStatus.FINISHED_LENGTH_CAPPED)
+                    continue
                 # Check if the sequence has reached max_tokens.
                 if seq.get_output_len() == sampling_params.max_tokens:
                     self.scheduler.free_seq(
                         seq, SequenceStatus.FINISHED_LENGTH_CAPPED)
                     continue
                 # Check if the sequence has generated the EOS token.
                 if not sampling_params.ignore_eos:
                     if seq.get_last_token_id() == self.tokenizer.eos_token_id:
-                        self.scheduler.free_seq(seq,
-                                                SequenceStatus.FINISHED_STOPPED)
+                        self.scheduler.free_seq(
+                            seq, SequenceStatus.FINISHED_STOPPED)
                         continue
 
     def _run_workers(
         self,
         method: str,
-        get_all_outputs: bool = False,
         *args,
+        get_all_outputs: bool = False,
         **kwargs,
     ) -> Any:
         """Runs the given method on all workers."""
         all_outputs = []
         for worker in self.workers:
             executor = getattr(worker, method)
             if self.parallel_config.worker_use_ray:
```

### Comparing `vllm-0.1.1/vllm/engine/ray_utils.py` & `vllm-0.1.2/vllm/engine/ray_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 try:
     import ray
 except ImportError:
     ray = None
 
 from vllm.config import ParallelConfig
 
-DeviceID = Tuple[int, Optional[str], int]  # rank, node resource (node IP), device id
+# rank, node resource (node IP), device id
+DeviceID = Tuple[int, Optional[str], int]
 
 
 def initialize_cluster(
     parallel_config: ParallelConfig,
     engine_use_ray: bool = False,
     ray_address: Optional[str] = None,
 ) -> Tuple[str, List[List[DeviceID]]]:
@@ -49,23 +50,23 @@
         return distributed_init_method, all_stage_devices
 
     # Assume we have a uniform cluster that each node has the same number of
     # GPUs for now.
     valid_node_resources = []
     num_devices_per_node = None
     for node in ray.nodes():
-        if (not node['Alive']) or node['Resources']['GPU'] <= 0:
+        if (not node["Alive"]) or node["Resources"]["GPU"] <= 0:
             continue
         if num_devices_per_node is None:
-            num_devices_per_node = node['Resources']['GPU']
+            num_devices_per_node = node["Resources"]["GPU"]
         else:
-            assert num_devices_per_node == node['Resources']['GPU'], (
+            assert num_devices_per_node == node["Resources"]["GPU"], (
                 "The number of GPUs per node is not uniform.")
-        for key in node['Resources']:
-            if key.startswith('node:'):
+        for key in node["Resources"]:
+            if key.startswith("node:"):
                 valid_node_resources.append(key)
 
     # Verify the parallel config.
     num_nodes = len(valid_node_resources)
     if parallel_config.world_size > num_nodes * num_devices_per_node:
         raise ValueError(
             "The number of required GPUs exceeds the total number of "
```

### Comparing `vllm-0.1.1/vllm/engine/tokenizer_utils.py` & `vllm-0.1.2/vllm/transformers_utils/tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 from typing import List, Tuple, Union
 
-from transformers import (AutoConfig, AutoTokenizer, PreTrainedTokenizer,
+from transformers import (AutoTokenizer, PreTrainedTokenizer,
                           PreTrainedTokenizerFast)
 
 from vllm.logger import init_logger
 
 logger = init_logger(__name__)
 
-_MODEL_TYPES_WITH_SLOW_TOKENIZER = []
+# A fast LLaMA tokenizer with the pre-processed `tokenizer.json` file.
+_FAST_LLAMA_TOKENIZER = "hf-internal-testing/llama-tokenizer"
 
 
 def get_tokenizer(
-    model_name: str,
+    tokenizer_name: str,
     *args,
+    tokenizer_mode: str = "auto",
     **kwargs,
 ) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
     """Gets a tokenizer for the given model name via Huggingface."""
-    config = AutoConfig.from_pretrained(model_name)
-    if "open_llama" in model_name:
-        kwargs["use_fast"] = False
-        logger.info(
-            "OpenLLaMA models do not support the fast tokenizer. "
-            "Using the slow tokenizer instead.")
-    elif config.model_type == "llama" and getattr(kwargs, "use_fast", True):
-        # LLaMA fast tokenizer causes protobuf errors in some environments.
-        # However, we found that the below LLaMA fast tokenizer works well in
-        # most environments.
-        model_name = "hf-internal-testing/llama-tokenizer"
-        logger.info(
-            f"Using the LLaMA fast tokenizer in '{model_name}' to avoid "
-            "potential protobuf errors.")
-    elif config.model_type in _MODEL_TYPES_WITH_SLOW_TOKENIZER:
-        if getattr(kwargs, "use_fast", False) == True:
+    if tokenizer_mode == "slow":
+        if kwargs.get("use_fast", False):
             raise ValueError(
-                f"Cannot use the fast tokenizer for {config.model_type} due to "
-                "bugs in the fast tokenizer.")
-        logger.info(
-            f"Using the slow tokenizer for {config.model_type} due to bugs in "
-            "the fast tokenizer. This could potentially lead to performance "
-            "degradation.")
+                "Cannot use the fast tokenizer in slow tokenizer mode.")
         kwargs["use_fast"] = False
-    return AutoTokenizer.from_pretrained(model_name, *args, **kwargs)
+
+    if "llama" in tokenizer_name.lower() and kwargs.get("use_fast", True):
+        logger.info(
+            "For some LLaMA-based models, initializing the fast tokenizer may "
+            "take a long time. To eliminate the initialization time, consider "
+            f"using '{_FAST_LLAMA_TOKENIZER}' instead of the original "
+            "tokenizer.")
+    try:
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name, *args,
+                                                  **kwargs)
+    except TypeError as e:
+        # The LLaMA tokenizer causes a protobuf error in some environments.
+        err_msg = (
+            "Failed to load the tokenizer. If you are using a LLaMA-based "
+            f"model, use '{_FAST_LLAMA_TOKENIZER}' instead of the original "
+            "tokenizer.")
+        raise RuntimeError(err_msg) from e
+
+    if not isinstance(tokenizer, PreTrainedTokenizerFast):
+        logger.warning(
+            "Using a slow tokenizer. This might cause a significant "
+            "slowdown. Consider using a fast tokenizer instead.")
+    return tokenizer
 
 
 def detokenize_incrementally(
     tokenizer: Union[PreTrainedTokenizer, PreTrainedTokenizerFast],
     prev_output_tokens: List[str],
     new_token_id: int,
     skip_special_tokens: bool,
@@ -64,15 +69,16 @@
     # Convert the tokens to a string.
     # Optimization: If the tokenizer does not have `added_tokens_encoder`,
     # then we can directly use `convert_tokens_to_string`.
     if not getattr(tokenizer, "added_tokens_encoder", {}):
         output_text = tokenizer.convert_tokens_to_string(output_tokens)
         return new_token, output_text
 
-    # Adapted from https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/tokenization_utils.py#L921
+    # Adapted from
+    # https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/tokenization_utils.py#L921
     # NOTE(woosuk): The following code is slow because it runs a for loop over
     # the output_tokens. In Python, running a for loop over a list can be slow
     # even when the loop body is very simple.
     sub_texts = []
     current_sub_text = []
     for token in output_tokens:
         if skip_special_tokens and token in tokenizer.all_special_ids:
```

### Comparing `vllm-0.1.1/vllm/entrypoints/api_server.py` & `vllm-0.1.2/vllm/entrypoints/api_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import uvicorn
 
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.sampling_params import SamplingParams
 from vllm.utils import random_uuid
 
-TIMEOUT_KEEP_ALIVE = 5 # seconds.
-TIMEOUT_TO_PREVENT_DEADLOCK = 1 # seconds
+TIMEOUT_KEEP_ALIVE = 5  # seconds.
+TIMEOUT_TO_PREVENT_DEADLOCK = 1  # seconds.
 app = FastAPI()
 
 
 @app.post("/generate")
 async def generate(request: Request) -> Response:
     """Generate completion for the request.
 
@@ -33,16 +33,15 @@
     results_generator = engine.generate(prompt, sampling_params, request_id)
 
     # Streaming case
     async def stream_results() -> AsyncGenerator[bytes, None]:
         async for request_output in results_generator:
             prompt = request_output.prompt
             text_outputs = [
-                prompt + output.text
-                for output in request_output.outputs
+                prompt + output.text for output in request_output.outputs
             ]
             ret = {"text": text_outputs}
             yield (json.dumps(ret) + "\0").encode("utf-8")
 
     async def abort_request() -> None:
         await engine.abort(request_id)
 
@@ -59,27 +58,27 @@
             # Abort the request if the client disconnects.
             await engine.abort(request_id)
             return Response(status_code=499)
         final_output = request_output
 
     assert final_output is not None
     prompt = final_output.prompt
-    text_outputs = [
-        prompt + output.text
-        for output in final_output.outputs
-    ]
+    text_outputs = [prompt + output.text for output in final_output.outputs]
     ret = {"text": text_outputs}
     return Response(content=json.dumps(ret))
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=8000)
     parser = AsyncEngineArgs.add_cli_args(parser)
     args = parser.parse_args()
 
     engine_args = AsyncEngineArgs.from_cli_args(args)
     engine = AsyncLLMEngine.from_engine_args(engine_args)
 
-    uvicorn.run(app, host=args.host, port=args.port, log_level="debug",
+    uvicorn.run(app,
+                host=args.host,
+                port=args.port,
+                log_level="debug",
                 timeout_keep_alive=TIMEOUT_KEEP_ALIVE)
```

### Comparing `vllm-0.1.1/vllm/entrypoints/llm.py` & `vllm-0.1.2/vllm/entrypoints/llm.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,49 +21,61 @@
 
     NOTE: This class is intended to be used for offline inference. For online
     serving, use the `AsyncLLMEngine` class instead.
     NOTE: For the comprehensive list of arguments, see `EngineArgs`.
 
     Args:
         model: The name or path of a HuggingFace Transformers model.
+        tokenizer: The name or path of a HuggingFace Transformers tokenizer.
+        tokenizer_mode: The tokenizer mode. "auto" will use the fast tokenizer
+            if available, and "slow" will always use the slow tokenizer.
         tensor_parallel_size: The number of GPUs to use for distributed
             execution with tensor parallelism.
         dtype: The data type for the model weights and activations. Currently,
             we support `float32`, `float16`, and `bfloat16`. If `auto`, we use
             the `torch_dtype` attribute specified in the model config file.
             However, if the `torch_dtype` in the config is `float32`, we will
             use `float16` instead.
         seed: The seed to initialize the random number generator for sampling.
     """
 
     def __init__(
         self,
         model: str,
+        tokenizer: Optional[str] = None,
+        tokenizer_mode: str = "auto",
         tensor_parallel_size: int = 1,
         dtype: str = "auto",
         seed: int = 0,
         **kwargs,
     ) -> None:
         if "disable_log_stats" not in kwargs:
             kwargs["disable_log_stats"] = True
         engine_args = EngineArgs(
             model=model,
+            tokenizer=tokenizer,
+            tokenizer_mode=tokenizer_mode,
             tensor_parallel_size=tensor_parallel_size,
             dtype=dtype,
             seed=seed,
             **kwargs,
         )
         self.llm_engine = LLMEngine.from_engine_args(engine_args)
         self.request_counter = Counter()
 
     def get_tokenizer(
-        self,
-    ) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
+            self) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
         return self.llm_engine.tokenizer
 
+    def set_tokenizer(
+        self,
+        tokenizer: Union[PreTrainedTokenizer, PreTrainedTokenizerFast],
+    ) -> None:
+        self.llm_engine.tokenizer = tokenizer
+
     def generate(
         self,
         prompts: Optional[Union[str, List[str]]] = None,
         sampling_params: Optional[SamplingParams] = None,
         prompt_token_ids: Optional[List[List[int]]] = None,
         use_tqdm: bool = True,
     ) -> List[RequestOutput]:
```

### Comparing `vllm-0.1.1/vllm/entrypoints/openai/api_server.py` & `vllm-0.1.2/vllm/entrypoints/openai/api_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,143 @@
-# Adapted from https://github.com/lm-sys/FastChat/blob/168ccc29d3f7edc50823016105c024fe2282732a/fastchat/serve/openai_api_server.py
+# Adapted from
+# https://github.com/lm-sys/FastChat/blob/168ccc29d3f7edc50823016105c024fe2282732a/fastchat/serve/openai_api_server.py
 
 import argparse
+import asyncio
 from http import HTTPStatus
 import json
 import time
 from typing import AsyncGenerator, Dict, List, Optional
 
 import fastapi
 from fastapi import BackgroundTasks, Request
 from fastapi.exceptions import RequestValidationError
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse, StreamingResponse
+from fastchat.conversation import Conversation, SeparatorStyle
+from fastchat.model.model_adapter import get_conversation_template
+
 import uvicorn
 
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
-from vllm.engine.tokenizer_utils import get_tokenizer
 from vllm.entrypoints.openai.protocol import (
     CompletionRequest, CompletionResponse, CompletionResponseChoice,
-    CompletionResponseStreamChoice, CompletionStreamResponse, ErrorResponse,
+    CompletionResponseStreamChoice, CompletionStreamResponse,
+    ChatCompletionRequest, ChatCompletionResponse,
+    ChatCompletionResponseChoice, ChatCompletionResponseStreamChoice,
+    ChatCompletionStreamResponse, ChatMessage, DeltaMessage, ErrorResponse,
     LogProbs, ModelCard, ModelList, ModelPermission, UsageInfo)
 from vllm.logger import init_logger
 from vllm.outputs import RequestOutput
 from vllm.sampling_params import SamplingParams
+from vllm.transformers_utils.tokenizer import get_tokenizer
 from vllm.utils import random_uuid
 
-TIMEOUT_KEEP_ALIVE = 5 # seconds
+TIMEOUT_KEEP_ALIVE = 5  # seconds
 
 logger = init_logger(__name__)
 served_model = None
 app = fastapi.FastAPI()
 
 
 def create_error_response(status_code: HTTPStatus,
                           message: str) -> JSONResponse:
-    return JSONResponse(
-        ErrorResponse(message=message, type="invalid_request_error").dict(),
-        status_code=status_code.value
-    )
+    return JSONResponse(ErrorResponse(message=message,
+                                      type="invalid_request_error").dict(),
+                        status_code=status_code.value)
 
 
 @app.exception_handler(RequestValidationError)
-async def validation_exception_handler(request, exc):
+async def validation_exception_handler(request, exc):  # pylint: disable=unused-argument
     return create_error_response(HTTPStatus.BAD_REQUEST, str(exc))
 
 
 async def check_model(request) -> Optional[JSONResponse]:
     if request.model == served_model:
         return
     ret = create_error_response(
         HTTPStatus.NOT_FOUND,
         f"The model `{request.model}` does not exist.",
     )
     return ret
 
 
+async def get_gen_prompt(request) -> str:
+    conv = get_conversation_template(request.model)
+    conv = Conversation(
+        name=conv.name,
+        system=conv.system,
+        roles=conv.roles,
+        messages=list(conv.messages),  # prevent in-place modification
+        offset=conv.offset,
+        sep_style=SeparatorStyle(conv.sep_style),
+        sep=conv.sep,
+        sep2=conv.sep2,
+        stop_str=conv.stop_str,
+        stop_token_ids=conv.stop_token_ids,
+    )
+
+    if isinstance(request.messages, str):
+        prompt = request.messages
+    else:
+        for message in request.messages:
+            msg_role = message["role"]
+            if msg_role == "system":
+                conv.system = message["content"]
+            elif msg_role == "user":
+                conv.append_message(conv.roles[0], message["content"])
+            elif msg_role == "assistant":
+                conv.append_message(conv.roles[1], message["content"])
+            else:
+                raise ValueError(f"Unknown role: {msg_role}")
+
+        # Add a blank message for the assistant.
+        conv.append_message(conv.roles[1], None)
+        prompt = conv.get_prompt()
+
+    return prompt
+
+
+async def check_length(request, prompt, model_config):
+    if hasattr(model_config.hf_config, "max_sequence_length"):
+        context_len = model_config.hf_config.max_sequence_length
+    elif hasattr(model_config.hf_config, "seq_length"):
+        context_len = model_config.hf_config.seq_length
+    elif hasattr(model_config.hf_config, "max_position_embeddings"):
+        context_len = model_config.hf_config.max_position_embeddings
+    elif hasattr(model_config.hf_config, "seq_length"):
+        context_len = model_config.hf_config.seq_length
+    else:
+        context_len = 2048
+
+    input_ids = tokenizer(prompt).input_ids
+    token_num = len(input_ids)
+
+    if token_num + request.max_tokens > context_len:
+        return create_error_response(
+            HTTPStatus.BAD_REQUEST,
+            f"This model's maximum context length is {context_len} tokens. "
+            f"However, you requested {request.max_tokens + token_num} tokens "
+            f"({token_num} in the messages, "
+            f"{request.max_tokens} in the completion). "
+            f"Please reduce the length of the messages or completion.",
+        )
+    else:
+        return None
+
+
 @app.get("/v1/models")
 async def show_available_models():
     """Show available models. Right now we only have one model."""
-    model_cards = [ModelCard(id=served_model, root=served_model,
-                             permission=[ModelPermission()])]
+    model_cards = [
+        ModelCard(id=served_model,
+                  root=served_model,
+                  permission=[ModelPermission()])
+    ]
     return ModelList(data=model_cards)
 
 
 def create_logprobs(token_ids: List[int],
                     id_logprobs: List[Dict[int, float]],
                     initial_text_offset: int = 0) -> LogProbs:
     """Create OpenAI-style logprobs."""
@@ -72,23 +146,194 @@
     for token_id, id_logprob in zip(token_ids, id_logprobs):
         token = tokenizer.convert_ids_to_tokens(token_id)
         logprobs.tokens.append(token)
         logprobs.token_logprobs.append(id_logprob[token_id])
         if len(logprobs.text_offset) == 0:
             logprobs.text_offset.append(initial_text_offset)
         else:
-            logprobs.text_offset.append(logprobs.text_offset[-1] + last_token_len)
+            logprobs.text_offset.append(logprobs.text_offset[-1] +
+                                        last_token_len)
         last_token_len = len(token)
 
-        logprobs.top_logprobs.append(
-            {tokenizer.convert_ids_to_tokens(i): p
-             for i, p in id_logprob.items()})
+        logprobs.top_logprobs.append({
+            tokenizer.convert_ids_to_tokens(i): p
+            for i, p in id_logprob.items()
+        })
     return logprobs
 
 
+@app.post("/v1/chat/completions")
+async def create_chat_completion(raw_request: Request):
+    """Completion API similar to OpenAI's API.
+
+    See  https://platform.openai.com/docs/api-reference/chat/create
+    for the API specification. This API mimics the OpenAI ChatCompletion API.
+
+    NOTE: Currently we do not support the following features:
+        - function_call (Users should implement this by themselves)
+        - logit_bias (to be supported by vLLM engine)
+    """
+    request = ChatCompletionRequest(**await raw_request.json())
+    logger.info(f"Received chat completion request: {request}")
+
+    error_check_ret = await check_model(request)
+    if error_check_ret is not None:
+        return error_check_ret
+
+    if request.logit_bias is not None:
+        # TODO: support logit_bias in vLLM engine.
+        return create_error_response(HTTPStatus.BAD_REQUEST,
+                                     "logit_bias is not currently supported")
+
+    prompt = await get_gen_prompt(request)
+    error_check_ret = await check_length(request, prompt, engine_model_config)
+    if error_check_ret is not None:
+        return error_check_ret
+
+    model_name = request.model
+    request_id = f"cmpl-{random_uuid()}"
+    created_time = int(time.time())
+    try:
+        sampling_params = SamplingParams(
+            n=request.n,
+            presence_penalty=request.presence_penalty,
+            frequency_penalty=request.frequency_penalty,
+            temperature=request.temperature,
+            top_p=request.top_p,
+            stop=request.stop,
+            max_tokens=request.max_tokens,
+            best_of=request.best_of,
+            top_k=request.top_k,
+            ignore_eos=request.ignore_eos,
+            use_beam_search=request.use_beam_search,
+        )
+    except ValueError as e:
+        return create_error_response(HTTPStatus.BAD_REQUEST, str(e))
+
+    result_generator = engine.generate(prompt, sampling_params, request_id)
+
+    async def abort_request() -> None:
+        await engine.abort(request_id)
+
+    def create_stream_response_json(
+        index: int,
+        text: str,
+        finish_reason: Optional[str] = None,
+    ) -> str:
+        choice_data = ChatCompletionResponseStreamChoice(
+            index=index,
+            delta=DeltaMessage(content=text),
+            finish_reason=finish_reason,
+        )
+        response = ChatCompletionStreamResponse(
+            id=request_id,
+            created=created_time,
+            model=model_name,
+            choices=[choice_data],
+        )
+        response_json = response.json(ensure_ascii=False)
+
+        return response_json
+
+    async def completion_stream_generator() -> AsyncGenerator[str, None]:
+        # First chunk with role
+        for i in range(request.n):
+            choice_data = ChatCompletionResponseStreamChoice(
+                index=i,
+                delta=DeltaMessage(role="assistant"),
+                finish_reason=None,
+            )
+            chunk = ChatCompletionStreamResponse(id=request_id,
+                                                 choices=[choice_data],
+                                                 model=model_name)
+            data = chunk.json(exclude_unset=True, ensure_ascii=False)
+            yield f"data: {data}\n\n"
+
+        previous_texts = [""] * request.n
+        previous_num_tokens = [0] * request.n
+        async for res in result_generator:
+            res: RequestOutput
+            for output in res.outputs:
+                i = output.index
+                delta_text = output.text[len(previous_texts[i]):]
+                previous_texts[i] = output.text
+                previous_num_tokens[i] = len(output.token_ids)
+                response_json = create_stream_response_json(
+                    index=i,
+                    text=delta_text,
+                )
+                yield f"data: {response_json}\n\n"
+                if output.finish_reason is not None:
+                    response_json = create_stream_response_json(
+                        index=i,
+                        text="",
+                        finish_reason=output.finish_reason,
+                    )
+                    yield f"data: {response_json}\n\n"
+            yield "data: [DONE]\n\n"
+
+    # Streaming response
+    if request.stream:
+        background_tasks = BackgroundTasks()
+        # Abort the request if the client disconnects.
+        background_tasks.add_task(abort_request)
+        return StreamingResponse(completion_stream_generator(),
+                                 media_type="text/event-stream",
+                                 background=background_tasks)
+
+    # Non-streaming response
+    final_res: RequestOutput = None
+    async for res in result_generator:
+        if await raw_request.is_disconnected():
+            # Abort the request if the client disconnects.
+            await abort_request()
+            return create_error_response(HTTPStatus.BAD_REQUEST,
+                                         "Client disconnected")
+        final_res = res
+    assert final_res is not None
+    choices = []
+    for output in final_res.outputs:
+        choice_data = ChatCompletionResponseChoice(
+            index=output.index,
+            message=ChatMessage(role="assistant", content=output.text),
+            finish_reason=output.finish_reason,
+        )
+        choices.append(choice_data)
+
+    num_prompt_tokens = len(final_res.prompt_token_ids)
+    num_generated_tokens = sum(
+        len(output.token_ids) for output in final_res.outputs)
+    usage = UsageInfo(
+        prompt_tokens=num_prompt_tokens,
+        completion_tokens=num_generated_tokens,
+        total_tokens=num_prompt_tokens + num_generated_tokens,
+    )
+    response = ChatCompletionResponse(
+        id=request_id,
+        created=created_time,
+        model=model_name,
+        choices=choices,
+        usage=usage,
+    )
+
+    if request.stream:
+        # When user requests streaming but we don't stream, we still need to
+        # return a streaming response with a single event.
+        response_json = response.json(ensure_ascii=False)
+
+        async def fake_stream_generator() -> AsyncGenerator[str, None]:
+            yield f"data: {response_json}\n\n"
+            yield "data: [DONE]\n\n"
+
+        return StreamingResponse(fake_stream_generator(),
+                                 media_type="text/event-stream")
+
+    return response
+
+
 @app.post("/v1/completions")
 async def create_completion(raw_request: Request):
     """Completion API similar to OpenAI's API.
 
     See https://platform.openai.com/docs/api-reference/completions/create
     for the API specification. This API mimics the OpenAI Completion API.
 
@@ -111,24 +356,34 @@
         # currently support getting the logprobs of prompt tokens.
         return create_error_response(HTTPStatus.BAD_REQUEST,
                                      "echo is not currently supported")
 
     if request.suffix is not None:
         # The language models we currently support do not support suffix.
         return create_error_response(HTTPStatus.BAD_REQUEST,
-                                    "suffix is not currently supported")
+                                     "suffix is not currently supported")
 
     if request.logit_bias is not None:
         # TODO: support logit_bias in vLLM engine.
         return create_error_response(HTTPStatus.BAD_REQUEST,
                                      "logit_bias is not currently supported")
 
     model_name = request.model
     request_id = f"cmpl-{random_uuid()}"
-    prompt = request.prompt
+    if isinstance(request.prompt, list):
+        if len(request.prompt) == 0:
+            return create_error_response(HTTPStatus.BAD_REQUEST,
+                                         "please provide at least one prompt")
+        if len(request.prompt) > 1:
+            return create_error_response(
+                HTTPStatus.BAD_REQUEST,
+                "multiple prompts in a batch is not currently supported")
+        prompt = request.prompt[0]
+    else:
+        prompt = request.prompt
     created_time = int(time.time())
     try:
         sampling_params = SamplingParams(
             n=request.n,
             best_of=request.best_of,
             presence_penalty=request.presence_penalty,
             frequency_penalty=request.frequency_penalty,
@@ -140,30 +395,31 @@
             max_tokens=request.max_tokens,
             logprobs=request.logprobs,
             use_beam_search=request.use_beam_search,
         )
     except ValueError as e:
         return create_error_response(HTTPStatus.BAD_REQUEST, str(e))
 
-    result_generator = engine.generate(prompt, sampling_params,
-                                       request_id)
+    result_generator = engine.generate(prompt, sampling_params, request_id)
 
     # Similar to the OpenAI API, when n != best_of, we do not stream the
     # results. In addition, we do not stream the results when use beam search.
-    stream = (request.stream and
-              (request.best_of is None or request.n == request.best_of) and
-              not request.use_beam_search)
+    stream = (request.stream
+              and (request.best_of is None or request.n == request.best_of)
+              and not request.use_beam_search)
 
     async def abort_request() -> None:
         await engine.abort(request_id)
 
-    def create_stream_response_json(index: int,
-                                    text: str,
-                                    logprobs: Optional[LogProbs] = None,
-                                    finish_reason: Optional[str] = None) -> str:
+    def create_stream_response_json(
+        index: int,
+        text: str,
+        logprobs: Optional[LogProbs] = None,
+        finish_reason: Optional[str] = None,
+    ) -> str:
         choice_data = CompletionResponseStreamChoice(
             index=index,
             text=text,
             logprobs=logprobs,
             finish_reason=finish_reason,
         )
         response = CompletionStreamResponse(
@@ -196,15 +452,16 @@
                 response_json = create_stream_response_json(
                     index=i,
                     text=delta_text,
                     logprobs=logprobs,
                 )
                 yield f"data: {response_json}\n\n"
                 if output.finish_reason is not None:
-                    logprobs = LogProbs() if request.logprobs is not None else None
+                    logprobs = (LogProbs()
+                                if request.logprobs is not None else None)
                     response_json = create_stream_response_json(
                         index=i,
                         text="",
                         logprobs=logprobs,
                         finish_reason=output.finish_reason,
                     )
                     yield f"data: {response_json}\n\n"
@@ -240,16 +497,16 @@
             text=output.text,
             logprobs=logprobs,
             finish_reason=output.finish_reason,
         )
         choices.append(choice_data)
 
     num_prompt_tokens = len(final_res.prompt_token_ids)
-    num_generated_tokens = sum(len(output.token_ids)
-                               for output in final_res.outputs)
+    num_generated_tokens = sum(
+        len(output.token_ids) for output in final_res.outputs)
     usage = UsageInfo(
         prompt_tokens=num_prompt_tokens,
         completion_tokens=num_generated_tokens,
         total_tokens=num_prompt_tokens + num_generated_tokens,
     )
     response = CompletionResponse(
         id=request_id,
@@ -259,61 +516,79 @@
         usage=usage,
     )
 
     if request.stream:
         # When user requests streaming but we don't stream, we still need to
         # return a streaming response with a single event.
         response_json = response.json(ensure_ascii=False)
+
         async def fake_stream_generator() -> AsyncGenerator[str, None]:
             yield f"data: {response_json}\n\n"
             yield "data: [DONE]\n\n"
+
         return StreamingResponse(fake_stream_generator(),
                                  media_type="text/event-stream")
 
     return response
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description="vLLM OpenAI-Compatible RESTful API server."
-    )
-    parser.add_argument("--host", type=str, default="localhost", help="host name")
+        description="vLLM OpenAI-Compatible RESTful API server.")
+    parser.add_argument("--host",
+                        type=str,
+                        default="localhost",
+                        help="host name")
     parser.add_argument("--port", type=int, default=8000, help="port number")
-    parser.add_argument(
-        "--allow-credentials", action="store_true", help="allow credentials"
-    )
-    parser.add_argument(
-        "--allowed-origins", type=json.loads, default=["*"], help="allowed origins"
-    )
-    parser.add_argument(
-        "--allowed-methods", type=json.loads, default=["*"], help="allowed methods"
-    )
-    parser.add_argument(
-        "--allowed-headers", type=json.loads, default=["*"], help="allowed headers"
-    )
-    parser.add_argument("--served-model-name", type=str, default=None,
-                        help="The model name used in the API. If not specified, "
-                             "the model name will be the same as the "
-                             "huggingface name.")
+    parser.add_argument("--allow-credentials",
+                        action="store_true",
+                        help="allow credentials")
+    parser.add_argument("--allowed-origins",
+                        type=json.loads,
+                        default=["*"],
+                        help="allowed origins")
+    parser.add_argument("--allowed-methods",
+                        type=json.loads,
+                        default=["*"],
+                        help="allowed methods")
+    parser.add_argument("--allowed-headers",
+                        type=json.loads,
+                        default=["*"],
+                        help="allowed headers")
+    parser.add_argument("--served-model-name",
+                        type=str,
+                        default=None,
+                        help="The model name used in the API. If not "
+                        "specified, the model name will be the same as "
+                        "the huggingface name.")
+
     parser = AsyncEngineArgs.add_cli_args(parser)
     args = parser.parse_args()
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=args.allowed_origins,
         allow_credentials=args.allow_credentials,
         allow_methods=args.allowed_methods,
         allow_headers=args.allowed_headers,
     )
 
     logger.info(f"args: {args}")
 
-    served_model = args.served_model_name or args.model
+    if args.served_model_name is not None:
+        served_model = args.served_model_name
+    else:
+        served_model = args.model
 
     engine_args = AsyncEngineArgs.from_cli_args(args)
     engine = AsyncLLMEngine.from_engine_args(engine_args)
+    engine_model_config = asyncio.run(engine.get_model_config())
 
     # A separate tokenizer to map token IDs to strings.
-    tokenizer = get_tokenizer(args.model)
+    tokenizer = get_tokenizer(engine_args.tokenizer,
+                              tokenizer_mode=engine_args.tokenizer_mode)
 
-    uvicorn.run(app, host=args.host, port=args.port, log_level="info",
+    uvicorn.run(app,
+                host=args.host,
+                port=args.port,
+                log_level="info",
                 timeout_keep_alive=TIMEOUT_KEEP_ALIVE)
```

### Comparing `vllm-0.1.1/vllm/logger.py` & `vllm-0.1.2/vllm/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Adapted from https://github.com/skypilot-org/skypilot/blob/86dc0f6283a335e4aa37b3c10716f90999f48ab6/sky/sky_logging.py
-
+# Adapted from
+# https://github.com/skypilot-org/skypilot/blob/86dc0f6283a335e4aa37b3c10716f90999f48ab6/sky/sky_logging.py
+"""Logging configuration for vLLM."""
 import logging
 import sys
 
-
 _FORMAT = "%(levelname)s %(asctime)s %(filename)s:%(lineno)d] %(message)s"
 _DATE_FORMAT = "%m-%d %H:%M:%S"
 
 
 class NewLineFormatter(logging.Formatter):
     """Adds logging prefix to newlines to align multi-line messages."""
```

### Comparing `vllm-0.1.1/vllm/model_executor/input_metadata.py` & `vllm-0.1.2/vllm/model_executor/input_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 from typing import Dict, List, Tuple
 
 import torch
-from xformers.ops.fmha.attn_bias import BlockDiagonalCausalMask
+from xformers.ops import AttentionBias
 
 from vllm.sampling_params import SamplingParams
 from vllm.sequence import SequenceData
 
 
 class InputMetadata:
+    """Metadata for input sequences. Used for PagedAttention.
+
+    Args:
+        seq_groups: List of (seq_ids, sampling_params).
+        seq_data: Seq_id -> SequenceData.
+        prompt_lens: Lengths of prompts.
+        slot_mapping: The address to write the new KV to of each token.
+        context_lens: the length of attention context for each generation token.
+        max_context_len: The maximum context length.
+        block_tables: The block tables. (Seq id -> list of physical block)
+    """
 
     def __init__(
         self,
-        seq_groups: List[Tuple[List[int], SamplingParams]],     # List of (seq_ids, sampling_params).
-        seq_data: Dict[int, SequenceData],                      # Seq_id -> SequenceData.
+        seq_groups: List[Tuple[List[int], SamplingParams]],
+        seq_data: Dict[int, SequenceData],
         prompt_lens: List[int],
         slot_mapping: torch.Tensor,
         context_lens: torch.Tensor,
         max_context_len: int,
         block_tables: torch.Tensor,
     ) -> None:
         self.seq_groups = seq_groups
         self.seq_data = seq_data
         self.prompt_lens = prompt_lens
         self.slot_mapping = slot_mapping
         self.context_lens = context_lens
         self.max_context_len = max_context_len
         self.block_tables = block_tables
 
-        self.attn_bias = BlockDiagonalCausalMask.from_seqlens(prompt_lens)
         self.num_prompts = len(prompt_lens)
         self.num_prompt_tokens = sum(prompt_lens)
         self.num_generation_tokens = context_lens.shape[0]
         self.num_valid_tokens = slot_mapping.shape[0]
         if block_tables.numel() > 0:
             self.max_num_blocks_per_seq = block_tables.shape[1]
         else:
             self.max_num_blocks_per_seq = 0
         assert block_tables.shape[0] == self.num_generation_tokens
         assert context_lens.shape[0] == self.num_generation_tokens
 
+        # Set during the execution of the first attention op.
+        self.attn_bias: List[AttentionBias] = []
+
     def __repr__(self) -> str:
         # Print only useful metadata.
         return (f'InputMetadata('
                 f'num_valid_tokens={self.num_valid_tokens}, '
                 f'num_prompt_tokens={self.num_prompt_tokens}, '
                 f'num_prompts={self.num_prompts}, '
                 f'prompt_lens={self.prompt_lens}, '
```

### Comparing `vllm-0.1.1/vllm/model_executor/layers/activation.py` & `vllm-0.1.2/vllm/model_executor/layers/activation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import torch
 import torch.nn as nn
 
 from vllm import activation_ops
 
 _ACTIVATION_REGISTRY = {
     "gelu": nn.GELU(),
-    "gelu_new": nn.GELU(approximate="tanh"),   # NOTE: This may introduce small rounding errors.
-    "gelu_fast": nn.GELU(approximate="tanh"),  # NOTE: This may introduce small rounding errors.
+    # NOTE: The following GELU functions may introduce small rounding errors.
+    "gelu_new": nn.GELU(approximate="tanh"),
+    "gelu_fast": nn.GELU(approximate="tanh"),
+    "gelu_pytorch_tanh": nn.GELU(approximate="tanh"),
     "relu": nn.ReLU(),
 }
 
 
 def get_act_fn(act_fn: str) -> nn.Module:
     """Get an activation function by name."""
     act_fn = act_fn.lower()
@@ -20,21 +22,19 @@
     raise ValueError(f"Activation function {act_fn!r} is not supported.")
 
 
 class SiluAndMul(nn.Module):
     """An activation function for SwiGLU.
 
     The function computes x -> silu(x[:d]) * x[d:] where d = x.shape[1] // 2.
-    """
 
-    def __init__(self):
-        super().__init__()
+    Shapes:
+        x: (num_tokens, 2 * d)
+        return: (num_tokens, d)
+    """
 
-    def forward(
-        self,
-        x: torch.Tensor,        # (num_tokens, 2 * d)
-    ) -> torch.Tensor:          # (num_tokens, d)
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         num_tokens = x.shape[0]
         d = x.shape[1] // 2
         out = torch.empty(num_tokens, d, dtype=x.dtype, device=x.device)
         activation_ops.silu_and_mul(out, x)
         return out
```

### Comparing `vllm-0.1.1/vllm/model_executor/layers/layernorm.py` & `vllm-0.1.2/vllm/model_executor/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/layers/sampler.py` & `vllm-0.1.2/vllm/model_executor/layers/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from vllm.model_executor.input_metadata import InputMetadata
 from vllm.model_executor.parallel_utils.tensor_parallel import (
     gather_from_tensor_model_parallel_region)
 from vllm.sampling_params import SamplingParams
 from vllm.sequence import SequenceOutputs
 
+_SAMPLING_EPS = 1e-5
+
 
 class Sampler(nn.Module):
     """Samples the next tokens from the model's outputs.
 
     This layer does the following:
     1. Discard the hidden states that are not used for sampling (i.e., all
         tokens except the final one in each prompt).
@@ -45,40 +47,43 @@
         logits = gather_from_tensor_model_parallel_region(logits)
         # Remove paddings in vocab (if any).
         logits = logits[:, :self.vocab_size]
 
         # Apply presence and frequency penalties.
         output_tokens = _get_output_tokens(input_metadata)
         assert len(output_tokens) == logits.shape[0]
-        presence_penalties, frequency_penalties = _get_penalties(input_metadata)
+        presence_penalties, frequency_penalties = _get_penalties(
+            input_metadata)
         assert len(presence_penalties) == logits.shape[0]
         assert len(frequency_penalties) == logits.shape[0]
-        logits = _apply_penalties(
-            logits, output_tokens, presence_penalties, frequency_penalties,
-            self.vocab_size)
+        logits = _apply_penalties(logits, output_tokens, presence_penalties,
+                                  frequency_penalties, self.vocab_size)
 
         # Apply temperature scaling.
         temperatures = _get_temperatures(input_metadata)
         assert len(temperatures) == logits.shape[0]
         if any(t != 1.0 for t in temperatures):
-            t = torch.tensor(
-                temperatures, dtype=logits.dtype, device=logits.device)
+            t = torch.tensor(temperatures,
+                             dtype=logits.dtype,
+                             device=logits.device)
             # Use in-place division to avoid creating a new tensor.
             logits.div_(t.unsqueeze(dim=1))
 
         # We use float32 for probabilities and log probabilities.
         # Compute the probabilities.
         probs = torch.softmax(logits, dim=-1, dtype=torch.float)
         # Compute the log probabilities (before applying top-p and top-k).
         logprobs = torch.log(probs)
 
         # Apply top-p and top-k truncation.
         top_ps, top_ks = _get_top_p_top_k(input_metadata, self.vocab_size)
         assert len(top_ps) == len(top_ks) == probs.shape[0]
-        if any(p < 1.0 for p in top_ps) or any(k != self.vocab_size for k in top_ks):
+        do_top_p = any(p < 1.0 - _SAMPLING_EPS for p in top_ps)
+        do_top_k = any(k != self.vocab_size for k in top_ks)
+        if do_top_p or do_top_k:
             probs = _apply_top_p_top_k(probs, top_ps, top_ks)
 
         # Sample the next tokens.
         return _sample(probs, logprobs, input_metadata)
 
 
 def _prune_hidden_states(
@@ -92,16 +97,15 @@
         start_idx += prompt_len
     last_token_indicies.extend(
         range(start_idx, start_idx + input_metadata.num_generation_tokens))
     return hidden_states[last_token_indicies]
 
 
 def _get_penalties(
-    input_metadata: InputMetadata,
-) -> Tuple[List[float], List[float]]:
+        input_metadata: InputMetadata) -> Tuple[List[float], List[float]]:
     # Collect the presence and frequency penalties.
     presence_penalties: List[float] = []
     frequency_penalties: List[float] = []
     for i, seq_group in enumerate(input_metadata.seq_groups):
         seq_ids, sampling_params = seq_group
         p = sampling_params.presence_penalty
         f = sampling_params.frequency_penalty
@@ -112,17 +116,15 @@
         else:
             # A generation token.
             presence_penalties += [p] * len(seq_ids)
             frequency_penalties += [f] * len(seq_ids)
     return presence_penalties, frequency_penalties
 
 
-def _get_output_tokens(
-    input_metadata: InputMetadata,
-) -> List[List[int]]:
+def _get_output_tokens(input_metadata: InputMetadata) -> List[List[int]]:
     output_tokens: List[List[int]] = []
     for i, seq_group in enumerate(input_metadata.seq_groups):
         seq_ids, _ = seq_group
         if i < input_metadata.num_prompts:
             # A prompt input.
             # NOTE: While the prompt input usually has no output tokens,
             # it may have output tokens in the case of recomputation.
@@ -148,15 +150,15 @@
     # Collect the indices of sequences that have non-zero penalties.
     indices = []
     for i in range(num_seqs):
         if not output_tokens[i]:
             continue
         p = presence_penalties[i]
         f = frequency_penalties[i]
-        if p == 0.0 and f == 0.0:
+        if p < _SAMPLING_EPS and f < _SAMPLING_EPS:
             continue
         indices.append(i)
 
     # Return early if all sequences have zero penalties.
     if not indices:
         return logits
 
@@ -164,37 +166,37 @@
     for i in indices:
         bin_counts.append(np.bincount(output_tokens[i], minlength=vocab_size))
     bin_counts = np.stack(bin_counts, axis=0)
     bin_counts = torch.from_numpy(bin_counts).to(dtype=logits.dtype,
                                                  device=logits.device)
 
     frequency_penalties = [frequency_penalties[i] for i in indices]
-    frequency_penalties = torch.tensor(
-        frequency_penalties, dtype=logits.dtype, device=logits.device)
+    frequency_penalties = torch.tensor(frequency_penalties,
+                                       dtype=logits.dtype,
+                                       device=logits.device)
     presence_penalties = [presence_penalties[i] for i in indices]
-    presence_penalties = torch.tensor(
-        presence_penalties, dtype=logits.dtype, device=logits.device)
+    presence_penalties = torch.tensor(presence_penalties,
+                                      dtype=logits.dtype,
+                                      device=logits.device)
 
     # We follow the definition in OpenAI API.
     # Refer to https://platform.openai.com/docs/api-reference/parameter-details
     logits[indices] -= frequency_penalties.unsqueeze(dim=1) * bin_counts
     presence_mask = (bin_counts > 0.0).to(dtype=logits.dtype)
     logits[indices] -= presence_penalties.unsqueeze(dim=1) * presence_mask
     return logits
 
 
-def _get_temperatures(
-    input_metadata: InputMetadata,
-) -> List[float]:
+def _get_temperatures(input_metadata: InputMetadata) -> List[float]:
     # Collect the temperatures for the logits.
     temperatures: List[float] = []
     for i, seq_group in enumerate(input_metadata.seq_groups):
         seq_ids, sampling_params = seq_group
         temperature = sampling_params.temperature
-        if temperature == 0.0:
+        if temperature < _SAMPLING_EPS:
             # NOTE: Zero temperature means deterministic sampling
             # (i.e., greedy sampling or beam search).
             # Set the temperature to 1 to avoid division by zero.
             temperature = 1.0
 
         if i < input_metadata.num_prompts:
             # A prompt input.
@@ -247,16 +249,17 @@
     # Create a mask for the top-k elements.
     top_k_mask = torch.arange(probs_idx.shape[-1], device=probs_idx.device)
     top_k_mask = top_k_mask.expand(probs_idx.shape[0], -1)
     top_k_mask = top_k_mask >= k.unsqueeze(dim=1)
     probs_sort[top_k_mask] = 0.0
 
     # Re-sort the probabilities.
-    probs = torch.gather(
-        probs_sort, dim=-1, index=torch.argsort(probs_idx, dim=-1))
+    probs = torch.gather(probs_sort,
+                         dim=-1,
+                         index=torch.argsort(probs_idx, dim=-1))
     return probs
 
 
 def _get_topk_logprobs(
     logprobs: torch.Tensor,
     num_logprobs: Optional[int],
 ) -> Dict[int, float]:
@@ -282,25 +285,26 @@
     sampling_params: SamplingParams,
 ) -> List[int]:
     if sampling_params.use_beam_search:
         # Beam search.
         beam_width = sampling_params.best_of
         _, next_token_ids = torch.topk(prob, beam_width)
         next_token_ids = next_token_ids.tolist()
-    elif sampling_params.temperature == 0.0:
+    elif sampling_params.temperature < _SAMPLING_EPS:
         # Greedy sampling.
         assert sampling_params.best_of == 1
         next_token_id = torch.argmax(prob)
         next_token_ids = [next_token_id.item()]
     else:
         # Random sampling.
         # Sample `best_of` tokens for the prompt.
         num_seqs = sampling_params.best_of
-        next_token_ids = torch.multinomial(
-            prob, num_samples=num_seqs, replacement=True)
+        next_token_ids = torch.multinomial(prob,
+                                           num_samples=num_seqs,
+                                           replacement=True)
         next_token_ids = next_token_ids.tolist()
     return next_token_ids
 
 
 def _sample_from_generation_tokens(
     seq_ids: List[int],
     probs: torch.Tensor,
@@ -310,16 +314,17 @@
 ) -> Tuple[List[int], List[int]]:
     # NOTE(woosuk): sampling_params.best_of can be greater than
     # len(seq_ids) because some sequences in the group might have
     # been already terminated.
     if sampling_params.use_beam_search:
         # Beam search.
         # Add cumulative logprobs for the sequences in the group.
-        seq_logprobs = torch.tensor(
-            seq_logprobs, dtype=torch.float, device=logprobs.device)
+        seq_logprobs = torch.tensor(seq_logprobs,
+                                    dtype=torch.float,
+                                    device=logprobs.device)
         logprobs = logprobs + seq_logprobs.unsqueeze(dim=1)
 
         vocab_size = logprobs.size(-1)
         beam_width = len(seq_ids)
         _, topk_ids = torch.topk(logprobs.flatten(), beam_width)
         topk_ids = topk_ids.tolist()
         seq_idx = [i // vocab_size for i in topk_ids]
@@ -339,25 +344,26 @@
         for seq_id in seq_ids:
             if seq_id not in beam_outputs:
                 beam_outputs[seq_id] = outstanding_beams.pop()
         assert not outstanding_beams
 
         parent_seq_ids = [beam_outputs[seq_id][0] for seq_id in seq_ids]
         next_token_ids = [beam_outputs[seq_id][1] for seq_id in seq_ids]
-    elif sampling_params.temperature == 0.0:
+    elif sampling_params.temperature < _SAMPLING_EPS:
         # Greedy sampling.
         assert len(seq_ids) == 1
         next_token_id = torch.argmax(probs, dim=-1)
         next_token_ids = [int(next_token_id.item())]
         parent_seq_ids = seq_ids
     else:
         # Random sampling.
         # Sample 1 token for each sequence in the group.
-        next_token_ids = torch.multinomial(
-            probs, num_samples=1, replacement=True)
+        next_token_ids = torch.multinomial(probs,
+                                           num_samples=1,
+                                           replacement=True)
         next_token_ids = next_token_ids.squeeze(dim=-1).tolist()
         parent_seq_ids = seq_ids
     return parent_seq_ids, next_token_ids
 
 
 def _sample(
     probs: torch.Tensor,
@@ -376,48 +382,51 @@
             prob = probs[idx]
             logprob = logprobs[idx]
             idx += 1
 
             # Sample the next tokens.
             next_token_ids = _sample_from_prompt(prob, sampling_params)
             # Get top-k log probabilities for the next tokens.
-            next_logprobs = _get_topk_logprobs(
-                logprob, sampling_params.logprobs)
+            next_logprobs = _get_topk_logprobs(logprob,
+                                               sampling_params.logprobs)
 
             # Build the output.
             for seq_id, next_token_id in zip(seq_ids, next_token_ids):
                 output_logprobs = next_logprobs.copy()
                 output_logprobs[next_token_id] = logprob[next_token_id].item()
-                seq_outputs[seq_id] = SequenceOutputs(
-                    seq_id, seq_id, next_token_id, output_logprobs)
+                seq_outputs[seq_id] = SequenceOutputs(seq_id, seq_id,
+                                                      next_token_id,
+                                                      output_logprobs)
         else:
             # Generate the next tokens for generation tokens.
             prob = probs[idx:idx + len(seq_ids)]
             logprob = logprobs[idx:idx + len(seq_ids)]
             idx += len(seq_ids)
 
             # Sample the next tokens.
             seq_logprobs = [
                 input_metadata.seq_data[seq_id].cumulative_logprob
-                for seq_id in seq_ids]
+                for seq_id in seq_ids
+            ]
             parent_seq_ids, next_token_ids = _sample_from_generation_tokens(
                 seq_ids, prob, logprob, seq_logprobs, sampling_params)
 
             # Get top-k log probabilities for the next tokens.
             next_logprobs: Dict[int, Dict[int, float]] = {}
-            for i, seq_id in enumerate(seq_ids):
+            for j, seq_id in enumerate(seq_ids):
                 next_logprobs[seq_id] = _get_topk_logprobs(
-                    logprob[i], sampling_params.logprobs)
+                    logprob[j], sampling_params.logprobs)
 
             # Build the output.
             for seq_id, parent_seq_id, next_token_id in zip(
-                seq_ids, parent_seq_ids, next_token_ids):
-                i = seq_ids.index(parent_seq_id)
+                    seq_ids, parent_seq_ids, next_token_ids):
+                j = seq_ids.index(parent_seq_id)
                 output_logprobs = next_logprobs[parent_seq_id].copy()
-                output_logprobs[next_token_id] = logprob[i, next_token_id].item()
+                output_logprobs[next_token_id] = logprob[j,
+                                                         next_token_id].item()
                 seq_outputs[seq_id] = SequenceOutputs(
                     seq_id,
                     parent_seq_id,
                     next_token_id,
                     output_logprobs,
                 )
```

### Comparing `vllm-0.1.1/vllm/model_executor/model_loader.py` & `vllm-0.1.2/vllm/model_executor/model_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 from typing import Type
 
 import torch
 import torch.nn as nn
 from transformers import PretrainedConfig
 
 from vllm.config import ModelConfig
-from vllm.model_executor.models import (GPT2LMHeadModel, GPTNeoXForCausalLM,
-                                        LlamaForCausalLM, OPTForCausalLM)
+from vllm.model_executor.models import *  # pylint: disable=wildcard-import
 from vllm.model_executor.weight_utils import initialize_dummy_weights
 
 # TODO(woosuk): Lazy-load the model classes.
 _MODEL_REGISTRY = {
+    "BloomForCausalLM": BloomForCausalLM,
     "GPT2LMHeadModel": GPT2LMHeadModel,
+    "GPTBigCodeForCausalLM": GPTBigCodeForCausalLM,
     "GPTNeoXForCausalLM": GPTNeoXForCausalLM,
     "LlamaForCausalLM": LlamaForCausalLM,
+    "LLaMAForCausalLM": LlamaForCausalLM,  # For decapoda-research/llama-*
+    "MPTForCausalLM": MPTForCausalLM,
     "OPTForCausalLM": OPTForCausalLM,
 }
 
 
 def _get_model_architecture(config: PretrainedConfig) -> Type[nn.Module]:
     architectures = getattr(config, "architectures", [])
     for arch in architectures:
         if arch in _MODEL_REGISTRY:
             return _MODEL_REGISTRY[arch]
     raise ValueError(
         f"Model architectures {architectures} are not supported for now. "
-        f"Supported architectures: {list(_MODEL_REGISTRY.keys())}"
-    )
+        f"Supported architectures: {list(_MODEL_REGISTRY.keys())}")
 
 
 def get_model(model_config: ModelConfig) -> nn.Module:
     model_class = _get_model_architecture(model_config.hf_config)
     torch.set_default_dtype(model_config.dtype)
 
     # Create a model instance.
@@ -40,12 +42,11 @@
     if model_config.use_dummy_weights:
         model = model.cuda()
         # NOTE(woosuk): For accurate performance evaluation, we assign
         # random values to the weights.
         initialize_dummy_weights(model)
     else:
         # Load the weights from the cached or downloaded files.
-        model.load_weights(
-            model_config.model, model_config.download_dir,
-            model_config.use_np_weights)
+        model.load_weights(model_config.model, model_config.download_dir,
+                           model_config.use_np_weights)
         model = model.cuda()
     return model.eval()
```

### Comparing `vllm-0.1.1/vllm/model_executor/models/gpt2.py` & `vllm-0.1.2/vllm/model_executor/models/gpt2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
-# Adapted from https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/gpt2/modeling_gpt2.py
+# Adapted from
+# https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/gpt2/modeling_gpt2.py
 # Copyright 2023 The vLLM team.
 # Copyright 2018 The OpenAI Team Authors and HuggingFace Inc. team.
 # Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
@@ -43,59 +44,69 @@
 
 class GPT2Attention(nn.Module):
 
     def __init__(self, config: GPT2Config):
         super().__init__()
         self.hidden_size = config.hidden_size
         total_num_heads = config.num_attention_heads
-        tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
+        tensor_model_parallel_world_size = (
+            get_tensor_model_parallel_world_size())
         assert total_num_heads % tensor_model_parallel_world_size == 0
         self.num_heads = total_num_heads // tensor_model_parallel_world_size
         self.head_dim = self.hidden_size // total_num_heads
-        self.scale = self.head_dim ** -0.5
+        self.scale = self.head_dim**-0.5
 
-        self.c_attn = ColumnParallelLinear(self.hidden_size, 3 * self.hidden_size,
-                                           bias=True, gather_output=False,
+        self.c_attn = ColumnParallelLinear(self.hidden_size,
+                                           3 * self.hidden_size,
+                                           bias=True,
+                                           gather_output=False,
                                            perform_initialization=False)
-        self.c_proj = RowParallelLinear(self.hidden_size, self.hidden_size,
-                                        bias=True, input_is_parallel=True,
+        self.c_proj = RowParallelLinear(self.hidden_size,
+                                        self.hidden_size,
+                                        bias=True,
+                                        input_is_parallel=True,
                                         perform_initialization=False)
-        self.attn = PagedAttention(self.num_heads, self.head_dim,
+        self.attn = PagedAttention(self.num_heads,
+                                   self.head_dim,
                                    scale=self.scale)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         qkv, _ = self.c_attn(hidden_states)
         q, k, v = qkv.chunk(chunks=3, dim=-1)
         key_cache, value_cache = kv_cache
-        attn_output = self.attn(
-            q, k, v, key_cache, value_cache, input_metadata, cache_event)
+        attn_output = self.attn(q, k, v, key_cache, value_cache,
+                                input_metadata, cache_event)
         attn_output, _ = self.c_proj(attn_output)
         return attn_output
 
 
 class GPT2MLP(nn.Module):
 
     def __init__(
         self,
         intermediate_size: int,
         config: GPT2Config,
     ):
         super().__init__()
         hidden_size = config.hidden_size
-        self.c_fc = ColumnParallelLinear(hidden_size, intermediate_size,
-                                         bias=True, gather_output=False,
+        self.c_fc = ColumnParallelLinear(hidden_size,
+                                         intermediate_size,
+                                         bias=True,
+                                         gather_output=False,
                                          perform_initialization=False)
-        self.c_proj = RowParallelLinear(intermediate_size, hidden_size,
-                                        bias=True, input_is_parallel=True,
+        self.c_proj = RowParallelLinear(intermediate_size,
+                                        hidden_size,
+                                        bias=True,
+                                        input_is_parallel=True,
                                         perform_initialization=False)
         self.act = get_act_fn(config.activation_function)
 
     def forward(self, hidden_states: torch.Tensor) -> torch.Tensor:
         hidden_states, _ = self.c_fc(hidden_states)
         hidden_states = self.act(hidden_states)
         hidden_states, _ = self.c_proj(hidden_states)
@@ -103,15 +114,16 @@
 
 
 class GPT2Block(nn.Module):
 
     def __init__(self, config: GPT2Config):
         super().__init__()
         hidden_size = config.hidden_size
-        inner_dim = config.n_inner if config.n_inner is not None else 4 * hidden_size
+        inner_dim = (config.n_inner if config.n_inner is not None else 4 *
+                     hidden_size)
 
         self.ln_1 = nn.LayerNorm(hidden_size, eps=config.layer_norm_epsilon)
         self.attn = GPT2Attention(config)
         self.ln_2 = nn.LayerNorm(hidden_size, eps=config.layer_norm_epsilon)
         self.mlp = GPT2MLP(inner_dim, config)
 
     def forward(
@@ -141,17 +153,17 @@
 
 
 class GPT2Model(nn.Module):
 
     def __init__(self, config: GPT2Config):
         super().__init__()
         self.config = config
-        assert config.add_cross_attention == False
-        assert config.scale_attn_by_inverse_layer_idx == False
-        assert config.reorder_and_upcast_attn == False
+        assert not config.add_cross_attention
+        assert not config.scale_attn_by_inverse_layer_idx
+        assert not config.reorder_and_upcast_attn
         self.embed_dim = config.hidden_size
 
         # Optimization: While the vocab size of GPT-2 is 50257, we extend it
         # to 50304 in order to make it divisible by 64.
         # This improves performance since GPUs are faster if the dimension
         # is divisible by 64. In addition, it allows us to shard the embedding
         # layer across 2, 4, 8, or more GPUs.
@@ -176,16 +188,16 @@
 
         for i in range(len(self.h)):
             if cache_events is None:
                 cache_event = None
             else:
                 cache_event = cache_events[i]
             layer = self.h[i]
-            hidden_states = layer(
-                hidden_states, kv_caches[i], input_metadata, cache_event)
+            hidden_states = layer(hidden_states, kv_caches[i], input_metadata,
+                                  cache_event)
 
         hidden_states = self.ln_f(hidden_states)
         return hidden_states
 
 
 class GPT2LMHeadModel(nn.Module):
 
@@ -202,77 +214,87 @@
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
         cache_events: Optional[List[torch.cuda.Event]],
     ) -> Dict[int, SequenceOutputs]:
-        hidden_states = self.transformer(
-            input_ids, positions, kv_caches, input_metadata, cache_events)
-        next_tokens = self.sampler(
-            self.lm_head_weight, hidden_states, input_metadata)
+        hidden_states = self.transformer(input_ids, positions, kv_caches,
+                                         input_metadata, cache_events)
+        next_tokens = self.sampler(self.lm_head_weight, hidden_states,
+                                   input_metadata)
         return next_tokens
 
     _column_parallel_weights = ["wte.weight", "c_fc.weight", "c_fc.bias"]
     _row_parallel_weights = ["c_proj.weight"]
 
-    def load_weights(self, model_name_or_path: str,
+    def load_weights(self,
+                     model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
-        tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
+        tensor_model_parallel_world_size = (
+            get_tensor_model_parallel_world_size())
         tensor_model_parallel_rank = get_tensor_model_parallel_rank()
         state_dict = self.state_dict()
 
         for name, loaded_weight in hf_model_weights_iterator(
-            model_name_or_path, cache_dir, use_np_cache):
+                model_name_or_path, cache_dir, use_np_cache):
             if "lm_head.weight" in name:
                 # GPT-2 ties the weights of the embedding layer and the final
                 # linear layer.
                 continue
-            if ".attn.bias" in name:
+            if ".attn.bias" in name or ".attn.masked_bias" in name:
                 # Skip attention mask.
                 # NOTE: "c_attn.bias" should not be skipped.
                 continue
-            name = "transformer." + name
+
+            if not name.startswith("transformer."):
+                name = "transformer." + name
 
             # The HF's GPT-2 implementation uses Conv1D instead of Linear.
             # Because of this, we need to transpose the weights.
             for conv1d_weight_name in ["c_attn", "c_proj", "c_fc"]:
                 if conv1d_weight_name not in name:
                     continue
                 if not name.endswith(".weight"):
                     continue
                 loaded_weight = loaded_weight.t()
             param = state_dict[name]
 
             if name == "transformer.wte.weight":
                 # Consider padding in the vocab size.
-                padded_vocab_size = param.shape[0] * tensor_model_parallel_world_size
+                padded_vocab_size = (param.shape[0] *
+                                     tensor_model_parallel_world_size)
                 num_extra_rows = padded_vocab_size - self.config.vocab_size
-                extra_rows = torch.empty(num_extra_rows, loaded_weight.shape[1])
+                extra_rows = torch.empty(num_extra_rows,
+                                         loaded_weight.shape[1])
                 extra_rows = extra_rows.to(loaded_weight)
                 loaded_weight = torch.cat([loaded_weight, extra_rows], dim=0)
 
             # For the fused QKV linear layer, manually shard the weights.
             if "c_attn" in name:
-                # GPT-2's fused QKV has the shape of [3 * num_heads * head_size, hidden_size].
-                # When tensor parallelism is used, we shard the weights along the head dimension.
+                # GPT-2's fused QKV has the shape of
+                # [3 * num_heads * head_size, hidden_size].
+                # When tensor parallelism is used, we shard the weights along
+                # the head dimension.
                 total_num_heads = self.config.num_attention_heads
                 hidden_size = self.config.hidden_size
                 head_size = hidden_size // total_num_heads
                 num_heads = total_num_heads // tensor_model_parallel_world_size
                 head_start = tensor_model_parallel_rank * num_heads
                 head_end = (tensor_model_parallel_rank + 1) * num_heads
 
                 if name.endswith(".weight"):
-                    loaded_weight = loaded_weight.view(3, total_num_heads, head_size, hidden_size)
+                    loaded_weight = loaded_weight.view(3, total_num_heads,
+                                                       head_size, hidden_size)
                     loaded_weight = loaded_weight[:, head_start:head_end, :, :]
                     loaded_weight = loaded_weight.reshape(-1, hidden_size)
                 elif name.endswith(".bias"):
-                    loaded_weight = loaded_weight.view(3, total_num_heads, head_size)
+                    loaded_weight = loaded_weight.view(3, total_num_heads,
+                                                       head_size)
                     loaded_weight = loaded_weight[:, head_start:head_end, :]
                     loaded_weight = loaded_weight.reshape(-1)
                 else:
                     raise ValueError(f"Unexpected parameter name {name}")
             load_tensor_parallel_weights(param, loaded_weight, name,
                                          self._column_parallel_weights,
                                          self._row_parallel_weights,
```

### Comparing `vllm-0.1.1/vllm/model_executor/models/gpt_neox.py` & `vllm-0.1.2/vllm/model_executor/models/gpt_neox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
-# Adapted from https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/gpt_neox/modeling_gpt_neox.py
+# Adapted from
+# https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/gpt_neox/modeling_gpt_neox.py
 # Copyright 2023 The vLLM team.
 # Copyright 2022 EleutherAI The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -44,59 +45,63 @@
 
     def __init__(self, config: GPTNeoXConfig):
         super().__init__()
         self.total_num_heads = config.num_attention_heads
         self.hidden_size = config.hidden_size
         self.head_size = self.hidden_size // self.total_num_heads
 
-        tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
+        tensor_model_parallel_world_size = (
+            get_tensor_model_parallel_world_size())
         assert self.total_num_heads % tensor_model_parallel_world_size == 0
-        self.num_heads = self.total_num_heads // tensor_model_parallel_world_size
+        self.num_heads = (self.total_num_heads //
+                          tensor_model_parallel_world_size)
 
-        self.query_key_value = ColumnParallelLinear(config.hidden_size,
-                                                    3 * config.hidden_size,
-                                                    gather_output=False,
-                                                    perform_initialization=False)
-        self.dense = RowParallelLinear(config.hidden_size, config.hidden_size,
+        self.query_key_value = ColumnParallelLinear(
+            config.hidden_size,
+            3 * config.hidden_size,
+            gather_output=False,
+            perform_initialization=False)
+        self.dense = RowParallelLinear(config.hidden_size,
+                                       config.hidden_size,
                                        input_is_parallel=True,
                                        perform_initialization=False)
 
-        scaling = self.head_size ** -0.5
+        scaling = self.head_size**-0.5
         rotary_dim = int(self.head_size * config.rotary_pct)
         assert rotary_dim % 2 == 0
         self.attn = PagedAttentionWithRoPE(self.num_heads, self.head_size,
                                            scaling, rotary_dim)
 
     def forward(
         self,
         position_ids: torch.Tensor,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         qkv, _ = self.query_key_value(hidden_states)
-
         q, k, v = qkv.chunk(chunks=3, dim=-1)
         k_cache, v_cache = kv_cache
-        attn_output = self.attn(
-            position_ids, q, k, v, k_cache, v_cache, input_metadata, cache_event)
+        attn_output = self.attn(position_ids, q, k, v, k_cache, v_cache,
+                                input_metadata, cache_event)
         output, _ = self.dense(attn_output)
         return output
 
 
 class GPTNeoXMLP(nn.Module):
 
     def __init__(self, config: GPTNeoXConfig):
         super().__init__()
         self.dense_h_to_4h = ColumnParallelLinear(config.hidden_size,
                                                   config.intermediate_size,
                                                   gather_output=False,
                                                   perform_initialization=False)
-        self.dense_4h_to_h = RowParallelLinear(config.intermediate_size, config.hidden_size,
+        self.dense_4h_to_h = RowParallelLinear(config.intermediate_size,
+                                               config.hidden_size,
                                                input_is_parallel=True,
                                                perform_initialization=False)
         self.act = get_act_fn(config.hidden_act)
 
     def forward(self, hidden_states):
         hidden_states, _ = self.dense_h_to_4h(hidden_states)
         hidden_states = self.act(hidden_states)
@@ -105,16 +110,18 @@
 
 
 class GPTNeoXLayer(nn.Module):
 
     def __init__(self, config: GPTNeoXConfig):
         super().__init__()
         self.use_parallel_residual = config.use_parallel_residual
-        self.input_layernorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
-        self.post_attention_layernorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.input_layernorm = nn.LayerNorm(config.hidden_size,
+                                            eps=config.layer_norm_eps)
+        self.post_attention_layernorm = nn.LayerNorm(config.hidden_size,
+                                                     eps=config.layer_norm_eps)
         self.attention = GPTNeoXAttention(config)
         self.mlp = GPTNeoXMLP(config)
 
     def forward(
         self,
         position_ids: torch.Tensor,
         hidden_states: torch.Tensor,
@@ -150,18 +157,21 @@
 
 class GPTNeoXModel(nn.Module):
 
     def __init__(self, config: GPTNeoXConfig):
         super().__init__()
         self.config = config
 
-        self.embed_in = VocabParallelEmbedding(config.vocab_size, config.hidden_size,
+        self.embed_in = VocabParallelEmbedding(config.vocab_size,
+                                               config.hidden_size,
                                                perform_initialization=False)
-        self.layers = nn.ModuleList([GPTNeoXLayer(config) for _ in range(config.num_hidden_layers)])
-        self.final_layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.layers = nn.ModuleList(
+            [GPTNeoXLayer(config) for _ in range(config.num_hidden_layers)])
+        self.final_layer_norm = nn.LayerNorm(config.hidden_size,
+                                             eps=config.layer_norm_eps)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         position_ids: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
@@ -187,64 +197,72 @@
 
 class GPTNeoXForCausalLM(nn.Module):
 
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.gpt_neox = GPTNeoXModel(config)
-        self.embed_out = ColumnParallelLinear(config.hidden_size, config.vocab_size,
-                                              bias=False, gather_output=False,
+        self.embed_out = ColumnParallelLinear(config.hidden_size,
+                                              config.vocab_size,
+                                              bias=False,
+                                              gather_output=False,
                                               perform_initialization=False)
         self.sampler = Sampler(config.vocab_size)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
         cache_events: Optional[List[torch.cuda.Event]],
     ) -> Dict[int, SequenceOutputs]:
-        hidden_states = self.gpt_neox(
-            input_ids, positions, kv_caches, input_metadata, cache_events)
-        next_tokens = self.sampler(
-            self.embed_out.weight, hidden_states, input_metadata)
+        hidden_states = self.gpt_neox(input_ids, positions, kv_caches,
+                                      input_metadata, cache_events)
+        next_tokens = self.sampler(self.embed_out.weight, hidden_states,
+                                   input_metadata)
         return next_tokens
 
-    _column_parallel_weights = ["embed_in.weight", "embed_out.weight", "dense_h_to_4h.weight", "dense_h_to_4h.bias"]
+    _column_parallel_weights = [
+        "embed_in.weight", "embed_out.weight", "dense_h_to_4h.weight",
+        "dense_h_to_4h.bias"
+    ]
     _row_parallel_weights = ["dense.weight", "dense_4h_to_h.weight"]
 
-    def load_weights(self, model_name_or_path: str,
+    def load_weights(self,
+                     model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
         tensor_model_parallel_rank = get_tensor_model_parallel_rank()
         state_dict = self.state_dict()
         for name, loaded_weight in hf_model_weights_iterator(
-            model_name_or_path, cache_dir, use_np_cache):
+                model_name_or_path, cache_dir, use_np_cache):
             if ("attention.bias" in name or "attention.masked_bias" in name
-                or "rotary_emb.inv_freq" in name):
+                    or "rotary_emb.inv_freq" in name):
                 continue
             param = state_dict[name]
             if "query_key_value" in name:
                 # NOTE(woosuk): GPT-NeoX's fused QKV has the shape of
                 # [num_heads * 3 * head_size, hidden_size], while the
                 # required shape is [3 * num_heads * head_size, hidden_size].
                 # Thus, we need weight conversion.
                 shard_size = param.shape[0]
-                loaded_weight = loaded_weight[shard_size * tensor_model_parallel_rank
-                                              :shard_size * (tensor_model_parallel_rank + 1)]
+                loaded_weight = loaded_weight[
+                    shard_size * tensor_model_parallel_rank:shard_size *
+                    (tensor_model_parallel_rank + 1)]
 
                 num_heads = self.config.num_attention_heads
                 hidden_size = self.config.hidden_size
                 head_size = hidden_size // num_heads
-                if 'query_key_value.weight' in name:
-                    loaded_weight = loaded_weight.view(-1, 3, head_size, hidden_size)
+                if "query_key_value.weight" in name:
+                    loaded_weight = loaded_weight.view(-1, 3, head_size,
+                                                       hidden_size)
                     loaded_weight = loaded_weight.transpose(0, 1)
                     loaded_weight = loaded_weight.reshape(-1, hidden_size)
-                elif 'query_key_value.bias' in name:
+                elif "query_key_value.bias" in name:
                     loaded_weight = loaded_weight.view(-1, 3, head_size)
                     loaded_weight = loaded_weight.transpose(0, 1)
                     loaded_weight = loaded_weight.reshape(-1)
                 else:
                     raise ValueError(f"Unexpected weight name: {name}")
             load_tensor_parallel_weights(param, loaded_weight, name,
                                          self._column_parallel_weights,
```

### Comparing `vllm-0.1.1/vllm/model_executor/models/llama.py` & `vllm-0.1.2/vllm/model_executor/models/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
-# Adapted from https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/llama/modeling_llama.py
+# Adapted from
+# https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/llama/modeling_llama.py
 # Copyright 2023 The vLLM team.
 # Copyright 2022 EleutherAI and the HuggingFace Inc. team. All rights reserved.
 #
 # This code is based on EleutherAI's GPT-NeoX library and the GPT-NeoX
 # and OPT implementations in this library. It has been modified from its
 # original forms to accommodate minor architectural differences compared
 # to GPT-NeoX and OPT used by the Meta AI team that trained the model.
@@ -26,15 +27,14 @@
 """
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 from transformers import LlamaConfig
 
-from vllm.sequence import SequenceOutputs
 from vllm.model_executor.input_metadata import InputMetadata
 from vllm.model_executor.layers.activation import SiluAndMul
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.attention import PagedAttentionWithRoPE
 from vllm.model_executor.layers.sampler import Sampler
 from vllm.model_executor.weight_utils import (hf_model_weights_iterator,
                                               load_tensor_parallel_weights)
@@ -52,23 +52,27 @@
     def __init__(
         self,
         hidden_size: int,
         intermediate_size: int,
         hidden_act: str,
     ):
         super().__init__()
-        self.gate_up_proj = ColumnParallelLinear(hidden_size, 2 * intermediate_size,
-                                                 bias=False, gather_output=False,
+        self.gate_up_proj = ColumnParallelLinear(hidden_size,
+                                                 2 * intermediate_size,
+                                                 bias=False,
+                                                 gather_output=False,
                                                  perform_initialization=False)
-        self.down_proj = RowParallelLinear(intermediate_size, hidden_size,
-                                           bias=False, input_is_parallel=True,
+        self.down_proj = RowParallelLinear(intermediate_size,
+                                           hidden_size,
+                                           bias=False,
+                                           input_is_parallel=True,
                                            perform_initialization=False)
-        if hidden_act != 'silu':
-            raise ValueError(f'Unsupported activation: {hidden_act}. '
-                             'Only silu is supported for now.')
+        if hidden_act != "silu":
+            raise ValueError(f"Unsupported activation: {hidden_act}. "
+                             "Only silu is supported for now.")
         self.act_fn = SiluAndMul()
 
     def forward(self, x):
         gate_up, _ = self.gate_up_proj(x)
         x = self.act_fn(gate_up)
         x, _ = self.down_proj(x)
         return x
@@ -79,20 +83,22 @@
     def __init__(
         self,
         hidden_size: int,
         num_heads: int,
     ):
         super().__init__()
         self.hidden_size = hidden_size
-        tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
+        tensor_model_parallel_world_size = (
+            get_tensor_model_parallel_world_size())
         self.total_num_heads = num_heads
         assert self.total_num_heads % tensor_model_parallel_world_size == 0
-        self.num_heads = self.total_num_heads // tensor_model_parallel_world_size
+        self.num_heads = (self.total_num_heads //
+                          tensor_model_parallel_world_size)
         self.head_dim = hidden_size // self.total_num_heads
-        self.scaling = self.head_dim ** -0.5
+        self.scaling = self.head_dim**-0.5
 
         self.qkv_proj = ColumnParallelLinear(
             hidden_size,
             3 * self.total_num_heads * self.head_dim,
             bias=False,
             gather_output=False,
             perform_initialization=False,
@@ -100,30 +106,32 @@
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
             input_is_parallel=True,
             perform_initialization=False,
         )
-        self.attn = PagedAttentionWithRoPE(self.num_heads, self.head_dim,
-                                           self.scaling, rotary_dim=self.head_dim)
+        self.attn = PagedAttentionWithRoPE(self.num_heads,
+                                           self.head_dim,
+                                           self.scaling,
+                                           rotary_dim=self.head_dim)
 
     def forward(
         self,
         positions: torch.Tensor,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         qkv, _ = self.qkv_proj(hidden_states)
         q, k, v = qkv.chunk(chunks=3, dim=-1)
         k_cache, v_cache = kv_cache
-        attn_output = self.attn(
-            positions, q, k, v, k_cache, v_cache, input_metadata, cache_event)
+        attn_output = self.attn(positions, q, k, v, k_cache, v_cache,
+                                input_metadata, cache_event)
         output, _ = self.o_proj(attn_output)
         return output
 
 
 class LlamaDecoderLayer(nn.Module):
 
     def __init__(self, config: LlamaConfig):
@@ -134,16 +142,18 @@
             num_heads=config.num_attention_heads,
         )
         self.mlp = LlamaMLP(
             hidden_size=self.hidden_size,
             intermediate_size=config.intermediate_size,
             hidden_act=config.hidden_act,
         )
-        self.input_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
-        self.post_attention_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.input_layernorm = RMSNorm(config.hidden_size,
+                                       eps=config.rms_norm_eps)
+        self.post_attention_layernorm = RMSNorm(config.hidden_size,
+                                                eps=config.rms_norm_eps)
 
     def forward(
         self,
         positions: torch.Tensor,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
@@ -173,17 +183,21 @@
 
     def __init__(self, config: LlamaConfig):
         super().__init__()
         self.config = config
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
 
-        self.embed_tokens = VocabParallelEmbedding(config.vocab_size, config.hidden_size,
-                                                   perform_initialization=False)
-        self.layers = nn.ModuleList([LlamaDecoderLayer(config) for _ in range(config.num_hidden_layers)])
+        self.embed_tokens = VocabParallelEmbedding(
+            config.vocab_size,
+            config.hidden_size,
+            perform_initialization=False)
+        self.layers = nn.ModuleList([
+            LlamaDecoderLayer(config) for _ in range(config.num_hidden_layers)
+        ])
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
@@ -205,14 +219,15 @@
                 cache_event,
             )
         hidden_states = self.norm(hidden_states)
         return hidden_states
 
 
 class LlamaForCausalLM(nn.Module):
+
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.model = LlamaModel(config)
         self.lm_head = ColumnParallelLinear(config.hidden_size,
                                             config.vocab_size,
                                             bias=False,
@@ -224,65 +239,68 @@
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
         cache_events: Optional[List[torch.cuda.Event]],
     ) -> Dict[int, SequenceOutputs]:
-        hidden_states = self.model(
-            input_ids, positions, kv_caches, input_metadata, cache_events)
-        next_tokens = self.sampler(
-            self.lm_head.weight, hidden_states, input_metadata)
+        hidden_states = self.model(input_ids, positions, kv_caches,
+                                   input_metadata, cache_events)
+        next_tokens = self.sampler(self.lm_head.weight, hidden_states,
+                                   input_metadata)
         return next_tokens
 
-    _column_parallel_weights = ["embed_tokens.weight", "lm_head.weight",
-                                "qkv_proj.weight", "gate_proj.weight",
-                                "up_proj.weight"]
+    _column_parallel_weights = [
+        "embed_tokens.weight", "lm_head.weight", "qkv_proj.weight",
+        "gate_proj.weight", "up_proj.weight"
+    ]
     _row_parallel_weights = ["o_proj.weight", "down_proj.weight"]
 
-    def load_weights(self, model_name_or_path: str,
+    def load_weights(self,
+                     model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
         tensor_model_parallel_rank = get_tensor_model_parallel_rank()
         state_dict = self.state_dict()
 
         for name, loaded_weight in hf_model_weights_iterator(
-            model_name_or_path, cache_dir, use_np_cache):
+                model_name_or_path, cache_dir, use_np_cache):
             if "rotary_emb.inv_freq" in name:
                 continue
 
             is_attention_weight = False
-            for stride_id, att_weight_name in enumerate(["q_proj", "k_proj", "v_proj"]):
+            for stride_id, att_weight_name in enumerate(
+                ["q_proj", "k_proj", "v_proj"]):
                 if att_weight_name not in name:
                     continue
                 param = state_dict[name.replace(att_weight_name, "qkv_proj")]
                 shard_size = param.shape[0] // 3
                 loaded_weight = loaded_weight[
-                    shard_size * tensor_model_parallel_rank
-                    :shard_size * (tensor_model_parallel_rank + 1)]
-                param_slice = param.data[shard_size * stride_id
-                                         :shard_size * (stride_id + 1)]
+                    shard_size * tensor_model_parallel_rank:shard_size *
+                    (tensor_model_parallel_rank + 1)]
+                param_slice = param.data[shard_size * stride_id:shard_size *
+                                         (stride_id + 1)]
                 assert param_slice.shape == loaded_weight.shape
                 param_slice.copy_(loaded_weight)
                 is_attention_weight = True
                 break
             if is_attention_weight:
                 continue
 
             is_gate_up_weight = False
             for stride_id, weight_name in enumerate(["gate_proj", "up_proj"]):
                 if weight_name not in name:
                     continue
                 param = state_dict[name.replace(weight_name, "gate_up_proj")]
                 shard_size = param.shape[0] // 2
                 loaded_weight = loaded_weight[
-                    shard_size * tensor_model_parallel_rank
-                    :shard_size * (tensor_model_parallel_rank + 1)]
-                param_slice = param.data[shard_size * stride_id
-                                         :shard_size * (stride_id + 1)]
+                    shard_size * tensor_model_parallel_rank:shard_size *
+                    (tensor_model_parallel_rank + 1)]
+                param_slice = param.data[shard_size * stride_id:shard_size *
+                                         (stride_id + 1)]
                 assert param_slice.shape == loaded_weight.shape
                 param_slice.copy_(loaded_weight)
                 is_gate_up_weight = True
                 break
             if is_gate_up_weight:
                 continue
```

### Comparing `vllm-0.1.1/vllm/model_executor/models/opt.py` & `vllm-0.1.2/vllm/model_executor/models/opt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # coding=utf-8
-# Adapted from https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/opt/modeling_opt.py
+# Adapted from
+# https://github.com/huggingface/transformers/blob/v4.28.0/src/transformers/models/opt/modeling_opt.py
 # Copyright 2023 The vLLM team.
-# Copyright 2022 The Fairseq Authors and The HuggingFace Inc. team. All rights reserved.
+# Copyright 2022 The Fairseq Authors and The HuggingFace Inc. team. All rights
+# reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,16 +41,17 @@
 
 KVCache = Tuple[torch.Tensor, torch.Tensor]
 
 
 class OPTLearnedPositionalEmbedding(nn.Embedding):
 
     def __init__(self, num_embeddings: int, embedding_dim: int):
-        # OPT is set up so that if padding_idx is specified then offset the embedding ids by 2
-        # and adjust num_embeddings appropriately. Other models don't have this hack
+        # OPT is set up so that if padding_idx is specified then offset the
+        # embedding ids by 2 and adjust num_embeddings appropriately. Other
+        # models don't have this hack
         self.offset = 2
         super().__init__(num_embeddings + self.offset, embedding_dim)
 
     def forward(self, positions: torch.Tensor):
         return super().forward(positions + self.offset)
 
 
@@ -58,42 +61,48 @@
         self,
         embed_dim: int,
         num_heads: int,
         bias: bool = True,
     ) -> None:
         super().__init__()
         self.embed_dim = embed_dim
-        tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
+        tensor_model_parallel_world_size = (
+            get_tensor_model_parallel_world_size())
         total_num_heads = num_heads
         assert num_heads % tensor_model_parallel_world_size == 0
         self.num_heads = total_num_heads // tensor_model_parallel_world_size
         self.head_dim = embed_dim // total_num_heads
-        self.scaling = self.head_dim ** -0.5
+        self.scaling = self.head_dim**-0.5
 
-        self.qkv_proj = ColumnParallelLinear(embed_dim, 3 * embed_dim, bias=bias,
+        self.qkv_proj = ColumnParallelLinear(embed_dim,
+                                             3 * embed_dim,
+                                             bias=bias,
                                              gather_output=False,
                                              perform_initialization=False)
-        self.out_proj = RowParallelLinear(embed_dim, embed_dim, bias=bias,
+        self.out_proj = RowParallelLinear(embed_dim,
+                                          embed_dim,
+                                          bias=bias,
                                           input_is_parallel=True,
                                           perform_initialization=False)
-        self.attn = PagedAttention(self.num_heads, self.head_dim,
+        self.attn = PagedAttention(self.num_heads,
+                                   self.head_dim,
                                    scale=self.scaling)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         qkv, _ = self.qkv_proj(hidden_states)
         q, k, v = qkv.chunk(chunks=3, dim=-1)
         key_cache, value_cache = kv_cache
-        attn_output = self.attn(
-            q, k, v, key_cache, value_cache, input_metadata, cache_event)
+        attn_output = self.attn(q, k, v, key_cache, value_cache,
+                                input_metadata, cache_event)
         output, _ = self.out_proj(attn_output)
         return output
 
 
 class OPTDecoderLayer(nn.Module):
 
     def __init__(self, config: OPTConfig):
@@ -105,43 +114,46 @@
             num_heads=config.num_attention_heads,
             bias=config.enable_bias,
         )
         self.do_layer_norm_before = config.do_layer_norm_before
         self.activation_fn = get_act_fn(config.activation_function)
 
         self.self_attn_layer_norm = nn.LayerNorm(
-            self.embed_dim, elementwise_affine=config.layer_norm_elementwise_affine)
-        self.fc1 = ColumnParallelLinear(self.embed_dim, config.ffn_dim,
+            self.embed_dim,
+            elementwise_affine=config.layer_norm_elementwise_affine)
+        self.fc1 = ColumnParallelLinear(self.embed_dim,
+                                        config.ffn_dim,
                                         bias=config.enable_bias,
                                         gather_output=False,
                                         perform_initialization=False)
-        self.fc2 = RowParallelLinear(config.ffn_dim, self.embed_dim,
+        self.fc2 = RowParallelLinear(config.ffn_dim,
+                                     self.embed_dim,
                                      bias=config.enable_bias,
                                      input_is_parallel=True,
                                      perform_initialization=False)
         self.final_layer_norm = nn.LayerNorm(
-            self.embed_dim, elementwise_affine=config.layer_norm_elementwise_affine)
+            self.embed_dim,
+            elementwise_affine=config.layer_norm_elementwise_affine)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
         kv_cache: KVCache,
         input_metadata: InputMetadata,
         cache_event: Optional[torch.cuda.Event],
     ) -> torch.Tensor:
         # Self Attention
         residual = hidden_states
         # 125m, 1.7B, ..., 175B applies layer norm BEFORE attention
         if self.do_layer_norm_before:
             hidden_states = self.self_attn_layer_norm(hidden_states)
-        hidden_states = self.self_attn(
-            hidden_states=hidden_states,
-            kv_cache=kv_cache,
-            input_metadata=input_metadata,
-            cache_event=cache_event)
+        hidden_states = self.self_attn(hidden_states=hidden_states,
+                                       kv_cache=kv_cache,
+                                       input_metadata=input_metadata,
+                                       cache_event=cache_event)
         hidden_states = residual + hidden_states
         # 350m applies layer norm AFTER attention
         if not self.do_layer_norm_before:
             hidden_states = self.self_attn_layer_norm(hidden_states)
 
         # Fully Connected
         residual = hidden_states
@@ -163,43 +175,50 @@
     def __init__(self, config: OPTConfig):
         super().__init__()
         self.config = config
         self.padding_idx = config.pad_token_id
         self.max_target_positions = config.max_position_embeddings
         self.vocab_size = config.vocab_size
 
-        self.embed_tokens = VocabParallelEmbedding(config.vocab_size,
-                                                   config.word_embed_proj_dim,
-                                                   perform_initialization=False)
+        self.embed_tokens = VocabParallelEmbedding(
+            config.vocab_size,
+            config.word_embed_proj_dim,
+            perform_initialization=False)
         # Positional embeddings are replicated (not sharded).
         self.embed_positions = OPTLearnedPositionalEmbedding(
             config.max_position_embeddings, config.hidden_size)
 
         # Project out & in will be replicated if they exist.
         if config.word_embed_proj_dim != config.hidden_size:
-            self.project_out = nn.Linear(config.hidden_size, config.word_embed_proj_dim, bias=False)
+            self.project_out = nn.Linear(config.hidden_size,
+                                         config.word_embed_proj_dim,
+                                         bias=False)
         else:
             self.project_out = None
 
         if config.word_embed_proj_dim != config.hidden_size:
-            self.project_in = nn.Linear(config.word_embed_proj_dim, config.hidden_size, bias=False)
+            self.project_in = nn.Linear(config.word_embed_proj_dim,
+                                        config.hidden_size,
+                                        bias=False)
         else:
             self.project_in = None
 
-        # Note that the only purpose of `config._remove_final_layer_norm` is to keep backward compatibility
-        # with checkpoints that have been fine-tuned before transformers v4.20.1
+        # Note that the only purpose of `config._remove_final_layer_norm` is to
+        # keep backward compatibility with checkpoints that have been fine-tuned
+        # before transformers v4.20.1
         # see https://github.com/facebookresearch/metaseq/pull/164
         if config.do_layer_norm_before and not config._remove_final_layer_norm:
             self.final_layer_norm = nn.LayerNorm(
-                config.hidden_size, elementwise_affine=config.layer_norm_elementwise_affine
-            )
+                config.hidden_size,
+                elementwise_affine=config.layer_norm_elementwise_affine)
         else:
             self.final_layer_norm = None
 
-        self.layers = nn.ModuleList([OPTDecoderLayer(config) for _ in range(config.num_hidden_layers)])
+        self.layers = nn.ModuleList(
+            [OPTDecoderLayer(config) for _ in range(config.num_hidden_layers)])
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
@@ -213,16 +232,16 @@
 
         for i in range(len(self.layers)):
             if cache_events is None:
                 cache_event = None
             else:
                 cache_event = cache_events[i]
             layer = self.layers[i]
-            hidden_states = layer(
-                hidden_states, kv_caches[i], input_metadata, cache_event)
+            hidden_states = layer(hidden_states, kv_caches[i], input_metadata,
+                                  cache_event)
 
         if self.final_layer_norm is not None:
             hidden_states = self.final_layer_norm(hidden_states)
         if self.project_out is not None:
             hidden_states = self.project_out(hidden_states)
         return hidden_states
 
@@ -237,16 +256,16 @@
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
         cache_events: Optional[List[torch.cuda.Event]],
     ) -> torch.Tensor:
-        return self.decoder(
-            input_ids, positions, kv_caches, input_metadata, cache_events)
+        return self.decoder(input_ids, positions, kv_caches, input_metadata,
+                            cache_events)
 
 
 class OPTForCausalLM(nn.Module):
 
     def __init__(self, config):
         super().__init__()
         self.config = config
@@ -260,48 +279,52 @@
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
         kv_caches: List[KVCache],
         input_metadata: InputMetadata,
         cache_events: Optional[List[torch.cuda.Event]],
     ) -> Dict[int, SequenceOutputs]:
-        hidden_states = self.model(
-            input_ids, positions, kv_caches, input_metadata, cache_events)
-        next_tokens = self.sampler(
-            self.lm_head_weight, hidden_states, input_metadata)
+        hidden_states = self.model(input_ids, positions, kv_caches,
+                                   input_metadata, cache_events)
+        next_tokens = self.sampler(self.lm_head_weight, hidden_states,
+                                   input_metadata)
         return next_tokens
 
-    _column_parallel_weights = ["embed_tokens.weight", "fc1.weight", "fc1.bias"]
+    _column_parallel_weights = [
+        "embed_tokens.weight", "fc1.weight", "fc1.bias"
+    ]
     _row_parallel_weights = ["out_proj.weight", "fc2.weight"]
 
-    def load_weights(self, model_name_or_path: str,
+    def load_weights(self,
+                     model_name_or_path: str,
                      cache_dir: Optional[str] = None,
                      use_np_cache: bool = False):
         tensor_model_parallel_rank = get_tensor_model_parallel_rank()
         state_dict = self.state_dict()
 
         for name, loaded_weight in hf_model_weights_iterator(
-            model_name_or_path, cache_dir, use_np_cache):
+                model_name_or_path, cache_dir, use_np_cache):
             if "lm_head.weight" in name:
                 continue
 
             if name.startswith("decoder."):
                 name = "model." + name
 
             is_attention_weight = False
-            for stride_id, att_weight_name in enumerate(["q_proj", "k_proj", "v_proj"]):
+            for stride_id, att_weight_name in enumerate(
+                ["q_proj", "k_proj", "v_proj"]):
                 if att_weight_name not in name:
                     continue
                 param = state_dict[name.replace(att_weight_name, "qkv_proj")]
                 shard_size = param.shape[0] // 3
                 loaded_weight = loaded_weight[
-                    shard_size * tensor_model_parallel_rank
-                    :shard_size * (tensor_model_parallel_rank + 1)]
-                param_slice = param.data[shard_size * stride_id
-                                         :shard_size * (stride_id + 1)]
+                    shard_size * tensor_model_parallel_rank:shard_size *
+                    (tensor_model_parallel_rank + 1)]
+                param_slice = param.data[shard_size * stride_id:shard_size *
+                                         (stride_id + 1)]
                 assert param_slice.shape == loaded_weight.shape
                 param_slice.copy_(loaded_weight)
                 is_attention_weight = True
                 break
             if is_attention_weight:
                 continue
```

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/parallel_state.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/parallel_state.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/layers.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/random.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py` & `vllm-0.1.2/vllm/model_executor/parallel_utils/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/utils.py` & `vllm-0.1.2/vllm/model_executor/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.1/vllm/model_executor/weight_utils.py` & `vllm-0.1.2/vllm/model_executor/weight_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,31 +40,31 @@
         hf_folder = model_name_or_path
 
     hf_bin_files = glob.glob(os.path.join(hf_folder, "*.bin"))
 
     if use_np_cache:
         # Convert the model weights from torch tensors to numpy arrays for
         # faster loading.
-        np_folder = os.path.join(hf_folder, 'np')
+        np_folder = os.path.join(hf_folder, "np")
         os.makedirs(np_folder, exist_ok=True)
-        weight_names_file = os.path.join(np_folder, 'weight_names.json')
+        weight_names_file = os.path.join(np_folder, "weight_names.json")
         with lock:
             if not os.path.exists(weight_names_file):
                 weight_names = []
                 for bin_file in hf_bin_files:
                     state = torch.load(bin_file, map_location="cpu")
                     for name, param in state.items():
                         param_path = os.path.join(np_folder, name)
                         with open(param_path, "wb") as f:
                             np.save(f, param.cpu().detach().numpy())
                         weight_names.append(name)
-                with open(weight_names_file, 'w') as f:
+                with open(weight_names_file, "w") as f:
                     json.dump(weight_names, f)
 
-        with open(weight_names_file, 'r') as f:
+        with open(weight_names_file, "r") as f:
             weight_names = json.load(f)
 
         for name in weight_names:
             param_path = os.path.join(np_folder, name)
             with open(param_path, "rb") as f:
                 param = np.load(f)
             yield name, torch.from_numpy(param)
@@ -82,27 +82,28 @@
     column_parallel_weight_names: List[str],
     row_parallel_weight_names: List[str],
     tensor_model_parallel_rank: int,
 ) -> None:
     for p in column_parallel_weight_names:
         if p in param_name:
             shard_size = param.shape[0]
-            loaded_weight = loaded_weight[
-                shard_size * tensor_model_parallel_rank
-                :shard_size * (tensor_model_parallel_rank + 1)]
+            start_idx = tensor_model_parallel_rank * shard_size
+            end_idx = (tensor_model_parallel_rank + 1) * shard_size
+            loaded_weight = loaded_weight[start_idx:end_idx]
             break
     for p in row_parallel_weight_names:
         if p in param_name:
             shard_size = param.shape[1]
-            loaded_weight = loaded_weight[
-                :,
-                shard_size * tensor_model_parallel_rank
-                :shard_size * (tensor_model_parallel_rank + 1)]
+            start_idx = tensor_model_parallel_rank * shard_size
+            end_idx = (tensor_model_parallel_rank + 1) * shard_size
+            loaded_weight = loaded_weight[:, start_idx:end_idx]
             break
-    assert param.shape == loaded_weight.shape
+    assert param.shape == loaded_weight.shape, (
+        f"{param_name} shape mismatch between model and checkpoint: "
+        f"{param.shape} != {loaded_weight.shape}")
     param.data.copy_(loaded_weight)
 
 
 def initialize_dummy_weights(
     model: torch.nn.Module,
     low: float = -1e-3,
     high: float = 1e-3,
```

### Comparing `vllm-0.1.1/vllm/outputs.py` & `vllm-0.1.2/vllm/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     Args:
         request_id: The unique ID of the request.
         prompt: The prompt string of the request.
         prompt_token_ids: The token IDs of the prompt.
         outputs: The output sequences of the request.
         finished: Whether the whole request is finished.
     """
+
     def __init__(
         self,
         request_id: str,
         prompt: str,
         prompt_token_ids: List[int],
         outputs: List[CompletionOutput],
         finished: bool,
@@ -71,16 +72,17 @@
 
     @classmethod
     def from_seq_group(cls, seq_group: SequenceGroup) -> "RequestOutput":
         # Get the top-n sequences.
         n = seq_group.sampling_params.n
         seqs = seq_group.get_seqs()
         assert n <= len(seqs)
-        sorted_seqs = sorted(
-            seqs, key=lambda seq: seq.get_cumulative_logprob(), reverse=True)
+        sorted_seqs = sorted(seqs,
+                             key=lambda seq: seq.get_cumulative_logprob(),
+                             reverse=True)
         top_n_seqs = sorted_seqs[:n]
 
         # Create the outputs.
         outputs: List[CompletionOutput] = []
         for seq in top_n_seqs:
             logprobs = seq.output_logprobs
             if seq_group.sampling_params.logprobs is None:
```

### Comparing `vllm-0.1.1/vllm/sampling_params.py` & `vllm-0.1.2/vllm/sampling_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Sampling parameters for text generation."""
 from typing import List, Optional, Union
 
+_SAMPLING_EPS = 1e-5
+
 
 class SamplingParams:
     """Sampling parameters for text generation.
 
     Overall, we follow the sampling parameters from the OpenAI text completion
     API (https://platform.openai.com/docs/api-reference/completions/create).
     In addition, we support beam search, which is not supported by OpenAI.
@@ -46,36 +48,41 @@
         best_of: Optional[int] = None,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         temperature: float = 1.0,
         top_p: float = 1.0,
         top_k: int = -1,
         use_beam_search: bool = False,
-        stop: Union[str, List[str]] = [],
+        stop: Union[None, str, List[str]] = None,
         ignore_eos: bool = False,
         max_tokens: int = 16,
         logprobs: Optional[int] = None,
     ) -> None:
         self.n = n
         self.best_of = best_of if best_of is not None else n
         self.presence_penalty = presence_penalty
         self.frequency_penalty = frequency_penalty
         self.temperature = temperature
         self.top_p = top_p
         self.top_k = top_k
         self.use_beam_search = use_beam_search
-        self.stop = [stop] if isinstance(stop, str) else list(stop)
+        if stop is None:
+            self.stop = []
+        elif isinstance(stop, str):
+            self.stop = [stop]
+        else:
+            self.stop = list(stop)
         self.ignore_eos = ignore_eos
         self.max_tokens = max_tokens
         self.logprobs = logprobs
 
         self._verify_args()
         if self.use_beam_search:
             self._verity_beam_search()
-        elif self.temperature == 0.0:
+        elif self.temperature < _SAMPLING_EPS:
             # Zero temperature means greedy sampling.
             self._verify_greedy_sampling()
 
     def _verify_args(self) -> None:
         if self.n < 1:
             raise ValueError(f"n must be at least 1, got {self.n}.")
         if self.best_of < self.n:
@@ -102,26 +109,26 @@
             raise ValueError(
                 f"logprobs must be non-negative, got {self.logprobs}.")
 
     def _verity_beam_search(self) -> None:
         if self.best_of == 1:
             raise ValueError("best_of must be greater than 1 when using beam "
                              f"search. Got {self.best_of}.")
-        if self.temperature > 0.0:
+        if self.temperature > _SAMPLING_EPS:
             raise ValueError("temperature must be 0 when using beam search.")
-        if self.top_p < 1.0:
+        if self.top_p < 1.0 - _SAMPLING_EPS:
             raise ValueError("top_p must be 1 when using beam search.")
         if self.top_k != -1:
             raise ValueError("top_k must be -1 when using beam search.")
 
     def _verify_greedy_sampling(self) -> None:
         if self.best_of > 1:
             raise ValueError("best_of must be 1 when using greedy sampling."
                              f"Got {self.best_of}.")
-        if self.top_p < 1.0:
+        if self.top_p < 1.0 - _SAMPLING_EPS:
             raise ValueError("top_p must be 1 when using greedy sampling.")
         if self.top_k != -1:
             raise ValueError("top_k must be -1 when using greedy sampling.")
 
     def __repr__(self) -> str:
         return (f"SamplingParams(n={self.n}, "
                 f"best_of={self.best_of}, "
```

### Comparing `vllm-0.1.1/vllm/utils.py` & `vllm-0.1.2/vllm/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+from platform import uname
 import uuid
 
 import psutil
 import torch
 
 
 class Device(enum.Enum):
@@ -12,17 +13,17 @@
 
 class Counter:
 
     def __init__(self, start: int = 0) -> None:
         self.counter = start
 
     def __next__(self) -> int:
-        id = self.counter
+        i = self.counter
         self.counter += 1
-        return id
+        return i
 
     def reset(self) -> None:
         self.counter = 0
 
 
 def get_gpu_memory(gpu: int = 0) -> int:
     """Returns the total memory of the GPU in bytes."""
@@ -32,7 +33,12 @@
 def get_cpu_memory() -> int:
     """Returns the total CPU memory of the node in bytes."""
     return psutil.virtual_memory().total
 
 
 def random_uuid() -> str:
     return str(uuid.uuid4().hex)
+
+
+def in_wsl() -> bool:
+    # Reference: https://github.com/microsoft/WSL/issues/4071
+    return "microsoft" in " ".join(uname()).lower()
```

### Comparing `vllm-0.1.1/vllm/worker/cache_engine.py` & `vllm-0.1.2/vllm/worker/cache_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """CacheEngine class for managing the KV cache."""
 from typing import Dict, List, Tuple
 
 import torch
 
 from vllm import cache_ops
 from vllm.config import CacheConfig, ModelConfig, ParallelConfig
+from vllm.logger import init_logger
+from vllm.utils import in_wsl
+
+logger = init_logger(__name__)
 
 KVCache = Tuple[torch.Tensor, torch.Tensor]
 
 
 class CacheEngine:
     """Manages the KV cache.
 
@@ -81,24 +85,30 @@
             gpu_cache.append((key_blocks, value_blocks))
         return gpu_cache
 
     def allocate_cpu_cache(self) -> List[KVCache]:
         cpu_cache: List[KVCache] = []
         key_block_shape = self.get_key_block_shape()
         value_block_shape = self.get_value_block_shape()
+        pin_memory = not in_wsl()
+        if not pin_memory:
+            # Pinning memory in WSL is not supported.
+            # https://docs.nvidia.com/cuda/wsl-user-guide/index.html#known-limitations-for-linux-cuda-applications
+            logger.warning("Using 'pin_memory=False' as WSL is detected. "
+                           "This may slow down the performance.")
         for _ in range(self.num_layers):
             key_blocks = torch.empty(
                 size=(self.num_cpu_blocks, *key_block_shape),
                 dtype=self.dtype,
-                pin_memory=True,
+                pin_memory=pin_memory,
             )
             value_blocks = torch.empty(
                 size=(self.num_cpu_blocks, *value_block_shape),
                 dtype=self.dtype,
-                pin_memory=True,
+                pin_memory=pin_memory,
             )
             cpu_cache.append((key_blocks, value_blocks))
         return cpu_cache
 
     def _swap(
         self,
         src: List[KVCache],
@@ -106,19 +116,18 @@
         src_to_dst: Dict[int, int],
     ) -> None:
         with torch.cuda.stream(self.cache_stream):
             for i in range(self.num_layers):
                 src_key_cache, src_value_cache = src[i]
                 dst_key_cache, dst_value_cache = dst[i]
                 # Copy the key blocks.
-                cache_ops.swap_blocks(
-                    src_key_cache, dst_key_cache, src_to_dst)
+                cache_ops.swap_blocks(src_key_cache, dst_key_cache, src_to_dst)
                 # Copy the value blocks.
-                cache_ops.swap_blocks(
-                    src_value_cache, dst_value_cache, src_to_dst)
+                cache_ops.swap_blocks(src_value_cache, dst_value_cache,
+                                      src_to_dst)
                 event = self.events[i]
                 event.record(stream=self.cache_stream)
 
     def swap_in(self, src_to_dst: Dict[int, int]) -> None:
         self._swap(self.cpu_cache, self.gpu_cache, src_to_dst)
 
     def swap_out(self, src_to_dst: Dict[int, int]) -> None:
```

### Comparing `vllm-0.1.1/vllm/worker/worker.py` & `vllm-0.1.2/vllm/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         torch.cuda.empty_cache()
         torch.cuda.reset_peak_memory_stats()
 
         # Profile memory usage with max_num_sequences sequences and the total
         # number of tokens equal to max_num_batched_tokens.
 
         # Enable top-k sampling to reflect the accurate memory usage.
-        sampling_params = SamplingParams(top_p=0.99,
-                                         top_k=self.model.config.vocab_size - 1)
+        vocab_size = self.model.config.vocab_size
+        sampling_params = SamplingParams(top_p=0.99, top_k=vocab_size - 1)
         max_num_batched_tokens = self.scheduler_config.max_num_batched_tokens
         max_num_seqs = self.scheduler_config.max_num_seqs
         seqs = []
         for group_id in range(max_num_seqs):
             seq_len = (max_num_batched_tokens // max_num_seqs +
                        (group_id < max_num_batched_tokens % max_num_seqs))
             seq_data = SequenceData([0] * seq_len)
@@ -87,15 +87,16 @@
                 is_prompt=True,
                 seq_data={group_id: seq_data},
                 sampling_params=sampling_params,
                 block_tables=None,
             )
             seqs.append(seq)
 
-        input_tokens, input_positions, input_metadata = self._prepare_inputs(seqs)
+        input_tokens, input_positions, input_metadata = self._prepare_inputs(
+            seqs)
 
         # Execute the model.
         num_layers = self.model_config.get_num_layers(self.parallel_config)
         self.model(
             input_ids=input_tokens,
             positions=input_positions,
             kv_caches=[(None, None)] * num_layers,
@@ -106,29 +107,32 @@
         # Calculate the number of blocks that can be allocated with the
         # profiled peak memory.
         torch.cuda.synchronize()
         peak_memory = torch.cuda.max_memory_allocated()
         total_gpu_memory = get_gpu_memory()
         cache_block_size = CacheEngine.get_cache_block_size(
             block_size, self.model_config, self.parallel_config)
-        num_gpu_blocks = int((total_gpu_memory * gpu_memory_utilization
-                              - peak_memory) // cache_block_size)
+        num_gpu_blocks = int(
+            (total_gpu_memory * gpu_memory_utilization - peak_memory) //
+            cache_block_size)
         num_cpu_blocks = int(cpu_swap_space // cache_block_size)
+        num_gpu_blocks = max(num_gpu_blocks, 0)
+        num_cpu_blocks = max(num_cpu_blocks, 0)
         torch.cuda.empty_cache()
 
         # Reset the seed to ensure that the random state is not affected by
         # the model initialization and profiling.
         set_random_seed(self.model_config.seed)
         return num_gpu_blocks, num_cpu_blocks
 
     def init_cache_engine(self, cache_config: CacheConfig) -> None:
         self.cache_config = cache_config
         self.block_size = cache_config.block_size
-        self.cache_engine = CacheEngine(
-            self.cache_config, self.model_config, self.parallel_config)
+        self.cache_engine = CacheEngine(self.cache_config, self.model_config,
+                                        self.parallel_config)
         self.cache_events = self.cache_engine.events
         self.gpu_cache = self.cache_engine.gpu_cache
 
     def _prepare_inputs(
         self,
         seq_group_metadata_list: List[SequenceGroupMetadata],
     ) -> Tuple[torch.Tensor, torch.Tensor, InputMetadata]:
@@ -196,16 +200,16 @@
                 position = context_len - 1
                 input_positions.append(position)
 
                 block_table = seq_group_metadata.block_tables[seq_id]
                 generation_block_tables.append(block_table)
 
                 max_context_len = max(max_context_len, context_len)
-                max_num_blocks_per_seq = max(
-                    max_num_blocks_per_seq, len(block_table))
+                max_num_blocks_per_seq = max(max_num_blocks_per_seq,
+                                             len(block_table))
                 context_lens.append(context_len)
 
                 block_number = block_table[position // self.block_size]
                 block_offset = position % self.block_size
                 slot = block_number * self.block_size + block_offset
                 slot_mapping.append(slot)
 
@@ -217,15 +221,16 @@
         # Convert to tensors.
         tokens_tensor = torch.cuda.LongTensor(input_tokens)
         positions_tensor = torch.cuda.LongTensor(input_positions)
         slot_mapping_tensor = torch.cuda.IntTensor(slot_mapping)
         context_lens_tensor = torch.cuda.IntTensor(context_lens)
         padded_block_tables = [
             _pad_to_max(block_table, max_num_blocks_per_seq)
-            for block_table in generation_block_tables]
+            for block_table in generation_block_tables
+        ]
         block_tables_tensor = torch.cuda.IntTensor(padded_block_tables)
 
         seq_data: Dict[int, SequenceData] = {}
         for seq_group_metadata in seq_group_metadata_list:
             seq_data.update(seq_group_metadata.seq_data)
 
         input_metadata = InputMetadata(
```

### Comparing `vllm-0.1.1/vllm.egg-info/PKG-INFO` & `vllm-0.1.2/vllm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
@@ -31,41 +31,44 @@
 | <a href="https://vllm.readthedocs.io/en/latest/"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://github.com/vllm-project/vllm/discussions"><b>Discussions</b></a> |
 
 </p>
 
 ---
 
 *Latest News* 🔥
-
-- [2023/06] We officially released vLLM! vLLM has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid April. Check out our [blog post](https://vllm.ai).
+- [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
+- [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).
 
 ---
 
 vLLM is a fast and easy-to-use library for LLM inference and serving.
 
 vLLM is fast with:
 
 - State-of-the-art serving throughput
 - Efficient management of attention key and value memory with **PagedAttention**
-- Dynamic batching of incoming requests
+- Continuous batching of incoming requests
 - Optimized CUDA kernels
 
 vLLM is flexible and easy to use with:
 
 - Seamless integration with popular HuggingFace models
 - High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
 - Tensor parallelism support for distributed inference
 - Streaming outputs
 - OpenAI-compatible API server
 
 vLLM seamlessly supports many Huggingface models, including the following architectures:
 
+- BLOOM (`bigscience/bloom`, `bigscience/bloomz`, etc.)
 - GPT-2 (`gpt2`, `gpt2-xl`, etc.)
-- GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
+- GPT BigCode (`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.)
+- GPT-NeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-tuned-alpha-7b`, etc.)
 - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`, `openlm-research/open_llama_13b`, etc.)
+- MPT (`mosaicml/mpt-7b`, `mosaicml/mpt-30b`, etc.)
 - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
 
 Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):
 
 ```bash
 pip install vllm
 ```
```

#### html2text {}

```diff
@@ -1,46 +1,53 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.1 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.2 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
                                      [vLLM]
            **** Easy, fast, and cheap LLM serving for everyone ****
                     | Documentation | Blog | Discussions |
---- *Latest News* ð¥ - [2023/06] We officially released vLLM! vLLM has
-powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid
-April. Check out our [blog post](https://vllm.ai). --- vLLM is a fast and easy-
-to-use library for LLM inference and serving. vLLM is fast with: - State-of-
-the-art serving throughput - Efficient management of attention key and value
-memory with **PagedAttention** - Dynamic batching of incoming requests -
-Optimized CUDA kernels vLLM is flexible and easy to use with: - Seamless
-integration with popular HuggingFace models - High-throughput serving with
-various decoding algorithms, including *parallel sampling*, *beam search*, and
-more - Tensor parallelism support for distributed inference - Streaming outputs
-- OpenAI-compatible API server vLLM seamlessly supports many Huggingface
-models, including the following architectures: - GPT-2 (`gpt2`, `gpt2-xl`,
-etc.) - GPTNeoX (`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`,
-`stabilityai/stablelm-tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`,
-`young-geng/koala`, `openlm-research/open_llama_13b`, etc.) - OPT (`facebook/
-opt-66b`, `facebook/opt-iml-max-30b`, etc.) Install vLLM with pip or [from
-source](https://vllm.readthedocs.io/en/latest/getting_started/
-installation.html#build-from-source): ```bash pip install vllm ``` ## Getting
-Started Visit our [documentation](https://vllm.readthedocs.io/en/latest/) to
-get started. - [Installation](https://vllm.readthedocs.io/en/latest/
-getting_started/installation.html) - [Quickstart](https://vllm.readthedocs.io/
-en/latest/getting_started/quickstart.html) - [Supported Models](https://
-vllm.readthedocs.io/en/latest/models/supported_models.html) ## Performance vLLM
-outperforms HuggingFace Transformers (HF) by up to 24x and Text Generation
-Inference (TGI) by up to 3.5x, in terms of throughput. For details, check out
-our [blog post](https://vllm.ai).
+--- *Latest News* ð¥ - [2023/06] Serving vLLM On any Cloud with SkyPilot.
+Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/
+master/llm/vllm) to start the vLLM demo, and the [blog post](https://
+blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/
+) for the story behind vLLM development on the clouds. - [2023/06] We
+officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna
+and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog
+post](https://vllm.ai). --- vLLM is a fast and easy-to-use library for LLM
+inference and serving. vLLM is fast with: - State-of-the-art serving throughput
+- Efficient management of attention key and value memory with
+**PagedAttention** - Continuous batching of incoming requests - Optimized CUDA
+kernels vLLM is flexible and easy to use with: - Seamless integration with
+popular HuggingFace models - High-throughput serving with various decoding
+algorithms, including *parallel sampling*, *beam search*, and more - Tensor
+parallelism support for distributed inference - Streaming outputs - OpenAI-
+compatible API server vLLM seamlessly supports many Huggingface models,
+including the following architectures: - BLOOM (`bigscience/bloom`,
+`bigscience/bloomz`, etc.) - GPT-2 (`gpt2`, `gpt2-xl`, etc.) - GPT BigCode
+(`bigcode/starcoder`, `bigcode/gpt_bigcode-santacoder`, etc.) - GPT-NeoX
+(`EleutherAI/gpt-neox-20b`, `databricks/dolly-v2-12b`, `stabilityai/stablelm-
+tuned-alpha-7b`, etc.) - LLaMA (`lmsys/vicuna-13b-v1.3`, `young-geng/koala`,
+`openlm-research/open_llama_13b`, etc.) - MPT (`mosaicml/mpt-7b`, `mosaicml/
+mpt-30b`, etc.) - OPT (`facebook/opt-66b`, `facebook/opt-iml-max-30b`, etc.)
+Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/
+getting_started/installation.html#build-from-source): ```bash pip install vllm
+``` ## Getting Started Visit our [documentation](https://vllm.readthedocs.io/
+en/latest/) to get started. - [Installation](https://vllm.readthedocs.io/en/
+latest/getting_started/installation.html) - [Quickstart](https://
+vllm.readthedocs.io/en/latest/getting_started/quickstart.html) - [Supported
+Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html) ##
+Performance vLLM outperforms HuggingFace Transformers (HF) by up to 24x and
+Text Generation Inference (TGI) by up to 3.5x, in terms of throughput. For
+details, check out our [blog post](https://vllm.ai).
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n1_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n1_light.png]
       Serving throughput when each request asks for 1 output completion.
   [https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/
   figures/perf_a10g_n3_light.png]    [https://raw.githubusercontent.com/vllm-
     project/vllm/main/docs/source/assets/figures/perf_a100_n3_light.png]
```

### Comparing `vllm-0.1.1/vllm.egg-info/SOURCES.txt` & `vllm-0.1.2/vllm.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 vllm/core/policy.py
 vllm/core/scheduler.py
 vllm/engine/__init__.py
 vllm/engine/arg_utils.py
 vllm/engine/async_llm_engine.py
 vllm/engine/llm_engine.py
 vllm/engine/ray_utils.py
-vllm/engine/tokenizer_utils.py
 vllm/entrypoints/__init__.py
 vllm/entrypoints/api_server.py
 vllm/entrypoints/llm.py
 vllm/entrypoints/openai/__init__.py
 vllm/entrypoints/openai/api_server.py
 vllm/entrypoints/openai/protocol.py
 vllm/model_executor/__init__.py
@@ -57,21 +56,29 @@
 vllm/model_executor/weight_utils.py
 vllm/model_executor/layers/__init__.py
 vllm/model_executor/layers/activation.py
 vllm/model_executor/layers/attention.py
 vllm/model_executor/layers/layernorm.py
 vllm/model_executor/layers/sampler.py
 vllm/model_executor/models/__init__.py
+vllm/model_executor/models/bloom.py
 vllm/model_executor/models/gpt2.py
+vllm/model_executor/models/gpt_bigcode.py
 vllm/model_executor/models/gpt_neox.py
 vllm/model_executor/models/llama.py
+vllm/model_executor/models/mpt.py
 vllm/model_executor/models/opt.py
 vllm/model_executor/parallel_utils/__init__.py
 vllm/model_executor/parallel_utils/parallel_state.py
 vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
 vllm/model_executor/parallel_utils/tensor_parallel/layers.py
 vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
 vllm/model_executor/parallel_utils/tensor_parallel/random.py
 vllm/model_executor/parallel_utils/tensor_parallel/utils.py
+vllm/transformers_utils/__init__.py
+vllm/transformers_utils/config.py
+vllm/transformers_utils/tokenizer.py
+vllm/transformers_utils/configs/__init__.py
+vllm/transformers_utils/configs/mpt.py
 vllm/worker/__init__.py
 vllm/worker/cache_engine.py
 vllm/worker/worker.py
```

