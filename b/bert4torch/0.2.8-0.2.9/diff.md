# Comparing `tmp/bert4torch-0.2.8.tar.gz` & `tmp/bert4torch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.2.8.tar", last modified: Thu May 18 15:21:02 2023, max compression
+gzip compressed data, was "bert4torch-0.2.9.tar", last modified: Wed Jul  5 15:31:43 2023, max compression
```

## Comparing `bert4torch-0.2.8.tar` & `bert4torch-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.252458 bert4torch-0.2.8/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    22857 2023-05-18 15:21:02.251446 bert4torch-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    22605 2023-05-18 15:17:35.000000 bert4torch-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.230447 bert4torch-0.2.8/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.2.8/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3117 2023-03-28 15:37:01.000000 bert4torch-0.2.8/bert4torch/activations.py
--rw-rw-rw-   0        0        0    11689 2023-05-15 14:15:22.000000 bert4torch-0.2.8/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    37983 2023-05-15 14:39:00.000000 bert4torch-0.2.8/bert4torch/generation.py
--rw-rw-rw-   0        0        0    89761 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/layers.py
--rw-rw-rw-   0        0        0    16592 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/losses.py
--rw-rw-rw-   0        0        0   121652 2023-05-16 11:38:12.000000 bert4torch-0.2.8/bert4torch/models.py
--rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.2.8/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    18596 2023-05-10 15:51:29.000000 bert4torch-0.2.8/bert4torch/quantization.py
--rw-rw-rw-   0        0        0    22590 2023-05-11 11:37:38.000000 bert4torch-0.2.8/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    35326 2023-04-28 12:14:08.000000 bert4torch-0.2.8/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:21:02.250446 bert4torch-0.2.8/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    22857 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-18 15:21:02.000000 bert4torch-0.2.8/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 15:21:01.000000 bert4torch-0.2.8/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:21:02.252458 bert4torch-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-05-18 15:12:22.000000 bert4torch-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.818426 bert4torch-0.2.9/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    23958 2023-07-05 15:31:43.818426 bert4torch-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    23706 2023-07-05 13:40:22.000000 bert4torch-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.797421 bert4torch-0.2.9/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.2.9/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.2.9/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    11080 2023-06-02 14:19:57.000000 bert4torch-0.2.9/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    38007 2023-05-23 15:20:25.000000 bert4torch-0.2.9/bert4torch/generation.py
+-rw-rw-rw-   0        0        0    93124 2023-07-05 14:53:38.000000 bert4torch-0.2.9/bert4torch/layers.py
+-rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.2.9/bert4torch/losses.py
+-rw-rw-rw-   0        0        0   127005 2023-07-05 14:16:53.000000 bert4torch-0.2.9/bert4torch/models.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.2.9/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    20836 2023-06-24 12:53:34.000000 bert4torch-0.2.9/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    20933 2023-06-26 16:27:26.000000 bert4torch-0.2.9/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35326 2023-04-28 12:14:08.000000 bert4torch-0.2.9/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.816424 bert4torch-0.2.9/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    23958 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 15:31:43.819426 bert4torch-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-07-05 15:30:52.000000 bert4torch-0.2.9/setup.py
```

### Comparing `bert4torch-0.2.8/LICENSE` & `bert4torch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.8/PKG-INFO` & `bert4torch-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.2.8
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bert4torch
-
-**一款用pytorch来复现bert4keras的简洁训练框架**
+![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
+[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
 
@@ -37,15 +26,15 @@
 ```shell
 pip install git+https://github.com/Tongjilibo/bert4torch
 ```
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
-- **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
+- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
 
 - **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
@@ -75,15 +64,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
@@ -97,14 +86,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
 | 0.2.3          | 0.0.2           |
@@ -112,14 +102,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
@@ -154,17 +145,19 @@
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
 | bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
 | roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
 | deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
 | guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
 | xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
@@ -183,17 +176,19 @@
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
 | Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -233,8 +228,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.2.8/README.md` & `bert4torch-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-# bert4torch
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.2.9
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-**一款用pytorch来复现bert4keras的简洁训练框架**
+![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
+[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
 
@@ -27,15 +36,15 @@
 ```shell
 pip install git+https://github.com/Tongjilibo/bert4torch
 ```
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
-- **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
+- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
 
 - **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
@@ -65,15 +74,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
@@ -87,14 +96,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
 | 0.2.3          | 0.0.2           |
@@ -102,14 +112,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
@@ -144,17 +155,19 @@
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
 | bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
 | roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
 | deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
 | guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
 | xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
@@ -173,17 +186,19 @@
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
 | Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -223,8 +238,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.2.8/bert4torch/activations.py` & `bert4torch-0.2.9/bert4torch/activations.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,18 +69,24 @@
     mish = nn.functional.mish
 
 
 def linear_act(x):
     return x
 
 
+def swiglu(x, dim=-1):
+    x = torch.chunk(x, 2, dim=dim)
+    return silu(x[0]) * x[1]
+
+
 ACT2FN = {
     "relu": nn.functional.relu,
     "silu": silu,
     "swish": silu,
+    "swiglu": swiglu,
     "gelu": gelu,
     "tanh": torch.tanh,
     "gelu_new": _gelu_new,
     "gelu_fast": gelu_fast,
     "quick_gelu": quick_gelu,
     "mish": mish,
     "linear": linear_act,
```

### Comparing `bert4torch-0.2.8/bert4torch/callbacks.py` & `bert4torch-0.2.9/bert4torch/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -224,27 +224,7 @@
         # 虚拟对抗训练
         elif self.mode == 'vat':
             logit = self.trainer.output[self.adversarial['rank']] if isinstance(self.trainer.output, (tuple, list)) else self.trainer.output
             adv_loss = self.ad_train.virtual_adversarial_training(self.trainer.train_X, logit)
             self.trainer.loss_detail.update({'loss_sup': self.trainer.loss.item(), 'loss_unsup': adv_loss})
             self.trainer.loss += (adv_loss if adv_loss else 0)
             self.trainer.loss.backward()
-
-
-class AccelerateCallback(Callback):
-    """Accelerate的Callback
-    """
-    def __init__(self, accelerator):
-        self.accelerator = accelerator
-
-    def get_module(self):
-        '''返回nn.Module模块
-        '''
-        unwrap_model = self.accelerator.unwrap_model(self.model)
-        return unwrap_model.module if hasattr(unwrap_model, 'module') else unwrap_model
-
-    def on_train_begin(self, logs=None):
-        self.trainer.loss_backward = False
-        self.trainer.get_module = self.get_module
-
-    def on_train_step_end(self, logs=None):
-        self.accelerator.backward(self.trainer.loss)
```

### Comparing `bert4torch-0.2.8/bert4torch/generation.py` & `bert4torch-0.2.9/bert4torch/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''自回归模型的生成
 '''
 
 import torch
 import torch.nn as nn
 import numpy as np
-from bert4torch.snippets import take_along_dim, torch_div, sequence_padding, create_position_ids_start_at_padding
+from bert4torch.snippets import take_along_dim, torch_div, sequence_padding, create_position_ids_start_at_padding, colorful
 
 class AutoRegressiveDecoder(object):
     """通用自回归生成模型解码基类
     包含beam search和random sample两种策略
 
     :param start_id: int, 解码使用的起始token_id，不同预训练模型设置可能不一样
     :param end_id: int, 解码使用的结束token_id，不同预训练模型设置可能不一样
@@ -607,15 +607,15 @@
     def batch_generate(self, text_list, topk=50, topp=1, temperature=1, min_ends=1):
         '''batch样本生成，use_states=True时要求pad_mode='pre', use_states=False时候对'''
         # 参数设定
         assert isinstance(text_list, (list,tuple)), 'Arg `text_list` must be list/tuple format'
         self.use_batch = True
         if self.use_states and (self.pad_mode in {'post', 'right'}):
             self.pad_mode = 'pre'
-            print("[WARNING] When arg `use_states`=True, you may set `pad_mode`='pre' to avoid error output, reset `pad_mode`='pre' instead")
+            print(colorful("[WARNING]") + "When arg `use_states`=True, you may set `pad_mode`='pre' to avoid error output, reset `pad_mode`='pre' instead")
 
         # 主流程
         inputs = self.pre_process(text_list)
         output_ids = self._generate(inputs, 1, topk, topp, temperature, min_ends)
         return self.post_process(output_ids)
 
     def stream_generate(self, text:str, topk=50, topp=1, temperature=1, min_ends=1):
```

### Comparing `bert4torch-0.2.8/bert4torch/layers.py` & `bert4torch-0.2.9/bert4torch/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 import numpy as np
 import math
 from bert4torch.snippets import get_sinusoid_encoding_table, take_along_dim, torch_div
 from bert4torch.activations import get_activation
 from typing import List, Optional, Union
 import random
 import warnings
-try:
-    import loralib as lora
-except ImportError:
-    lora = None
+
 
 class LayerNorm(nn.Module):
     def __init__(self, hidden_size, eps=1e-12, conditional_size=False, weight=True, bias=True, norm_mode='normal', **kwargs):
         """layernorm 层，这里自行实现，目的是为了兼容 conditianal layernorm，使得可以做条件文本生成、条件分类等任务
            条件layernorm来自于苏剑林的想法，详情：https://spaces.ac.cn/archives/7124
         """
         super(LayerNorm, self).__init__()
@@ -35,15 +32,20 @@
             # 这里采用全零初始化, 目的是在初始状态不干扰原来的预训练权重
             self.dense1 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense1.weight.data.uniform_(0, 0)
             self.dense2 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense2.weight.data.uniform_(0, 0)
 
     def forward(self, inputs):
-        x = inputs[0]
+        if isinstance(inputs, (list,tuple)):
+            x = inputs[0]
+        elif isinstance(inputs, torch.Tensor):
+            x = inputs
+        else:
+            raise ValueError('LayerNorm inputs format error')
 
         if self.norm_mode == 'rmsnorm':
             # t5使用的是RMSnorm
             variance = x.float().pow(2).mean(-1, keepdim=True)
             o = (x.float() * torch.rsqrt(variance + self.eps)).type_as(x)
         else:
             u = x.mean(-1, keepdim=True)
@@ -76,34 +78,42 @@
         self.output_attentions = output_attentions
         self.bias = bias
 
         # t5_pegasus_small中hidden_size/num_attention_heads != 0
         # 苏神的roberta small中qk的维度和v不同
         self.attention_head_size = kwargs.get('attention_head_size', int(hidden_size/num_attention_heads))
         self.attention_key_size = kwargs.get('attention_key_size', self.attention_head_size)
-        self.qk_inner_dim = self.attention_key_size * self.num_attention_heads
-        self.v_inner_dim = self.attention_head_size * self.num_attention_heads
-
-        self.q = nn.Linear(hidden_size, self.qk_inner_dim, bias=bias, device=kwargs['skip_init'])
-        self.k = nn.Linear(hidden_size, self.qk_inner_dim, bias=bias, device=kwargs['skip_init'])
-        self.v = nn.Linear(hidden_size, self.v_inner_dim, bias=bias, device=kwargs['skip_init'])
-        self.o = nn.Linear(self.v_inner_dim, hidden_size, bias=bias, device=kwargs['skip_init'])
+        q_inner_dim = self.attention_key_size * self.num_attention_heads
+        k_inner_dim = q_inner_dim
+        v_inner_dim = self.attention_head_size * self.num_attention_heads
+
+        # multi query attention
+        if kwargs.get('multi_query_group_num') is not None:
+            self.multi_query_group_num = kwargs.get('multi_query_group_num')
+            k_inner_dim_tmp = self.attention_head_size * self.multi_query_group_num
+            v_inner_dim_tmp = k_inner_dim_tmp
+
+        self.q = nn.Linear(hidden_size, q_inner_dim, bias=bias)
+        self.k = nn.Linear(hidden_size, k_inner_dim_tmp if hasattr(self, 'multi_query_group_num') else k_inner_dim, bias=bias)
+        self.v = nn.Linear(hidden_size, v_inner_dim_tmp if hasattr(self, 'multi_query_group_num') else v_inner_dim, bias=bias)
+        self.o = nn.Linear(v_inner_dim, hidden_size, bias=bias)
         self.dropout = nn.Dropout(attention_probs_dropout_prob)
 
         self.a_bias, self.p_bias = kwargs.get('a_bias'), kwargs.get('p_bias')
 
         if self.p_bias == 'typical_relative':  # nezha
             self.relative_positions_encoding = RelativePositionsEncoding(qlen=kwargs.get('max_position'),
                                                                          klen=kwargs.get('max_position'),
                                                                          embedding_size=self.attention_head_size,
                                                                          max_relative_position=kwargs.get('max_relative_position'))
         elif self.p_bias == 'rotary':  # roformer, llama, chatglm
             # position_encoding_2d 目前仅在chatglm中使用
             self.position_encoding_2d = kwargs.get('position_encoding_2d', False)
-            embedding_size = self.attention_head_size//2 if self.position_encoding_2d else self.attention_head_size
+            self.position_encoding_2d_v2 = kwargs.get('position_encoding_2d_v2', False)
+            embedding_size = self.attention_head_size//2 if self.position_encoding_2d or self.position_encoding_2d_v2 else self.attention_head_size
             self.relative_positions_encoding = RoPEPositionEncoding(embedding_size=embedding_size, rope_rank=kwargs.get('rope_rank', 'adjacent'))
         elif self.p_bias == 't5_relative':  # t5
             self.relative_positions = RelativePositionsEncodingT5(qlen=kwargs.get('max_position'), 
                                                                   klen=kwargs.get('max_position'), 
                                                                   relative_attention_num_buckets=kwargs.get('relative_attention_num_buckets'), 
                                                                   is_decoder=kwargs.get('is_decoder'))
             self.relative_positions_encoding = nn.Embedding(kwargs.get('relative_attention_num_buckets'), self.num_attention_heads)
@@ -127,78 +137,36 @@
                                                                          max_position=kwargs.get('max_position'))
             self.relative_positions_encoding = nn.Embedding(kwargs.get('max_position'), self.hidden_size)
             self.norm_rel_ebd = [x.strip() for x in kwargs.get("norm_rel_ebd", "none").lower().split("|")]
             if "layer_norm" in self.norm_rel_ebd:
                 self.layernorm = nn.LayerNorm(self.hidden_size, kwargs.get('layer_norm_eps', 1e-12), elementwise_affine=True)
             self.pos_dropout = nn.Dropout(dropout_rate)
 
-    def transpose_for_qk_scores(self, x):
+    def transpose_for_q_scores(self, x):
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_key_size)
         x = x.view(*new_x_shape)
         return x.permute(0, 2, 1, 3)
-    
-    def transpose_for_v_scores(self, x):
-        new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
+
+    def transpose_for_k_scores(self, x):
+        if hasattr(self, 'multi_query_group_num'):
+            new_x_shape = x.size()[:-1] + (self.multi_query_group_num, self.attention_key_size)
+        else:
+            new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_key_size)
         x = x.view(*new_x_shape)
         return x.permute(0, 2, 1, 3)
-    
-    def forward(self, hidden_states=None, attention_mask=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, **model_kwargs):
-        # hidden_states shape: [batch_size, seq_q, hidden_size]
-        # attention_mask shape: [batch_size, 1, 1, seq_q] 或者 [batch_size, 1, seq_q, seq_q]
-        # encoder_hidden_states shape: [batch_size, seq_k, hidden_size]
-        # encoder_attention_mask shape: [batch_size, 1, 1, seq_k]
-        # past_key_value shape: ([batch_size, num_attention_heads, key_len_cache, attention_head_size], ...)
-
-        query_layer = self.transpose_for_qk_scores(self.q(hidden_states))
 
-        # 参考hf增加了关于past_key_value的逻辑
-        if self.p_bias == 'rotary':
-            # rotary有cache情况下，需要先rope后再和past_key_value concat
-            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
-            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
-        elif (encoder_hidden_states is not None) and past_key_value is not None:
-            key_layer = past_key_value[0]
-            value_layer = past_key_value[1]
-            attention_mask = encoder_attention_mask
-        elif encoder_hidden_states is not None:
-            key_layer = self.transpose_for_qk_scores(self.k(encoder_hidden_states))
-            value_layer = self.transpose_for_v_scores(self.v(encoder_hidden_states))
-            attention_mask = encoder_attention_mask
-        elif past_key_value is not None:
-            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
-            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
-            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
-            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+    def transpose_for_v_scores(self, x):
+        if hasattr(self, 'multi_query_group_num'):
+            new_x_shape = x.size()[:-1] + (self.multi_query_group_num, self.attention_head_size)
         else:
-            key_layer = self.transpose_for_qk_scores(self.k(hidden_states))
-            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
-        # query_layer shape: [batch_size, num_attention_heads, query_len, attention_head_size]
-        # key_layer shape: [batch_size, num_attention_heads, key_len, attention_head_size]
-        # value_layer shape: [batch_size, num_attention_heads, value_len, attention_head_size]
-
-        if self.p_bias == 'rotary':
-            if self.position_encoding_2d:  # chatglm独有逻辑
-                q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
-                k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
-                q1 = self.relative_positions_encoding(q1, model_kwargs['position_ids'][:, 0, :])
-                k1 = self.relative_positions_encoding(k1, model_kwargs['position_ids'][:, 0, :])
-                q2 = self.relative_positions_encoding(q2, model_kwargs['position_ids'][:, 1, :])
-                k2 = self.relative_positions_encoding(k2, model_kwargs['position_ids'][:, 1, :])
-                query_layer = torch.concat([q1, q2], dim=(q1.ndim - 1))
-                key_layer = torch.concat([k1, k2], dim=(k1.ndim - 1))
-            else:  # 原rotary逻辑
-                query_layer = self.relative_positions_encoding(query_layer, model_kwargs['position_ids'])
-                key_layer = self.relative_positions_encoding(key_layer, model_kwargs['position_ids'])
-            if past_key_value is not None:  # 过了rope再concat
-                key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
-                value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
-
-        if self.is_decoder:
-            past_key_value = (key_layer, value_layer)
-
+            new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
+        x = x.view(*new_x_shape)
+        return x.permute(0, 2, 1, 3)
+    
+    def get_context_layer(self, query_layer, key_layer, value_layer, attention_mask):
         # 交换k的最后两个维度，然后q和k执行点积, 获得attention score
         attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
 
         # attention_scores shape: [batch_size, num_attention_heads, query_len, key_len]
         if (self.p_bias == 'typical_relative') and hasattr(self, 'relative_positions_encoding'):
             relations_keys = self.relative_positions_encoding(attention_scores.shape[-1], attention_scores.shape[-1])  # [to_seq_len, to_seq_len, d_hid]
             # 旧实现，方便读者理解维度转换
@@ -231,19 +199,14 @@
             attention_scores = attention_scores + rel_att
 
         elif self.attention_scale:
             attention_scores = attention_scores / math.sqrt(self.attention_head_size)
         # 执行attention mask，对于mask为0部分的attention mask，
         # 值为-1e10，经过softmax后，attention_probs几乎为0，所以不会attention到mask为0的部分
         if attention_mask is not None:
-            # attention_mask最后两维是[q_len, k_ken]，如果维度不匹配补齐，目前是在ptuning_v2中使用
-            if attention_mask.shape[-1] < attention_scores.shape[-1]:
-                size_ = attention_mask.shape[:3] + torch.Size([attention_scores.shape[-1]-attention_mask.shape[-1]])
-                pre_attention_mask = torch.ones(size_).to(attention_mask)
-                attention_mask = torch.cat([pre_attention_mask, attention_mask], dim=-1)
             # attention_mask = attention_mask * attention_mask.squeeze(-2).unsqueeze(-1)  # deberta_v2中使用，但是不使用也不影响
             # attention_scores = attention_scores.masked_fill(attention_mask == 0, -1e10)  # 下一行的另一种写法
             attention_mask = (1.0 - attention_mask) * -10000.0  # 所以传入的mask的非padding部分为1, padding部分为0
             attention_scores = attention_scores + attention_mask
 
         # 将attention score 归一化到0-1
         attention_probs = F.softmax(attention_scores, dim=-1)
@@ -263,16 +226,109 @@
             context_layer = context_layer + value_position_scores_r_t
 
         # context_layer shape: [batch_size, query_len, num_attention_heads, attention_head_size]
         # transpose、permute等维度变换操作后，tensor在内存中不再是连续存储的，而view操作要求tensor的内存连续存储，
         # 所以在调用view之前，需要contiguous来返回一个contiguous copy；
         context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
 
-        new_context_layer_shape = context_layer.size()[:-2] + (self.v_inner_dim,)
+        new_context_layer_shape = context_layer.size()[:-2] + (context_layer.size()[-2]*context_layer.size()[-1],)
         context_layer = context_layer.view(*new_context_layer_shape)
+        return context_layer, attention_scores
+
+    def apply_rotary_pos_emb(self, query_layer, key_layer, value_layer, position_ids, past_key_value):
+        if self.position_encoding_2d:  # chatglm独有逻辑
+            q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
+            k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
+            q1 = self.relative_positions_encoding(q1, position_ids[:, 0, :])
+            k1 = self.relative_positions_encoding(k1, position_ids[:, 0, :])
+            q2 = self.relative_positions_encoding(q2, position_ids[:, 1, :])
+            k2 = self.relative_positions_encoding(k2, position_ids[:, 1, :])
+            query_layer = torch.concat([q1, q2], dim=(q1.ndim - 1))
+            key_layer = torch.concat([k1, k2], dim=(k1.ndim - 1))
+        elif self.position_encoding_2d_v2:  # chatglm2的独有逻辑
+            q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
+            k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
+            q1 = torch.cat([q1[..., ::2], q1[..., 1::2]], dim=-1)
+            k1 = torch.cat([k1[..., ::2], k1[..., 1::2]], dim=-1)
+            q1 = self.relative_positions_encoding(q1, position_ids)
+            k1 = self.relative_positions_encoding(k1, position_ids)
+            query_layer = torch.concat([q1, q2], dim=(q1.ndim - 1))
+            key_layer = torch.concat([k1, k2], dim=(k1.ndim - 1))
+        else:  # 原rotary逻辑
+            query_layer = self.relative_positions_encoding(query_layer, position_ids)
+            key_layer = self.relative_positions_encoding(key_layer, position_ids)
+        if past_key_value is not None:  # 过了rope再concat
+            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+        return query_layer, key_layer, value_layer
+
+    def forward(self, hidden_states=None, attention_mask=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, position_ids=None, **model_kwargs):
+        # hidden_states shape: [batch_size, seq_q, hidden_size]
+        # attention_mask shape: [batch_size, 1, 1, seq_q] 或者 [batch_size, 1, seq_q, seq_q]
+        # encoder_hidden_states shape: [batch_size, seq_k, hidden_size]
+        # encoder_attention_mask shape: [batch_size, 1, 1, seq_k]
+        # past_key_value shape: ([batch_size, num_attention_heads, key_len_cache, attention_head_size], ...)
+
+        query_layer = self.transpose_for_q_scores(self.q(hidden_states))
+
+        # 参考hf增加了关于past_key_value的逻辑
+        if self.p_bias == 'rotary':
+            # rotary有cache情况下，需要先rope后再和past_key_value concat
+            key_layer = self.transpose_for_k_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
+        elif (encoder_hidden_states is not None) and past_key_value is not None:
+            key_layer = past_key_value[0]
+            value_layer = past_key_value[1]
+            attention_mask = encoder_attention_mask
+        elif encoder_hidden_states is not None:
+            key_layer = self.transpose_for_k_scores(self.k(encoder_hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(encoder_hidden_states))
+            attention_mask = encoder_attention_mask
+        elif past_key_value is not None:
+            key_layer = self.transpose_for_k_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
+            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+        else:
+            key_layer = self.transpose_for_k_scores(self.k(hidden_states))
+            value_layer = self.transpose_for_v_scores(self.v(hidden_states))
+        # query_layer shape: [batch_size, num_attention_heads, query_len, attention_head_size]
+        # key_layer shape: [batch_size, num_attention_heads, key_len, attention_head_size]
+        # value_layer shape: [batch_size, num_attention_heads, value_len, attention_head_size]
+
+        if self.p_bias == 'rotary':
+            query_layer, key_layer, value_layer = self.apply_rotary_pos_emb(query_layer, key_layer, value_layer, position_ids, past_key_value)
+
+        if self.is_decoder:
+            past_key_value = (key_layer, value_layer)
+
+        # multi_query_attention
+        if hasattr(self, 'multi_query_group_num'):
+            key_layer = key_layer.unsqueeze(2)
+            key_layer = key_layer.expand(-1, -1, self.num_attention_heads // self.multi_query_group_num, -1, -1)
+            key_layer = key_layer.contiguous().view(key_layer.shape[:1] + (self.num_attention_heads,) + key_layer.shape[-2:])
+            value_layer = value_layer.unsqueeze(2)
+            value_layer = value_layer.expand(-1, -1, self.num_attention_heads // self.multi_query_group_num, -1, -1)
+            value_layer = value_layer.contiguous().view(value_layer.shape[:1] + (self.num_attention_heads,) + value_layer.shape[-2:])
+
+        # attention_mask最后两维是[q_len, k_ken]，如果维度不匹配补齐，目前是在ptuning_v2中使用
+        if attention_mask.shape[-1] < key_layer.shape[-2]:
+            size_ = attention_mask.shape[:3] + torch.Size([key_layer.shape[-2]-attention_mask.shape[-1]])
+            pre_attention_mask = torch.ones(size_).to(attention_mask)
+            attention_mask = torch.cat([pre_attention_mask, attention_mask], dim=-1)
+
+        # 是否使用torch2.0的flash_attention加速
+        if int(torch.__version__.split('.')[0]) >= 2:
+            context_layer = torch.nn.functional.scaled_dot_product_attention(query_layer, key_layer, value_layer, attention_mask.bool())
+            context_layer = context_layer.permute(0, 2, 1, 3)
+            new_context_layer_shape = context_layer.size()[:-2] + (context_layer.size()[-2]*context_layer.size()[-1],)
+            context_layer = context_layer.reshape(*new_context_layer_shape)
+            attention_scores = None
+        else:
+            context_layer, attention_scores = self.get_context_layer(query_layer, key_layer, value_layer, attention_mask)
 
         # 是否返回attention scores
         outputs = (self.o(context_layer), attention_scores) if self.output_attentions else (self.o(context_layer),)
         return outputs + (past_key_value,) if self.is_decoder else outputs
 
     def disentangled_attention_bias(self, query_layer, key_layer, relative_pos, rel_embeddings, scale_factor):
         '''deberta_v2使用，和原版区别是query_layer是4维'''
@@ -289,16 +345,16 @@
             raise ValueError(f"Relative position ids must be of dim 2 or 3 or 4. {relative_pos.dim()}")
 
         att_span = self.pos_ebd_size
         relative_pos = relative_pos.long().to(query_layer.device)
 
         rel_embeddings = rel_embeddings[0 : att_span * 2, :].unsqueeze(0)
         if self.share_att_key:
-            pos_query_layer = self.transpose_for_qk_scores(self.q(rel_embeddings)).repeat(btz, 1, 1, 1)
-            pos_key_layer = self.transpose_for_qk_scores(self.k(rel_embeddings)).repeat(btz, 1, 1, 1)
+            pos_query_layer = self.transpose_for_q_scores(self.q(rel_embeddings)).repeat(btz, 1, 1, 1)
+            pos_key_layer = self.transpose_for_k_scores(self.k(rel_embeddings)).repeat(btz, 1, 1, 1)
         else:
             # 这里逻辑去掉了
             pass
 
         score = 0
         # content->position
         if "c2p" in self.pos_att_type:
@@ -332,16 +388,16 @@
         # 这样不统一做法的原因不得而知，不过有没有这一层，差别可能不会很大；
 
         # 为了适配是否dropout，用is_dropout，dropout_rate两个参数控制；如果是实现原始的transformer，直接使用默认参数即可；如果是实现bert，则is_dropout为False，此时的dropout_rate参数并不会使用.
         super(PositionWiseFeedForward, self).__init__()
 
         self.is_dropout = is_dropout
         self.intermediate_act_fn = get_activation(hidden_act)
-        self.intermediateDense = nn.Linear(hidden_size, intermediate_size, bias=bias, device=kwargs['skip_init'])
-        self.outputDense = nn.Linear(intermediate_size, hidden_size, bias=bias, device=kwargs['skip_init'])
+        self.intermediateDense = nn.Linear(hidden_size, intermediate_size*2 if hidden_act=='swiglu' else intermediate_size, bias=bias)
+        self.outputDense = nn.Linear(intermediate_size, hidden_size, bias=bias)
         if self.is_dropout:
             self.dropout = nn.Dropout(dropout_rate)
 
     def forward(self, x):
         # x shape: (batch size, seq len, hidden_size)
         if self.is_dropout:
             x = self.dropout(self.intermediate_act_fn(self.intermediateDense(x)))
@@ -447,44 +503,45 @@
             return out.unbind(dim = -2)
 
 
 class BertEmbeddings(nn.Module):
     """embeddings层
        构造word, position and token_type embeddings.
     """
-    def __init__(self, vocab_size, embedding_size, hidden_size, max_position, segment_vocab_size, shared_segment_embeddings, dropout_rate, conditional_size=False, pad_token_id=0, **kwargs):
+    def __init__(self, vocab_size, embedding_size, hidden_size, max_position, segment_vocab_size, shared_segment_embeddings, dropout_rate, conditional_size=False, 
+                 pad_token_id=0, **kwargs):
         super(BertEmbeddings, self).__init__()
         self.shared_segment_embeddings = shared_segment_embeddings
-        self.word_embeddings = nn.Embedding(vocab_size, embedding_size, padding_idx=pad_token_id, device=kwargs['skip_init'])
+        self.word_embeddings = nn.Embedding(vocab_size, embedding_size, padding_idx=pad_token_id)
 
         # 位置编码
         if kwargs.get('p_bias') == 'sinusoid':
             self.position_embeddings = SinusoidalPositionEncoding(max_position, embedding_size)
         elif kwargs.get('p_bias') in {'rotary', 'typical_relative', 't5_relative', 'other_relative', 'deberta_v2'}:
             # 如果使用相对位置编码，则不声明PositionEmbeddings
             pass
         elif max_position > 0:
-            self.position_embeddings = nn.Embedding(max_position, embedding_size, device=kwargs['skip_init'])
+            self.position_embeddings = nn.Embedding(max_position, embedding_size)
         
         # segement编码
         if (segment_vocab_size > 0) and (not shared_segment_embeddings) and kwargs.get('use_segment_embedding', True):
             # use_segment_embedding用于lm, unilm场景，不使用segment_embeddings但是传入segment_ids用于计算mask
             # 一般无需设置，目前仅在guwenbert中使用
-            self.segment_embeddings = nn.Embedding(segment_vocab_size, embedding_size, device=kwargs['skip_init'])
+            self.segment_embeddings = nn.Embedding(segment_vocab_size, embedding_size)
 
         # emb_scale
         self.emb_scale = kwargs.get('emb_scale', 1)  # transform_xl, xlnet特有
 
         # LayerNorm
         self.layerNorm = LayerNorm(embedding_size, eps=kwargs.get('layer_norm_eps', 1e-12), conditional_size=conditional_size, **kwargs)
         self.dropout = nn.Dropout(dropout_rate)
 
         # 如果embedding_size != hidden_size，则再有一个linear(适用于albert矩阵分解)
         if embedding_size != hidden_size:
-            self.embedding_hidden_mapping_in = nn.Linear(embedding_size, hidden_size, device=kwargs['skip_init'])
+            self.embedding_hidden_mapping_in = nn.Linear(embedding_size, hidden_size)
 
     def forward(self, token_ids=None, segment_ids=None, position_ids=None, conditional_emb=None, additional_embs=None, attention_mask=None):
         if (not token_ids.requires_grad) and (token_ids.dtype in {torch.long, torch.int}):
             words_embeddings = self.word_embeddings(token_ids)
         else:
             words_embeddings = token_ids  # 自定义word_embedding，目前仅有VAT中使用
 
@@ -549,25 +606,26 @@
         self.is_decoder = kwargs.get('is_decoder', False)
         self.add_cross_attention = kwargs.get('add_cross_attention', False)
         if self.add_cross_attention and self.is_decoder:
             self.crossAttention = MultiHeadAttentionLayer(hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate, **kwargs)
             self.dropout3 = nn.Dropout(dropout_rate)
             self.layerNorm3 = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
 
-    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, cross_past_key_value=None, **model_kwargs):
+    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, 
+                cross_past_key_value=None, position_ids=None, **model_kwargs):
         # self attention
         x = self.layerNorm1((hidden_states, conditional_emb)) if self.pre_post_norm == 'pre' else hidden_states
-        self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)  # self.decoder为true时候，这里的attention_mask是三角的
+        self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, position_ids=position_ids)  # self.decoder为true时候，这里的attention_mask是三角的
         hidden_states = hidden_states + self.dropout1(self_attn_output[0])
         if self.pre_post_norm == 'post':
             hidden_states = self.layerNorm1((hidden_states, conditional_emb))
         
         # cross attention
         if self.is_decoder and encoder_hidden_states is not None:
-            cross_attn_output = self.crossAttention(hidden_states, None, encoder_hidden_states, encoder_attention_mask, cross_past_key_value, **model_kwargs)
+            cross_attn_output = self.crossAttention(hidden_states, None, encoder_hidden_states, encoder_attention_mask, cross_past_key_value, position_ids=position_ids)
             hidden_states = hidden_states + self.dropout3(cross_attn_output[0])
             model_kwargs['cross_past_key_value'] = cross_attn_output[-1]
             if self.pre_post_norm == 'post':
                 hidden_states = self.layerNorm3((hidden_states, conditional_emb))
 
         # feedforward
         x = self.layerNorm2((hidden_states, conditional_emb)) if self.pre_post_norm == 'pre' else hidden_states
@@ -594,15 +652,16 @@
             self.feedForward = self.T5PositionWiseFeedForward(**kwargs)
 
         # decoder中间有crossAttention
         if self.add_cross_attention and self.is_decoder and hasattr(self.crossAttention, 'relative_positions_encoding'):
             del self.crossAttention.relative_positions_encoding
             del self.crossAttention.relative_positions
 
-    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, cross_past_key_value=None, **model_kwargs):
+    def forward(self, hidden_states=None, attention_mask=None, conditional_emb=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, 
+                cross_past_key_value=None, **model_kwargs):
         # bert的layernorm是在attn/ffc之后，Openai-gpt2是在之前
         x = self.layerNorm1((hidden_states, conditional_emb))
         self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value)
         hidden_states = hidden_states + self.dropout1(self_attn_output[0])
 
         # cross attention
         if self.is_decoder and encoder_hidden_states is not None:
@@ -724,16 +783,16 @@
             # w: 词向量[btz, q_len, hdsz], cat: w和mem_i拼接后向量[btz, k_len, hdsz], r：相对位置向量[r_len, hdsz]
             qlen, rlen, bsz = w.size(1), r.size(0), w.size(0)
             
             mixed_query_layer = self.q(cat)[:, -qlen:, :]  # 仅取用query部分，不适用mem部分
             mixed_key_layer = self.k(cat)
             mixed_value_layer = self.v(cat)
 
-            w_head_q = self.transpose_for_qk_scores(mixed_query_layer)  # [btz, n_head, q_len, d_head]
-            w_head_k = self.transpose_for_qk_scores(mixed_key_layer)  # [btz, n_head, k_len, d_head]
+            w_head_q = self.transpose_for_q_scores(mixed_query_layer)  # [btz, n_head, q_len, d_head]
+            w_head_k = self.transpose_for_k_scores(mixed_key_layer)  # [btz, n_head, k_len, d_head]
             w_head_v = self.transpose_for_v_scores(mixed_value_layer)  # [btz, n_head, k_len, d_head]
 
             r_head_k = self.r(r)  # [hdsz, nhead*headsize] = [r_len, 1, nhead*headsize]
             r_head_k = r_head_k.view(rlen, self.num_attention_heads, self.attention_head_size)  # rlen x n_head x d_head
 
             #### compute attention score
             rw_head_q = w_head_q + self.r_w_bias.unsqueeze(1)  # [btz, n_head, q_len, d_head]
@@ -1007,15 +1066,15 @@
         if self.rope_rank == 'adjacent':
             cos_position = position_embeddings[:, 1::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
             sin_position = position_embeddings[:, ::2].repeat_interleave(2, dim=-1)  # [seq_len, hdsz]
         elif self.rope_rank == 'updown':  # 目前仅chatglm使用
             cos_position = position_embeddings[:, 1::2].repeat(1,2)  # [seq_len, hdsz]
             sin_position = position_embeddings[:, ::2].repeat(1,2)  # [seq_len, hdsz]
         else:
-            raise ValueError('Args `rope_rank` only support `adjacent` and `adjacent` mode')
+            raise ValueError('Args `rope_rank` only support `adjacent` and `updown` mode')
         return cos_position, sin_position
     
     def forward(self, qw, position_ids=None, seq_dim=-2):
         # MultiHeadAttentionLayer中qw是[btz, n_heads, seq_len, head_size]
         # GlobalPointer中*转置*后qw是[btz, n_heads, seq_len, head_size]
         # EfficientGlobalPointer中qw是[btz, seq_len, head_size]
         if self.rope_rank == 'adjacent':
```

### Comparing `bert4torch-0.2.8/bert4torch/losses.py` & `bert4torch-0.2.9/bert4torch/losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             elif self.rank == 'updown':
                 half_btz = y_true.shape[0] // 2
                 y_pred1 = y_pred[:half_btz]
                 y_pred2 = y_pred[half_btz:]
         # y_pred是两个tensor
         else:
             y_pred1, y_pred2, y_true = args
-            loss_sup = self.loss_sup(y_pred1, y_true)
+            loss_sup = (self.loss_sup(y_pred1, y_true) + self.loss_sup(y_pred2, y_true)) / 2
 
         loss_rdrop1 = self.loss_rdrop(F.log_softmax(y_pred1, dim=-1), F.softmax(y_pred2, dim=-1))
         loss_rdrop2 = self.loss_rdrop(F.log_softmax(y_pred2, dim=-1), F.softmax(y_pred1, dim=-1))
         return loss_sup + torch.mean(loss_rdrop1 + loss_rdrop2) / 4 * self.alpha
 
 
 class UDALoss(nn.Module):
```

### Comparing `bert4torch-0.2.8/bert4torch/models.py` & `bert4torch-0.2.9/bert4torch/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 ''' 模型
     v0.2.2版本前Trainer是在bert4torch内部实现的，之后单独为Trainer做了一个包torch4keras
     v0.2.5版本开始，对抗训练模块不在complile中使用，而是用callback方式实现
 '''
 import torch
 from torch import nn, Tensor
 import torch.nn.functional as F
+from torch.utils.checkpoint import checkpoint
 import copy
 import json
 import re
 from bert4torch.layers import LayerNorm, BertEmbeddings, BertLayer, BlockIdentity, T5Layer, GatedAttentionUnit, XlnetLayer
 from bert4torch.layers import AdaptiveEmbedding, XlnetPositionsEncoding, ConvLayer
-from bert4torch.snippets import insert_arguments, delete_arguments, print_trainable_parameters, torch_div
+from bert4torch.snippets import insert_arguments, delete_arguments, print_trainable_parameters, torch_div, colorful
 from bert4torch.snippets import take_along_dim, create_position_ids_start_at_padding, DottableDict, get_parameter_device
 from bert4torch.activations import get_activation
 import warnings
 from torch4keras.model import *
-from torch.utils.checkpoint import checkpoint as grad_checkpoint
 from tqdm import tqdm
+import inspect
 
 
 class BERT_BASE(nn.Module):
     """模型基类
     """
     def __init__(
             self,
@@ -40,14 +41,15 @@
             keep_tokens=None,  # 要保留的词ID列表
             compound_tokens=None,  # 扩展Embedding
             residual_attention_scores=False,  # Attention矩阵加残差
             keep_hidden_layers=None, # 保留的hidden_layer层的id
             hierarchical_position=None,  # 是否层次分解位置编码
             gradient_checkpoint=False, # 是否使用gradient_checkpoint
             output_all_encoded_layers=False, # 是否返回所有layer的hidden_states
+            tie_emb_prj_weight=False,  # 是否绑定embedding和lm_head的权重
             **kwargs
     ):
         super(BERT_BASE, self).__init__()
         if keep_tokens is not None:
             vocab_size = len(keep_tokens)
         if compound_tokens is not None:
             vocab_size += len(compound_tokens)
@@ -73,14 +75,38 @@
         self.keep_hidden_layers = set(range(num_hidden_layers)) if keep_hidden_layers is None else set(keep_hidden_layers)
         self.hierarchical_position = hierarchical_position
         self.gradient_checkpoint = gradient_checkpoint
         self.quantized = False
         self.output_all_encoded_layers = output_all_encoded_layers
         self.skip_init = kwargs['skip_init']
         self.add_trainer = kwargs['add_trainer']
+        self.tie_emb_prj_weight = tie_emb_prj_weight
+
+    def tie_weights(self):
+        pass
+    
+    def gradient_checkpointing_enable(self):
+        self.gradient_checkpoint=True
+
+    def enable_input_require_grads(self):
+        """transformer移植来
+        Enables the gradients for the input embeddings. This is useful for fine-tuning adapter weights while keeping
+        the model weights fixed.
+        """
+
+        def make_inputs_require_grads(module, input, output):
+            output.requires_grad_(True)
+
+        self._require_grads_hook = self.get_input_embeddings().register_forward_hook(make_inputs_require_grads)
+
+    def disable_input_require_grads(self):
+        """transformer移植来
+        Removes the `_require_grads_hook`.
+        """
+        self._require_grads_hook.remove()
 
     def get_kw(self, *args, **kwargs):
         '''把self.属性设置到kwargs中, 方便传参'''
         for arg in args:
             kwargs[arg] = getattr(self, arg)
         return kwargs
 
@@ -117,16 +143,16 @@
         :return: List[torch.Tensor] or torch.Tensor, 模型输出，默认顺序为[last_hidden_state/all_encoded_layers, pooled_output(若有), mlm_scores(若有), nsp_scores(若有)]
         """
         self.eval()
         return self.forward(*inputs, **model_kwargs)
 
     def init_model_weights(self, module):
         """ 初始化权重 """
-        if self.skip_init == 'meta':
-            if isinstance(module, (nn.Linear, nn.Embedding)):
+        if self.skip_init is True:
+            if hasattr(module, 'weight') and module.weight.device == torch.device('meta'):
                 module.to_empty(device='cpu')
         elif isinstance(module, (nn.Linear, nn.Embedding)) and (module.weight.requires_grad):
             # bert参数初始化, tf版本在linear和Embedding层使用的是截断正太分布, pytorch没有实现该函数,
             # 此种初始化对于加载预训练模型后进行finetune没有任何影响，
             # cf https://github.com/pytorch/pytorch/pull/5617
             # 固定的相对位置编码如Sinusoidal无需初始化
             module.weight.data.normal_(mean=0.0, std=self.initializer_range)
@@ -211,17 +237,17 @@
                 model_params.remove(new_key)
             needed_keys.append(old_key)
         del file_state_dict
 
         # mismatch keys的处理
         if verbose != 0:
             for key in missing_keys:
-                print(f'[WARNING] {key} not found in pretrain models')
+                print(colorful('[WARNING]') + f' {key} not found in pretrain models')
             for key in model_params:
-                print(f'[WARNING] Parameter {key} not loaded from pretrain models')
+                print(colorful('[WARNING]') + f' Parameter {key} not loaded from pretrain models')
 
         # 将ckpt的权重load到模型结构中
         self.load_state_dict(state_dict_new, strict=False)
         del state_dict_new
         return missing_keys, needed_keys
 
     def load_weights_from_pytorch_checkpoints(self, checkpoints, mapping=None, verbose=1):
@@ -232,41 +258,48 @@
             all_missing_keys = []
             for checkpoint in tqdm(checkpoints, desc='Loading checkpoint shards'):
                 missing_keys, needed_keys = self.load_weights_from_pytorch_checkpoint(checkpoint, mapping=mapping, verbose=0)
                 all_missing_keys.extend(missing_keys)
             all_missing_set = set(all_missing_keys).difference(set(needed_keys))
             if verbose != 0:
                 for key in all_missing_set:
-                    print(f'[WARNING] {key} not found in pretrain models')
+                    print(colorful('[WARNING]') + f' {key} not found in pretrain models')
         else:
             raise ValueError('Args `checkpoint_path` only support `str` or `list(str)` format')
 
     def apply_embeddings(self, *inputs, **model_kwargs):
         raise NotImplementedError
 
     def apply_main_layers(self, *inputs, **model_kwargs):
         raise NotImplementedError
 
     def apply_final_layers(self, *inputs, **model_kwargs):
         raise NotImplementedError
     
     def apply_on_layer_begin(self, l_i, **model_kwargs):
         '''新增对layer block输入进行操作的函数'''
-        model_kwargs['past_key_value'] = model_kwargs.get('past_key_values', [None]*self.num_hidden_layers)[l_i]
-        model_kwargs['cross_past_key_value'] = model_kwargs.get('cross_past_key_values', [None]*self.num_hidden_layers)[l_i]
+        if ('past_key_values' not in model_kwargs) or (model_kwargs.get('past_key_values') is None):
+            model_kwargs['past_key_value'] = None
+        else:
+            model_kwargs['past_key_value'] = model_kwargs['past_key_values'][l_i]
+
+        if ('cross_past_key_values' not in model_kwargs) or (model_kwargs.get('cross_past_key_values') is None):
+            model_kwargs['cross_past_key_value'] = None
+        else:
+            model_kwargs['cross_past_key_value'] = model_kwargs['cross_past_key_values'][l_i]
         return model_kwargs
     
     def apply_on_layer_end(self, l_i, **model_kwargs):
         '''新增对layer block输出进行操作的函数, 目前仅在MixUp中使用'''
         if model_kwargs.get('past_key_value', None) is not None:
-            if 'past_key_values' not in model_kwargs:
+            if ('past_key_values' not in model_kwargs) or (model_kwargs.get('past_key_values') is None):
                 model_kwargs['past_key_values'] = [None]*self.num_hidden_layers
             model_kwargs['past_key_values'][l_i] = model_kwargs['past_key_value']
         if model_kwargs.get('cross_past_key_value', None) is not None:
-            if 'cross_past_key_values' not in model_kwargs:
+            if ('cross_past_key_values' not in model_kwargs) or (model_kwargs.get('cross_past_key_values') is None):
                 model_kwargs['cross_past_key_values'] = [None]*self.num_hidden_layers
             model_kwargs['cross_past_key_values'][l_i] = model_kwargs['cross_past_key_value']
         return model_kwargs
 
     def compute_attention_bias(self, inputs=None):
         """定义每一层的Attention Bias"""
         return self.attention_bias
@@ -283,28 +316,34 @@
         outputs = outputs[:]
         self.outputs = outputs
         if len(outputs) > 1:
             self.output = outputs
         else:
             self.output = outputs[0]
 
-    def quantize(self, bits: int, use_quantization_cache=True, empty_init=False, target_modules=None, **kwargs):
+    def quantize(self, quantization_method, **kwargs):
         '''量化'''
-        if bits == 0:
-            return
-
-        from .quantization import quantize
-
         if self.quantized:
             print("Already quantized.")
             return self
+        
+        # chatglm的量化方式
+        if quantization_method == 'cpm_kernels':
+            from .quantization import quantize_cpm_kernels
+            self = quantize_cpm_kernels(self, **kwargs)
+        # load_in_8bit, load_in_4bit
+        elif quantization_method in {'load_in_8bit', 'load_in_4bit'}:
+            from .quantization import quantize_load_in_kbit
+            load_in_8bit = True if quantization_method == 'load_in_8bit' else False
+            load_in_4bit = True if quantization_method == 'load_in_4bit' else False
+            self = quantize_load_in_kbit(self, load_in_8bit=load_in_8bit, load_in_4bit=load_in_4bit, **kwargs)
+        else:
+            raise ValueError('Please check args `quantization_method`')
 
         self.quantized = True
-        self.quantization_bit = bits
-        self = quantize(self, bits, empty_init=empty_init, use_quantization_cache=use_quantization_cache, target_modules=target_modules, **kwargs)
         return self
 
     def add_adapter(self, adapter_method='bottleneck', bottlenect_size=64):
         '''增加adapter层'''
         from bert4torch.layers import add_adapter
         self = add_adapter(self, adapter_method, bottlenect_size)
         self.print_trainable_parameters()
@@ -318,15 +357,15 @@
         self.peft_config = {adapter_name: peft_config}
         if isinstance(peft_config, peft.LoraConfig):
             model = peft.LoraModel(self, self.peft_config, adapter_name)
         elif isinstance(peft_config, peft.AdaLoraConfig):
             model = peft.AdaLoraModel(self, self.peft_config, adapter_name)
         
         # 返回的model无法使用torch4keras的trainer
-        self =  add_trainer(model) if self.add_trainer else model
+        self = add_trainer(model) if self.add_trainer else model
         self.print_trainable_parameters()
         return self
 
     def print_trainable_parameters(self):
         """打印可训练的参数量"""
         print_trainable_parameters(self)
     
@@ -439,20 +478,44 @@
             self.pooler_activation = None
 
         if self.with_mlm:
             self.mlmDense = nn.Linear(self.hidden_size, self.embedding_size)  # 允许hidden_size和embedding_size不同
             self.transform_act_fn = get_activation(self.hidden_act)
             self.mlmLayerNorm = LayerNorm(self.embedding_size, eps=1e-12, conditional_size=self.conditional_size)
             self.mlmDecoder = nn.Linear(self.embedding_size, self.vocab_size, bias=False)
-            if kwargs.get('tie_emb_prj_weight') is True:
-                self.mlmDecoder.weight = self.embeddings.word_embeddings.weight
+            self.tie_weights()
             self.mlmBias = nn.Parameter(torch.zeros(self.vocab_size))
             self.mlmDecoder.bias = self.mlmBias
         # 下述继承于BERT的有声明新的参数，在这里初始化不能统一初始化到
 
+    def tie_weights(self):
+        """权重的tie"""
+        if self.tie_emb_prj_weight is True:
+            self.mlmDecoder.weight = self.embeddings.word_embeddings.weight
+    
+    def get_input_embeddings(self):
+        """获取word_embeddings"""
+        return self.embeddings.word_embeddings
+    
+    def layer_forward(self, layer, model_kwargs, use_reentrant=False):
+        """transformer block的forward"""
+        if self.gradient_checkpoint and self.training:
+            if use_reentrant is True:
+                # TODO: 此种方式要求输入输入是list类型，目前实现了输入，输出的dict默认没有梯度
+                args = []
+                __args = inspect.getargspec(type(layer).forward)
+                arg_names, arg_defaults = __args[0][1:], __args[-1]
+                for i, arg_name in enumerate(arg_names):
+                    args.append(model_kwargs.get(arg_name, arg_defaults[i]))
+                return checkpoint(layer, *args)
+            else:
+                return checkpoint(layer, use_reentrant=use_reentrant, **model_kwargs)
+        else:
+            return layer(**model_kwargs)
+
     def apply_embeddings(self, *inputs, **model_kwargs):
         """BERT的embedding是token、position、segment三者embedding之和
 
         :param inputs: List[torch.Tensor], 默认顺序是[token_ids, segment_ids(若有), position_ids(若有), custom_attention_mask(若有), conditional_input(若有), additional_input(若有)]
         :return: List[torch.Tensor], [hidden_states, attention_mask, conditional_emb, ...]
         """
         assert isinstance(inputs, (tuple, list)), f'Inputs only support list,tuple format but passed {type(inputs)}'
@@ -555,15 +618,15 @@
         
         :param inputs: List[torch.Tensor], 默认顺序为[hidden_states, attention_mask, conditional_emb]
         :return: List[torch.Tensor], 默认顺序为[encoded_layers, conditional_emb]
         """
         encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.encoderLayer):
             model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
-            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
             model_kwargs.update(outputs)
             hidden_states = model_kwargs['hidden_states']
             model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 encoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
@@ -681,15 +744,15 @@
         顺序:Att --> Add --> LN --> FFN --> Add --> LN
         """
 
         encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i in range(self.num_hidden_layers):
             model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
             layer_module = self.encoderLayer[0]
-            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
             model_kwargs.update(outputs)
             hidden_states = model_kwargs['hidden_states']
             model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 encoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
@@ -982,15 +1045,15 @@
     def apply_main_layers(self, **model_kwargs):
         """DebertaV2：主要区别是第0层后，会通过卷积层
         """
 
         encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.encoderLayer):
             model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
-            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
             model_kwargs.update(outputs)
             # 第0层要经过卷积
             if l_i == 0 and self.conv is not None:
                 model_kwargs['hidden_states'] = self.conv(encoded_layers[0], model_kwargs['hidden_states'], model_kwargs['attention_mask'].squeeze(1).squeeze(1))
             model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
@@ -1083,42 +1146,45 @@
         outputs, model_kwargs = super().forward(*inputs, use_states=True, **model_kwargs)
         # return: [encoder_hidden_states, encoder_attention_mask]
         return ([outputs] if isinstance(outputs, torch.Tensor) else outputs) + [model_kwargs['attention_mask']]
 
 
 class Decoder(LM_Mask, BERT):
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
-    def __init__(self, *args, with_lm=True, tie_emb_prj_weight=False, logit_scale=True, **kwargs):
+    def __init__(self, *args, with_lm=True, logit_scale=True, **kwargs):
         kwargs['vocab_size'] = kwargs.get('tgt_vocab_size', kwargs['vocab_size'])
         kwargs['is_decoder'] = True  # 标记是decoder
         super().__init__(*args, **kwargs)
         self.decoderLayer = self.encoderLayer
         del self.encoderLayer
         self.with_lm = with_lm
 
         # 从hidden_states映射到logit
         if self.with_lm:
             self.final_dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
             # decoder底层的embedding和顶层的全连接共享
             # [True]: fudan_bart和uer_t5的t5, [False]: mt5和t5_pegasus
-            if tie_emb_prj_weight:
-                self.final_dense.weight = self.embeddings.word_embeddings.weight
+            self.tie_weights()
             if logit_scale:  # T5默认会有logit_scale, bart默认没有，所以bart要传入false
                 self.x_logit_scale = (self.hidden_size ** -0.5)
             else:
                 self.x_logit_scale = 1.
 
+    def tie_weights(self):
+        if self.tie_emb_prj_weight is True:
+            self.final_dense.weight = self.embeddings.word_embeddings.weight
+
     def apply_main_layers(self, **model_kwargs):
         """Dencoder主体是基于Self-Attention、Cross-Attention的模块；
         顺序：Att1 --> Add --> LN --> Att2 --> Add -->  LN --> FFN --> Add --> LN
         """
         decoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.decoderLayer):
             model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
-            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
             model_kwargs.update(outputs)
             hidden_states = model_kwargs['hidden_states']
             model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
 
             if self.output_all_encoded_layers:
                 decoded_layers.append(hidden_states)
         if not self.output_all_encoded_layers:
@@ -1553,19 +1619,24 @@
         kwargs.update({'p_bias': 'rotary', 'weight': True, 'bias': False, 'norm_mode': 'rmsnorm', 'is_decoder': True})
         super().__init__(*args, **kwargs)
         del self.embeddings.layerNorm
         layer = self.TransformerBlock(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
                                                     'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', **kwargs))
         self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
         self.LayerNormFinal = LayerNorm(self.hidden_size, eps=1e-12, conditional_size=self.conditional_size, norm_mode=kwargs['norm_mode'], bias=kwargs['bias'])
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False, device=kwargs['skip_init']) 
+        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False) 
         self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
         # 修改feedword
         for layer in self.encoderLayer:
             layer.feedForward = self.FeedForward(self.hidden_size, self.hidden_size*4, **kwargs)
+        self.tie_weights()
+
+    def tie_weights(self):
+        if self.tie_emb_prj_weight:
+            self.dense.weight = self.embeddings.word_embeddings.weight
 
     def apply_final_layers(self, **model_kwargs):
         hidden_state = super().apply_final_layers(**model_kwargs)
         logit = self.dense(self.LayerNormFinal([hidden_state]))
         return self.final_activation(logit)
 
     def load_variable(self, state_dict, name):
@@ -1603,45 +1674,50 @@
         
     class FeedForward(nn.Module):
         '''FeedForward和Bert的不一致，Bert只有两个全连接'''
         def __init__(self, dim: int, hidden_dim: int, multiple_of: int, **kwargs):
             super().__init__()
             hidden_dim = int(2 * hidden_dim / 3)
             hidden_dim = multiple_of * ((hidden_dim + multiple_of - 1) // multiple_of)
-            self.intermediateDense = nn.Linear(dim, hidden_dim, bias=False, device=kwargs['skip_init'])
-            self.outputDense = nn.Linear(hidden_dim, dim, bias=False, device=kwargs['skip_init'])
-            self.intermediateDense2 = nn.Linear(dim, hidden_dim, bias=False, device=kwargs['skip_init'])
+            self.intermediateDense = nn.Linear(dim, hidden_dim, bias=False)
+            self.outputDense = nn.Linear(hidden_dim, dim, bias=False)
+            self.intermediateDense2 = nn.Linear(dim, hidden_dim, bias=False)
 
         def forward(self, x):
             return self.outputDense(F.silu(self.intermediateDense(x)) * self.intermediateDense2(x))
 
 
 class GLM(LM_Mask, BERT):
-    '''GLM: https://github.com/THUDM/GLM
+    '''GLM: https://github.com/THUDM/GLM, ChatGLM-6B: https://github.com/THUDM/ChatGLM-6B
     Unilm设计，可定义为GLM(UniLM_MASK, BERT)但是要求传入segement_ids比较麻烦，这里继承LM_MASK并使用get_masks()重新构造attention_mask
     模型结构特点：
     1）rotary使用的updown+position_encoding_2d
     2）qkv合并成一个权重convert时不是concat在一起的
     3）attention_mask类似于Unilm，最后一个token仅能访问之前的，之前的tokens可以互相访问
     4）跳跃连接有权重设计
     '''
     @delete_arguments('with_pool', 'with_mlm', 'with_nsp')
     def __init__(self, *args, **kwargs):
         kwargs.update({'p_bias': 'rotary', 'weight': True, 'is_decoder': True})
         super().__init__(*args, **kwargs)
-        self.bos_token_id, self.mask_token_id, self.gmask_token_id = kwargs['bos_token_id'], kwargs['mask_token_id'], kwargs['gmask_token_id']
+        self.bos_token_id, self.mask_token_id, self.gmask_token_id = kwargs.get('bos_token_id'), kwargs.get('mask_token_id'), kwargs.get('gmask_token_id')
         self.position_encoding_2d = kwargs.get('position_encoding_2d', True)
         del self.embeddings.layerNorm
         layer = self.GLMBlock(**self.get_kw('hidden_size', 'num_attention_heads', 'dropout_rate', 'attention_probs_dropout_prob', 
                                             'intermediate_size', 'hidden_act', 'is_dropout', 'conditional_size', 'num_hidden_layers', **kwargs))
         self.encoderLayer = nn.ModuleList([copy.deepcopy(layer) if layer_id in self.keep_hidden_layers else BlockIdentity() for layer_id in range(self.num_hidden_layers)])
         self.LayerNormFinal = torch.nn.LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-12))
-        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False, device=kwargs['skip_init'])
+        self.dense = nn.Linear(self.hidden_size, self.vocab_size, bias=False)
         self.final_activation = get_activation(kwargs.get('final_activation', 'linear'))
+        self.tie_weights()
 
+    def tie_weights(self):
+        if self.tie_emb_prj_weight:
+            self.dense.weight = self.embeddings.word_embeddings.weight
+    
     def load_variable(self, state_dict, name, prefix='transformer'):
         """加载单个变量的函数, 这里的名称均为映射前的
         """
         variable = state_dict[name]
         if name in {f'{prefix}.embeddings.word_embeddings.weight', 'lm_head.weight'}:
             return self.load_embeddings(variable)
         else:
@@ -1710,24 +1786,24 @@
         device = position_ids.device
         seqs = token_ids.tolist()
         mask_positions = [seq.index(mask_token) for seq in seqs]
         context_lens = [seq.index(self.bos_token_id) for seq in seqs]  # bos_token_id是倒数第一位
         seq_len = token_ids.shape[1]
 
         # 1）generation阶段use_states=True且step>0的时候(用cache)
-        if model_kwargs.get('use_states', False) and (model_kwargs.get('step') > 0):
+        if model_kwargs.get('use_states', False) and (model_kwargs.get('past_key_values') is not None):
             if self.position_encoding_2d:  # [btz, 2, 1]
                 position_ids = torch.tensor([[mask_position, seq_len - context_len] for mask_position, context_len in
                                             zip(mask_positions, context_lens)], dtype=torch.long, device=device).unsqueeze(-1)
             else:  # [btz, 1]
                 position_ids = torch.tensor([mask_position for mask_position in mask_positions], dtype=torch.long, device=device).unsqueeze(-1)
             model_kwargs['position_ids'] = position_ids
         # 1）train阶段；2）generation阶段use_states=False；3）use_states=True且step=0的时候
         else:
-            prepad_lens = [(ts[:l]==3).sum().item() for l, ts in zip(context_lens, token_ids)]
+            prepad_lens = [(ts[:l]==self.pad_token_id).sum().item() for l, ts in zip(context_lens, token_ids)]
             model_kwargs['attention_mask'] = self.get_masks(model_kwargs['attention_mask'], context_lens, prepad_lens)
             model_kwargs['position_ids'] = self.get_position_ids(position_ids, seq_len, context_lens, mask_positions, prepad_lens, gmask=use_gmask)
         return model_kwargs
 
     def apply_embeddings(self, *inputs, **model_kwargs):
         model_kwargs = super().apply_embeddings(*inputs, **model_kwargs)
         model_kwargs = self.prepare_inputs(*inputs, **model_kwargs)
@@ -1760,14 +1836,54 @@
             hidden_states = x *alpha +  self.feedForward(x)
 
             if self.is_decoder:
                 model_kwargs['past_key_value'] = self_attn_output[-1]
             model_kwargs['hidden_states'] = hidden_states
             return model_kwargs
 
+        
+class GLM2(GLM):
+    """CHATGLM2-6B: https://github.com/THUDM/ChatGLM2-6B
+    主要修改：1）不使用Unilm式的mask
+             2) flash_attention
+             3) multi_query_attention
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.LayerNormFinal = LayerNorm(self.hidden_size, eps=kwargs.get('layer_norm_eps', 1e-5), norm_mode='rmsnorm', bias=False)
+        
+    def prepare_inputs(self, *inputs, **model_kwargs):
+        return model_kwargs
+    
+    class GLMBlock(BertLayer):
+        '''顺序：LN --> Att --> Add --> LN --> FFN --> Add'''
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.num_hidden_layers = kwargs['num_hidden_layers']
+            hidden_size, eps = kwargs['hidden_size'], kwargs.get('layer_norm_eps', 1e-5)
+            self.layerNorm1 = LayerNorm(hidden_size, eps=eps, norm_mode='rmsnorm', bias=False)
+            self.layerNorm2 = LayerNorm(hidden_size, eps=eps, norm_mode='rmsnorm', bias=False)
+            self.multiHeadAttention.o.register_parameter('bias', None)
+            self.feedForward.intermediateDense.register_parameter('bias', None)
+            self.feedForward.outputDense.register_parameter('bias', None)
+
+        def forward(self, hidden_states=None, attention_mask=None, past_key_value=None, **model_kwargs):
+            # 和bert区别有两点，一个是有alpha, 还有一个是跳跃链接用的是经过了layernorm后的
+            x = self.layerNorm1(hidden_states)
+            self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, **model_kwargs)
+            hidden_states = hidden_states + self.dropout1(self_attn_output[0])
+
+            x = self.layerNorm2(hidden_states)
+            hidden_states = hidden_states + self.dropout2(self.feedForward(x))
+
+            if self.is_decoder:
+                model_kwargs['past_key_value'] = self_attn_output[-1]
+            model_kwargs['hidden_states'] = hidden_states
+            return model_kwargs
+
 
 class Transformer_XL(BERT):
     '''构建transformer-xl模型, 已加载；
     项目: https://github.com/kimiyoung/transformer-xl；
     不同点:  
     1) 简化了原有的AdaptiveEmbedding(可选)和未使用ProjectedAdaptiveLogSoftmax, 直接输出last_hidden_state；
     2) mems修改了transformer中初始化为zero_tensor, 改为包含最后一层, 原项目初始化为empty_tensor；
@@ -1900,15 +2016,15 @@
 
     def apply_main_layers(self, **model_kwargs):
         encoded_layers = [model_kwargs['hidden_states']] # 添加embedding的输出
         for l_i, layer_module in enumerate(self.encoderLayer):
             mems_i = None if self.mems is None else self.mems[l_i]
             model_kwargs['mems_i'] = mems_i
             model_kwargs = self.apply_on_layer_begin(l_i, **model_kwargs)
-            outputs = grad_checkpoint(layer_module, **model_kwargs) if self.gradient_checkpoint else layer_module(**model_kwargs)
+            outputs = self.layer_forward(layer_module, model_kwargs)
             model_kwargs.update(outputs)
             hidden_states = model_kwargs['hidden_states']
             model_kwargs = self.apply_on_layer_end(l_i, **model_kwargs)
             encoded_layers.append(hidden_states)
         
         # 原实现中word_emb, pos_emb和core_out(hidden_states)使用同一个dropout
         hidden_states = self.dropout(hidden_states)
@@ -2016,15 +2132,22 @@
                             f'encoderLayer.{i}.feedForward.outputDense.bias': prefix_i + 'ff.layer_2.bias',
                             f'encoderLayer.{i}.layerNorm2.weight': prefix_i + 'ff.layer_norm.weight',
                             f'encoderLayer.{i}.layerNorm2.bias': prefix_i + 'ff.layer_norm.bias'
                             })
         return mapping
 
 
-def build_transformer_model(config_path=None, checkpoint_path=None, model='bert', application='encoder', **kwargs):
+def extend_with_base_model(InputModel):
+    """添加torch4keras的BaseModel"""
+    class BertBaseModel(InputModel, BERT_BASE, BaseModel):
+        pass
+    return BertBaseModel
+
+
+def build_transformer_model(config_path=None, checkpoint_path=None, model='bert', application='encoder', add_trainer=False, **kwargs):
     """根据配置文件构建模型，可选加载checkpoint权重
 
     :param config_path: str, 模型的config文件地址
     :param checkpoint_path: str/list[str], 模型文件地址, 默认值None表示不加载预训练模型
     :param model: str, 加载的模型结构, 这里Model也可以基于nn.Module自定义后传入, 默认为'bert'
     :param application: str, 模型应用, 支持encoder, lm和unilm格式, 默认为'encoder'
     :param segment_vocab_size: int, type_token_ids数量, 默认为2, 如不传入segment_ids则需设置为0
@@ -2055,16 +2178,16 @@
     configs.update(kwargs)
     if 'max_position' not in configs:
         configs['max_position'] = configs.get('max_position_embeddings', 512)
     if 'dropout_rate' not in configs:
         configs['dropout_rate'] = configs.get('hidden_dropout_prob')
     if 'segment_vocab_size' not in configs:
         configs['segment_vocab_size'] = configs.get('type_vocab_size', 2)
-    configs['skip_init'] = 'meta' if configs.get('skip_init') is True else 'cpu'
-    configs['add_trainer'] = configs.get('add_trainer', False)
+    configs['skip_init'] = configs.get('skip_init', False)
+    configs['add_trainer'] = add_trainer
 
     models = {
         'bert': BERT,
         'roberta': BERT,  
         'albert': ALBERT,
         'albert_unshared': ALBERT_Unshared,
         'nezha': NEZHA,
@@ -2080,14 +2203,17 @@
         'transformer': Transformer,
         'bart': BART,
         'gpt': GPT,
         'gpt2': GPT2,
         'gpt2_ml': GPT2_ML,
         'llama': LLaMA,
         'glm': GLM,
+        'chatglm': GLM,
+        'glm2': GLM2,
+        'chatglm2': GLM2,
         't5': T5,
         't5_encoder': T5_Encoder,
         't5_decoder': T5_Decoder,
         't5.1.0': T5,
         't5.1.0_encoder': T5_Encoder,
         't5.1.0_decoder': T5_Decoder,
         't5.1.1': T5,
@@ -2103,39 +2229,42 @@
     if isinstance(model, str):  # string表示使用自带的模型
         MODEL = models[model.lower()]
         if model.endswith('t5.1.1'):
             configs['version'] = model
     elif isinstance(model, type) and issubclass(model, BERT_BASE): # nn.Module表示使用自定义的模型：
         MODEL = model
     else:
-        raise ValueError('"model" args type should be string or nn.Module')
+        raise ValueError('Args `model` type should be string or BERT_BASE')
 
     # 使用 lm/unilm
     application = application.lower()
     if application in ['lm', 'unilm'] and model in ['electra', 't5', ]:
         raise ValueError(f'"{model}" model can not be used as "{application}" application.\n')
     if application == 'lm':
         MODEL = extend_with_language_model(MODEL)
     elif application == 'unilm':
         MODEL = extend_with_unified_language_model(MODEL)
 
     # 动态继承BaseModel
-    if configs['add_trainer']:
-        class MyModel(MODEL, BaseModel): 
-            pass
-        MODEL = MyModel
+    if add_trainer:
+        MODEL = extend_with_base_model(MODEL)
 
     # 生成网络结构
-    transformer = MODEL(**configs)
+    if configs['skip_init']:
+        from accelerate import init_empty_weights
+        with init_empty_weights():
+            transformer = MODEL(**configs)
+    else:
+        transformer = MODEL(**configs)
     transformer.apply(transformer.init_model_weights)  # 初始化权重
 
-    # 预训练模型是否已量化, 加载量化后的权重使用，如果是加载原权重再自行量化这里不需要甚至恶
-    if configs.get('quantization_bit') is not None:
-        bits = configs.pop('quantization_bit')
-        transformer = transformer.half().quantize(bits=bits, **configs)
+    # 预训练模型是否已量化, 加载量化后的权重使用，如果是加载原权重再自行量化这里不需要设置
+    if configs.get('quantization_method') is not None:
+        transformer = transformer.half().quantize(**configs)
 
     # 权重加载
     if checkpoint_path is not None:
         verbose = not configs.get('ignore_invalid_weights', False)
         transformer.load_weights_from_pytorch_checkpoints(checkpoint_path, verbose=verbose)
+    transformer.tie_weights()  # 权重tie
     transformer.configs = transformer.config = configs
-    return transformer
+    return transformer
```

### Comparing `bert4torch-0.2.8/bert4torch/optimizers.py` & `bert4torch-0.2.9/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.8/bert4torch/quantization.py` & `bert4torch-0.2.9/bert4torch/quantization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-''' 从chagglm-6b移植过来的的量化，方便以int8和int4进行推理
-    源链接：https://huggingface.co/THUDM/chatglm-6b/blob/main/quantization.py
+''' 量化模块
 '''
 from torch.nn import Linear, Embedding
 from torch.nn.parameter import Parameter
 import torch.nn.functional as F
 import bz2
 import torch
 import base64
 import ctypes
 from typing import List
 import re
 from tqdm import tqdm
 from functools import partial
-import logging
-logger = logging.getLogger(__name__)
+import inspect
+from bert4torch.snippets import info_level_prefix
 
 try:
     from cpm_kernels.kernels.base import LazyKernelCModule, KernelFunction, round_up
 
     class Kernel:
         def __init__(self, code: bytes, function_names: List[str]):
             self.code = code
@@ -37,15 +36,15 @@
             "int4WeightExtractionHalf",
             "int8WeightExtractionFloat",
             "int8WeightExtractionHalf",
         ],
     )
 except Exception as exception:
     kernels = None
-    logger.warning("Failed to load cpm_kernels:" + str(exception))
+    print(info_level_prefix("Failed to load cpm_kernels:" + str(exception)), 'e')
 
 
 class W8A16Linear(torch.autograd.Function):
     @staticmethod
     def forward(ctx, inp: torch.Tensor, quant_w: torch.Tensor, scale_w: torch.Tensor, weight_bit_width):
         ctx.inp_shape = inp.size()
         ctx.weight_bit_width = weight_bit_width
@@ -218,16 +217,19 @@
         output = F.embedding(
             input, original_weight, self.padding_idx, self.max_norm,
             self.norm_type, self.scale_grad_by_freq, self.sparse
         )
         return output
 
 
-def quantize(model, weight_bit_width, use_quantization_cache=False, empty_init=False, target_modules=None, **kwargs):
-    """Replace fp16 linear with quantized linear
+def quantize_cpm_kernels(model, quantization_bit, use_quantization_cache=False, empty_init=False, target_modules=None, **kwargs):
+    """从chagglm-6b移植过来的的量化，方便以int8和int4进行推理
+    源链接：https://huggingface.co/THUDM/chatglm-6b/blob/main/quantization.py
+    
+    Replace fp16 linear with quantized linear
     这里修改了hard code, 可以适配其他模型
     target_modules: str/list, 指定对某些层做量化
     """
     modules_trans = {}
     for name, module in model.named_modules():
         # target_modules=None, 表示对所有Linear层替换
         if (target_modules is None) and isinstance(module, Linear):
@@ -242,15 +244,15 @@
     
     # TODO: 暂时只支持cuda
     current_device = torch.cuda.current_device()
     dtype = torch.half
 
     QuantizedLinearWithPara = partial(
         QuantizedLinear,
-        weight_bit_width=weight_bit_width,
+        weight_bit_width=quantization_bit,
         bias=True,
         dtype=dtype,
         empty_init=empty_init
     )
         
     cache = dict()
     for name, module in tqdm(modules_trans.items(), desc='Quantize linear layers'):
@@ -271,7 +273,50 @@
         name_new = list(name)
         for iter_ in re.finditer('\.[0-9]+\.', name):
             iter_str = name[iter_.start():iter_.end()]
             name_new[iter_.start():iter_.end()] = [''] * (iter_.end()-iter_.start())
             name_new[iter_.start()] = '[' + iter_str[1:-1] + '].'
         exec('model.' + ''.join(name_new) + ' = module')
     return model
+
+
+def quantize_load_in_kbit(model, load_in_8bit=False, load_in_4bit=False, keep_in_fp32_modules=[], llm_int8_skip_modules=[], quantization_config=None, **kwargs):
+    '''transformer的load_in_8bit, 源自transformer源代码'''
+    from transformers.utils.bitsandbytes import replace_with_bnb_linear, set_module_quantized_tensor_to_device
+    from transformers.utils.quantization_config import BitsAndBytesConfig
+    if quantization_config is None:
+        quantization_config, kwargs = BitsAndBytesConfig.from_dict(
+            config_dict={"load_in_8bit": load_in_8bit, "load_in_4bit": load_in_4bit}, return_unused_kwargs=True, **kwargs
+        )
+    elif quantization_config is not None:
+        load_in_8bit = quantization_config.load_in_8bit
+        load_in_4bit = quantization_config.load_in_4bit
+        quantization_config_kwargs = {
+            k: v for k, v in kwargs.items() if k in inspect.signature(BitsAndBytesConfig).parameters
+        }
+
+        if len(quantization_config_kwargs) > 0:
+            raise ValueError(
+                "You can't pass `load_in_8bit` or any other `BitsAndBytesConfig` argument as a kwarg when passing "
+                "`quantization_config` argument at the same time."
+            )
+
+    load_in_8bit_skip_modules = quantization_config.llm_int8_skip_modules or []
+
+    # We keep some modules such as the lm_head in their original dtype for numerical stability reasons
+    modules_to_not_convert = load_in_8bit_skip_modules
+    if not isinstance(modules_to_not_convert, list):
+        modules_to_not_convert = [modules_to_not_convert]
+
+    modules_to_not_convert.extend(keep_in_fp32_modules)
+    modules_to_not_convert.extend(llm_int8_skip_modules)
+
+    state_dict = model.state_dict()
+    model = replace_with_bnb_linear(model, modules_to_not_convert=modules_to_not_convert, quantization_config=quantization_config)
+
+    for key, param in model.named_parameters():
+        if param.device == torch.device("meta"):
+            set_module_quantized_tensor_to_device(model, key, 'cpu', value=state_dict[key], fp16_statistics=None)
+
+    model.is_loaded_in_8bit = load_in_8bit
+    model.is_loaded_in_4bit = load_in_4bit
+    return model
```

### Comparing `bert4torch-0.2.8/bert4torch/snippets.py` & `bert4torch-0.2.9/bert4torch/snippets.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 
 import unicodedata
 import six
 import numpy as np
 import re
 import torch
 from torch.nn.utils.rnn import pad_sequence
-from torch import nn, Tensor
 import math
 import gc
 import json
 import random
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from torch4keras.snippets import *
 try:
     # torch4keras0.0.7增加了callbacks，这里为了兼容老的example，在snippets中import了
     # 建议使用方式: from bert4torch.callbacks import *
     from torch4keras.callbacks import *
 except:
     pass
@@ -508,51 +506,7 @@
 
 def create_position_ids_start_at_padding(input_ids, padding_idx, past_key_values_length=0, start_padding_idx=True):
     """生成padding_ids, 从padding_idx+1开始。忽略填充符号"""
     # The series of casts and type-conversions here are carefully balanced to both work with ONNX export and XLA.
     mask = input_ids.ne(padding_idx).int()
     incremental_indices = (torch.cumsum(mask, dim=1).type_as(mask) + past_key_values_length) * mask    
     return incremental_indices.long() + (padding_idx if start_padding_idx else 0)
-
-
-class DottableDict(dict):
-    '''支持点操作符的字典'''
-    def __init__(self, *args, **kwargs):
-        dict.__init__(self, *args, **kwargs)
-        self.__dict__ = self
-    def allowDotting(self, state=True):
-        if state:
-            self.__dict__ = self
-        else:
-            self.__dict__ = dict()
-
-
-def print_trainable_parameters(module):
-    """打印可训练的参数量"""
-    trainable_params = 0
-    all_param = 0
-    for _, param in module.named_parameters():
-        num_params = param.numel()
-        # if using DS Zero 3 and the weights are initialized empty
-        if num_params == 0 and hasattr(param, "ds_numel"):
-            num_params = param.ds_numel
-
-        all_param += num_params
-        if param.requires_grad:
-            trainable_params += num_params
-    print(f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}")
-
-
-def get_parameter_device(parameter):
-    '''获取device, 从transformers包迁移过来'''
-    try:
-        return next(parameter.parameters()).device
-    except StopIteration:
-        # For nn.DataParallel compatibility in PyTorch 1.5
-
-        def find_tensor_attributes(module: nn.Module) -> List[Tuple[str, Tensor]]:
-            tuples = [(k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)]
-            return tuples
-
-        gen = parameter._named_members(get_members_fn=find_tensor_attributes)
-        first_tuple = next(gen)
-        return first_tuple[1].device
```

### Comparing `bert4torch-0.2.8/bert4torch/tokenizers.py` & `bert4torch-0.2.9/bert4torch/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.8/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.2.9/bert4torch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.2.8
+Version: 0.2.9
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bert4torch
-
-**一款用pytorch来复现bert4keras的简洁训练框架**
+![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
+[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
 
 [Documentation](https://bert4torch.readthedocs.io) |
 [Torch4keras](https://github.com/Tongjilibo/torch4keras) |
 [Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 
 ## 1. 下载安装
 
@@ -37,15 +36,15 @@
 ```shell
 pip install git+https://github.com/Tongjilibo/bert4torch
 ```
 
 - **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
 - **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
 - **自行训练**：针对自己的数据，修改相应的数据处理代码块
-- **开发环境**：使用`torch==1.10`版本进行开发，如其他版本遇到不适配，欢迎反馈
+- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
 
 ## 2. 功能
 
 - **LLM模型**: 加载chatglm-6b和llama-7b进行推理和finetune
 - **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
 - [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
 - **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/README.md)
@@ -75,15 +74,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.2.8**：20230518 增加chatglm-6b/llama-7b预训练模型, 修改rope为不使用max_position，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax，更新fnlp的bart2.0。增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持(skykiseki用户); 修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax; 增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理; 增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
 - **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
@@ -97,14 +96,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
 | 0.2.3          | 0.0.2           |
@@ -112,14 +112,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
+- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
@@ -154,17 +155,19 @@
 - 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
 | bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
 | roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
 | deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
 | guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
 | xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
@@ -183,17 +186,19 @@
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
+|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
 | vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
 | Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
```

### Comparing `bert4torch-0.2.8/setup.py` & `bert4torch-0.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.2.8',
+    version='v0.2.9',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.0.7.post3'],
+    install_requires=['torch>1.6', 'torch4keras==0.0.8'],
     packages=find_packages()
 )
```

