# Comparing `tmp/textgen-0.2.7.tar.gz` & `tmp/textgen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.2.7.tar", last modified: Fri Jun  2 10:03:19 2023, max compression
+gzip compressed data, was "textgen-1.0.0.tar", last modified: Wed Jul  5 09:26:35 2023, max compression
```

## Comparing `textgen-0.2.7.tar` & `textgen-1.0.0.tar`

### file list

```diff
@@ -1,74 +1,70 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.800119 textgen-0.2.7/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-05-09 12:23:08.000000 textgen-0.2.7/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    48702 2023-06-02 10:03:19.800631 textgen-0.2.7/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    42917 2023-06-02 08:56:04.000000 textgen-0.2.7/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-06-02 10:03:19.801245 textgen-0.2.7/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1410 2023-06-02 10:03:03.000000 textgen-0.2.7/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.738898 textgen-0.2.7/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1484 2023-06-02 09:09:48.000000 textgen-0.2.7/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.746810 textgen-0.2.7/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.749637 textgen-0.2.7/textgen/bloom/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/bloom/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    27971 2023-05-31 14:18:45.000000 textgen-0.2.7/textgen/bloom/bloom_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5982 2023-05-14 03:36:28.000000 textgen-0.2.7/textgen/bloom/bloom_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.753431 textgen-0.2.7/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       79 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    28661 2023-05-31 14:18:45.000000 textgen-0.2.7/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6280 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/chatglm/chatglm_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     1265 2023-05-12 09:34:43.000000 textgen-0.2.7/textgen/chatglm/merge_peft_adapter.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.755559 textgen-0.2.7/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    17084 2023-06-02 09:16:52.000000 textgen-0.2.7/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.756762 textgen-0.2.7/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.759330 textgen-0.2.7/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    43533 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.764734 textgen-0.2.7/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      231 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10113 2023-06-01 03:08:56.000000 textgen-0.2.7/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.770915 textgen-0.2.7/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56955 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65717 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.776806 textgen-0.2.7/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    29558 2023-06-02 09:14:22.000000 textgen-0.2.7/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     9562 2023-06-02 09:16:52.000000 textgen-0.2.7/textgen/llama/llama_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    13250 2023-05-23 07:17:43.000000 textgen-0.2.7/textgen/llama/merge_peft_adapter.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.786664 textgen-0.2.7/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73253 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.794062 textgen-0.2.7/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50615 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50652 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.798695 textgen-0.2.7/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2023-05-09 12:23:08.000000 textgen-0.2.7/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-02 10:03:19.742148 textgen-0.2.7/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    48702 2023-06-02 10:03:19.000000 textgen-0.2.7/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1850 2023-06-02 10:03:19.000000 textgen-0.2.7/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-02 10:03:19.000000 textgen-0.2.7/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      160 2023-06-02 10:03:19.000000 textgen-0.2.7/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-06-02 10:03:19.000000 textgen-0.2.7/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.726122 textgen-1.0.0/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-05-09 12:23:08.000000 textgen-1.0.0/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-05 09:26:35.727118 textgen-1.0.0/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    44817 2023-07-04 04:37:00.000000 textgen-1.0.0/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-07-05 09:26:35.728308 textgen-1.0.0/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1394 2023-06-15 08:23:08.000000 textgen-1.0.0/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.630591 textgen-1.0.0/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1379 2023-06-16 09:50:52.000000 textgen-1.0.0/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.647338 textgen-1.0.0/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.653495 textgen-1.0.0/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       79 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    31716 2023-07-03 13:12:15.000000 textgen-1.0.0/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8514 2023-06-16 12:38:08.000000 textgen-1.0.0/textgen/chatglm/chatglm_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1265 2023-05-12 09:34:43.000000 textgen-1.0.0/textgen/chatglm/merge_peft_adapter.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.658100 textgen-1.0.0/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15117 2023-07-03 13:03:20.000000 textgen-1.0.0/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.660239 textgen-1.0.0/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.667556 textgen-1.0.0/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    43533 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.675423 textgen-1.0.0/textgen/gpt/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/gpt/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    29197 2023-07-03 13:11:09.000000 textgen-1.0.0/textgen/gpt/gpt_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7407 2023-06-16 12:38:08.000000 textgen-1.0.0/textgen/gpt/gpt_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13145 2023-06-19 08:05:18.000000 textgen-1.0.0/textgen/gpt/merge_peft_adapter.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.681933 textgen-1.0.0/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      231 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10113 2023-06-01 03:08:56.000000 textgen-1.0.0/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.689188 textgen-1.0.0/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56955 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65717 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.704430 textgen-1.0.0/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73253 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.718227 textgen-1.0.0/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50615 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50652 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.723766 textgen-1.0.0/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.637750 textgen-1.0.0/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1754 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      144 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.2.7/LICENSE` & `textgen-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/PKG-INFO` & `textgen-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.7
+Version: 1.0.0
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
-Description: <div align="center">
+Description: [**🇨🇳中文**](https://github.com/shibing624/textgen/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/textgen/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+        
+        <div align="center">
           <a href="https://github.com/shibing624/textgen">
             <img src="https://github.com/shibing624/textgen/blob/main/docs/logo.svg" alt="Logo">
           </a>
         </div>
         
         -----------------
         
@@ -23,14 +25,20 @@
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         ## 📖 Introduction
         
         **TextGen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
+        ## 🔥 News
+        [2023/06/15] v1.0.0版本: 新增ChatGLM/LLaMA/Bloom模型的多轮对话微调训练，并发布医疗问诊LoRA模型[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)。详见[Release-v1.0.0](https://github.com/shibing624/MedicalGPT/releases/tag/1.0.0)
+        
+        [2023/06/02] v0.2.7版本: 新增ChatGLM/LLaMA/Bloom模型的SFT微调训练，并发布适用于通用对话和中文纠错的LoRA模型。详见[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
+        
+        
         ## 😊 Feature
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
         - [BLOOM](textgen/bloom)：本项目基于PyTorch实现了BLOOM模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
         - [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
@@ -40,30 +48,29 @@
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
         
-        | Model                                                                                                     | Arch       | Introduce                                                                                                                                                                | Training                                                                                                                                     | Inference                                                                                                             | 
+        | Model                                                                                                     | Arch       | Introduction                                                                                                                                                                | Train Script                                                                                                                                 | Predict Script                                                                                                        | 
         |:----------------------------------------------------------------------------------------------------------|:-----------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-        | [shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)             | T5         | 中文NLP多任务Prompt模型                                                                                                                                                         | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
         | [shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)                     | T5         | fine-tuned中文对联后的模型                                                                                                                                                       | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-        | [shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)                 | SongNet    | SongNet预训练模型                                                                                                                                                             | -                                                                                                                                            | -                                                                                                                     |
         | [shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)   | SongNet    | fine-tuned宋词后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-        | [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        | [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
         | [shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)             | ChatGLM-6B | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                        | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
         | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)         | ChatGLM-6B | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                           | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
         | [shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)           | LLaMA-13B  | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                            | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
-        | [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
-        | [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+        | [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+        | [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+        | [shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)     | LLaMA-13B  | 在240万条中英文医疗数据集[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)上微调了一版Ziya-LLaMA-13B模型，医疗问答效果有提升，发布微调后的LoRA权重                                      | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
         
         ### Evaluation
         
-        | Model                                                                                                                                       | Arch       | Introduce                                                                                                                                                                                                                                                                                     | Score    |
+        | Model                                                                                                                                       | Arch       | Introduction                                                                                                                                                                                                                                                                                     | Score    |
         |:--------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------|
         | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         | LLaMA-7B   | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 4.92     |
         | [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       | LLaMA-13B  | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 7.05     |
         | [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                                                                                                                                                                                                 | 7.16     |
         | [ChatGLM-6B-v1.1](https://huggingface.co/THUDM/chatglm-6b)                                                                                  | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`v1.1英文优化版模型评估测试集得分                                                                                                                                                                                                                                                      | **7.18** |
         | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           | ChatGLM-6B | 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                                                                                                                                                                                                     | 7.03     |
         | [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                | LLaMA-13B  | 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                                                                                                                                                                                               | 4.13     |  
@@ -116,29 +123,29 @@
         
         ## ▶️ Usage
         
         ### ChatGLM-6B 模型
         
         #### 使用 ChatGLM-6B 微调后的模型
         
-        example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+        example: [examples/chatglm/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/inference_demo.py)
         
         ```python
         from textgen import ChatGlmModel
         
         model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
         PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
         
         #### 训练 ChatGLM-6B 微调模型
         
-        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[examples/data/json_files/belle_10.json](https://github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
         2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
         3. 支持多卡训练，支持混合精度训练
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
         单卡训练：
         ```shell
@@ -170,31 +177,31 @@
         --output_dir：指定保存全量模型权重的目录，默认为./merged
         ```
         
         ### LLaMA 模型
         
         #### 使用 LLaMA 微调后的模型
         
-        example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+        example: [examples/gpt/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt/inference_demo.py)
         
         <details>
         <summary>show code example and result</summary>
         
         ```python
         import sys
         
         sys.path.append('../..')
-        from textgen import LlamaModel
+        from textgen import GptModel
         
         
         def generate_prompt(instruction):
           return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
         
         
-        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
+        model = GptModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
         </details>
         
@@ -209,15 +216,15 @@
         #### 基于微调(LoRA)模型继续训练
         如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
         
         单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
         
         执行以下命令：
         ```shell
-        python -m textgen/llama/merge_peft_adapter.py \
+        python -m textgen/gpt/merge_peft_adapter.py \
             --base_model_name_or_path path_to_original_base_model_dir \
             --peft_model_path path_to_chinese_llama_or_alpaca_lora \
             --output_type [pth|huggingface]
             --output_dir path_to_output_dir 
         ```
         参数说明：
         ```
@@ -225,20 +232,15 @@
         --peft_model_path：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
         --output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为huggingface
         --output_dir：指定保存全量模型权重的目录，默认为./merged
         --offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
         ```
         
         #### 训练领域模型
-        
-        | Notebook     | Description |    |
-        |:----------|:------------|------:|
-        | [training_medical_model.ipynb](https://github.com/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb)  | 训练医疗大模型     |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-        
-        # Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning]单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
+        Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning)单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
         
         ### BLOOM 模型
         
         #### 训练 BLOOM 微调模型
         
         example: [examples/bloom/training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/examples/bloom/training_bloom_demo.py)
         
@@ -571,28 +573,42 @@
         
         前10句是真实用户评论，后10句是生成的。
         
         </details>
         
         ## 📚 Dataset 
         
-        1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-        2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
-        4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
-        6. 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+        #### SFT datasets
+        - 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+        - 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+        - 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        - 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        - 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        - 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+        - 5万条英文ChatGPT多轮对话数据集：[RyokoAI/ShareGPT52K](https://huggingface.co/datasets/RyokoAI/ShareGPT52K)
+        - 80万条中文ChatGPT多轮对话数据集：[BelleGroup/multiturn_chat_0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+        - 116万条中文ChatGPT多轮对话数据集：[fnlp/moss-002-sft-data](https://huggingface.co/datasets/fnlp/moss-002-sft-data)
+        
+        #### Reward Model datasets
+        - 原版的oasst1数据集：[OpenAssistant/oasst1](https://huggingface.co/datasets/OpenAssistant/oasst1)
+        - 2万条多语言oasst1的reward数据集：[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/tasksource/oasst1_pairwise_rlhf_reward)
+        - 11万条英文hh-rlhf的reward数据集：[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/Dahoas/full-hh-rlhf)
+        - 9万条英文reward数据集(来自Anthropic's Helpful Harmless dataset)：[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/static-hh)
+        - 7万条英文reward数据集（来源同上）：[Dahoas/rm-static](https://huggingface.co/datasets/Dahoas/rm-static)
+        - 7万条繁体中文的reward数据集（翻译自rm-static）[liswei/rm-static-m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh)
+        - 7万条英文Reward数据集：[yitingxie/rlhf-reward-datasets](https://huggingface.co/datasets/yitingxie/rlhf-reward-datasets)
+        - 3千条中文知乎问答偏好数据集：[liyucheng/zhihu_rlhf_3k](https://huggingface.co/datasets/liyucheng/zhihu_rlhf_3k)
         
         ## ✅ Todo
         
-        1. [ ] 新增多轮对话数据微调方法
-        2. [ ] add reward model finetuning
-        3. [ ] add rl finetuning
-        4. [ ] add medical reward dataset
-        5. [ ] add llama in4 training
+        1. [x] add multiple rounds of dialogue data fine-tuning method
+        2. [x] add reward model finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+        3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+        4. [x] add medical reward dataset
+        5. [x] add llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
         6. [ ] add all training and predict demo in colab
         
         ## ☎️ Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
@@ -603,23 +619,26 @@
         ## 😇 Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
-          author={Xu Ming},
+          author={Ming Xu},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
         ## 🤗 License
+        This repository is licensed under [The Apache License 2.0](LICENSE).
+        
+        Please follow the [Model Card](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) to use the LLaMA model.
         
-        授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
+        Please follow the [RAIL License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM & BLOOMZ model.
         
         ## 😍 Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
```

#### html2text {}

```diff
@@ -1,23 +1,35 @@
-Metadata-Version: 2.1 Name: textgen Version: 0.2.7 Summary: Text Generation
+Metadata-Version: 2.1 Name: textgen Version: 1.0.0 Summary: Text Generation
 Model Home-page: https://github.com/shibing624/textgen Author: XuMing Author-
-email: xuming624@qq.com License: Apache 2.0 Description:
+email: xuming624@qq.com License: Apache 2.0 Description: [**ð¨ð³ä¸­æ**]
+(https://github.com/shibing624/textgen/blob/main/README.md) | [**ðEnglish**]
+(https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**ðææ¡£/
+Docs**](https://github.com/shibing624/textgen/wiki) | [**ð¤æ¨¡å/Models**]
+(https://huggingface.co/shibing624)
                                     [Logo]
 ----------------- # TextGen: Implementation of Text Generation models [![PyPI
 version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/
 textgen) [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/
 project/textgen) [![Contributions welcome](https://img.shields.io/badge/
 contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![License Apache 2.0]
 (https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE) [!
 [python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)]
 (requirements.txt) [![GitHub issues](https://img.shields.io/github/issues/
 shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) ## ð Introduction
 **TextGen**å®ç°äºå¤ç§ææ¬çææ¨¡åï¼åæ¬ï¼LLaMAãChatGLMãUDAãGPT2ãSeq2SeqãBARTãT5ãSongNetç­æ¨¡åï¼å¼ç®±å³ç¨ã
+## ð¥ News [2023/06/15] v1.0.0çæ¬: æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçå¤è½®å¯¹è¯å¾®è°è®­ç»ï¼å¹¶åå¸å»çé®è¯LoRAæ¨¡å
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora)ãè¯¦è§[Release-v1.0.0](https://github.com/
+shibing624/MedicalGPT/releases/tag/1.0.0) [2023/06/02] v0.2.7çæ¬:
+æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçSFTå¾®è°è®­ç»ï¼å¹¶åå¸éç¨äºéç¨å¯¹è¯åä¸­æçº éçLoRAæ¨¡åãè¯¦è§
+[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
 ## ð Feature - [ChatGLM](textgen/
 chatglm)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºChatGLM-
 6Bæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¥å­çº éãå¯¹è¯ç­ææ¬çæä»»å¡
 - [LLaMA](textgen/
 llama)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºLLaMAæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
 - [BLOOM](textgen/
 bloom)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºBLOOMæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
@@ -34,37 +46,30 @@
 songnet_model.py)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºSongNetæ¨¡åè®­ç»åé¢æµï¼å¯ä»¥ç¨äºè§èæ ¼å¼çè¯è¯ãæ­è¯ç­ææ¬çæä»»å¡
 - [TGLS](textgen/unsup_generation)ï¼æ¬é¡¹ç®å®ç°äº[TGLS](https://
 www.jiqizhixin.com/articles/2020-08-11-
 5)æ çç£ç¸ä¼¼ææ¬çææ¨¡åï¼æ¯ä¸ç§âåæç´¢åå­¦ä¹ âçææ¬çææ¹æ³ï¼éè¿åå¤è¿­ä»£å­¦ä¹ åééï¼æç»æ¨¡åè½çæç±»ä¼¼åééçé«è´¨éç¸ä¼¼ææ¬
 ### Release Models
 releaseåºäº`textgen`è®­ç»çä¸­ææ¨¡åï¼æ¨¡åå·²ç»releaseå°HuggingFace
 modelsï¼æå®æ¨¡ååç§°`textgen`ä¼èªå¨ä¸è½½æ¨¡åï¼å¯ç´æ¥ä½¿ç¨ã
-| Model | Arch | Introduce | Training | Inference | |:-------------------------
+| Model | Arch | Introduction | Train Script | Predict Script | |:-------------
 -------------------------------------------------------------------------------
---|:-----------|:--------------------------------------------------------------
+--------------|:-----------|:--------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------|:-------------------------------------------------
+----------------------------------------|:-------------------------------------
 -------------------------------------------------------------------------------
--------------|:----------------------------------------------------------------
-------------------------------------------------------| | [shibing624/prompt-
-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese) | T5
-| ä¸­æNLPå¤ä»»å¡Promptæ¨¡å | [prompt-t5-base-chinese.md](https://
-github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md) |
-[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_prompt_demo.py) | | [shibing624/t5-chinese-couplet](https://huggingface.co/
-shibing624/t5-chinese-couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å |
-[å¯¹èçææ¨¡åè°ç ](https://github.com/shibing624/textgen/blob/main/
-docs/
+-------------------------|:----------------------------------------------------
+------------------------------------------------------------------| |
+[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-
+couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å | [å¯¹èçææ¨¡åè°ç ]
+(https://github.com/shibing624/textgen/blob/main/docs/
 %E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) |
 [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_couplet_demo.py) | | [shibing624/songnet-base-chinese](https://
-huggingface.co/shibing624/songnet-base-chinese) | SongNet |
-SongNeté¢è®­ç»æ¨¡å | - | - | | [shibing624/songnet-base-chinese-songci]
-(https://huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet |
-fine-tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
+t5_couplet_demo.py) | | [shibing624/songnet-base-chinese-songci](https://
+huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet | fine-
+tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
 songnet_songci_demo.py) | | [shibing624/songnet-base-chinese-couplet](https://
 huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet | fine-
 tunedå¯¹èåçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
@@ -103,31 +108,39 @@
 [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/
 chinese-alpaca-plus-13b-hf) | LLaMA-13B | [ä¸­æLLaMA-Plus, Alpaca-Plus
 13Bçæ¬](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/
 v3.1)ï¼å¨LLaMA-
 13Bä¸æ©åäºä¸­æè¯è¡¨å¹¶ç»§ç»­é¢è®­ç»120Gææ¬ï¼éç¨é¢åï¼ï¼å¨4.3Mæä»¤æ°æ®éä¸å¾®è°åå¾å°çä¸­æAlpaca-
 plusæ¨¡å | [training script](https://github.com/shibing624/textgen/blob/main/
 examples/llama/training_llama_demo.py) | [predict script](https://github.com/
-shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | ###
-Evaluation | Model | Arch | Introduce | Score | |:-----------------------------
+shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | |
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora) | LLaMA-13B | å¨240ä¸æ¡ä¸­è±æå»çæ°æ®é
+[shibing624/medical](https://huggingface.co/datasets/shibing624/
+medical)ä¸å¾®è°äºä¸çZiya-LLaMA-
+13Bæ¨¡åï¼å»çé®ç­ææææåï¼åå¸å¾®è°åçLoRAæé |
+[training script](https://github.com/shibing624/textgen/blob/main/examples/
+llama/training_llama_demo.py) | [predict script](https://github.com/shibing624/
+textgen/blob/main/examples/llama/training_llama_demo.py) | ### Evaluation |
+Model | Arch | Introduction | Score | |:---------------------------------------
 -------------------------------------------------------------------------------
---------------------------------|:-----------|:--------------------------------
+----------------------|:-----------|:------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://
-huggingface.co/ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/
+-------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/
+ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/Chinese-LLaMA-
+Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/
+README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca](https://
+huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B | å¤ç¨[ymcui/
 Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/
-examples/README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca]
-(https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B |
-å¤ç¨[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-
-Alpaca/blob/main/examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-
-6B](https://huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/
-chatglm-6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://
+examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-6B](https://
 huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
+6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://huggingface.co/
+THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
 6b`v1.1è±æä¼åçæ¨¡åè¯ä¼°æµè¯éå¾å | **7.18** | | [shibing624/
 chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-
 zh-lora) | ChatGLM-6B | åºäº`THUDM/chatglm-6b`å è½½`shibing624/chatglm-6b-
 belle-zh-lora`LoRAæ¨¡ååè¯ä¼°æµè¯éå¾å | 7.03 | | [facat/alpaca-lora-
 cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b) | LLaMA-13B |
 åºäº`decapoda-research/llama-13b-hf`å è½½`facat/alpaca-lora-cn-
 13b`LoRAæ¨¡ååè¯ä¼°æµè¯éå¹¶æ æ³¨å¾å | 4.13 | | [Chinese-Vicuna/
@@ -175,26 +188,27 @@
 examples/gradio_demo.py ``` model trained by [examples/t5/
 T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/
 main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb) ## ð¾ Install ```shell
 pip install -U textgen ``` or install develop version: ```shell pip install
 torch # conda install pytorch git clone https://github.com/shibing624/
 textgen.git cd textgen python setup.py install ``` ## â¶ï¸ Usage ### ChatGLM-
 6B æ¨¡å #### ä½¿ç¨ ChatGLM-6B å¾®è°åçæ¨¡å example: [examples/chatglm/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-chatglm/predict_demo.py) ```python from textgen import ChatGlmModel model =
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+chatglm/inference_demo.py) ```python from textgen import ChatGlmModel model =
 ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-
 csc-zh-lora") r = model.predict(
 ["å¯¹ä¸é¢ä¸­ææ¼åçº éï¼\nå°åéåå è¯¥ä¸ºèäººè®©åã\nç­ï¼"])
 print(r) # ['å°åéååºè¯¥ä¸ºèäººè®©åº§ã\néè¯¯å­ï¼å ï¼å'] ```
 PSï¼ç±äºä½¿ç¨äºå¼åä¸­çpeftåºï¼å¯è½ç±äºçæ¬æ´æ°ï¼å¯¼è´LoRAæ¨¡åå è½½å¤±è´¥ï¼å»ºè®®ä½¿ç¨ä¸é¢çè®­ç»æ¹æ³ï¼èªå·±è®­ç»LoRAæ¨¡åã
 #### è®­ç» ChatGLM-6B å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
-data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
-datasets/shibing624/alpaca-zh) 2.
+data/zh_csc_test.tsv)æè[examples/data/json_files/belle_10.json](https://
+github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
+2.
 æ¯æAdaLoRAãLoRAãP_TuningãPrefix_Tuningç­é¨ååæ°å¾®è°æ¹æ³ï¼ä¹æ¯æå¨åå¾®è°
 3. æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç» example: [examples/chatglm/
 training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/chatglm/training_chatglm_demo.py) åå¡è®­ç»ï¼ ```shell cd
 examples/chatglm CUDA_VISIBLE_DEVICES=0 python training_chatglm_demo.py --
 do_train --do_predict --num_epochs 1 --output_dir outputs_chatglm ```
 å¤å¡è®­ç»ï¼ ```shell cd examples/chatglm CUDA_VISIBLE_DEVICES=0,1 torchrun
@@ -205,23 +219,23 @@
 m textgen/chatglm/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path path_to_peft_model_dir \ --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --
 peft_model_pathï¼å­æ¾PEFTæ ¼å¼çå¾®è°æ¨¡åæéåéç½®æä»¶çç®å½
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged ```
-### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/llama/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-llama/predict_demo.py)  show code example and result ```python import sys
-sys.path.append('../..') from textgen import LlamaModel def generate_prompt
+### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/gpt/
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+gpt/inference_demo.py)  show code example and result ```python import sys
+sys.path.append('../..') from textgen import GptModel def generate_prompt
 (instruction): return f"""Below is an instruction that describes a task. Write
 a response that appropriately completes the request.\n\n### Instruction:
-{instruction}\n\n### Response:""" model = LlamaModel("llama", "decapoda-
-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
-predict_sentence = generate_prompt
+{instruction}\n\n### Response:""" model = GptModel("llama", "decapoda-research/
+llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b") predict_sentence =
+generate_prompt
 ("é®ï¼ç¨ä¸å¥è¯æè¿°å°çä¸ºä»ä¹æ¯ç¬ä¸æ äºçã\nç­ï¼") r =
 model.predict([predict_sentence]) print(r) #
 ['å°çæ¯å¯ä¸ä¸é¢æ¥æçå½çè¡æã'] ```  #### è®­ç» LLaMA
 å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
 data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
@@ -231,34 +245,29 @@
 æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç»ï¼ä½¿ç¨æ¹æ³åä¸ï¼ChatGLMå¤å¡è®­ç»ï¼
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/
 textgen/blob/main/examples/llama/training_llama_demo.py) #### åºäºå¾®è°
 (LoRA)æ¨¡åç»§ç»­è®­ç»
 å¦æéè¦åºäºLoraæ¨¡åç»§ç»­è®­ç»ï¼å¯ä»¥ä½¿ç¨ä¸é¢çèæ¬åå¹¶æ¨¡åä¸ºæ°çbase
 modelï¼åå¾®è°è®­ç»å³å¯ã åLoRAæéåå¹¶ï¼éç¨äº Chinese-LLaMA,
 Chinese-LLaMA-Plus, Chinese-Alpacaï¼ æ§è¡ä»¥ä¸å½ä»¤ï¼ ```shell python -
-m textgen/llama/merge_peft_adapter.py \ --base_model_name_or_path
+m textgen/gpt/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path
 path_to_chinese_llama_or_alpaca_lora \ --output_type [pth|huggingface] --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --peft_model_pathï¼ä¸­æLLaMA/Alpaca
 LoRAè§£ååæä»¶æå¨ç®å½ï¼ä¹å¯ä½¿ç¨HFä¸çLoraæ¨¡ååç§°ï¼å¦`ziqingyang/
 chinese-alpaca-lora-7b`ä¼èªå¨ä¸è½½å¯¹åºæ¨¡å --output_type:
 æå®è¾åºæ ¼å¼ï¼å¯ä¸ºpthæhuggingfaceãè¥ä¸æå®ï¼é»è®¤ä¸ºhuggingface
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged --
 offload_dirï¼å¯éï¼ï¼å¯¹äºä½åå­ç¨æ·éè¦æå®ä¸ä¸ªoffloadç¼å­è·¯å¾
-``` #### è®­ç»é¢åæ¨¡å | Notebook | Description | | |:----------|:--------
-----|------:| | [training_medical_model.ipynb](https://github.com/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-è®­ç»å»çå¤§æ¨¡å |[![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) | # Note:
+``` #### è®­ç»é¢åæ¨¡å Note:
 ä¸ºäºå¨é¢çä»ç»è®­ç»å»çå¤§æ¨¡åçè¿ç¨ï¼æ4é¶æ®µè®­ç»æ¹æ³
-[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
-Learning]åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
+(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
+Learning)åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
 github.com/shibing624/MedicalGPT)ï¼è¯·ç§»æ­¥è¯¥repoæ¥çè®­ç»æ¹æ³ã ###
 BLOOM æ¨¡å #### è®­ç» BLOOM å¾®è°æ¨¡å example: [examples/bloom/
 training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/bloom/training_bloom_demo.py) ### ConvSeq2Seq æ¨¡å
 è®­ç»å¹¶é¢æµConvSeq2Seqæ¨¡åï¼ example: [examples/seq2sesq/
 training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/
 main/examples/seq2seq/training_convseq2seq_model_demo.py)  show code example
@@ -436,42 +445,68 @@
 ä¸æå¼åè£éé¢çç²¾åååå¥½ï¼ç¨äºè¡¥æ°´è¡¥æ°´ææä¸éï¼ç©æµéå¸¸å¿«ã
 ç®è¤å¾åæ»ðæ¯ä¸å»éåº¦å¿«ä¸å¤©å°±å°äºã
 åä¸¤å¤©ç®è¤å¹²ç¥è¿ç»­æ·äºä¸¤ä¸ªæä¸æè§è¿ä¸éðè¡¥æ°´ææææ¾ï¼å¯æ³èç¥ç²¾åæ¶²åå¤åè¶³ðæ·ä¸ä»¥åååçå¾èæã
 è¡¥æ°´ææä¸è¬å§ï½ä½æ¯æç¨çé©å½èåæ¥çé¢èçº¸ä¸ç®èï¼å¸æå¥½ç¨ä¼åè´­çï¼æ·ä¸è¸æè§æ¯è¾æ¸ç½ï½ä»·æ ¼è¿ä¸ä¾¿å®ã
 å¸æå¥½ç¨ï¼é¢èç¨è¿äºå¾å¥½ç¨ï¼ç®è¤æ°´å«©åæ»ç½çï¼è¡¥æ°´ä¸éï¼ä»·æ ¼ä¹åéã
 å°±æ¯ç²¾åæ¶²å¤ªå°äºï¼ä¿æ¹¿ææä¸éã
 é¢èçè¡¥æ°´ææéå¸¸å¥½ï¼ä¿æ¹¿ææç¡®å®å¾èµï¼è¿ä¸ªé¢èç¸å¯¹äºè¶åèç½åç¾ç½çé£ä¸¤æ¬¾çé¢èçº¸è¦åä¸äºï¼ççä»·æ ¼åéã
-``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset 1.
-50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_0.5M_CN](https://
-huggingface.co/datasets/BelleGroup/train_0.5M_CN) 2.
+``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset
+#### SFT datasets - 50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/
+train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN) -
 100ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_1M_CN](https://
-huggingface.co/datasets/BelleGroup/train_1M_CN) 3.
+huggingface.co/datasets/BelleGroup/train_1M_CN) -
 5ä¸æ¡è±æChatGPTæä»¤Alpacaæ°æ®éï¼[50k English Stanford Alpaca
-dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) 4.
+dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) -
 2ä¸æ¡ä¸­æChatGPTæä»¤Alpacaæ°æ®éï¼[shibing624/alpaca-zh](https://
-huggingface.co/datasets/shibing624/alpaca-zh) 5.
+huggingface.co/datasets/shibing624/alpaca-zh) -
 69ä¸æ¡ä¸­ææä»¤Guanacoæ°æ®é(Belle50ä¸æ¡+Guanaco19ä¸æ¡)ï¼[Chinese-
 Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-
-Vicuna/guanaco_belle_merge_v1.0) 6. 240ä¸æ¡ä¸­æå»çæ°æ®é
+Vicuna/guanaco_belle_merge_v1.0) - 240ä¸æ¡ä¸­æå»çæ°æ®é
 (åæ¬é¢è®­ç»æ°æ®åæä»¤å¾®è°æ°æ®é)ï¼[shibing624/medical](https://
-huggingface.co/datasets/shibing624/medical) ## â Todo 1. [ ]
-æ°å¢å¤è½®å¯¹è¯æ°æ®å¾®è°æ¹æ³ 2. [ ] add reward model finetuning 3. [ ]
-add rl finetuning 4. [ ] add medical reward dataset 5. [ ] add llama in4
-training 6. [ ] add all training and predict demo in colab ## âï¸ Contact -
-Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/github/issues/
-shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) -
-é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
+huggingface.co/datasets/shibing624/medical) -
+5ä¸æ¡è±æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[RyokoAI/ShareGPT52K](https://
+huggingface.co/datasets/RyokoAI/ShareGPT52K) -
+80ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[BelleGroup/multiturn_chat_0.8M]
+(https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M) -
+116ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[fnlp/moss-002-sft-data](https://
+huggingface.co/datasets/fnlp/moss-002-sft-data) #### Reward Model datasets -
+åççoasst1æ°æ®éï¼[OpenAssistant/oasst1](https://huggingface.co/
+datasets/OpenAssistant/oasst1) - 2ä¸æ¡å¤è¯­è¨oasst1çrewardæ°æ®éï¼
+[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/
+tasksource/oasst1_pairwise_rlhf_reward) - 11ä¸æ¡è±æhh-
+rlhfçrewardæ°æ®éï¼[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/
+Dahoas/full-hh-rlhf) - 9ä¸æ¡è±ærewardæ°æ®é(æ¥èªAnthropic's Helpful
+Harmless dataset)ï¼[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/
+static-hh) - 7ä¸æ¡è±ærewardæ°æ®éï¼æ¥æºåä¸ï¼ï¼[Dahoas/rm-
+static](https://huggingface.co/datasets/Dahoas/rm-static) -
+7ä¸æ¡ç¹ä½ä¸­æçrewardæ°æ®éï¼ç¿»è¯èªrm-staticï¼[liswei/rm-static-
+m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh) -
+7ä¸æ¡è±æRewardæ°æ®éï¼[yitingxie/rlhf-reward-datasets](https://
+huggingface.co/datasets/yitingxie/rlhf-reward-datasets) -
+3åæ¡ä¸­æç¥ä¹é®ç­åå¥½æ°æ®éï¼[liyucheng/zhihu_rlhf_3k](https://
+huggingface.co/datasets/liyucheng/zhihu_rlhf_3k) ## â Todo 1. [x] add
+multiple rounds of dialogue data fine-tuning method 2. [x] add reward model
+finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/
+MedicalGPT) 3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://
+github.com/shibing624/MedicalGPT) 4. [x] add medical reward dataset 5. [x] add
+llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/
+shibing624/MedicalGPT) 6. [ ] add all training and predict demo in colab ##
+âï¸ Contact - Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/
+github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/
+issues) - é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
 å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-å¬å¸å-NLP* è¿NLPäº¤æµç¾¤ã
 [docs/wechat.jpeg] ## ð Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtextgenï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ ```latex
-@misc{textgen, title={textgen: Text Generation Tool}, author={Xu Ming}, year=
+@misc{textgen, title={textgen: Text Generation Tool}, author={Ming Xu}, year=
 {2021}, howpublished={\url{https://github.com/shibing624/textgen}}, } ``` ##
-ð¤ License ææåè®®ä¸º [The Apache License 2.0](/
-LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå textgençé¾æ¥åææåè®®ã
-## ð Contribute
+ð¤ License This repository is licensed under [The Apache License 2.0]
+(LICENSE). Please follow the [Model Card](https://github.com/facebookresearch/
+llama/blob/main/MODEL_CARD.md) to use the LLaMA model. Please follow the [RAIL
+License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM &
+BLOOMZ model. ## ð Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -
 m pytest`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
 ä¹åå³å¯æäº¤PRã ## ð Acknowledgements - [PaddlePaddle/ERNIE](https:/
 /github.com/PaddlePaddle/ERNIE) - [minimaxir/textgenrnn](https://github.com/
 minimaxir/textgenrnn) - [minimaxir/gpt-2-simple](https://github.com/minimaxir/
 gpt-2-simple) - [asyml/texar](https://github.com/asyml/texar) - [yangjianxin1/
```

### Comparing `textgen-0.2.7/README.md` & `textgen-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[**🇨🇳中文**](https://github.com/shibing624/textgen/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/textgen/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+
 <div align="center">
   <a href="https://github.com/shibing624/textgen">
     <img src="https://github.com/shibing624/textgen/blob/main/docs/logo.svg" alt="Logo">
   </a>
 </div>
 
 -----------------
@@ -15,14 +17,20 @@
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
 ## 📖 Introduction
 
 **TextGen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
 
+## 🔥 News
+[2023/06/15] v1.0.0版本: 新增ChatGLM/LLaMA/Bloom模型的多轮对话微调训练，并发布医疗问诊LoRA模型[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)。详见[Release-v1.0.0](https://github.com/shibing624/MedicalGPT/releases/tag/1.0.0)
+
+[2023/06/02] v0.2.7版本: 新增ChatGLM/LLaMA/Bloom模型的SFT微调训练，并发布适用于通用对话和中文纠错的LoRA模型。详见[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
+
+
 ## 😊 Feature
 
 - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
 - [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
 - [BLOOM](textgen/bloom)：本项目基于PyTorch实现了BLOOM模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
 - [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
 - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
@@ -32,30 +40,29 @@
 - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
 
 ### Release Models
 
 release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
 
 
-| Model                                                                                                     | Arch       | Introduce                                                                                                                                                                | Training                                                                                                                                     | Inference                                                                                                             | 
+| Model                                                                                                     | Arch       | Introduction                                                                                                                                                                | Train Script                                                                                                                                 | Predict Script                                                                                                        | 
 |:----------------------------------------------------------------------------------------------------------|:-----------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-| [shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)             | T5         | 中文NLP多任务Prompt模型                                                                                                                                                         | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
 | [shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)                     | T5         | fine-tuned中文对联后的模型                                                                                                                                                       | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-| [shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)                 | SongNet    | SongNet预训练模型                                                                                                                                                             | -                                                                                                                                            | -                                                                                                                     |
 | [shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)   | SongNet    | fine-tuned宋词后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-| [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+| [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
 | [shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)             | ChatGLM-6B | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                        | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
 | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)         | ChatGLM-6B | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                           | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
 | [shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)           | LLaMA-13B  | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                            | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
-| [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
-| [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+| [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+| [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+| [shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)     | LLaMA-13B  | 在240万条中英文医疗数据集[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)上微调了一版Ziya-LLaMA-13B模型，医疗问答效果有提升，发布微调后的LoRA权重                                      | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
 
 ### Evaluation
 
-| Model                                                                                                                                       | Arch       | Introduce                                                                                                                                                                                                                                                                                     | Score    |
+| Model                                                                                                                                       | Arch       | Introduction                                                                                                                                                                                                                                                                                     | Score    |
 |:--------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------|
 | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         | LLaMA-7B   | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 4.92     |
 | [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       | LLaMA-13B  | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 7.05     |
 | [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                                                                                                                                                                                                 | 7.16     |
 | [ChatGLM-6B-v1.1](https://huggingface.co/THUDM/chatglm-6b)                                                                                  | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`v1.1英文优化版模型评估测试集得分                                                                                                                                                                                                                                                      | **7.18** |
 | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           | ChatGLM-6B | 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                                                                                                                                                                                                     | 7.03     |
 | [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                | LLaMA-13B  | 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                                                                                                                                                                                               | 4.13     |  
@@ -108,29 +115,29 @@
 
 ## ▶️ Usage
 
 ### ChatGLM-6B 模型
 
 #### 使用 ChatGLM-6B 微调后的模型
 
-example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+example: [examples/chatglm/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/inference_demo.py)
 
 ```python
 from textgen import ChatGlmModel
 
 model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
 r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
 print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
 ```
 
 PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
 
 #### 训练 ChatGLM-6B 微调模型
 
-1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[examples/data/json_files/belle_10.json](https://github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
 2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
 3. 支持多卡训练，支持混合精度训练
 
 example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
 
 单卡训练：
 ```shell
@@ -162,31 +169,31 @@
 --output_dir：指定保存全量模型权重的目录，默认为./merged
 ```
 
 ### LLaMA 模型
 
 #### 使用 LLaMA 微调后的模型
 
-example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+example: [examples/gpt/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt/inference_demo.py)
 
 <details>
 <summary>show code example and result</summary>
 
 ```python
 import sys
 
 sys.path.append('../..')
-from textgen import LlamaModel
+from textgen import GptModel
 
 
 def generate_prompt(instruction):
   return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
 
 
-model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
+model = GptModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
 predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
 r = model.predict([predict_sentence])
 print(r)  # ['地球是唯一一颗拥有生命的行星。']
 ```
 
 </details>
 
@@ -201,15 +208,15 @@
 #### 基于微调(LoRA)模型继续训练
 如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
 
 单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
 
 执行以下命令：
 ```shell
-python -m textgen/llama/merge_peft_adapter.py \
+python -m textgen/gpt/merge_peft_adapter.py \
     --base_model_name_or_path path_to_original_base_model_dir \
     --peft_model_path path_to_chinese_llama_or_alpaca_lora \
     --output_type [pth|huggingface]
     --output_dir path_to_output_dir 
 ```
 参数说明：
 ```
@@ -217,20 +224,15 @@
 --peft_model_path：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
 --output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为huggingface
 --output_dir：指定保存全量模型权重的目录，默认为./merged
 --offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
 ```
 
 #### 训练领域模型
-
-| Notebook     | Description |    |
-|:----------|:------------|------:|
-| [training_medical_model.ipynb](https://github.com/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb)  | 训练医疗大模型     |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-
-# Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning]单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
+Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning)单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
 
 ### BLOOM 模型
 
 #### 训练 BLOOM 微调模型
 
 example: [examples/bloom/training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/examples/bloom/training_bloom_demo.py)
 
@@ -563,28 +565,42 @@
 
 前10句是真实用户评论，后10句是生成的。
 
 </details>
 
 ## 📚 Dataset 
 
-1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
-4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
-6. 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+#### SFT datasets
+- 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+- 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+- 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+- 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+- 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+- 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+- 5万条英文ChatGPT多轮对话数据集：[RyokoAI/ShareGPT52K](https://huggingface.co/datasets/RyokoAI/ShareGPT52K)
+- 80万条中文ChatGPT多轮对话数据集：[BelleGroup/multiturn_chat_0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+- 116万条中文ChatGPT多轮对话数据集：[fnlp/moss-002-sft-data](https://huggingface.co/datasets/fnlp/moss-002-sft-data)
+
+#### Reward Model datasets
+- 原版的oasst1数据集：[OpenAssistant/oasst1](https://huggingface.co/datasets/OpenAssistant/oasst1)
+- 2万条多语言oasst1的reward数据集：[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/tasksource/oasst1_pairwise_rlhf_reward)
+- 11万条英文hh-rlhf的reward数据集：[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/Dahoas/full-hh-rlhf)
+- 9万条英文reward数据集(来自Anthropic's Helpful Harmless dataset)：[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/static-hh)
+- 7万条英文reward数据集（来源同上）：[Dahoas/rm-static](https://huggingface.co/datasets/Dahoas/rm-static)
+- 7万条繁体中文的reward数据集（翻译自rm-static）[liswei/rm-static-m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh)
+- 7万条英文Reward数据集：[yitingxie/rlhf-reward-datasets](https://huggingface.co/datasets/yitingxie/rlhf-reward-datasets)
+- 3千条中文知乎问答偏好数据集：[liyucheng/zhihu_rlhf_3k](https://huggingface.co/datasets/liyucheng/zhihu_rlhf_3k)
 
 ## ✅ Todo
 
-1. [ ] 新增多轮对话数据微调方法
-2. [ ] add reward model finetuning
-3. [ ] add rl finetuning
-4. [ ] add medical reward dataset
-5. [ ] add llama in4 training
+1. [x] add multiple rounds of dialogue data fine-tuning method
+2. [x] add reward model finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+4. [x] add medical reward dataset
+5. [x] add llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
 6. [ ] add all training and predict demo in colab
 
 ## ☎️ Contact
 
 - Issue(建议)
   ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 - 邮件我：xuming: xuming624@qq.com
@@ -595,23 +611,26 @@
 ## 😇 Citation
 
 如果你在研究中使用了textgen，请按如下格式引用：
 
 ```latex
 @misc{textgen,
   title={textgen: Text Generation Tool},
-  author={Xu Ming},
+  author={Ming Xu},
   year={2021},
   howpublished={\url{https://github.com/shibing624/textgen}},
 }
 ```
 
 ## 🤗 License
+This repository is licensed under [The Apache License 2.0](LICENSE).
+
+Please follow the [Model Card](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) to use the LLaMA model.
 
-授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
+Please follow the [RAIL License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM & BLOOMZ model.
 
 ## 😍 Contribute
 
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
 - 在`tests`添加相应的单元测试
 - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
```

#### html2text {}

```diff
@@ -1,20 +1,32 @@
+[**ð¨ð³ä¸­æ**](https://github.com/shibing624/textgen/blob/main/README.md)
+| [**ðEnglish**](https://github.com/shibing624/textgen/blob/main/
+README_EN.md) | [**ðææ¡£/Docs**](https://github.com/shibing624/textgen/
+wiki) | [**ð¤æ¨¡å/Models**](https://huggingface.co/shibing624)
                                     [Logo]
 ----------------- # TextGen: Implementation of Text Generation models [![PyPI
 version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/
 textgen) [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/
 project/textgen) [![Contributions welcome](https://img.shields.io/badge/
 contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![License Apache 2.0]
 (https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE) [!
 [python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)]
 (requirements.txt) [![GitHub issues](https://img.shields.io/github/issues/
 shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) ## ð Introduction
 **TextGen**å®ç°äºå¤ç§ææ¬çææ¨¡åï¼åæ¬ï¼LLaMAãChatGLMãUDAãGPT2ãSeq2SeqãBARTãT5ãSongNetç­æ¨¡åï¼å¼ç®±å³ç¨ã
+## ð¥ News [2023/06/15] v1.0.0çæ¬: æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçå¤è½®å¯¹è¯å¾®è°è®­ç»ï¼å¹¶åå¸å»çé®è¯LoRAæ¨¡å
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora)ãè¯¦è§[Release-v1.0.0](https://github.com/
+shibing624/MedicalGPT/releases/tag/1.0.0) [2023/06/02] v0.2.7çæ¬:
+æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçSFTå¾®è°è®­ç»ï¼å¹¶åå¸éç¨äºéç¨å¯¹è¯åä¸­æçº éçLoRAæ¨¡åãè¯¦è§
+[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
 ## ð Feature - [ChatGLM](textgen/
 chatglm)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºChatGLM-
 6Bæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¥å­çº éãå¯¹è¯ç­ææ¬çæä»»å¡
 - [LLaMA](textgen/
 llama)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºLLaMAæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
 - [BLOOM](textgen/
 bloom)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºBLOOMæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
@@ -31,37 +43,30 @@
 songnet_model.py)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºSongNetæ¨¡åè®­ç»åé¢æµï¼å¯ä»¥ç¨äºè§èæ ¼å¼çè¯è¯ãæ­è¯ç­ææ¬çæä»»å¡
 - [TGLS](textgen/unsup_generation)ï¼æ¬é¡¹ç®å®ç°äº[TGLS](https://
 www.jiqizhixin.com/articles/2020-08-11-
 5)æ çç£ç¸ä¼¼ææ¬çææ¨¡åï¼æ¯ä¸ç§âåæç´¢åå­¦ä¹ âçææ¬çææ¹æ³ï¼éè¿åå¤è¿­ä»£å­¦ä¹ åééï¼æç»æ¨¡åè½çæç±»ä¼¼åééçé«è´¨éç¸ä¼¼ææ¬
 ### Release Models
 releaseåºäº`textgen`è®­ç»çä¸­ææ¨¡åï¼æ¨¡åå·²ç»releaseå°HuggingFace
 modelsï¼æå®æ¨¡ååç§°`textgen`ä¼èªå¨ä¸è½½æ¨¡åï¼å¯ç´æ¥ä½¿ç¨ã
-| Model | Arch | Introduce | Training | Inference | |:-------------------------
+| Model | Arch | Introduction | Train Script | Predict Script | |:-------------
 -------------------------------------------------------------------------------
---|:-----------|:--------------------------------------------------------------
+--------------|:-----------|:--------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------|:-------------------------------------------------
+----------------------------------------|:-------------------------------------
 -------------------------------------------------------------------------------
--------------|:----------------------------------------------------------------
-------------------------------------------------------| | [shibing624/prompt-
-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese) | T5
-| ä¸­æNLPå¤ä»»å¡Promptæ¨¡å | [prompt-t5-base-chinese.md](https://
-github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md) |
-[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_prompt_demo.py) | | [shibing624/t5-chinese-couplet](https://huggingface.co/
-shibing624/t5-chinese-couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å |
-[å¯¹èçææ¨¡åè°ç ](https://github.com/shibing624/textgen/blob/main/
-docs/
+-------------------------|:----------------------------------------------------
+------------------------------------------------------------------| |
+[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-
+couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å | [å¯¹èçææ¨¡åè°ç ]
+(https://github.com/shibing624/textgen/blob/main/docs/
 %E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) |
 [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_couplet_demo.py) | | [shibing624/songnet-base-chinese](https://
-huggingface.co/shibing624/songnet-base-chinese) | SongNet |
-SongNeté¢è®­ç»æ¨¡å | - | - | | [shibing624/songnet-base-chinese-songci]
-(https://huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet |
-fine-tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
+t5_couplet_demo.py) | | [shibing624/songnet-base-chinese-songci](https://
+huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet | fine-
+tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
 songnet_songci_demo.py) | | [shibing624/songnet-base-chinese-couplet](https://
 huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet | fine-
 tunedå¯¹èåçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
@@ -100,31 +105,39 @@
 [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/
 chinese-alpaca-plus-13b-hf) | LLaMA-13B | [ä¸­æLLaMA-Plus, Alpaca-Plus
 13Bçæ¬](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/
 v3.1)ï¼å¨LLaMA-
 13Bä¸æ©åäºä¸­æè¯è¡¨å¹¶ç»§ç»­é¢è®­ç»120Gææ¬ï¼éç¨é¢åï¼ï¼å¨4.3Mæä»¤æ°æ®éä¸å¾®è°åå¾å°çä¸­æAlpaca-
 plusæ¨¡å | [training script](https://github.com/shibing624/textgen/blob/main/
 examples/llama/training_llama_demo.py) | [predict script](https://github.com/
-shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | ###
-Evaluation | Model | Arch | Introduce | Score | |:-----------------------------
+shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | |
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora) | LLaMA-13B | å¨240ä¸æ¡ä¸­è±æå»çæ°æ®é
+[shibing624/medical](https://huggingface.co/datasets/shibing624/
+medical)ä¸å¾®è°äºä¸çZiya-LLaMA-
+13Bæ¨¡åï¼å»çé®ç­ææææåï¼åå¸å¾®è°åçLoRAæé |
+[training script](https://github.com/shibing624/textgen/blob/main/examples/
+llama/training_llama_demo.py) | [predict script](https://github.com/shibing624/
+textgen/blob/main/examples/llama/training_llama_demo.py) | ### Evaluation |
+Model | Arch | Introduction | Score | |:---------------------------------------
 -------------------------------------------------------------------------------
---------------------------------|:-----------|:--------------------------------
+----------------------|:-----------|:------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://
-huggingface.co/ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/
+-------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/
+ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/Chinese-LLaMA-
+Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/
+README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca](https://
+huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B | å¤ç¨[ymcui/
 Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/
-examples/README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca]
-(https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B |
-å¤ç¨[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-
-Alpaca/blob/main/examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-
-6B](https://huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/
-chatglm-6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://
+examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-6B](https://
 huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
+6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://huggingface.co/
+THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
 6b`v1.1è±æä¼åçæ¨¡åè¯ä¼°æµè¯éå¾å | **7.18** | | [shibing624/
 chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-
 zh-lora) | ChatGLM-6B | åºäº`THUDM/chatglm-6b`å è½½`shibing624/chatglm-6b-
 belle-zh-lora`LoRAæ¨¡ååè¯ä¼°æµè¯éå¾å | 7.03 | | [facat/alpaca-lora-
 cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b) | LLaMA-13B |
 åºäº`decapoda-research/llama-13b-hf`å è½½`facat/alpaca-lora-cn-
 13b`LoRAæ¨¡ååè¯ä¼°æµè¯éå¹¶æ æ³¨å¾å | 4.13 | | [Chinese-Vicuna/
@@ -172,26 +185,27 @@
 examples/gradio_demo.py ``` model trained by [examples/t5/
 T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/
 main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb) ## ð¾ Install ```shell
 pip install -U textgen ``` or install develop version: ```shell pip install
 torch # conda install pytorch git clone https://github.com/shibing624/
 textgen.git cd textgen python setup.py install ``` ## â¶ï¸ Usage ### ChatGLM-
 6B æ¨¡å #### ä½¿ç¨ ChatGLM-6B å¾®è°åçæ¨¡å example: [examples/chatglm/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-chatglm/predict_demo.py) ```python from textgen import ChatGlmModel model =
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+chatglm/inference_demo.py) ```python from textgen import ChatGlmModel model =
 ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-
 csc-zh-lora") r = model.predict(
 ["å¯¹ä¸é¢ä¸­ææ¼åçº éï¼\nå°åéåå è¯¥ä¸ºèäººè®©åã\nç­ï¼"])
 print(r) # ['å°åéååºè¯¥ä¸ºèäººè®©åº§ã\néè¯¯å­ï¼å ï¼å'] ```
 PSï¼ç±äºä½¿ç¨äºå¼åä¸­çpeftåºï¼å¯è½ç±äºçæ¬æ´æ°ï¼å¯¼è´LoRAæ¨¡åå è½½å¤±è´¥ï¼å»ºè®®ä½¿ç¨ä¸é¢çè®­ç»æ¹æ³ï¼èªå·±è®­ç»LoRAæ¨¡åã
 #### è®­ç» ChatGLM-6B å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
-data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
-datasets/shibing624/alpaca-zh) 2.
+data/zh_csc_test.tsv)æè[examples/data/json_files/belle_10.json](https://
+github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
+2.
 æ¯æAdaLoRAãLoRAãP_TuningãPrefix_Tuningç­é¨ååæ°å¾®è°æ¹æ³ï¼ä¹æ¯æå¨åå¾®è°
 3. æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç» example: [examples/chatglm/
 training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/chatglm/training_chatglm_demo.py) åå¡è®­ç»ï¼ ```shell cd
 examples/chatglm CUDA_VISIBLE_DEVICES=0 python training_chatglm_demo.py --
 do_train --do_predict --num_epochs 1 --output_dir outputs_chatglm ```
 å¤å¡è®­ç»ï¼ ```shell cd examples/chatglm CUDA_VISIBLE_DEVICES=0,1 torchrun
@@ -202,23 +216,23 @@
 m textgen/chatglm/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path path_to_peft_model_dir \ --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --
 peft_model_pathï¼å­æ¾PEFTæ ¼å¼çå¾®è°æ¨¡åæéåéç½®æä»¶çç®å½
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged ```
-### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/llama/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-llama/predict_demo.py)  show code example and result ```python import sys
-sys.path.append('../..') from textgen import LlamaModel def generate_prompt
+### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/gpt/
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+gpt/inference_demo.py)  show code example and result ```python import sys
+sys.path.append('../..') from textgen import GptModel def generate_prompt
 (instruction): return f"""Below is an instruction that describes a task. Write
 a response that appropriately completes the request.\n\n### Instruction:
-{instruction}\n\n### Response:""" model = LlamaModel("llama", "decapoda-
-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
-predict_sentence = generate_prompt
+{instruction}\n\n### Response:""" model = GptModel("llama", "decapoda-research/
+llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b") predict_sentence =
+generate_prompt
 ("é®ï¼ç¨ä¸å¥è¯æè¿°å°çä¸ºä»ä¹æ¯ç¬ä¸æ äºçã\nç­ï¼") r =
 model.predict([predict_sentence]) print(r) #
 ['å°çæ¯å¯ä¸ä¸é¢æ¥æçå½çè¡æã'] ```  #### è®­ç» LLaMA
 å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
 data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
@@ -228,34 +242,29 @@
 æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç»ï¼ä½¿ç¨æ¹æ³åä¸ï¼ChatGLMå¤å¡è®­ç»ï¼
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/
 textgen/blob/main/examples/llama/training_llama_demo.py) #### åºäºå¾®è°
 (LoRA)æ¨¡åç»§ç»­è®­ç»
 å¦æéè¦åºäºLoraæ¨¡åç»§ç»­è®­ç»ï¼å¯ä»¥ä½¿ç¨ä¸é¢çèæ¬åå¹¶æ¨¡åä¸ºæ°çbase
 modelï¼åå¾®è°è®­ç»å³å¯ã åLoRAæéåå¹¶ï¼éç¨äº Chinese-LLaMA,
 Chinese-LLaMA-Plus, Chinese-Alpacaï¼ æ§è¡ä»¥ä¸å½ä»¤ï¼ ```shell python -
-m textgen/llama/merge_peft_adapter.py \ --base_model_name_or_path
+m textgen/gpt/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path
 path_to_chinese_llama_or_alpaca_lora \ --output_type [pth|huggingface] --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --peft_model_pathï¼ä¸­æLLaMA/Alpaca
 LoRAè§£ååæä»¶æå¨ç®å½ï¼ä¹å¯ä½¿ç¨HFä¸çLoraæ¨¡ååç§°ï¼å¦`ziqingyang/
 chinese-alpaca-lora-7b`ä¼èªå¨ä¸è½½å¯¹åºæ¨¡å --output_type:
 æå®è¾åºæ ¼å¼ï¼å¯ä¸ºpthæhuggingfaceãè¥ä¸æå®ï¼é»è®¤ä¸ºhuggingface
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged --
 offload_dirï¼å¯éï¼ï¼å¯¹äºä½åå­ç¨æ·éè¦æå®ä¸ä¸ªoffloadç¼å­è·¯å¾
-``` #### è®­ç»é¢åæ¨¡å | Notebook | Description | | |:----------|:--------
-----|------:| | [training_medical_model.ipynb](https://github.com/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-è®­ç»å»çå¤§æ¨¡å |[![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) | # Note:
+``` #### è®­ç»é¢åæ¨¡å Note:
 ä¸ºäºå¨é¢çä»ç»è®­ç»å»çå¤§æ¨¡åçè¿ç¨ï¼æ4é¶æ®µè®­ç»æ¹æ³
-[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
-Learning]åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
+(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
+Learning)åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
 github.com/shibing624/MedicalGPT)ï¼è¯·ç§»æ­¥è¯¥repoæ¥çè®­ç»æ¹æ³ã ###
 BLOOM æ¨¡å #### è®­ç» BLOOM å¾®è°æ¨¡å example: [examples/bloom/
 training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/bloom/training_bloom_demo.py) ### ConvSeq2Seq æ¨¡å
 è®­ç»å¹¶é¢æµConvSeq2Seqæ¨¡åï¼ example: [examples/seq2sesq/
 training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/
 main/examples/seq2seq/training_convseq2seq_model_demo.py)  show code example
@@ -433,42 +442,68 @@
 ä¸æå¼åè£éé¢çç²¾åååå¥½ï¼ç¨äºè¡¥æ°´è¡¥æ°´ææä¸éï¼ç©æµéå¸¸å¿«ã
 ç®è¤å¾åæ»ðæ¯ä¸å»éåº¦å¿«ä¸å¤©å°±å°äºã
 åä¸¤å¤©ç®è¤å¹²ç¥è¿ç»­æ·äºä¸¤ä¸ªæä¸æè§è¿ä¸éðè¡¥æ°´ææææ¾ï¼å¯æ³èç¥ç²¾åæ¶²åå¤åè¶³ðæ·ä¸ä»¥åååçå¾èæã
 è¡¥æ°´ææä¸è¬å§ï½ä½æ¯æç¨çé©å½èåæ¥çé¢èçº¸ä¸ç®èï¼å¸æå¥½ç¨ä¼åè´­çï¼æ·ä¸è¸æè§æ¯è¾æ¸ç½ï½ä»·æ ¼è¿ä¸ä¾¿å®ã
 å¸æå¥½ç¨ï¼é¢èç¨è¿äºå¾å¥½ç¨ï¼ç®è¤æ°´å«©åæ»ç½çï¼è¡¥æ°´ä¸éï¼ä»·æ ¼ä¹åéã
 å°±æ¯ç²¾åæ¶²å¤ªå°äºï¼ä¿æ¹¿ææä¸éã
 é¢èçè¡¥æ°´ææéå¸¸å¥½ï¼ä¿æ¹¿ææç¡®å®å¾èµï¼è¿ä¸ªé¢èç¸å¯¹äºè¶åèç½åç¾ç½çé£ä¸¤æ¬¾çé¢èçº¸è¦åä¸äºï¼ççä»·æ ¼åéã
-``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset 1.
-50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_0.5M_CN](https://
-huggingface.co/datasets/BelleGroup/train_0.5M_CN) 2.
+``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset
+#### SFT datasets - 50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/
+train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN) -
 100ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_1M_CN](https://
-huggingface.co/datasets/BelleGroup/train_1M_CN) 3.
+huggingface.co/datasets/BelleGroup/train_1M_CN) -
 5ä¸æ¡è±æChatGPTæä»¤Alpacaæ°æ®éï¼[50k English Stanford Alpaca
-dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) 4.
+dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) -
 2ä¸æ¡ä¸­æChatGPTæä»¤Alpacaæ°æ®éï¼[shibing624/alpaca-zh](https://
-huggingface.co/datasets/shibing624/alpaca-zh) 5.
+huggingface.co/datasets/shibing624/alpaca-zh) -
 69ä¸æ¡ä¸­ææä»¤Guanacoæ°æ®é(Belle50ä¸æ¡+Guanaco19ä¸æ¡)ï¼[Chinese-
 Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-
-Vicuna/guanaco_belle_merge_v1.0) 6. 240ä¸æ¡ä¸­æå»çæ°æ®é
+Vicuna/guanaco_belle_merge_v1.0) - 240ä¸æ¡ä¸­æå»çæ°æ®é
 (åæ¬é¢è®­ç»æ°æ®åæä»¤å¾®è°æ°æ®é)ï¼[shibing624/medical](https://
-huggingface.co/datasets/shibing624/medical) ## â Todo 1. [ ]
-æ°å¢å¤è½®å¯¹è¯æ°æ®å¾®è°æ¹æ³ 2. [ ] add reward model finetuning 3. [ ]
-add rl finetuning 4. [ ] add medical reward dataset 5. [ ] add llama in4
-training 6. [ ] add all training and predict demo in colab ## âï¸ Contact -
-Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/github/issues/
-shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) -
-é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
+huggingface.co/datasets/shibing624/medical) -
+5ä¸æ¡è±æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[RyokoAI/ShareGPT52K](https://
+huggingface.co/datasets/RyokoAI/ShareGPT52K) -
+80ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[BelleGroup/multiturn_chat_0.8M]
+(https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M) -
+116ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[fnlp/moss-002-sft-data](https://
+huggingface.co/datasets/fnlp/moss-002-sft-data) #### Reward Model datasets -
+åççoasst1æ°æ®éï¼[OpenAssistant/oasst1](https://huggingface.co/
+datasets/OpenAssistant/oasst1) - 2ä¸æ¡å¤è¯­è¨oasst1çrewardæ°æ®éï¼
+[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/
+tasksource/oasst1_pairwise_rlhf_reward) - 11ä¸æ¡è±æhh-
+rlhfçrewardæ°æ®éï¼[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/
+Dahoas/full-hh-rlhf) - 9ä¸æ¡è±ærewardæ°æ®é(æ¥èªAnthropic's Helpful
+Harmless dataset)ï¼[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/
+static-hh) - 7ä¸æ¡è±ærewardæ°æ®éï¼æ¥æºåä¸ï¼ï¼[Dahoas/rm-
+static](https://huggingface.co/datasets/Dahoas/rm-static) -
+7ä¸æ¡ç¹ä½ä¸­æçrewardæ°æ®éï¼ç¿»è¯èªrm-staticï¼[liswei/rm-static-
+m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh) -
+7ä¸æ¡è±æRewardæ°æ®éï¼[yitingxie/rlhf-reward-datasets](https://
+huggingface.co/datasets/yitingxie/rlhf-reward-datasets) -
+3åæ¡ä¸­æç¥ä¹é®ç­åå¥½æ°æ®éï¼[liyucheng/zhihu_rlhf_3k](https://
+huggingface.co/datasets/liyucheng/zhihu_rlhf_3k) ## â Todo 1. [x] add
+multiple rounds of dialogue data fine-tuning method 2. [x] add reward model
+finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/
+MedicalGPT) 3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://
+github.com/shibing624/MedicalGPT) 4. [x] add medical reward dataset 5. [x] add
+llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/
+shibing624/MedicalGPT) 6. [ ] add all training and predict demo in colab ##
+âï¸ Contact - Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/
+github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/
+issues) - é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
 å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-å¬å¸å-NLP* è¿NLPäº¤æµç¾¤ã
 [docs/wechat.jpeg] ## ð Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtextgenï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ ```latex
-@misc{textgen, title={textgen: Text Generation Tool}, author={Xu Ming}, year=
+@misc{textgen, title={textgen: Text Generation Tool}, author={Ming Xu}, year=
 {2021}, howpublished={\url{https://github.com/shibing624/textgen}}, } ``` ##
-ð¤ License ææåè®®ä¸º [The Apache License 2.0](/
-LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå textgençé¾æ¥åææåè®®ã
-## ð Contribute
+ð¤ License This repository is licensed under [The Apache License 2.0]
+(LICENSE). Please follow the [Model Card](https://github.com/facebookresearch/
+llama/blob/main/MODEL_CARD.md) to use the LLaMA model. Please follow the [RAIL
+License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM &
+BLOOMZ model. ## ð Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -
 m pytest`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
 ä¹åå³å¯æäº¤PRã ## ð Acknowledgements - [PaddlePaddle/ERNIE](https:/
 /github.com/PaddlePaddle/ERNIE) - [minimaxir/textgenrnn](https://github.com/
 minimaxir/textgenrnn) - [minimaxir/gpt-2-simple](https://github.com/minimaxir/
 gpt-2-simple) - [asyml/texar](https://github.com/asyml/texar) - [yangjianxin1/
```

### Comparing `textgen-0.2.7/setup.py` & `textgen-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.2.7',
+    version='1.0.0',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
@@ -24,20 +24,20 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     python_requires=">=3.6",
     keywords='textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation',
     install_requires=[
         'loguru',
         'jieba>=0.39',
-        'transformers>=4.28.1',
+        'transformers',
         'datasets',
         'gensim>=4.0.0',
         'text2vec',
         'tensorboard',
-        'tqdm>=4.47.0',
+        'tqdm',
         'pandas',
         'wandb>=0.10.32',
         'sacremoses',
         'Rouge',
         'cpm_kernels',
         'peft>=0.3.0',
     ],
```

### Comparing `textgen-0.2.7/textgen/__init__.py` & `textgen-1.0.0/textgen/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.2.7'
+__version__ = '1.0.0'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
@@ -31,12 +31,10 @@
 from textgen.t5.copyt5_utils import ZHTokenizer
 
 from textgen.unsup_generation.tgls_model import TglsModel
 
 from textgen.config.model_args import ChatGlmArgs
 from textgen.chatglm.chatglm_model import ChatGlmModel
 
-from textgen.config.model_args import LlamaArgs
-from textgen.llama.llama_model import LlamaModel
+from textgen.config.model_args import GptArgs
+from textgen.gpt.gpt_model import GptModel
 
-from textgen.config.model_args import BloomArgs
-from textgen.bloom.bloom_model import BloomModel
```

### Comparing `textgen-0.2.7/textgen/augment/sentence_level_augment.py` & `textgen-1.0.0/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/augment/text_augment.py` & `textgen-1.0.0/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/augment/tokenizer.py` & `textgen-1.0.0/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/augment/translate_api.py` & `textgen-1.0.0/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/augment/word_level_augment.py` & `textgen-1.0.0/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/augment/word_vocab.py` & `textgen-1.0.0/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/bloom/bloom_model.py` & `textgen-1.0.0/textgen/gpt/gpt_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,99 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
+
+modified from https://github.com/tloen/alpaca-lora/blob/main/finetune.py
 """
 import math
 import os
 import random
-import sys
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 import numpy as np
 import torch
 from loguru import logger
 from peft import (
     get_peft_model,
     LoraConfig,
     TaskType,
     PeftModel,
     prepare_model_for_int8_training,
     set_peft_model_state_dict,
 )
-from tqdm.auto import tqdm
-from transformers import BloomForCausalLM, BloomTokenizerFast
-from transformers import GenerationConfig, DataCollatorForSeq2Seq
-from transformers import Trainer, TrainingArguments, AutoConfig
+from tqdm import tqdm
+from transformers import (
+    LlamaForCausalLM,
+    LlamaTokenizerFast,
+    BloomTokenizerFast,
+    BloomForCausalLM,
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    Trainer,
+    TrainingArguments,
+    GenerationConfig,
+    DataCollatorForSeq2Seq,
+    BitsAndBytesConfig,
+    deepspeed,
+)
 from transformers.trainer import TRAINING_ARGS_NAME
 
-from textgen.bloom.bloom_utils import load_hf_dataset, BloomDataset
-from textgen.config.model_args import BloomArgs
+from textgen.config.model_args import GptArgs
+from textgen.gpt.gpt_utils import InstructionDataset, PROMPT_DICT
 
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
-    "bloom": (AutoConfig, BloomForCausalLM, BloomTokenizerFast),
+    "llama": (LlamaForCausalLM, LlamaTokenizerFast),
+    "bloom": (BloomForCausalLM, BloomTokenizerFast),
+    "baichuan": (AutoModelForCausalLM, AutoTokenizer),
+    "auto": (AutoModelForCausalLM, AutoTokenizer),
 }
 
 
-class BloomModel:
+class GptModel:
     def __init__(
             self,
-            model_type="bloom",
-            model_name="bigscience/bloomz-560m",
-            peft_name=None,
-            args=None,
-            use_cuda=has_cuda,
-            cuda_device=-1,
+            model_type,
+            model_name,
+            peft_name: Optional[str] = None,
+            args: Optional[dict] = None,
+            use_cuda: Optional[bool] = has_cuda,
+            cuda_device: Optional[int] = -1,
             **kwargs,
     ):
 
         """
-        Initializes a BloomModel model.
+        Initializes a GptModel model.
 
         Args:
-            model_type: The type of model (llama)
+            model_type: The type of model (llama, bloom, baichuan, auto)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
             peft_name (optional): Peft model name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
             cuda_device (int, optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
 
         if isinstance(args, dict):
             self.args.update_from_dict(args)
-        elif isinstance(args, BloomArgs):
+        elif isinstance(args, GptArgs):
             self.args = args
 
         if self.args.manual_seed:
             random.seed(self.args.manual_seed)
             np.random.seed(self.args.manual_seed)
             torch.manual_seed(self.args.manual_seed)
-            if torch.cuda.is_available():
+            if torch.cuda.is_available() > 0:
                 torch.cuda.manual_seed_all(self.args.manual_seed)
 
         self.device_map = "auto"
         if use_cuda:
             if torch.cuda.is_available():
                 if cuda_device == -1:
                     self.device = torch.device("cuda")
@@ -89,72 +104,81 @@
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
             if torch.backends.mps.is_available():
                 self.device = torch.device("mps")
+                self.device_map = {"": "mps"}
             else:
                 self.device = "cpu"
                 self.device_map = {"": "cpu"}
         logger.debug(f"Device: {self.device}")
         if not use_cuda:
             self.args.fp16 = False
             self.args.int8 = False
         world_size = int(os.environ.get("WORLD_SIZE", 1))
         self.ddp = world_size != 1
         if self.ddp:
             self.device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
 
         self.results = {}
-        config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
+        model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
-        config = AutoConfig.from_pretrained(model_name, **kwargs)
 
         if torch.cuda.is_bf16_supported() and not self.args.bf16:
             logger.warning("GPU supports bf16, you can enable bf16.")
         self.torch_dtype = torch.bfloat16 if self.args.bf16 else (torch.float16 if self.args.fp16 else torch.float32)
         self.model = model_class.from_pretrained(
             model_name,
-            config=config,
             load_in_8bit=self.args.int8,
             torch_dtype=self.torch_dtype,
             device_map=self.device_map,
+            trust_remote_code=self.args.trust_remote_code,
+            quantization_config=BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_compute_dtype=self.torch_dtype,
+            ) if self.args.qlora else None,
+            **kwargs,
         )
 
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
-            self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name)
+            self.tokenizer = tokenizer_class.from_pretrained(
+                self.args.tokenizer_name, trust_remote_code=self.args.trust_remote_code)
         else:
-            self.tokenizer = tokenizer_class.from_pretrained(model_name)
+            self.tokenizer = tokenizer_class.from_pretrained(
+                model_name, trust_remote_code=self.args.trust_remote_code)
             self.args.tokenizer_name = self.args.model_name
 
         self.args.model_type = model_type
         if model_name is None:
-            self.args.model_name = "Bloom_from_scratch"
+            self.args.model_name = "Llama_from_scratch"
         else:
             self.args.model_name = model_name
 
         self.peft_name = peft_name
-        if self.args.use_peft:
+        if self.args.use_peft and self.peft_name:
             self.load_peft_model()
+        # Set padding side equal to Collator padding side
+        self.tokenizer.padding_side = "left"
+        self.tokenizer.pad_token_id = 0
 
-    def resize_model_embeddings(self, tokenizer_vocab_size):
-        """Resizes model embeddings to match the tokenizer vocab size."""
-        model_vocab_size = self.model.get_input_embeddings().weight.size(0)
-        if model_vocab_size != tokenizer_vocab_size:
-            logger.debug(
-                f"Resize model embeddings to fit tokenizer, "
-                f"Vocab of the base model: {model_vocab_size}, "
-                f"Vocab of the tokenizer: {tokenizer_vocab_size}"
-            )
-            self.model.resize_token_embeddings(tokenizer_vocab_size)
-            assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
-            logger.debug(f"Model token embeddings updated, size: {len(self.tokenizer)}")
+    def load_peft_model(self):
+        """Load peft model"""
+        self.model = PeftModel.from_pretrained(
+            self.model,
+            self.peft_name,
+            torch_dtype=self.torch_dtype,
+            device_map=self.device_map,
+        )
+        logger.info(f"Loaded peft model from {self.peft_name}")
 
     def find_all_linear_names(self, int4=False, int8=False):
         cls = torch.nn.Linear
         if int4 or int8:
             import bitsandbytes as bnb
             if int4:
                 cls = bnb.nn.Linear4bit
@@ -215,26 +239,50 @@
                 and os.listdir(output_dir)
                 and not self.args.overwrite_output_dir
         ):
             raise ValueError(
                 "Output directory ({}) already exists and is not empty."
                 " Set args.overwrite_output_dir = True to overcome.".format(output_dir)
             )
-        # update model train config
-        self.model.gradient_checkpointing_enable()
-        self.model.enable_input_require_grads()
-        if not self.ddp and torch.cuda.device_count() > 1:
-            # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
-            self.model.is_parallelizable = True
-            self.model.model_parallel = True
-        self.model.config.use_cache = False
+
+        # Setup train args
+        training_args = TrainingArguments(
+            output_dir=output_dir,
+            learning_rate=self.args.learning_rate,
+            num_train_epochs=self.args.num_train_epochs,
+            logging_dir=f"{output_dir}/logs",
+            logging_steps=self.args.logging_steps,
+            max_steps=self.args.max_steps,
+            per_device_train_batch_size=self.args.per_device_train_batch_size,
+            per_device_eval_batch_size=self.args.per_device_train_batch_size,
+            gradient_checkpointing=self.args.gradient_checkpointing,
+            torch_compile=self.args.torch_compile,
+            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
+            warmup_steps=self.args.warmup_steps,
+            save_steps=self.args.save_steps,
+            optim=self.args.optimizer,
+            save_strategy=self.args.save_strategy,
+            evaluation_strategy='steps' if eval_data is not None else 'no',
+            eval_steps=self.args.eval_steps if eval_data is not None else None,
+            load_best_model_at_end=True if eval_data is not None else False,
+            ddp_find_unused_parameters=False if self.ddp else None,
+            save_total_limit=self.args.save_total_limit,
+            fp16=self.args.fp16,
+            bf16=self.args.bf16,
+            remove_unused_columns=self.args.remove_unused_columns,
+            report_to=self.args.report_to,
+            overwrite_output_dir=self.args.overwrite_output_dir,
+            no_cuda=True if self.device == "cpu" else False,
+            **kwargs
+        )
         resume_from_checkpoint = self.args.resume_from_checkpoint
+        if self.args.qlora and (len(training_args.fsdp) > 0 or deepspeed.is_deepspeed_zero3_enabled()):
+            logger.warning("FSDP and ZeRO3 are both currently incompatible with QLoRA.")
         if 'all' in self.args.lora_target_modules:
             self.args.lora_target_modules = self.find_all_linear_names(self.args.int4, self.args.int8)
-
         # setup peft
         if self.args.use_peft:
             peft_type = self.args.peft_type.upper()
             logger.info(f"Using PEFT type: {peft_type}")
             # add peft config
             if peft_type == 'LORA':
                 logger.debug(f"Using list modules for LoRA: {self.args.lora_target_modules}")
@@ -318,76 +366,65 @@
                         resume_from_checkpoint, "adapter_model.bin")  # only LoRA model - LoRA config above has to fit
                     resume_from_checkpoint = (
                         False  # So the trainer won't try loading its state
                     )
                 # The two files above have a different name depending on how they were saved, but are actually the same.
                 if os.path.exists(checkpoint_name):
                     logger.info(f"Restarting from {checkpoint_name}")
-                    adapters_weights = torch.load(checkpoint_name)
+                    adapters_weights = torch.load(checkpoint_name, map_location='cpu')
                     set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
         else:
             logger.warning("Now full model params fine-tune, which is slow, set `use_peft=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
+        logger.debug(f"Tokenizer: {self.tokenizer}")
+        logger.debug(f"Model: {self.model}")
 
         # load dataset
         train_dataset = self.load_and_cache_examples(train_data)
         if verbose:
             logger.debug(f"train_dataset len: {len(train_dataset)}, train_dataset[0]: {train_dataset[0]}")
+            logger.debug(f"text of train_dataset[0]: {self.tokenizer.decode(train_dataset[0]['input_ids'])}")
         eval_dataset = None
         if eval_data is not None:
             eval_dataset = self.load_and_cache_examples(eval_data, evaluate=True)
             if verbose:
                 logger.debug(f"eval_dataset len: {len(eval_dataset)}, eval_dataset[0]: {eval_dataset[0]}")
 
-        # start train
-        training_args = TrainingArguments(
-            output_dir=output_dir,
-            learning_rate=self.args.learning_rate,
-            num_train_epochs=self.args.num_train_epochs,
-            logging_dir=f"{output_dir}/logs",
-            logging_steps=self.args.logging_steps,
-            max_steps=self.args.max_steps,
-            per_device_train_batch_size=self.args.per_device_train_batch_size,
-            per_device_eval_batch_size=self.args.per_device_train_batch_size,
-            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
-            warmup_steps=self.args.warmup_steps,
-            save_steps=self.args.save_steps,
-            optim=self.args.optimizer,
-            save_strategy=self.args.save_strategy,
-            evaluation_strategy='steps' if eval_data is not None else 'no',
-            eval_steps=self.args.eval_steps if eval_data is not None else None,
-            load_best_model_at_end=True if eval_data is not None else False,
-            ddp_find_unused_parameters=False if self.ddp else None,
-            save_total_limit=self.args.save_total_limit,
-            fp16=self.args.fp16,
-            bf16=self.args.bf16,
-            remove_unused_columns=self.args.remove_unused_columns,
-            report_to=self.args.report_to,
-            overwrite_output_dir=self.args.overwrite_output_dir,
-            no_cuda=True if self.device == "cpu" else False,
-            **kwargs
-        )
         # Log on each process the small summary:
         logger.warning(
             f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
             + f"distributed training: {bool(training_args.local_rank != -1)}, 16-bits training: {training_args.fp16}"
         )
         if training_args.local_rank <= 0:
             logger.info(f"Training/evaluation parameters {training_args}")
 
+        # Update model train config
+        if self.args.gradient_checkpointing:
+            self.model.gradient_checkpointing_enable()
+            self.model.config.use_cache = False
+        else:
+            self.model.config.use_cache = True
+        self.model.enable_input_require_grads()
+        if torch.cuda.device_count() > 1:
+            # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
+            self.model.is_parallelizable = True
+            self.model.model_parallel = True
+
+        # Initialize our Trainer
         data_collator = DataCollatorForSeq2Seq(
             self.tokenizer,
             return_tensors="pt",
             padding="max_length",
             max_length=self.args.max_seq_length + self.args.max_length
         )
+
         if self.args.use_peft:
             trainer = SavePeftModelTrainer(
                 model=self.model,
                 train_dataset=train_dataset,
                 eval_dataset=eval_dataset if eval_data is not None else None,
                 args=training_args,
                 tokenizer=self.tokenizer,
@@ -399,104 +436,83 @@
                 train_dataset=train_dataset,
                 eval_dataset=eval_dataset if eval_data is not None else None,
                 args=training_args,
                 tokenizer=self.tokenizer,
                 data_collator=data_collator,
             )
 
-        if self.args.enable_torch_compile and torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
-
+        # Training
         logger.info("*** Train ***")
+        logger.debug(f"Train dataloader example: {next(iter(trainer.get_train_dataloader()))}")
         (global_step, training_loss, metrics) = trainer.train(resume_from_checkpoint=resume_from_checkpoint)
-        self.handle_metrics("train", metrics, output_dir)
         self.results.update(metrics)
+        trainer.log_metrics("train", metrics)
+        trainer.save_metrics("train", metrics)
+        trainer.save_state()
         self.save_model(model=self.model)
 
         if eval_data is not None:
             logger.info("*** Evaluate ***")
             if self.args.fp16:
                 self.model.half()
             metrics = trainer.evaluate(metric_key_prefix="eval")
+            metrics['eval_samples'] = len(eval_dataset)
             try:
                 perplexity = math.exp(metrics["eval_loss"])
             except OverflowError:
                 perplexity = float("inf")
             metrics["perplexity"] = perplexity
             logger.debug(f"eval metrics: {metrics}")
-            self.handle_metrics("eval", metrics, output_dir)
             self.results.update(metrics)
+            trainer.log_metrics("eval", metrics)
+            trainer.save_metrics("eval", metrics)
 
         if verbose and training_args.local_rank <= 0:
             logger.debug(f"metrics: {self.results}")
             logger.info(
                 " Training of {} model complete. Saved to {}.".format(
                     self.args.model_name, output_dir
                 )
             )
         return global_step, training_loss
 
-    @staticmethod
-    def handle_metrics(split, metrics, output_dir):
-        """
-        Log and save metrics
-
-        Args:
-        - split: one of train, val, test
-        - metrics: metrics dict
-        - output_dir: where to save the metrics
-        """
-
-        logger.info(f"***** {split} metrics *****")
-        for key in sorted(metrics.keys()):
-            logger.info(f"  {key} = {metrics[key]}")
-        output_file = os.path.join(output_dir, f"{split}_results.txt")
-        with open(output_file, "w") as writer:
-            for key in sorted(metrics.keys()):
-                writer.write("{} = {}\n".format(key, str(metrics[key])))
-
-    def load_peft_model(self):
-        """Load peft model"""
-        if self.peft_name:
-            if os.path.isdir(self.peft_name) and os.path.exists(
-                    os.path.join(self.peft_name, "tokenizer_config.json")):
-                update_tokenizer = True
-            else:
-                update_tokenizer = False
-            if update_tokenizer:
-                self.tokenizer = BloomTokenizerFast.from_pretrained(self.peft_name)
-                self.resize_model_embeddings(len(self.tokenizer))
-            self.model = PeftModel.from_pretrained(
-                self.model,
-                self.peft_name,
-                torch_dtype=self.torch_dtype,
-                device_map=self.device_map,
-            )
-            logger.info(f"Loaded peft model from {self.peft_name}")
-        else:
-            # Load peft model from output_dir
-            peft_path = os.path.join(self.args.output_dir, self.args.peft_bin_name)
-            if peft_path and os.path.exists(peft_path):
-                self.model = PeftModel.from_pretrained(
-                    self.model,
-                    self.args.output_dir,
-                    torch_dtype=self.torch_dtype,
-                    device_map=self.device_map,
-                )
-                logger.info(f"Loaded peft model from {peft_path}")
-
-    @torch.no_grad()
-    def predict(self, sentences: List[str], keep_prompt: bool = False, max_length: int = None, **kwargs):
+    @torch.inference_mode()
+    def predict(
+            self,
+            sentences: List[str],
+            keep_prompt: bool = False,
+            add_system_prompt: bool = False,
+            max_length: int = 256,
+            temperature: float = 0.95,
+            top_p: float = 0.9,
+            top_k: int = 40,
+            do_sample: bool = True,
+            repetition_penalty: float = 1.3,
+            length_penalty: float = 2.0,
+            num_beams: int = 1,
+            num_return_sequences: int = 1,
+            **kwargs
+    ) -> List[str]:
         """
         Performs predictions on a list of text.
 
         Args:
             sentences: A python list of text (str) to be sent to the model for prediction. Note that the prefix should be prepended to the text.
             keep_prompt: Whether to keep the prompt in the generated text.
+            add_system_prompt: Whether to add the system prompt to the prompt text.
             max_length: The maximum length of the generated text.
+            temperature: The value used to module the next token probabilities.
+            top_p: The cumulative probability of parameter highest probability vocabulary tokens to keep for nucleus sampling.
+            top_k: The number of highest probability vocabulary tokens to keep for top-k-filtering.
+            do_sample: Whether or not to use sampling ; use greedy decoding otherwise.
+            repetition_penalty: The parameter for repetition penalty. 1.0 means no penalty.
+            length_penalty: The parameter that penalizes longer sequences.
+            num_beams: The number of beams to use for beam search. 1 means no beam search.
+            num_return_sequences: The number of independently computed returned sequences for each element in the batch.
+            **kwargs: Additional arguments for generating sequences.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if self.device == 'cpu':
             self.model.float()
@@ -510,102 +526,108 @@
                 [
                     sentences[i: i + self.args.eval_batch_size]
                     for i in range(0, len(sentences), self.args.eval_batch_size)
                 ],
                 desc="Generating outputs",
                 disable=self.args.silent,
         ):
-            inputs = self.tokenizer(batch, padding=True, return_tensors='pt').to(self.device)
+            if add_system_prompt:
+                batch = [PROMPT_DICT['prompt_no_input'].format(instruction=s) for s in batch]
+            inputs = self.tokenizer(batch, padding=True, return_tensors='pt')
             generation_config = GenerationConfig(
                 max_new_tokens=max_length if max_length else self.args.max_length,
-                temperature=self.args.temperature,
-                top_p=self.args.top_p,
-                top_k=self.args.top_k,
-                do_sample=self.args.do_sample,
-                repetition_penalty=self.args.repetition_penalty,
-                length_penalty=self.args.length_penalty,
-                num_beams=self.args.num_beams,
+                temperature=temperature if temperature is not None else self.args.temperature,
+                top_p=top_p if top_p else self.args.top_p,
+                top_k=top_k if top_k else self.args.top_k,
+                do_sample=do_sample if do_sample is not None else self.args.do_sample,
+                repetition_penalty=repetition_penalty if repetition_penalty else self.args.repetition_penalty,
+                length_penalty=length_penalty if length_penalty else self.args.length_penalty,
+                num_beams=num_beams if num_beams else self.args.num_beams,
                 eos_token_id=self.tokenizer.eos_token_id,
                 pad_token_id=self.tokenizer.pad_token_id,
-                num_return_sequences=self.args.num_return_sequences,
+                num_return_sequences=num_return_sequences if num_return_sequences else self.args.num_return_sequences,
                 return_dict_in_generate=True,
                 output_scores=True,
                 **kwargs,
             )
-            outputs = self.model.generate(**inputs, generation_config=generation_config)
+            outputs = self.model.generate(
+                input_ids=inputs['input_ids'].to(self.device),
+                generation_config=generation_config
+            )
             for idx, (prompt_text, generated_sequence) in enumerate(zip(batch, outputs.sequences)):
                 # Decode text
                 text = self.tokenizer.decode(generated_sequence, skip_special_tokens=True)
                 prompt_len = len(prompt_text)
                 gen_text = text[prompt_len:]
                 if keep_prompt:
                     total_sequence = prompt_text + gen_text
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
         return all_outputs
 
-    @torch.no_grad()
-    def chat(self, query: str, history: List[Tuple[str, str]] = None,
-             keep_prompt: bool = False, max_length: int = 128, **kwargs):
+    @torch.inference_mode()
+    def chat(
+            self,
+            query: str,
+            history: List[Tuple[str, str]] = None,
+            keep_prompt: bool = False,
+            add_system_prompt=True,
+            max_length: int = 2048,
+            **kwargs
+    ):
         """
         Chat with the model
         :param query:
         :param history:
         :param keep_prompt:
         :param max_length:
+        :param add_system_prompt:
         :param kwargs:
         :return: response, history
         """
         if history is None:
             history = []
         if not history:
             prompt = query
         else:
             prompt = ""
-            for i, (old_query, response) in enumerate(history):
-                prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
-            prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
+            for i, (q, a) in enumerate(history):
+                prompt += "\n### Human: {}\n### Assistant: {}\n".format(q, a)
+            prompt += "\n### Human: {}\n### Assistant: ".format(query)
+        if add_system_prompt:
+            prompt = PROMPT_DICT['prompt_multi_round_no_input'].format(instruction=prompt, output_text="")
         response = self.predict([prompt], keep_prompt=keep_prompt, max_length=len(prompt) + max_length, **kwargs)[0]
         history = history + [(query, response)]
         return response, history
 
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
-        Creates a BloomDataset from data.
+        Creates a LlamaDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
         """
 
         tokenizer = self.tokenizer
         args = self.args
 
         if not no_cache:
             no_cache = args.no_cache
 
         if not no_cache:
             os.makedirs(self.args.cache_dir, exist_ok=True)
 
         mode = "dev" if evaluate else "train"
-
-        if self.args.use_hf_datasets:
-            dataset = load_hf_dataset(data, tokenizer, self.args, mode)
-            return dataset
-        elif args.dataset_class:
+        if args.dataset_class:
             CustomDataset = args.dataset_class
             return CustomDataset(tokenizer, args, data, mode)
         else:
-            return BloomDataset(
-                tokenizer,
-                self.args,
-                data,
-                mode,
-            )
+            return InstructionDataset(tokenizer, args, data, mode)
 
     def save_model(
             self, output_dir=None, optimizer=None, scheduler=None, model=None, results=None
     ):
         """Save the model and the tokenizer."""
         if not output_dir:
             output_dir = self.args.output_dir
@@ -628,22 +650,22 @@
             self.save_model_args(output_dir)
 
     def save_model_args(self, output_dir):
         os.makedirs(output_dir, exist_ok=True)
         self.args.save(output_dir)
 
     def _load_model_args(self, input_dir):
-        args = BloomArgs()
+        args = GptArgs()
         args.load(input_dir)
         return args
 
 
 class SavePeftModelTrainer(Trainer):
     """
-    Trainer for save models
+    Trainer for lora models
     """
 
     def save_model(self, output_dir=None, _internal_call=False):
         """Save the LoRA model."""
         os.makedirs(output_dir, exist_ok=True)
         torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
         self.model.save_pretrained(output_dir)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `textgen-0.2.7/textgen/bloom/bloom_utils.py` & `textgen-1.0.0/textgen/gpt/gpt_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,127 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
-
 import os
 import pickle
-from multiprocessing import Pool
+import re
 
 import datasets
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
 from loguru import logger
 from torch.utils.data import Dataset
-from tqdm.auto import tqdm
 
 PROMPT_DICT = {
     "prompt_input": (
         "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
-        "### Instruction:\n{instruction}\n{input_text}\n\n### Response:"
+        "### Instruction:\n{instruction}\n{input_text}\n\n### Response: "
     ),
     "prompt_no_input": (
         "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
-        "### Instruction:\n{instruction}\n\n### Response:"
+        "### Instruction:\n{instruction}\n\n### Response: "
     ),
-    "prompt_multiround_input": (
+    "prompt_multi_round_no_input": (
         "Below is an multi-round dialogue between human and assistant. "
         "Write a response as an assistant that appropriately completes the human request in each round by incorporating previous context.\n\n"
-        "{instruction}"
+        "{instruction}{output_text}"
     ),
 }
 
 
+def generate_prompt(instruction, input_text, output_text):
+    """Generate prompt for instruction."""
+    if 'Human:' in instruction and 'Assistant:' in instruction:
+        instruction = instruction.replace('Human:', '### Human:')
+        instruction = instruction.replace('Assistant:', '### Assistant:')
+        prompt = PROMPT_DICT['prompt_multi_round_no_input'].format(instruction=instruction, output_text=output_text)
+        return prompt, 'multi_round'
+    else:
+        if input_text:
+            prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
+        else:
+            prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
+        return prompt, 'single_round'
+
+
 def preprocess_data(data):
     instruction, input_text, target_text, tokenizer, args = data
+    IGNORE_INDEX = -100
+    EOS_TOKEN = tokenizer.eos_token
+    full_max_length = args.max_seq_length + args.max_length
 
-    if input_text:
-        prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
+    prompt, round_type = generate_prompt(instruction, input_text, target_text)
+    if round_type == 'multi_round':
+        prompt = re.sub(r'(?<!\n)\n### ', f'\n{EOS_TOKEN}### ', prompt)
+        prompt += EOS_TOKEN
+        example = tokenizer(prompt, max_length=full_max_length, truncation=True, padding=False)
+        labels = example['input_ids'].copy()
+
+        if not args.is_train_on_prompt:
+            source_len = len(tokenizer(
+                PROMPT_DICT['prompt_multi_round_no_input'].split('\n\n')[0] + '\n\n')['input_ids'])
+            labels[:source_len] = [IGNORE_INDEX] * source_len
+            input_tokens = tokenizer.convert_ids_to_tokens(example["input_ids"])
+            matches = re.finditer(r'### (?!Assistant:)(.*?)</s>', prompt, re.DOTALL)
+            for match in matches:
+                start_pos, end_pos = match.span()
+                start_idx = None
+                end_idx = None
+                current_pos = 0
+                current_idx = 0
+
+                while current_pos < start_pos:
+                    current_pos += len(input_tokens[current_idx]) + 1
+                    current_idx += 1
+                start_idx = current_idx
+
+                while current_pos < end_pos:
+                    current_pos += len(input_tokens[current_idx]) + 1
+                    current_idx += 1
+                end_idx = current_idx - 1
+
+                if start_idx is not None and end_idx is not None:
+                    for i in range(start_idx, end_idx - 1):
+                        labels[i] = IGNORE_INDEX
+        # Padding labels to full max length
+        example['labels'] = [IGNORE_INDEX] * (full_max_length - len(labels)) + labels
     else:
-        prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
-
-    full_prompt = prompt + target_text + tokenizer.eos_token
-    full_max_length = args.max_seq_length + args.max_length
-    example = tokenizer(
-        full_prompt,
-        truncation=True,
-        max_length=full_max_length,
-        padding=False,
-        add_special_tokens=False
-    )
-    example["labels"] = example["input_ids"].copy()
-    if not args.is_train_on_prompt:
-        user_example = tokenizer(
-            prompt,
+        full_prompt = prompt + target_text + tokenizer.eos_token
+        example = tokenizer(
+            full_prompt,
             truncation=True,
-            max_length=args.max_seq_length,
+            max_length=full_max_length,
             padding=False,
             add_special_tokens=False
         )
-        user_prompt_len = len(user_example["input_ids"])
-        # set labels to full max length to adjust for DataCollatorForSeq2Seq padding
-        example["labels"] = [-100] * (full_max_length - len(example['labels']) + user_prompt_len) + \
-                            example["labels"][user_prompt_len:]
-
-    return example
+        example["labels"] = example["input_ids"].copy()
+        if not args.is_train_on_prompt:
+            user_example = tokenizer(
+                prompt,
+                truncation=True,
+                max_length=args.max_seq_length,
+                padding=False,
+                add_special_tokens=False
+            )
+            user_prompt_len = len(user_example["input_ids"])
+            # Padding labels to full max length to equalize the length of input_ids after collator
+            example["labels"] = [IGNORE_INDEX] * (full_max_length - len(example['labels']) + user_prompt_len) + \
+                                example["labels"][user_prompt_len:]
+    return {"input_ids": example['input_ids'], "labels": example["labels"]}
 
 
-def preprocess_batch_for_hf_dataset(example, tokenizer, args):
+def preprocess_batch_for_hf_instruction_dataset(example, tokenizer, args):
     data = (example["instruction"], example["input"], example["output"], tokenizer, args)
     example = preprocess_data(data)
     return example
 
 
-def load_hf_dataset(data, tokenizer, args, mode):
+def load_hf_instruction_dataset(tokenizer, args, data, mode):
     if isinstance(data, str):
         if data.endswith('.json') or data.endswith('.jsonl'):
             dataset = load_dataset("json", data_files=data)
         elif os.path.isdir(data):
             dataset = datasets.load_from_disk(data)
         else:
             dataset = load_dataset(
@@ -90,22 +135,22 @@
         if mode == 'dev' and args.max_eval_samples is not None:
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
     dataset = dataset.shuffle().map(
-        lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
+        lambda x: preprocess_batch_for_hf_instruction_dataset(x, tokenizer=tokenizer, args=args),
         batched=False, remove_columns=dataset.column_names
     ).filter(lambda x: len(x['input_ids']) > 0)
 
     return dataset
 
 
-class BloomDataset(Dataset):
+class InstructionDataset(Dataset):
     def __init__(self, tokenizer, args, data, mode):
         cached_features_file = os.path.join(
             args.cache_dir,
             args.model_name.replace("/", "_")
             + "_cached_"
             + str(args.max_seq_length)
             + str(len(data)),
@@ -115,41 +160,17 @@
                 (not args.reprocess_input_data and not args.no_cache)
                 or (mode == "dev" and args.use_cached_eval_features and not args.no_cache)
         ):
             logger.info(" Loading features from cached file %s" % cached_features_file)
             with open(cached_features_file, "rb") as handle:
                 self.examples = pickle.load(handle)
         else:
-            logger.info(" Creating features from dataset file at %s" % args.cache_dir)
+            logger.debug(" Creating features from dataset file at %s" % args.cache_dir)
 
-            data = [
-                (instruction, input_text, target_text, tokenizer, args)
-                for instruction, input_text, target_text in zip(
-                    data["instruction"], data["input"], data["output"]
-                )
-            ]
-
-            if (mode == "train" and args.use_multiprocessing) or (
-                    mode == "dev" and args.use_multiprocessing_for_evaluation
-            ):
-                if args.multiprocessing_chunksize == -1:
-                    chunksize = max(len(data) // (args.process_count * 2), 500)
-                else:
-                    chunksize = args.multiprocessing_chunksize
-
-                with Pool(args.process_count) as p:
-                    self.examples = list(
-                        tqdm(
-                            p.imap(preprocess_data, data, chunksize=chunksize),
-                            total=len(data),
-                            disable=args.silent,
-                        )
-                    )
-            else:
-                self.examples = [preprocess_data(d) for d in tqdm(data, disable=args.silent)]
+            self.examples = list(load_hf_instruction_dataset(tokenizer, args, data, mode))
             if not args.no_cache:
                 logger.info(" Saving features into cached file %s" % cached_features_file)
                 with open(cached_features_file, "wb") as handle:
                     pickle.dump(self.examples, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     def __len__(self):
         return len(self.examples)
```

### Comparing `textgen-0.2.7/textgen/chatglm/chatglm_model.py` & `textgen-1.0.0/textgen/chatglm/chatglm_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,42 +3,49 @@
 @author:XuMing(xuming624@qq.com)
 @description:
 """
 import math
 import os
 import random
 import re
-import sys
 from typing import List, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from loguru import logger
 from peft import (
     get_peft_model,
     LoraConfig,
     TaskType,
     PeftModel,
     prepare_model_for_int8_training,
     set_peft_model_state_dict,
 )
-from tqdm.auto import tqdm
-from transformers import Trainer, TrainingArguments, AutoTokenizer, AutoModel, AutoConfig
+from tqdm import tqdm
+from transformers import (
+    Trainer,
+    TrainingArguments,
+    AutoTokenizer,
+    AutoModel,
+    DataCollatorForSeq2Seq,
+    BitsAndBytesConfig,
+    deepspeed,
+)
 from transformers.trainer import TRAINING_ARGS_NAME
 
-from textgen.chatglm.chatglm_utils import load_hf_dataset, ChatGlmDataset
+from textgen.chatglm.chatglm_utils import ChatGlmDataset, PROMPT_DICT
 from textgen.config.model_args import ChatGlmArgs
 
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
-    "chatglm": (AutoConfig, AutoModel, AutoTokenizer),
+    "chatglm": (AutoModel, AutoTokenizer),
 }
 
 
 class ChatGlmModel:
     def __init__(
             self,
             model_type="chatglm",
@@ -88,43 +95,49 @@
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
             if torch.backends.mps.is_available():
                 self.device = torch.device("mps")
+                self.device_map = {"": "mps"}
             else:
                 self.device = "cpu"
                 self.device_map = {"": "cpu"}
         logger.debug(f"Device: {self.device}")
         if self.device == "cpu":
             self.args.fp16 = False
             self.args.int8 = False
 
         world_size = int(os.environ.get("WORLD_SIZE", 1))
         self.ddp = world_size != 1
         if self.ddp:
             self.device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
 
         self.results = {}
-        config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
+        model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
-        config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, **kwargs)
 
         if torch.cuda.is_bf16_supported() and not self.args.bf16:
             logger.warning("GPU supports bf16, you can enable bf16.")
         self.torch_dtype = torch.bfloat16 if self.args.bf16 else (torch.float16 if self.args.fp16 else torch.float32)
         self.model = model_class.from_pretrained(
             model_name,
-            config=config,
-            trust_remote_code=True,
             load_in_8bit=self.args.int8,
             torch_dtype=self.torch_dtype,
             device_map=self.device_map,
+            trust_remote_code=True,
+            quantization_config=BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_compute_dtype=self.torch_dtype,
+            ) if self.args.qlora else None,
+            **kwargs,
         )
 
         if self.args.int8 or self.args.int4:
             quantization_bit = 8 if self.args.int8 else 4
             logger.debug(f"Quantized to {quantization_bit} bit")
             self.model = self.model.quantize(quantization_bit)
         self.tokenizer_class = tokenizer_class
@@ -137,44 +150,26 @@
         self.args.model_type = model_type
         if model_name is None:
             self.args.model_name = "ChatGLM_from_scratch"
         else:
             self.args.model_name = model_name
 
         self.peft_name = peft_name
-        if self.args.use_peft:
+        if self.args.use_peft and self.peft_name:
             self.load_peft_model()
 
-    def data_collator(self, batch):
-        """
-        Data collator that will dynamically pad the inputs received.
-            set padding side = left, pad on the left side of the sequences
-            if chat task, set prompt ids to -100 of the labels
-            if not, set labels = input_ids
-        """
-        len_ids = [len(example) for example in batch]
-        longest = max(len_ids)
-        input_ids = []
-        labels_list = []
-        for ids_l, example in sorted(zip(len_ids, batch), key=lambda x: -x[0]):
-            ids = list(example)
-            seq_len = ids.index(self.tokenizer.bos_token_id) + 1  # is equal to prompt length
-            pad_ids = ids + [self.tokenizer.pad_token_id] * (longest - ids_l)
-            tensor_ids = torch.LongTensor(pad_ids)
-            if not self.args.is_train_on_prompt:
-                labels = ([-100] * (seq_len - 1) + ids[(seq_len - 1):] + [-100] * (longest - ids_l))
-                labels = torch.LongTensor(labels)
-            else:
-                labels = tensor_ids
-
-            input_ids.append(tensor_ids)
-            labels_list.append(labels)
-        input_ids = torch.stack(input_ids)
-        labels = torch.stack(labels_list)
-        return {"input_ids": input_ids, "labels": labels}
+    def load_peft_model(self):
+        """Load peft model."""
+        self.model = PeftModel.from_pretrained(
+            self.model,
+            self.peft_name,
+            torch_dtype=self.torch_dtype,
+            device_map=self.device_map,
+        )
+        logger.info(f"Loaded peft model from {self.peft_name}")
 
     def find_all_linear_names(self, int4=False, int8=False):
         cls = torch.nn.Linear
         if int4 or int8:
             import bitsandbytes as bnb
             if int4:
                 cls = bnb.nn.Linear4bit
@@ -235,26 +230,50 @@
                 and os.listdir(output_dir)
                 and not self.args.overwrite_output_dir
         ):
             raise ValueError(
                 "Output directory ({}) already exists and is not empty."
                 " Set args.overwrite_output_dir = True to overcome.".format(output_dir)
             )
-        # update model train config
-        self.model.gradient_checkpointing_enable()
-        self.model.enable_input_require_grads()
-        if torch.cuda.device_count() > 1:
-            self.model.is_parallelizable = True
-            self.model.model_parallel = True
-        self.model.lm_head = CastOutputToFloat(self.model.lm_head)
-        self.model.config.use_cache = False
+
+        # Setup train args
+        training_args = TrainingArguments(
+            output_dir=output_dir,
+            learning_rate=self.args.learning_rate,
+            num_train_epochs=self.args.num_train_epochs,
+            logging_dir=f"{output_dir}/logs",
+            logging_steps=self.args.logging_steps,
+            max_steps=self.args.max_steps,
+            per_device_train_batch_size=self.args.per_device_train_batch_size,
+            per_device_eval_batch_size=self.args.per_device_train_batch_size,
+            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
+            gradient_checkpointing=self.args.gradient_checkpointing,
+            torch_compile=self.args.torch_compile,
+            warmup_steps=self.args.warmup_steps,
+            save_steps=self.args.save_steps,
+            optim=self.args.optimizer,
+            save_strategy=self.args.save_strategy,
+            evaluation_strategy='steps' if eval_data is not None else 'no',
+            eval_steps=self.args.eval_steps if eval_data is not None else None,
+            load_best_model_at_end=True if eval_data is not None else False,
+            ddp_find_unused_parameters=False if self.ddp else None,
+            save_total_limit=self.args.save_total_limit,
+            fp16=self.args.fp16,
+            bf16=self.args.bf16,
+            remove_unused_columns=self.args.remove_unused_columns,
+            report_to=self.args.report_to,
+            overwrite_output_dir=self.args.overwrite_output_dir,
+            no_cuda=True if self.device == "cpu" else False,
+            **kwargs
+        )
         resume_from_checkpoint = self.args.resume_from_checkpoint
+        if self.args.qlora and (len(training_args.fsdp) > 0 or deepspeed.is_deepspeed_zero3_enabled()):
+            logger.warning("FSDP and ZeRO3 are both currently incompatible with QLoRA.")
         if 'all' in self.args.lora_target_modules:
             self.args.lora_target_modules = self.find_all_linear_names(self.args.int4, self.args.int8)
-
         # setup peft
         if self.args.use_peft:
             peft_type = self.args.peft_type.upper()
             logger.info(f"Using PEFT type: {peft_type}")
             # add peft config
             if peft_type == 'LORA':
                 logger.debug(f"Using list modules for LoRA: {self.args.lora_target_modules}")
@@ -338,162 +357,117 @@
                         resume_from_checkpoint, "adapter_model.bin")  # only LoRA model - LoRA config above has to fit
                     resume_from_checkpoint = (
                         False  # So the trainer won't try loading its state
                     )
                 # The two files above have a different name depending on how they were saved, but are actually the same.
                 if os.path.exists(checkpoint_name):
                     logger.info(f"Restarting from {checkpoint_name}")
-                    adapters_weights = torch.load(checkpoint_name)
+                    adapters_weights = torch.load(checkpoint_name, map_location='cpu')
                     set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
         else:
             logger.warning("Now full model params fine-tune, which is slow, set `use_peft=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
+        logger.debug(f"Tokenizer: {self.tokenizer}")
+        logger.debug(f"Model: {self.model}")
 
         # load dataset
         train_dataset = self.load_and_cache_examples(train_data)
         if verbose:
             logger.debug(f"train_dataset len: {len(train_dataset)}, train_dataset[0]: {train_dataset[0]}")
+            logger.debug(f"text of train_dataset[0]: {self.tokenizer.decode(train_dataset[0]['input_ids'])}")
         eval_dataset = None
         if eval_data is not None:
             eval_dataset = self.load_and_cache_examples(eval_data, evaluate=True)
             if verbose:
                 logger.debug(f"eval_dataset len: {len(eval_dataset)}, eval_dataset[0]: {eval_dataset[0]}")
 
-        # start train
-        training_args = TrainingArguments(
-            output_dir=output_dir,
-            learning_rate=self.args.learning_rate,
-            num_train_epochs=self.args.num_train_epochs,
-            logging_dir=f"{output_dir}/logs",
-            logging_steps=self.args.logging_steps,
-            max_steps=self.args.max_steps,
-            per_device_train_batch_size=self.args.per_device_train_batch_size,
-            per_device_eval_batch_size=self.args.per_device_train_batch_size,
-            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
-            warmup_steps=self.args.warmup_steps,
-            save_steps=self.args.save_steps,
-            optim=self.args.optimizer,
-            save_strategy=self.args.save_strategy,
-            evaluation_strategy='steps' if eval_data is not None else 'no',
-            eval_steps=self.args.eval_steps if eval_data is not None else None,
-            load_best_model_at_end=True if eval_data is not None else False,
-            ddp_find_unused_parameters=False if self.ddp else None,
-            save_total_limit=self.args.save_total_limit,
-            fp16=self.args.fp16,
-            bf16=self.args.bf16,
-            remove_unused_columns=self.args.remove_unused_columns,
-            report_to=self.args.report_to,
-            overwrite_output_dir=self.args.overwrite_output_dir,
-            no_cuda=True if self.device == "cpu" else False,
-            **kwargs
-        )
         # Log on each process the small summary:
         logger.warning(
             f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
             + f"distributed training: {bool(training_args.local_rank != -1)}, 16-bits training: {training_args.fp16}"
         )
         if training_args.local_rank <= 0:
             logger.info(f"Training/evaluation parameters {training_args}")
 
+        # Update model train config
+        if self.args.gradient_checkpointing:
+            self.model.gradient_checkpointing_enable()
+            self.model.config.use_cache = False
+        else:
+            self.model.config.use_cache = True
+        self.model.enable_input_require_grads()
+        if torch.cuda.device_count() > 1:
+            # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
+            self.model.is_parallelizable = True
+            self.model.model_parallel = True
+        self.model.lm_head = CastOutputToFloat(self.model.lm_head)
+
+        data_collator = DataCollatorForSeq2Seq(
+            self.tokenizer,
+            return_tensors="pt",
+            padding="max_length",
+            max_length=self.args.max_seq_length + self.args.max_length
+        )
         if self.args.use_peft:
             trainer = SavePeftModelTrainer(
                 model=self.model,
                 train_dataset=train_dataset,
                 eval_dataset=eval_dataset if eval_data is not None else None,
                 args=training_args,
                 tokenizer=self.tokenizer,
-                data_collator=self.data_collator,
+                data_collator=data_collator,
             )
         else:
             trainer = Trainer(
                 model=self.model,
                 train_dataset=train_dataset,
                 eval_dataset=eval_dataset if eval_data is not None else None,
                 args=training_args,
                 tokenizer=self.tokenizer,
-                data_collator=self.data_collator,
+                data_collator=data_collator,
             )
 
-        if self.args.enable_torch_compile and torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
-
+        # Training
         logger.info("*** Train ***")
+        logger.debug(f"Train dataloader example: {next(iter(trainer.get_train_dataloader()))}")
         (global_step, training_loss, metrics) = trainer.train(resume_from_checkpoint=resume_from_checkpoint)
-        self.handle_metrics("train", metrics, output_dir)
         self.results.update(metrics)
+        trainer.log_metrics("train", metrics)
+        trainer.save_metrics("train", metrics)
+        trainer.save_state()
         self.save_model(model=self.model)
 
         if eval_data is not None:
             logger.info("*** Evaluate ***")
             if self.args.fp16:
                 self.model.half()
             metrics = trainer.evaluate(metric_key_prefix="eval")
             try:
                 perplexity = math.exp(metrics["eval_loss"])
             except OverflowError:
                 perplexity = float("inf")
             metrics["perplexity"] = perplexity
             logger.debug(f"eval metrics: {metrics}")
-            self.handle_metrics("eval", metrics, output_dir)
             self.results.update(metrics)
+            trainer.log_metrics("eval", metrics)
+            trainer.save_metrics("eval", metrics)
 
         if verbose and training_args.local_rank <= 0:
             logger.debug(f"metrics: {self.results}")
             logger.info(
                 " Training of {} model complete. Saved to {}.".format(
                     self.args.model_name, output_dir
                 )
             )
         return global_step, training_loss
 
-    @staticmethod
-    def handle_metrics(split, metrics, output_dir):
-        """
-        Log and save metrics
-
-        Args:
-        - split: one of train, val, test
-        - metrics: metrics dict
-        - output_dir: where to save the metrics
-        """
-
-        logger.info(f"***** {split} metrics *****")
-        for key in sorted(metrics.keys()):
-            logger.info(f"  {key} = {metrics[key]}")
-        output_file = os.path.join(output_dir, f"{split}_results.txt")
-        with open(output_file, "w") as writer:
-            for key in sorted(metrics.keys()):
-                writer.write("{} = {}\n".format(key, str(metrics[key])))
-
-    def load_peft_model(self):
-        """Load peft model."""
-        if self.peft_name:
-            self.model = PeftModel.from_pretrained(
-                self.model,
-                self.peft_name,
-                torch_dtype=self.torch_dtype,
-                device_map=self.device_map,
-            )
-            logger.info(f"Loaded peft model from {self.peft_name}")
-        else:
-            # Load peft model from output_dir
-            peft_path = os.path.join(self.args.output_dir, self.args.peft_bin_name)
-            if peft_path and os.path.exists(peft_path):
-                self.model = PeftModel.from_pretrained(
-                    self.model,
-                    self.args.output_dir,
-                    torch_dtype=self.torch_dtype,
-                    device_map=self.device_map,
-                )
-                logger.info(f"Loaded peft model from {peft_path}")
-
     def process_response(self, response):
         """Process response text."""
         response = response.strip()
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
@@ -501,23 +475,48 @@
             ["\\?", "？"],
         ]
         for item in punkts:
             response = re.sub(r"([\u4e00-\u9fff])%s" % item[0], r"\1%s" % item[1], response)
             response = re.sub(r"%s([\u4e00-\u9fff])" % item[0], r"%s\1" % item[1], response)
         return response
 
-    @torch.no_grad()
-    def predict(self, sentences: List[str], keep_prompt: bool = False, max_length: int = None, **kwargs):
+    @torch.inference_mode()
+    def predict(
+            self,
+            sentences: List[str],
+            keep_prompt: bool = False,
+            add_system_prompt=False,
+            max_length: int = 256,
+            temperature: float = 0.95,
+            top_p: float = 0.7,
+            top_k: int = 40,
+            do_sample: bool = True,
+            repetition_penalty: float = 1.0,
+            length_penalty: float = 2.0,
+            num_beams: int = 1,
+            num_return_sequences: int = 1,
+            **kwargs
+    ) -> List[str]:
         """
         Performs predictions on a list of text.
 
         Args:
             sentences: A python list of text (str) to be sent to the model for prediction. 
             keep_prompt: Whether to keep the prompt in the generated text.
+            add_system_prompt: Whether to add the system prompt to the prompt text.
             max_length: The maximum length of the generated text.
+            temperature: The value used to module the next token probabilities.
+            top_p: The cumulative probability of parameter highest probability vocabulary tokens to keep for nucleus sampling.
+            top_k: The number of highest probability vocabulary tokens to keep for top-k-filtering.
+            do_sample: Whether or not to use sampling ; use greedy decoding otherwise.
+            repetition_penalty: The parameter for repetition penalty. 1.0 means no penalty.
+            length_penalty: The parameter that penalizes longer sequences.
+            num_beams: The number of beams to use for beam search. 1 means no beam search.
+            num_return_sequences: The number of independently computed returned sequences for each element in the batch.
+            **kwargs: Additional arguments for generating sequences.
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if self.device == 'cpu':
             self.model.float()
@@ -531,27 +530,29 @@
                 [
                     sentences[i: i + self.args.eval_batch_size]
                     for i in range(0, len(sentences), self.args.eval_batch_size)
                 ],
                 desc="Generating outputs",
                 disable=self.args.silent,
         ):
+            if add_system_prompt:
+                batch = [PROMPT_DICT['prompt_no_input'].format(instruction=s) for s in batch]
             inputs = self.tokenizer(batch, padding=True, return_tensors='pt').to(self.device)
             gen_kwargs = {
                 "max_new_tokens": max_length if max_length else self.args.max_length,
-                "temperature": self.args.temperature,
-                "top_p": self.args.top_p,
-                "top_k": self.args.top_k,
-                "do_sample": self.args.do_sample,
-                "repetition_penalty": self.args.repetition_penalty,
-                "length_penalty": self.args.length_penalty,
-                "num_beams": self.args.num_beams,
+                "temperature": temperature if temperature is not None else self.args.temperature,
+                "top_p": top_p if top_p else self.args.top_p,
+                "top_k": top_k if top_k else self.args.top_k,
+                "do_sample": do_sample if do_sample is not None else self.args.do_sample,
+                "repetition_penalty": repetition_penalty if repetition_penalty else self.args.repetition_penalty,
+                "length_penalty": length_penalty if length_penalty else self.args.length_penalty,
+                "num_beams": num_beams if num_beams else self.args.num_beams,
                 "eos_token_id": self.tokenizer.eos_token_id,
                 "pad_token_id": self.tokenizer.pad_token_id,
-                "num_return_sequences": self.args.num_return_sequences,
+                "num_return_sequences": num_return_sequences if num_return_sequences else self.args.num_return_sequences,
                 **kwargs
             }
             outputs = self.model.generate(**inputs, **gen_kwargs)
             for idx, (prompt_text, generated_sequence) in enumerate(zip(batch, outputs)):
                 # Decode text
                 text = self.tokenizer.decode(generated_sequence)
                 prompt_len = len(prompt_text)
@@ -560,39 +561,100 @@
                 if keep_prompt:
                     total_sequence = prompt_text + gen_text
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
         return all_outputs
 
-    @torch.no_grad()
-    def chat(self, query: str, history: List[Tuple[str, str]] = None,
-             keep_prompt: bool = False, max_length: int = 128, **kwargs):
+    @torch.inference_mode()
+    def chat(
+            self,
+            query: str,
+            history: List[Tuple[str, str]] = None,
+            keep_prompt: bool = False,
+            add_system_prompt=True,
+            max_length: int = 2048,
+            **kwargs
+    ):
         """
         Chat with the model
         :param query:
         :param history:
         :param keep_prompt:
         :param max_length:
+        :param add_system_prompt:
         :param kwargs:
         :return: response, history
         """
         if history is None:
             history = []
         if not history:
             prompt = query
         else:
             prompt = ""
-            for i, (old_query, response) in enumerate(history):
-                prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
-            prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
-        response = self.predict([prompt], keep_prompt=keep_prompt, max_length=len(prompt) + max_length, **kwargs)[0]
+            for i, (q, a) in enumerate(history):
+                prompt += "\n### Human: {}\n### Assistant: {}\n".format(q, a)
+            prompt += "\n### Human: {}\n### Assistant: ".format(query)
+        if add_system_prompt:
+            prompt = PROMPT_DICT['prompt_multi_round_no_input'].format(instruction=prompt, output_text="")
+        response = self.predict([prompt], keep_prompt=keep_prompt, max_length=max_length, **kwargs)[0]
         history = history + [(query, response)]
         return response, history
 
+    @torch.inference_mode()
+    def stream_chat(
+            self,
+            query: str,
+            history: List[Tuple[str, str]] = None,
+            add_system_prompt=True,
+            max_length: int = 2048,
+            temperature: float = 0.95,
+            top_p: float = 0.7,
+            top_k: int = 40,
+            do_sample: bool = True,
+            repetition_penalty: float = 1.0,
+            length_penalty: float = 2.0,
+            num_beams: int = 1,
+            num_return_sequences: int = 1,
+            **kwargs
+    ):
+        """Chat with the model in a streaming fashion"""
+        if history is None:
+            history = []
+        gen_kwargs = {
+            "max_new_tokens": max_length if max_length else self.args.max_length,
+            "temperature": temperature if temperature is not None else self.args.temperature,
+            "top_p": top_p if top_p else self.args.top_p,
+            "top_k": top_k if top_k else self.args.top_k,
+            "do_sample": do_sample if do_sample is not None else self.args.do_sample,
+            "repetition_penalty": repetition_penalty if repetition_penalty else self.args.repetition_penalty,
+            "length_penalty": length_penalty if length_penalty else self.args.length_penalty,
+            "num_beams": num_beams if num_beams else self.args.num_beams,
+            "eos_token_id": self.tokenizer.eos_token_id,
+            "pad_token_id": self.tokenizer.pad_token_id,
+            "num_return_sequences": num_return_sequences if num_return_sequences else self.args.num_return_sequences,
+            **kwargs
+        }
+        if not history:
+            prompt = query
+        else:
+            prompt = ""
+            for i, (q, a) in enumerate(history):
+                prompt += "\n### Human: {}\n### Assistant: {}\n".format(q, a)
+            prompt += "\n### Human: {}\n### Assistant: ".format(query)
+        if add_system_prompt:
+            prompt = PROMPT_DICT['prompt_multi_round_no_input'].format(instruction=prompt, output_text="")
+        inputs = self.tokenizer([prompt], return_tensors="pt").to(self.device)
+        for outputs in self.model.stream_generate(**inputs, **gen_kwargs):
+            outputs = outputs.tolist()[0][len(inputs["input_ids"][0]):]
+            response = self.tokenizer.decode(outputs)
+            response = self.process_response(response)
+            new_history = history + [(query, response)]
+            yield response, new_history
+
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
         Creates a ChatGLMDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
@@ -605,27 +667,19 @@
             no_cache = args.no_cache
 
         if not no_cache:
             os.makedirs(self.args.cache_dir, exist_ok=True)
 
         mode = "dev" if evaluate else "train"
 
-        if self.args.use_hf_datasets:
-            dataset = load_hf_dataset(data, tokenizer, self.args, mode)
-            return dataset
-        elif args.dataset_class:
+        if args.dataset_class:
             CustomDataset = args.dataset_class
             return CustomDataset(tokenizer, args, data, mode)
         else:
-            return ChatGlmDataset(
-                tokenizer,
-                self.args,
-                data,
-                mode,
-            )
+            return ChatGlmDataset(tokenizer, args, data, mode)
 
     def save_model(
             self, output_dir=None, optimizer=None, scheduler=None, model=None, results=None
     ):
         """Save the model and the tokenizer to the `output_dir`."""
         if not output_dir:
             output_dir = self.args.output_dir
```

### Comparing `textgen-0.2.7/textgen/chatglm/chatglm_utils.py` & `textgen-1.0.0/textgen/t5/copyt5_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,163 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
-
 import os
 import pickle
 from multiprocessing import Pool
 
-import datasets
-import numpy as np
+import jieba
+import torch.nn.functional as F
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
 from loguru import logger
-from rouge import Rouge
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
+from transformers import BertTokenizer
 
+jieba.setLogLevel('ERROR')
 
-def preprocess_data(data):
-    instruction, input_text, target_text, tokenizer, args = data
 
-    prompt = f"问：{instruction}\n"
-    if input_text:
-        prompt += f"{input_text}\n"
-    prompt += "答："
-
-    prompt_ids = tokenizer.encode(prompt, max_length=args.max_seq_length, truncation=True)
-    target_ids = tokenizer.encode(target_text, max_length=args.max_length, truncation=True,
-                                  add_special_tokens=False)
-    input_ids = prompt_ids + target_ids
-    input_ids = input_ids[:(args.max_seq_length + args.max_length)] + [tokenizer.eos_token_id]
+class ZHTokenizer(BertTokenizer):
+    def __init__(self, pre_tokenizer=lambda x: jieba.cut(x, HMM=False), *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.pre_tokenizer = pre_tokenizer
+
+    def _tokenize(self, text, *arg, **kwargs):
+        split_tokens = []
+        for text in self.pre_tokenizer(text):
+            if text in self.vocab:
+                split_tokens.append(text)
+            else:
+                split_tokens.extend(super()._tokenize(text))
+        return split_tokens
+
+
+def mask_select(inputs, mask):
+    input_dim = inputs.ndim
+    mask_dim = mask.ndim
+    mask = mask.reshape(-1).bool()
+    if input_dim > mask_dim:
+        inputs = inputs.reshape((int(mask.size(-1)), -1))[mask]
+    else:
+        inputs = inputs.reshape(-1)[mask]
+    return inputs
 
-    return input_ids
+
+def copy_loss(inputs, targets, mask, eps=1e-6):
+    mask = mask[:, 1:]
+    inputs = inputs[:, :-1]
+    targets = targets[:, 1:]
+    inputs = mask_select(inputs, mask)
+    targets = mask_select(targets, mask)
+    log_preds = (inputs + eps).log()
+    loss = F.nll_loss(log_preds, targets)
+    return loss
+
+
+def ce_loss(inputs, targets, mask):
+    mask = mask[:, 1:]
+    inputs = inputs[:, :-1]
+    targets = targets[:, 1:]
+    inputs = mask_select(inputs, mask)
+    targets = mask_select(targets, mask)
+    loss = F.cross_entropy(inputs, targets)
+    return loss
 
 
 def preprocess_batch_for_hf_dataset(dataset, tokenizer, args):
-    data = (dataset["instruction"], dataset["input"], dataset["output"], tokenizer, args)
-    dataset['input_ids'] = preprocess_data(data)
-    return dataset
+    if args.preprocess_inputs:
+        return tokenizer.prepare_seq2seq_batch(
+            src_texts=[
+                prefix + ": " + input_text
+                for prefix, input_text in zip(dataset["prefix"], dataset["input_text"])
+            ],
+            tgt_texts=dataset["target_text"],
+            max_length=args.max_seq_length,
+            max_target_length=args.max_length,
+            padding="max_length",
+            return_tensors="np",
+            truncation=True,
+        )
+    else:
+        return tokenizer.prepare_seq2seq_batch(
+            src_texts=[
+                prefix + input_text
+                for prefix, input_text in zip(dataset["prefix"], dataset["input_text"])
+            ],
+            tgt_texts=dataset["target_text"],
+            max_length=args.max_seq_length,
+            max_target_length=args.max_length,
+            padding="max_length",
+            return_tensors="np",
+            truncation=True,
+        )
 
 
-def load_hf_dataset(data, tokenizer, args, mode):
+def load_hf_dataset(data, tokenizer, args):
     if isinstance(data, str):
-        if data.endswith('.json') or data.endswith('.jsonl'):
-            dataset = load_dataset("json", data_files=data)
-        elif os.path.isdir(data):
-            dataset = datasets.load_from_disk(data)
-        else:
-            dataset = load_dataset(
-                data,
-                download_mode="force_redownload"
-                if args.reprocess_input_data
-                else "reuse_dataset_if_exists",
-            )
-        # This is not necessarily a train dataset. The datasets library insists on calling it train.
-        dataset = dataset['train']
-        if mode == 'dev' and args.max_eval_samples is not None:
-            max_eval_samples = min(len(dataset), args.max_eval_samples)
-            dataset = dataset.select(range(max_eval_samples))
+        dataset = load_dataset(
+            "csv",
+            data_files=data,
+            delimiter="\t",
+            download_mode="force_redownload"
+            if args.reprocess_input_data
+            else "reuse_dataset_if_exists",
+        )
     else:
         dataset = HFDataset.from_pandas(data)
 
-    dataset = dataset.shuffle().map(
+    dataset = dataset.map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
-        batched=False, remove_columns=dataset.column_names
-    ).filter(lambda x: tokenizer.gmask_token_id in list(x['input_ids']))  # exclude samples without gmask
+        batched=True,
+    )
+
+    dataset.set_format(type="pt", columns=["input_ids", "attention_mask"])
+
+    if isinstance(data, str):
+        # This is not necessarily a train dataset. The datasets library insists on calling it train.
+        return dataset["train"]
+    else:
+        return dataset
 
-    dataset.set_format(type="np", columns=["input_ids"])
 
-    return dataset["input_ids"]
+def preprocess_data(data):
+    prefix, input_text, target_text, tokenizer, args = data
+
+    src = tokenizer(
+        [prefix + ": " + input_text],
+        padding="max_length",
+        return_tensors='pt',
+        max_length=args.max_seq_length,
+        truncation=True,
+        return_attention_mask=True,
+        return_token_type_ids=False,
+    )
+    input_ids = src["input_ids"][0]
+    attention_mask = src["attention_mask"][0]
+    with tokenizer.as_target_tokenizer():
+        tgt = tokenizer(
+            [target_text],
+            padding="max_length",
+            return_tensors='pt',
+            max_length=args.max_seq_length,
+            truncation=True,
+            return_attention_mask=True,
+            return_token_type_ids=False,
+        )
+    labels = tgt["input_ids"][0]
+    decoder_attention_mask = tgt["attention_mask"][0]
+    decoder_input_ids = tgt['input_ids'][0]
 
+    return input_ids, attention_mask, labels, decoder_attention_mask, decoder_input_ids
 
-class ChatGlmDataset(Dataset):
+
+class CopyT5Dataset(Dataset):
     def __init__(self, tokenizer, args, data, mode):
         cached_features_file = os.path.join(
             args.cache_dir,
             args.model_name.replace("/", "_")
             + "_cached_"
             + str(args.max_seq_length)
             + str(len(data)),
@@ -89,17 +170,17 @@
             logger.info(" Loading features from cached file %s" % cached_features_file)
             with open(cached_features_file, "rb") as handle:
                 self.examples = pickle.load(handle)
         else:
             logger.info(" Creating features from dataset file at %s" % args.cache_dir)
 
             data = [
-                (instruction, input_text, target_text, tokenizer, args)
-                for instruction, input_text, target_text in zip(
-                    data["instruction"], data["input"], data["output"]
+                (prefix, input_text, target_text, tokenizer, args)
+                for prefix, input_text, target_text in zip(
+                    data["prefix"], data["input_text"], data["target_text"]
                 )
             ]
 
             if (mode == "train" and args.use_multiprocessing) or (
                     mode == "dev" and args.use_multiprocessing_for_evaluation
             ):
                 if args.multiprocessing_chunksize == -1:
@@ -123,45 +204,7 @@
                     pickle.dump(self.examples, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     def __len__(self):
         return len(self.examples)
 
     def __getitem__(self, index):
         return self.examples[index]
-
-
-def compute_bleu(label, pred, weights=None):
-    from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
-    weights = weights or (0.25, 0.25, 0.25, 0.25)
-    return np.mean([sentence_bleu(references=[list(a)], hypothesis=list(b),
-                                  smoothing_function=SmoothingFunction().method1, weights=weights)
-                    for a, b in zip(label, pred)])
-
-
-def compute_rouge(label, pred, weights=None, mode='weighted'):
-    weights = weights or (0.2, 0.4, 0.4)
-    if isinstance(label, str):
-        label = [label]
-    if isinstance(pred, str):
-        pred = [pred]
-    label = [' '.join(x) for x in label]
-    pred = [' '.join(x) for x in pred]
-
-    def _compute_rouge(label, pred):
-        try:
-            scores = Rouge().get_scores(hyps=label, refs=pred)[0]
-            scores = [scores['rouge-1']['f'], scores['rouge-2']['f'], scores['rouge-l']['f']]
-        except ValueError:
-            scores = [0, 0, 0]
-        return scores
-
-    scores = np.mean([_compute_rouge(*x) for x in zip(label, pred)], axis=0)
-    if mode == 'weighted':
-        return {'rouge': sum(s * w for s, w in zip(scores, weights))}
-    elif mode == '1':
-        return {'rouge-1': scores[0]}
-    elif mode == '2':
-        return {'rouge-2': scores[1]}
-    elif mode == 'l':
-        return {'rouge-l': scores[2]}
-    elif mode == 'all':
-        return {'rouge-1': scores[0], 'rouge-2': scores[1], 'rouge-l': scores[2]}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `textgen-0.2.7/textgen/chatglm/merge_peft_adapter.py` & `textgen-1.0.0/textgen/chatglm/merge_peft_adapter.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/config/global_args.py` & `textgen-1.0.0/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/config/model_args.py` & `textgen-1.0.0/textgen/config/model_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -364,15 +364,14 @@
     num_return_sequences: int = 1
     repetition_penalty: float = 1.0
     temperature: float = 0.95
     special_tokens_list: list = field(default_factory=list)
     top_k: float = None
     top_p: float = 0.7
     model_name_or_path: Optional[str] = field(default="THUDM/chatglm-6b")
-    dataset_name_or_path: Optional[str] = field(default="shibing624/alpaca-zh")
     use_peft: bool = True
     peft_type: str = "LORA"
     peft_bin_name: str = "adapter_model.bin"
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
     lora_target_modules = ["all"]  # ["all"] or ["query_key_value"]
@@ -385,37 +384,39 @@
     num_virtual_tokens: int = 20
     prompt_encoder_hidden_size: int = 128
     num_train_epochs = 1
     max_steps = -1
     per_device_train_batch_size = 2
     eval_batch_size: int = 4
     gradient_accumulation_steps = 1
-    save_total_limit = 3
+    gradient_checkpointing: bool = True
+    torch_compile: bool = False
+    save_total_limit = 10
     remove_unused_columns = False
     logging_steps = 50
     resume_from_checkpoint: str = None
-    enable_torch_compile: bool = True
+    qlora: bool = False
 
 
 @dataclass
-class LlamaArgs(ModelArgs):
+class GptArgs(ModelArgs):
     """
-    Model args for a LlamaModel
+    Model args for a GptModel
     """
 
-    model_class: str = "LlamaArgs"
+    model_class: str = "GptArgs"
     dataset_class: Dataset = None
     learning_rate: float = 2e-5
     fp16: bool = True
     bf16: bool = False
     int8: bool = False
     int4: bool = False
     debug: bool = False
     max_seq_length: int = 256  # max length of input sequence
-    max_length = 384  # max length of the sequence to be generated
+    max_length = 256  # max length of the sequence to be generated
     do_sample: bool = True
     early_stopping: bool = True
     evaluate_generated_text: bool = True
     is_train_on_prompt: bool = False  # if compute loss with prompt labels
     warmup_steps: int = 50
     report_to = "tensorboard"
     optimizer: str = "adamw_torch"
@@ -424,104 +425,40 @@
     save_steps: int = 400
     pad_to_multiple_of: int = 8
     max_eval_samples: int = 20
     length_penalty: float = 2.0
     num_beams: int = 1
     num_return_sequences: int = 1
     repetition_penalty: float = 1.3
-    temperature: float = 0.2
+    temperature: float = 0.4
     special_tokens_list: list = field(default_factory=list)
     top_k: float = 40
     top_p: float = 0.9
-    model_name_or_path: Optional[str] = field(default="decapoda-research/llama-7b-hf")
+    model_name_or_path: Optional[str] = field(default="shibing624/chinese-alpaca-plus-7b-hf")
     use_peft: bool = True
     peft_type: str = "LORA"
     peft_bin_name: str = "adapter_model.bin"
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
-    lora_target_modules = ["all"]  # ["all"] or target module names
+    lora_target_modules = ["all"]  # ["all"] or ["k_proj"]
     lora_bias = "none"
     adalora_init_r: int = 12
     adalora_tinit: int = 200
     adalora_tfinal: int = 1000
     adalora_delta_t: int = 10
     lora_beta: float = 0.85
     num_virtual_tokens: int = 20
     prompt_encoder_hidden_size: int = 128
     num_train_epochs = 3
     max_steps = -1
     per_device_train_batch_size = 2
     eval_batch_size: int = 4
     gradient_accumulation_steps = 1
-    save_total_limit = 3
+    save_total_limit = 10
     remove_unused_columns = False
     logging_steps = 50
     resume_from_checkpoint: str = None
-    enable_torch_compile: bool = True
-    is_pretraining: bool = False
-    block_size: int = 1024
-
-
-
-@dataclass
-class BloomArgs(ModelArgs):
-    """
-    Model args for a BloomModel
-    """
-
-    model_class: str = "BloomArgs"
-    dataset_class: Dataset = None
-    learning_rate: float = 2e-5
-    fp16: bool = True
-    bf16: bool = False
-    int8: bool = False
-    int4: bool = False
-    debug: bool = False
-    max_seq_length: int = 256  # max length of input sequence
-    max_length = 384  # max length of the sequence to be generated
-    do_sample: bool = True
-    early_stopping: bool = True
-    evaluate_generated_text: bool = True
-    is_train_on_prompt: bool = False  # if compute loss with prompt labels
-    warmup_steps: int = 50
-    report_to = "tensorboard"
-    optimizer: str = "adamw_torch"
-    save_strategy: str = "steps"
-    eval_steps: int = 200
-    save_steps: int = 400
-    pad_to_multiple_of: int = 8
-    max_eval_samples: int = 20
-    length_penalty: float = 2.0
-    num_beams: int = 1
-    num_return_sequences: int = 1
-    repetition_penalty: float = 1.3
-    temperature: float = 0.2
-    special_tokens_list: list = field(default_factory=list)
-    top_k: float = 40
-    top_p: float = 0.9
-    model_name_or_path: Optional[str] = field(default="bigscience/bloomz-7b1-mt")
-    use_peft: bool = True
-    peft_type: str = "LORA"
-    peft_bin_name: str = "adapter_model.bin"
-    lora_r: int = 8
-    lora_alpha = 16
-    lora_dropout = 0.05
-    lora_target_modules = ["all"]  # ["all"] or ["query_key_value"]
-    lora_bias = "none"
-    adalora_init_r: int = 12
-    adalora_tinit: int = 200
-    adalora_tfinal: int = 1000
-    adalora_delta_t: int = 10
-    lora_beta: float = 0.85
-    num_virtual_tokens: int = 20
-    prompt_encoder_hidden_size: int = 128
-    num_train_epochs = 3
-    max_steps = -1
-    per_device_train_batch_size = 2
-    eval_batch_size: int = 4
-    gradient_accumulation_steps = 1
-    save_total_limit = 3
-    remove_unused_columns = False
-    logging_steps = 50
-    resume_from_checkpoint: str = None
-    enable_torch_compile: bool = True
+    gradient_checkpointing: bool = True
+    torch_compile: bool = False
+    trust_remote_code: bool = True
+    qlora: bool = False
```

### Comparing `textgen-0.2.7/textgen/custom_models/models.py` & `textgen-1.0.0/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/data/HowNetPOSWord.txt` & `textgen-1.0.0/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/data/stopwords.txt` & `textgen-1.0.0/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_generation/language_generation_model.py` & `textgen-1.0.0/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_generation/language_generation_utils.py` & `textgen-1.0.0/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_modeling/language_modeling_model.py` & `textgen-1.0.0/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_modeling/language_modeling_utils.py` & `textgen-1.0.0/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_modeling/songnet_model.py` & `textgen-1.0.0/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/language_modeling/songnet_utils.py` & `textgen-1.0.0/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/llama/llama_utils.py` & `textgen-1.0.0/textgen/chatglm/chatglm_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,128 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
+
 import os
 import pickle
-from itertools import chain
-from multiprocessing import Pool
+import re
 
 import datasets
+import numpy as np
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
 from loguru import logger
+from rouge import Rouge
 from torch.utils.data import Dataset
-from tqdm.auto import tqdm
 
 PROMPT_DICT = {
     "prompt_input": (
-        "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
-        "### Instruction:\n{instruction}\n{input_text}\n\n### Response:\n\n"
+        "问：{instruction}\n{input_text}\n答："
     ),
     "prompt_no_input": (
-        "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n"
-        "### Instruction:\n{instruction}\n\n### Response:\n\n"
+        "问：{instruction}\n答："
+    ),
+    "prompt_multi_round_no_input": (
+        "Below is an multi-round dialogue between human and assistant. "
+        "Write a response as an assistant that appropriately completes the human request in each round by incorporating previous context.\n\n"
+        "{instruction}{output_text}"
     ),
 }
 
 
-def preprocess_instruction_data(data):
-    instruction, input_text, target_text, tokenizer, args = data
-
-    if input_text:
-        prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
+def generate_prompt(instruction, input_text, output_text):
+    """Generate prompt for instruction."""
+    if 'Human:' in instruction and 'Assistant:' in instruction:
+        instruction = instruction.replace('Human:', '### Human:')
+        instruction = instruction.replace('Assistant:', '### Assistant:')
+        prompt = PROMPT_DICT['prompt_multi_round_no_input'].format(instruction=instruction, output_text=output_text)
+        return prompt, 'multi_round'
     else:
-        prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
+        if input_text:
+            prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
+        else:
+            prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
+        return prompt, 'single_round'
 
-    full_prompt = prompt + target_text + tokenizer.eos_token
+
+def preprocess_data(data):
+    instruction, input_text, target_text, tokenizer, args = data
+    IGNORE_INDEX = -100
+    EOS_TOKEN = tokenizer.eos_token
     full_max_length = args.max_seq_length + args.max_length
-    example = tokenizer(
-        full_prompt,
-        truncation=True,
-        max_length=full_max_length,
-        padding=False,
-        add_special_tokens=False
-    )
-    example["labels"] = example["input_ids"].copy()
-    if not args.is_train_on_prompt:
-        user_example = tokenizer(
-            prompt,
+
+    prompt, round_type = generate_prompt(instruction, input_text, target_text)
+
+    if round_type == 'multi_round':
+        prompt = re.sub(r'(?<!\n)\n### ', f'\n{EOS_TOKEN}### ', prompt)
+        prompt += EOS_TOKEN
+        example = tokenizer(prompt, max_length=full_max_length, truncation=True, padding=False)
+        labels = example['input_ids'].copy()
+        if not args.is_train_on_prompt:
+            source_len = len(tokenizer(
+                PROMPT_DICT['prompt_multi_round_no_input'].split('\n\n')[0] + '\n\n')['input_ids'])
+            labels[:source_len] = [IGNORE_INDEX] * source_len
+            input_tokens = tokenizer.convert_ids_to_tokens(example["input_ids"])
+            matches = re.finditer(r'### (?!Assistant:)(.*?)</s>', prompt, re.DOTALL)
+            for match in matches:
+                start_pos, end_pos = match.span()
+                start_idx = None
+                end_idx = None
+                current_pos = 0
+                current_idx = 0
+
+                while current_pos < start_pos:
+                    current_pos += len(input_tokens[current_idx]) + 1
+                    current_idx += 1
+                start_idx = current_idx
+
+                while current_pos < end_pos:
+                    current_pos += len(input_tokens[current_idx]) + 1
+                    current_idx += 1
+                end_idx = current_idx - 1
+
+                if start_idx is not None and end_idx is not None:
+                    for i in range(start_idx, end_idx - 1):
+                        labels[i] = IGNORE_INDEX
+        # Padding labels to full max length
+        example['labels'] = [IGNORE_INDEX] * (full_max_length - len(labels)) + labels
+    else:
+        full_prompt = prompt + target_text + tokenizer.eos_token
+        example = tokenizer(
+            full_prompt,
             truncation=True,
-            max_length=args.max_seq_length,
+            max_length=full_max_length,
             padding=False,
             add_special_tokens=False
         )
-        user_prompt_len = len(user_example["input_ids"])
-        # set labels to full max length to adjust for DataCollatorForSeq2Seq padding
-        example["labels"] = [-100] * (full_max_length - len(example['labels']) + user_prompt_len) + \
-                            example["labels"][user_prompt_len:]
-
-    return example
+        example["labels"] = example["input_ids"].copy()
+        if not args.is_train_on_prompt:
+            user_example = tokenizer(
+                prompt,
+                truncation=True,
+                max_length=args.max_seq_length,
+                padding=False,
+                add_special_tokens=False
+            )
+            user_prompt_len = len(user_example["input_ids"])
+            # Padding labels to full max length to equalize the length of input_ids after collator
+            example["labels"] = [IGNORE_INDEX] * (full_max_length - len(example['labels']) + user_prompt_len) + \
+                                example["labels"][user_prompt_len:]
+    return {"input_ids": example['input_ids'], "labels": example["labels"]}
 
 
-def preprocess_batch_for_hf_instruction_dataset(example, tokenizer, args):
-    data = (example["instruction"], example["input"], example["output"], tokenizer, args)
-    example = preprocess_instruction_data(data)
-    return example
+def preprocess_batch_for_hf_dataset(dataset, tokenizer, args):
+    data = (dataset["instruction"], dataset["input"], dataset["output"], tokenizer, args)
+    dataset = preprocess_data(data)
+    return dataset
 
 
-def load_hf_instruction_dataset(data, tokenizer, args, mode):
+def load_hf_dataset(tokenizer, args, data, mode):
     if isinstance(data, str):
         if data.endswith('.json') or data.endswith('.jsonl'):
             dataset = load_dataset("json", data_files=data)
         elif os.path.isdir(data):
             dataset = datasets.load_from_disk(data)
         else:
             dataset = load_dataset(
@@ -85,22 +136,21 @@
         if mode == 'dev' and args.max_eval_samples is not None:
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
     dataset = dataset.shuffle().map(
-        lambda x: preprocess_batch_for_hf_instruction_dataset(x, tokenizer=tokenizer, args=args),
+        lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
         batched=False, remove_columns=dataset.column_names
-    ).filter(lambda x: len(x['input_ids']) > 0)
-
+    )
     return dataset
 
 
-class LlamaInstructionDataset(Dataset):
+class ChatGlmDataset(Dataset):
     def __init__(self, tokenizer, args, data, mode):
         cached_features_file = os.path.join(
             args.cache_dir,
             args.model_name.replace("/", "_")
             + "_cached_"
             + str(args.max_seq_length)
             + str(len(data)),
@@ -110,137 +160,58 @@
                 (not args.reprocess_input_data and not args.no_cache)
                 or (mode == "dev" and args.use_cached_eval_features and not args.no_cache)
         ):
             logger.info(" Loading features from cached file %s" % cached_features_file)
             with open(cached_features_file, "rb") as handle:
                 self.examples = pickle.load(handle)
         else:
-            logger.debug(" Creating features from dataset file at %s" % args.cache_dir)
+            logger.info(" Creating features from dataset file at %s" % args.cache_dir)
 
-            data = [
-                (instruction, input_text, target_text, tokenizer, args)
-                for instruction, input_text, target_text in zip(
-                    data["instruction"], data["input"], data["output"]
-                )
-            ]
-
-            if (mode == "train" and args.use_multiprocessing) or (
-                    mode == "dev" and args.use_multiprocessing_for_evaluation
-            ):
-                if args.multiprocessing_chunksize == -1:
-                    chunksize = max(len(data) // (args.process_count * 2), 500)
-                else:
-                    chunksize = args.multiprocessing_chunksize
-
-                with Pool(args.process_count) as p:
-                    self.examples = list(
-                        tqdm(
-                            p.imap(preprocess_instruction_data, data, chunksize=chunksize),
-                            total=len(data),
-                            disable=args.silent,
-                        )
-                    )
-            else:
-                self.examples = [preprocess_instruction_data(d) for d in tqdm(data, disable=args.silent)]
+            self.examples = list(load_hf_dataset(tokenizer, args, data, mode))
             if not args.no_cache:
                 logger.info(" Saving features into cached file %s" % cached_features_file)
                 with open(cached_features_file, "wb") as handle:
                     pickle.dump(self.examples, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     def __len__(self):
         return len(self.examples)
 
     def __getitem__(self, index):
         return self.examples[index]
 
 
-def tokenize_function(examples, tokenizer):
-    return tokenizer(examples["text"])
-
-
-def group_texts(examples, block_size: int = 1024):
-    # Concatenate all texts.
-    concatenated_examples = {k: list(chain(*examples[k])) for k in examples.keys()}
-    total_length = len(concatenated_examples[list(examples.keys())[0]])
-    # We drop the small remainder, we could add padding if the model supported it instead of this drop, you can
-    # customize this part to your needs.
-    if total_length >= block_size:
-        total_length = (total_length // block_size) * block_size
-    # Split by chunks of max_len.
-    result = {
-        k: [t[i: i + block_size] for i in range(0, total_length, block_size)]
-        for k, t in concatenated_examples.items()
-    }
-    result["labels"] = result["input_ids"].copy()
-    return result
-
-
-def load_hf_pretraining_dataset(data, tokenizer, args, mode):
-    if isinstance(data, str):
-        if data.endswith('.json') or data.endswith('.jsonl'):
-            dataset = load_dataset("json", data_files=data)
-        elif data.endswith('.txt'):
-            dataset = load_dataset("text", data_files=data)
-        elif os.path.isdir(data):
-            dataset = datasets.load_from_disk(data)
-        else:
-            dataset = load_dataset(
-                data,
-                download_mode="force_redownload"
-                if args.reprocess_input_data
-                else "reuse_dataset_if_exists",
-            )
-        # This is not necessarily a train dataset. The datasets library insists on calling it train.
-        dataset = dataset['train']
-        if mode == 'dev' and args.max_eval_samples is not None:
-            max_eval_samples = min(len(dataset), args.max_eval_samples)
-            dataset = dataset.select(range(max_eval_samples))
-    else:
-        dataset = HFDataset.from_pandas(data)
-
-    tokenized_dataset = dataset.map(
-        lambda x: tokenize_function(x, tokenizer=tokenizer),
-        batched=True,
-        remove_columns=dataset.column_names,
-        desc="Running tokenizer on dataset",
-    )
-    grouped_datasets = tokenized_dataset.map(
-        lambda x: group_texts(x, block_size=args.block_size),
-        batched=True,
-        desc=f"Grouping texts in chunks of {args.block_size}",
-    ).filter(lambda x: len(x['input_ids']) > 0)
-    dataset = grouped_datasets
-
-    return dataset
-
-
-class LlamaPretrainingDataset(Dataset):
-    def __init__(self, tokenizer, args, data, mode):
-        cached_features_file = os.path.join(
-            args.cache_dir,
-            args.model_name.replace("/", "_")
-            + "_cached_"
-            + str(args.max_seq_length)
-            + str(len(data)),
-        )
-
-        if os.path.exists(cached_features_file) and (
-                (not args.reprocess_input_data and not args.no_cache)
-                or (mode == "dev" and args.use_cached_eval_features and not args.no_cache)
-        ):
-            logger.info(" Loading features from cached file %s" % cached_features_file)
-            with open(cached_features_file, "rb") as handle:
-                self.examples = pickle.load(handle)
-        else:
-            logger.debug(" Creating features from dataset file at %s" % args.cache_dir)
-            dataset = load_hf_pretraining_dataset(data, tokenizer, args, mode)
-            self.examples = list(dataset)
-            if not args.no_cache:
-                logger.info(" Saving features into cached file %s" % cached_features_file)
-                with open(cached_features_file, "wb") as handle:
-                    pickle.dump(self.examples, handle, protocol=pickle.HIGHEST_PROTOCOL)
-
-    def __len__(self):
-        return len(self.examples)
-
-    def __getitem__(self, index):
-        return self.examples[index]
+def compute_bleu(label, pred, weights=None):
+    from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
+    weights = weights or (0.25, 0.25, 0.25, 0.25)
+    return np.mean([sentence_bleu(references=[list(a)], hypothesis=list(b),
+                                  smoothing_function=SmoothingFunction().method1, weights=weights)
+                    for a, b in zip(label, pred)])
+
+
+def compute_rouge(label, pred, weights=None, mode='weighted'):
+    weights = weights or (0.2, 0.4, 0.4)
+    if isinstance(label, str):
+        label = [label]
+    if isinstance(pred, str):
+        pred = [pred]
+    label = [' '.join(x) for x in label]
+    pred = [' '.join(x) for x in pred]
+
+    def _compute_rouge(label, pred):
+        try:
+            scores = Rouge().get_scores(hyps=label, refs=pred)[0]
+            scores = [scores['rouge-1']['f'], scores['rouge-2']['f'], scores['rouge-l']['f']]
+        except ValueError:
+            scores = [0, 0, 0]
+        return scores
+
+    scores = np.mean([_compute_rouge(*x) for x in zip(label, pred)], axis=0)
+    if mode == 'weighted':
+        return {'rouge': sum(s * w for s, w in zip(scores, weights))}
+    elif mode == '1':
+        return {'rouge-1': scores[0]}
+    elif mode == '2':
+        return {'rouge-2': scores[1]}
+    elif mode == 'l':
+        return {'rouge-l': scores[2]}
+    elif mode == 'all':
+        return {'rouge-1': scores[0], 'rouge-2': scores[1], 'rouge-l': scores[2]}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `textgen-0.2.7/textgen/llama/merge_peft_adapter.py` & `textgen-1.0.0/textgen/gpt/merge_peft_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 import os
 
 import peft
 import torch
 from huggingface_hub import hf_hub_download
 from peft import PeftModel
-from transformers import LlamaForCausalLM, LlamaTokenizer
+from transformers import AutoModelForCausalLM, AutoTokenizer
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--base_model_name_or_path', default=None, required=True, type=str, help="Base model name or path")
 parser.add_argument('--peft_model_path', default=None, required=True,
                     type=str,
                     help="Please specify LoRA models to be merged (ordered); use commas to separate multiple LoRA models.")
 parser.add_argument('--offload_dir', default=None, type=str,
@@ -213,26 +213,26 @@
 
     print(f"Base model: {base_model_path}")
     print(f"LoRA model(s) {lora_model_paths}:")
 
     if offload_dir is not None:
         # Load with offloading, which is useful for low-RAM machines.
         # Note that if you have enough RAM, please use original method instead, as it is faster.
-        base_model = LlamaForCausalLM.from_pretrained(
+        base_model = AutoModelForCausalLM.from_pretrained(
             base_model_path,
             load_in_8bit=False,
             torch_dtype=torch.float16,
             offload_folder=offload_dir,
             offload_state_dict=True,
             low_cpu_mem_usage=True,
             device_map={"": "cpu"},
         )
     else:
         # Original method without offloading
-        base_model = LlamaForCausalLM.from_pretrained(
+        base_model = AutoModelForCausalLM.from_pretrained(
             base_model_path,
             load_in_8bit=False,
             torch_dtype=torch.float16,
             device_map="auto",
         )
 
     ## infer the model size from the checkpoint
@@ -242,15 +242,15 @@
     print(f"Loading LoRA for {model_size} model")
 
     lora_model = None
     lora_model_sd = None
     tokenizer = None
     for lora_index, lora_model_path in enumerate(lora_model_paths):
         print(f"Loading LoRA {lora_model_path}")
-        tokenizer = LlamaTokenizer.from_pretrained(lora_model_path)
+        tokenizer = AutoTokenizer.from_pretrained(lora_model_path)
         if base_model.get_input_embeddings().weight.size(0) != len(tokenizer):
             base_model.resize_token_embeddings(len(tokenizer))
             print(f"Extended vocabulary size to {len(tokenizer)}")
 
         first_weight = base_model.model.layers[0].self_attn.q_proj.weight
         first_weight_old = first_weight.clone()
 
@@ -292,22 +292,19 @@
                 lora_b_key = k.replace('lora_A', 'lora_B')
                 base_model_sd[original_key] += (
                         transpose(lora_model_sd[lora_b_key].float() @ lora_model_sd[lora_a_key].float(),
                                   fan_in_fan_out) * lora_scaling
                 )
                 assert base_model_sd[original_key].dtype == torch.float16
 
-        # did we do anything?
-        assert not torch.allclose(first_weight_old, first_weight)
-
     tokenizer.save_pretrained(output_dir)
 
     if output_type == 'huggingface':
         print("Saving to Hugging Face format...")
-        LlamaForCausalLM.save_pretrained(base_model, output_dir)
+        base_model.save_pretrained(output_dir)
     else:  # output_type=='pth'
         print("Saving to pth format...")
 
         base_model_sd = base_model.state_dict()
         del lora_model, base_model, lora_model_sd
 
         params = params_of_models[model_size]
```

### Comparing `textgen-0.2.7/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-1.0.0/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-1.0.0/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-1.0.0/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/seq2seq/data_reader.py` & `textgen-1.0.0/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/seq2seq/seq2seq_model.py` & `textgen-1.0.0/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/seq2seq/seq2seq_trainer.py` & `textgen-1.0.0/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/t5/copyt5_model.py` & `textgen-1.0.0/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/t5/copyt5_utils.py` & `textgen-1.0.0/textgen/t5/t5_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
-@description: 
+@description: adjust for chinese tokenizer
 """
 import os
 import pickle
 from multiprocessing import Pool
 
-import jieba
-import torch.nn.functional as F
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
-from loguru import logger
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
-from transformers import BertTokenizer
-
-jieba.setLogLevel('ERROR')
-
-
-class ZHTokenizer(BertTokenizer):
-    def __init__(self, pre_tokenizer=lambda x: jieba.cut(x, HMM=False), *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.pre_tokenizer = pre_tokenizer
-
-    def _tokenize(self, text, *arg, **kwargs):
-        split_tokens = []
-        for text in self.pre_tokenizer(text):
-            if text in self.vocab:
-                split_tokens.append(text)
-            else:
-                split_tokens.extend(super()._tokenize(text))
-        return split_tokens
-
-
-def mask_select(inputs, mask):
-    input_dim = inputs.ndim
-    mask_dim = mask.ndim
-    mask = mask.reshape(-1).bool()
-    if input_dim > mask_dim:
-        inputs = inputs.reshape((int(mask.size(-1)), -1))[mask]
-    else:
-        inputs = inputs.reshape(-1)[mask]
-    return inputs
-
-
-def copy_loss(inputs, targets, mask, eps=1e-6):
-    mask = mask[:, 1:]
-    inputs = inputs[:, :-1]
-    targets = targets[:, 1:]
-    inputs = mask_select(inputs, mask)
-    targets = mask_select(targets, mask)
-    log_preds = (inputs + eps).log()
-    loss = F.nll_loss(log_preds, targets)
-    return loss
-
-
-def ce_loss(inputs, targets, mask):
-    mask = mask[:, 1:]
-    inputs = inputs[:, :-1]
-    targets = targets[:, 1:]
-    inputs = mask_select(inputs, mask)
-    targets = mask_select(targets, mask)
-    loss = F.cross_entropy(inputs, targets)
-    return loss
+from rouge import Rouge
+from loguru import logger
 
 
 def preprocess_batch_for_hf_dataset(dataset, tokenizer, args):
     if args.preprocess_inputs:
         return tokenizer.prepare_seq2seq_batch(
             src_texts=[
                 prefix + ": " + input_text
@@ -121,43 +70,40 @@
     else:
         return dataset
 
 
 def preprocess_data(data):
     prefix, input_text, target_text, tokenizer, args = data
 
-    src = tokenizer(
-        [prefix + ": " + input_text],
-        padding="max_length",
-        return_tensors='pt',
-        max_length=args.max_seq_length,
-        truncation=True,
-        return_attention_mask=True,
-        return_token_type_ids=False,
-    )
-    input_ids = src["input_ids"][0]
-    attention_mask = src["attention_mask"][0]
-    with tokenizer.as_target_tokenizer():
-        tgt = tokenizer(
-            [target_text],
+    # Add EOS again if truncated?
+    if args.preprocess_inputs:
+        batch = tokenizer.prepare_seq2seq_batch(
+            src_texts=[prefix + ": " + input_text],
+            tgt_texts=[target_text],
+            max_length=args.max_seq_length,
             padding="max_length",
-            return_tensors='pt',
+            return_tensors="pt",
+            truncation=True,
+        )
+    else:
+        batch = tokenizer.prepare_seq2seq_batch(
+            src_texts=[prefix + ": " + input_text],
+            tgt_texts=[target_text],
             max_length=args.max_seq_length,
+            padding="max_length",
+            return_tensors="pt",
             truncation=True,
-            return_attention_mask=True,
-            return_token_type_ids=False,
         )
-    labels = tgt["input_ids"][0]
-    decoder_attention_mask = tgt["attention_mask"][0]
-    decoder_input_ids = tgt['input_ids'][0]
-
-    return input_ids, attention_mask, labels, decoder_attention_mask, decoder_input_ids
+    input_ids = batch["input_ids"][0]
+    attention_mask = batch["attention_mask"][0]
+    labels = batch["labels"][0]
+    return (input_ids, attention_mask, labels)
 
 
-class CopyT5Dataset(Dataset):
+class T5Dataset(Dataset):
     def __init__(self, tokenizer, args, data, mode):
         cached_features_file = os.path.join(
             args.cache_dir,
             args.model_name.replace("/", "_")
             + "_cached_"
             + str(args.max_seq_length)
             + str(len(data)),
@@ -204,7 +150,65 @@
                     pickle.dump(self.examples, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
     def __len__(self):
         return len(self.examples)
 
     def __getitem__(self, index):
         return self.examples[index]
+
+
+def dynamic_lcs(X, Y):
+    # find the length of the strings
+    m = len(X)
+    n = len(Y)
+
+    # declaring the array for storing the dp values
+    L = [[None] * (n + 1) for i in range(m + 1)]
+
+    """Following steps build L[m + 1][n + 1] in bottom up fashion
+    Note: L[i][j] contains length of LCS of X[0..i-1]
+    and Y[0..j-1]"""
+    for i in range(m + 1):
+        for j in range(n + 1):
+            if i == 0 or j == 0:
+                L[i][j] = 0
+            elif X[i - 1] == Y[j - 1]:
+                L[i][j] = L[i - 1][j - 1] + 1
+            else:
+                L[i][j] = max(L[i - 1][j], L[i][j - 1])
+
+    # L[m][n] contains the length of LCS of X[0..n-1] & Y[0..m-1]
+    return L[m][n]
+
+
+def f1_sim(text_a, text_b):
+    """F1相似度
+    说明：算出两个文本的最长公共子序列长度，然后乘2并处以两者
+    长度之和。
+    脚本见：https://github.com/CLUEbenchmark/pCLUE/blob/main/evaluate_pclue.py
+    计算pCLUE任务总分，及子分数
+    """
+    if not text_a and not text_b:
+        return 0.
+    lcs_len = dynamic_lcs(text_a, text_b)
+    return 2. * lcs_len / (len(text_a) + len(text_b))
+
+
+def rouge_l_zh(target, pred):
+    """计算Rouge-l得分，Rouge-l指标常用于评估自动文本摘要及翻译任务
+    target: 真实标签
+    pred: 预测标签"""
+
+    if not (isinstance(target, str) or isinstance(pred, str)):
+        logger.error("target或pred为非字符串！请检查!")
+        return 0
+    rouge = Rouge()
+    scores = rouge.get_scores(" ".join(list(pred)), " ".join(list(target)))
+    score = scores[0]["rouge-l"]
+    return score["f"]
+
+
+if __name__ == '__main__':
+    a = '123444'
+    b = '23411'
+    print(f1_sim(a, b))
+    print(dynamic_lcs(a, b))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `textgen-0.2.7/textgen/t5/t5_model.py` & `textgen-1.0.0/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/unsup_generation/tgls_model.py` & `textgen-1.0.0/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen/unsup_generation/tgls_util.py` & `textgen-1.0.0/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.7/textgen.egg-info/PKG-INFO` & `textgen-1.0.0/textgen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.7
+Version: 1.0.0
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
-Description: <div align="center">
+Description: [**🇨🇳中文**](https://github.com/shibing624/textgen/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/textgen/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+        
+        <div align="center">
           <a href="https://github.com/shibing624/textgen">
             <img src="https://github.com/shibing624/textgen/blob/main/docs/logo.svg" alt="Logo">
           </a>
         </div>
         
         -----------------
         
@@ -23,14 +25,20 @@
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         ## 📖 Introduction
         
         **TextGen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
+        ## 🔥 News
+        [2023/06/15] v1.0.0版本: 新增ChatGLM/LLaMA/Bloom模型的多轮对话微调训练，并发布医疗问诊LoRA模型[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)。详见[Release-v1.0.0](https://github.com/shibing624/MedicalGPT/releases/tag/1.0.0)
+        
+        [2023/06/02] v0.2.7版本: 新增ChatGLM/LLaMA/Bloom模型的SFT微调训练，并发布适用于通用对话和中文纠错的LoRA模型。详见[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
+        
+        
         ## 😊 Feature
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
         - [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
         - [BLOOM](textgen/bloom)：本项目基于PyTorch实现了BLOOM模型LoRA微调训练和预测，可以用于对话生成任务和领域微调训练
         - [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
@@ -40,30 +48,29 @@
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
         
-        | Model                                                                                                     | Arch       | Introduce                                                                                                                                                                | Training                                                                                                                                     | Inference                                                                                                             | 
+        | Model                                                                                                     | Arch       | Introduction                                                                                                                                                                | Train Script                                                                                                                                 | Predict Script                                                                                                        | 
         |:----------------------------------------------------------------------------------------------------------|:-----------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-        | [shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)             | T5         | 中文NLP多任务Prompt模型                                                                                                                                                         | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
         | [shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)                     | T5         | fine-tuned中文对联后的模型                                                                                                                                                       | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-        | [shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)                 | SongNet    | SongNet预训练模型                                                                                                                                                             | -                                                                                                                                            | -                                                                                                                     |
         | [shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)   | SongNet    | fine-tuned宋词后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-        | [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        | [shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet    | fine-tuned对联后的模型                                                                                                                                                         | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
         | [shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)             | ChatGLM-6B | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                        | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
         | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)         | ChatGLM-6B | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                           | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
         | [shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)           | LLaMA-13B  | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                            | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
-        | [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
-        | [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+        | [shibing624/chinese-alpaca-plus-7b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-7b-hf)       | LLaMA-7B   | [中文LLaMA-Plus, Alpaca-Plus 7B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型     | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+        | [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/chinese-alpaca-plus-13b-hf)     | LLaMA-13B  | [中文LLaMA-Plus, Alpaca-Plus 13B版本](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.1)，在LLaMA-13B上扩充了中文词表并继续预训练120G文本（通用领域），在4.3M指令数据集上微调后得到的中文Alpaca-plus模型 | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
+        | [shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/ziya-llama-13b-medical-lora)     | LLaMA-13B  | 在240万条中英文医疗数据集[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)上微调了一版Ziya-LLaMA-13B模型，医疗问答效果有提升，发布微调后的LoRA权重                                      | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                                     | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)               |
         
         ### Evaluation
         
-        | Model                                                                                                                                       | Arch       | Introduce                                                                                                                                                                                                                                                                                     | Score    |
+        | Model                                                                                                                                       | Arch       | Introduction                                                                                                                                                                                                                                                                                     | Score    |
         |:--------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------|
         | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         | LLaMA-7B   | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 4.92     |
         | [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       | LLaMA-13B  | 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分                                                                                                                                                                          | 7.05     |
         | [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                                                                                                                                                                                                 | 7.16     |
         | [ChatGLM-6B-v1.1](https://huggingface.co/THUDM/chatglm-6b)                                                                                  | ChatGLM-6B | 基于原生`THUDM/chatglm-6b`v1.1英文优化版模型评估测试集得分                                                                                                                                                                                                                                                      | **7.18** |
         | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           | ChatGLM-6B | 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                                                                                                                                                                                                     | 7.03     |
         | [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                | LLaMA-13B  | 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                                                                                                                                                                                               | 4.13     |  
@@ -116,29 +123,29 @@
         
         ## ▶️ Usage
         
         ### ChatGLM-6B 模型
         
         #### 使用 ChatGLM-6B 微调后的模型
         
-        example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+        example: [examples/chatglm/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/inference_demo.py)
         
         ```python
         from textgen import ChatGlmModel
         
         model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
         PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
         
         #### 训练 ChatGLM-6B 微调模型
         
-        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[examples/data/json_files/belle_10.json](https://github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
         2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
         3. 支持多卡训练，支持混合精度训练
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
         单卡训练：
         ```shell
@@ -170,31 +177,31 @@
         --output_dir：指定保存全量模型权重的目录，默认为./merged
         ```
         
         ### LLaMA 模型
         
         #### 使用 LLaMA 微调后的模型
         
-        example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+        example: [examples/gpt/inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt/inference_demo.py)
         
         <details>
         <summary>show code example and result</summary>
         
         ```python
         import sys
         
         sys.path.append('../..')
-        from textgen import LlamaModel
+        from textgen import GptModel
         
         
         def generate_prompt(instruction):
           return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
         
         
-        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
+        model = GptModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
         </details>
         
@@ -209,15 +216,15 @@
         #### 基于微调(LoRA)模型继续训练
         如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
         
         单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
         
         执行以下命令：
         ```shell
-        python -m textgen/llama/merge_peft_adapter.py \
+        python -m textgen/gpt/merge_peft_adapter.py \
             --base_model_name_or_path path_to_original_base_model_dir \
             --peft_model_path path_to_chinese_llama_or_alpaca_lora \
             --output_type [pth|huggingface]
             --output_dir path_to_output_dir 
         ```
         参数说明：
         ```
@@ -225,20 +232,15 @@
         --peft_model_path：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
         --output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为huggingface
         --output_dir：指定保存全量模型权重的目录，默认为./merged
         --offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
         ```
         
         #### 训练领域模型
-        
-        | Notebook     | Description |    |
-        |:----------|:------------|------:|
-        | [training_medical_model.ipynb](https://github.com/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb)  | 训练医疗大模型     |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-        
-        # Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning]单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
+        Note: 为了全面的介绍训练医疗大模型的过程，把4阶段训练方法(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement Learning)单独新建了一个repo：[shibing624/MedicalGPT](https://github.com/shibing624/MedicalGPT)，请移步该repo查看训练方法。
         
         ### BLOOM 模型
         
         #### 训练 BLOOM 微调模型
         
         example: [examples/bloom/training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/examples/bloom/training_bloom_demo.py)
         
@@ -571,28 +573,42 @@
         
         前10句是真实用户评论，后10句是生成的。
         
         </details>
         
         ## 📚 Dataset 
         
-        1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-        2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
-        4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
-        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
-        6. 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+        #### SFT datasets
+        - 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+        - 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+        - 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        - 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        - 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        - 240万条中文医疗数据集(包括预训练数据和指令微调数据集)：[shibing624/medical](https://huggingface.co/datasets/shibing624/medical)
+        - 5万条英文ChatGPT多轮对话数据集：[RyokoAI/ShareGPT52K](https://huggingface.co/datasets/RyokoAI/ShareGPT52K)
+        - 80万条中文ChatGPT多轮对话数据集：[BelleGroup/multiturn_chat_0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+        - 116万条中文ChatGPT多轮对话数据集：[fnlp/moss-002-sft-data](https://huggingface.co/datasets/fnlp/moss-002-sft-data)
+        
+        #### Reward Model datasets
+        - 原版的oasst1数据集：[OpenAssistant/oasst1](https://huggingface.co/datasets/OpenAssistant/oasst1)
+        - 2万条多语言oasst1的reward数据集：[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/tasksource/oasst1_pairwise_rlhf_reward)
+        - 11万条英文hh-rlhf的reward数据集：[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/Dahoas/full-hh-rlhf)
+        - 9万条英文reward数据集(来自Anthropic's Helpful Harmless dataset)：[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/static-hh)
+        - 7万条英文reward数据集（来源同上）：[Dahoas/rm-static](https://huggingface.co/datasets/Dahoas/rm-static)
+        - 7万条繁体中文的reward数据集（翻译自rm-static）[liswei/rm-static-m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh)
+        - 7万条英文Reward数据集：[yitingxie/rlhf-reward-datasets](https://huggingface.co/datasets/yitingxie/rlhf-reward-datasets)
+        - 3千条中文知乎问答偏好数据集：[liyucheng/zhihu_rlhf_3k](https://huggingface.co/datasets/liyucheng/zhihu_rlhf_3k)
         
         ## ✅ Todo
         
-        1. [ ] 新增多轮对话数据微调方法
-        2. [ ] add reward model finetuning
-        3. [ ] add rl finetuning
-        4. [ ] add medical reward dataset
-        5. [ ] add llama in4 training
+        1. [x] add multiple rounds of dialogue data fine-tuning method
+        2. [x] add reward model finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+        3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
+        4. [x] add medical reward dataset
+        5. [x] add llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/shibing624/MedicalGPT)
         6. [ ] add all training and predict demo in colab
         
         ## ☎️ Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
@@ -603,23 +619,26 @@
         ## 😇 Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
-          author={Xu Ming},
+          author={Ming Xu},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
         ## 🤗 License
+        This repository is licensed under [The Apache License 2.0](LICENSE).
+        
+        Please follow the [Model Card](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) to use the LLaMA model.
         
-        授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
+        Please follow the [RAIL License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM & BLOOMZ model.
         
         ## 😍 Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
```

#### html2text {}

```diff
@@ -1,23 +1,35 @@
-Metadata-Version: 2.1 Name: textgen Version: 0.2.7 Summary: Text Generation
+Metadata-Version: 2.1 Name: textgen Version: 1.0.0 Summary: Text Generation
 Model Home-page: https://github.com/shibing624/textgen Author: XuMing Author-
-email: xuming624@qq.com License: Apache 2.0 Description:
+email: xuming624@qq.com License: Apache 2.0 Description: [**ð¨ð³ä¸­æ**]
+(https://github.com/shibing624/textgen/blob/main/README.md) | [**ðEnglish**]
+(https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**ðææ¡£/
+Docs**](https://github.com/shibing624/textgen/wiki) | [**ð¤æ¨¡å/Models**]
+(https://huggingface.co/shibing624)
                                     [Logo]
 ----------------- # TextGen: Implementation of Text Generation models [![PyPI
 version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/
 textgen) [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/
 project/textgen) [![Contributions welcome](https://img.shields.io/badge/
 contributions-welcome-brightgreen.svg)](CONTRIBUTING.md) [![License Apache 2.0]
 (https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE) [!
 [python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)]
 (requirements.txt) [![GitHub issues](https://img.shields.io/github/issues/
 shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) ## ð Introduction
 **TextGen**å®ç°äºå¤ç§ææ¬çææ¨¡åï¼åæ¬ï¼LLaMAãChatGLMãUDAãGPT2ãSeq2SeqãBARTãT5ãSongNetç­æ¨¡åï¼å¼ç®±å³ç¨ã
+## ð¥ News [2023/06/15] v1.0.0çæ¬: æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçå¤è½®å¯¹è¯å¾®è°è®­ç»ï¼å¹¶åå¸å»çé®è¯LoRAæ¨¡å
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora)ãè¯¦è§[Release-v1.0.0](https://github.com/
+shibing624/MedicalGPT/releases/tag/1.0.0) [2023/06/02] v0.2.7çæ¬:
+æ°å¢ChatGLM/LLaMA/
+Bloomæ¨¡åçSFTå¾®è°è®­ç»ï¼å¹¶åå¸éç¨äºéç¨å¯¹è¯åä¸­æçº éçLoRAæ¨¡åãè¯¦è§
+[Release-v0.2.7](https://github.com/shibing624/MedicalGPT/releases/tag/0.2.7)
 ## ð Feature - [ChatGLM](textgen/
 chatglm)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºChatGLM-
 6Bæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¥å­çº éãå¯¹è¯ç­ææ¬çæä»»å¡
 - [LLaMA](textgen/
 llama)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºLLaMAæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
 - [BLOOM](textgen/
 bloom)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºBLOOMæ¨¡åLoRAå¾®è°è®­ç»åé¢æµï¼å¯ä»¥ç¨äºå¯¹è¯çæä»»å¡åé¢åå¾®è°è®­ç»
@@ -34,37 +46,30 @@
 songnet_model.py)ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºSongNetæ¨¡åè®­ç»åé¢æµï¼å¯ä»¥ç¨äºè§èæ ¼å¼çè¯è¯ãæ­è¯ç­ææ¬çæä»»å¡
 - [TGLS](textgen/unsup_generation)ï¼æ¬é¡¹ç®å®ç°äº[TGLS](https://
 www.jiqizhixin.com/articles/2020-08-11-
 5)æ çç£ç¸ä¼¼ææ¬çææ¨¡åï¼æ¯ä¸ç§âåæç´¢åå­¦ä¹ âçææ¬çææ¹æ³ï¼éè¿åå¤è¿­ä»£å­¦ä¹ åééï¼æç»æ¨¡åè½çæç±»ä¼¼åééçé«è´¨éç¸ä¼¼ææ¬
 ### Release Models
 releaseåºäº`textgen`è®­ç»çä¸­ææ¨¡åï¼æ¨¡åå·²ç»releaseå°HuggingFace
 modelsï¼æå®æ¨¡ååç§°`textgen`ä¼èªå¨ä¸è½½æ¨¡åï¼å¯ç´æ¥ä½¿ç¨ã
-| Model | Arch | Introduce | Training | Inference | |:-------------------------
+| Model | Arch | Introduction | Train Script | Predict Script | |:-------------
 -------------------------------------------------------------------------------
---|:-----------|:--------------------------------------------------------------
+--------------|:-----------|:--------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------|:-------------------------------------------------
+----------------------------------------|:-------------------------------------
 -------------------------------------------------------------------------------
--------------|:----------------------------------------------------------------
-------------------------------------------------------| | [shibing624/prompt-
-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese) | T5
-| ä¸­æNLPå¤ä»»å¡Promptæ¨¡å | [prompt-t5-base-chinese.md](https://
-github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md) |
-[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_prompt_demo.py) | | [shibing624/t5-chinese-couplet](https://huggingface.co/
-shibing624/t5-chinese-couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å |
-[å¯¹èçææ¨¡åè°ç ](https://github.com/shibing624/textgen/blob/main/
-docs/
+-------------------------|:----------------------------------------------------
+------------------------------------------------------------------| |
+[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-
+couplet) | T5 | fine-tunedä¸­æå¯¹èåçæ¨¡å | [å¯¹èçææ¨¡åè°ç ]
+(https://github.com/shibing624/textgen/blob/main/docs/
 %E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) |
 [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/
-t5_couplet_demo.py) | | [shibing624/songnet-base-chinese](https://
-huggingface.co/shibing624/songnet-base-chinese) | SongNet |
-SongNeté¢è®­ç»æ¨¡å | - | - | | [shibing624/songnet-base-chinese-songci]
-(https://huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet |
-fine-tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
+t5_couplet_demo.py) | | [shibing624/songnet-base-chinese-songci](https://
+huggingface.co/shibing624/songnet-base-chinese-songci) | SongNet | fine-
+tunedå®è¯åçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
 songnet_songci_demo.py) | | [shibing624/songnet-base-chinese-couplet](https://
 huggingface.co/shibing624/songnet-base-chinese-couplet) | SongNet | fine-
 tunedå¯¹èåçæ¨¡å | [training script](https://github.com/shibing624/
 textgen/blob/main/examples/songnet/training_zh_songnet_demo.py) | [predict
 script](https://github.com/shibing624/textgen/blob/main/examples/songnet/
@@ -103,31 +108,39 @@
 [shibing624/chinese-alpaca-plus-13b-hf](https://huggingface.co/shibing624/
 chinese-alpaca-plus-13b-hf) | LLaMA-13B | [ä¸­æLLaMA-Plus, Alpaca-Plus
 13Bçæ¬](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/
 v3.1)ï¼å¨LLaMA-
 13Bä¸æ©åäºä¸­æè¯è¡¨å¹¶ç»§ç»­é¢è®­ç»120Gææ¬ï¼éç¨é¢åï¼ï¼å¨4.3Mæä»¤æ°æ®éä¸å¾®è°åå¾å°çä¸­æAlpaca-
 plusæ¨¡å | [training script](https://github.com/shibing624/textgen/blob/main/
 examples/llama/training_llama_demo.py) | [predict script](https://github.com/
-shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | ###
-Evaluation | Model | Arch | Introduce | Score | |:-----------------------------
+shibing624/textgen/blob/main/examples/llama/training_llama_demo.py) | |
+[shibing624/ziya-llama-13b-medical-lora](https://huggingface.co/shibing624/
+ziya-llama-13b-medical-lora) | LLaMA-13B | å¨240ä¸æ¡ä¸­è±æå»çæ°æ®é
+[shibing624/medical](https://huggingface.co/datasets/shibing624/
+medical)ä¸å¾®è°äºä¸çZiya-LLaMA-
+13Bæ¨¡åï¼å»çé®ç­ææææåï¼åå¸å¾®è°åçLoRAæé |
+[training script](https://github.com/shibing624/textgen/blob/main/examples/
+llama/training_llama_demo.py) | [predict script](https://github.com/shibing624/
+textgen/blob/main/examples/llama/training_llama_demo.py) | ### Evaluation |
+Model | Arch | Introduction | Score | |:---------------------------------------
 -------------------------------------------------------------------------------
---------------------------------|:-----------|:--------------------------------
+----------------------|:-----------|:------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://
-huggingface.co/ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/
+-------|:---------| | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/
+ziqingyang/chinese-alpaca-lora-7b) | LLaMA-7B | å¤ç¨[ymcui/Chinese-LLaMA-
+Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/
+README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca](https://
+huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B | å¤ç¨[ymcui/
 Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/
-examples/README.md)çè¯ä¼°caseåå¾å | 4.92 | | [LLaMA-13B-Chinese-Alpaca]
-(https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b) | LLaMA-13B |
-å¤ç¨[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-
-Alpaca/blob/main/examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-
-6B](https://huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/
-chatglm-6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://
+examples/README.md)çè¯ä¼°caseåå¾å | 7.05 | | [ChatGLM-6B](https://
 huggingface.co/THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
+6b`è¯ä¼°æµè¯éå¾å | 7.16 | | [ChatGLM-6B-v1.1](https://huggingface.co/
+THUDM/chatglm-6b) | ChatGLM-6B | åºäºåç`THUDM/chatglm-
 6b`v1.1è±æä¼åçæ¨¡åè¯ä¼°æµè¯éå¾å | **7.18** | | [shibing624/
 chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-
 zh-lora) | ChatGLM-6B | åºäº`THUDM/chatglm-6b`å è½½`shibing624/chatglm-6b-
 belle-zh-lora`LoRAæ¨¡ååè¯ä¼°æµè¯éå¾å | 7.03 | | [facat/alpaca-lora-
 cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b) | LLaMA-13B |
 åºäº`decapoda-research/llama-13b-hf`å è½½`facat/alpaca-lora-cn-
 13b`LoRAæ¨¡ååè¯ä¼°æµè¯éå¹¶æ æ³¨å¾å | 4.13 | | [Chinese-Vicuna/
@@ -175,26 +188,27 @@
 examples/gradio_demo.py ``` model trained by [examples/t5/
 T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/
 main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb) ## ð¾ Install ```shell
 pip install -U textgen ``` or install develop version: ```shell pip install
 torch # conda install pytorch git clone https://github.com/shibing624/
 textgen.git cd textgen python setup.py install ``` ## â¶ï¸ Usage ### ChatGLM-
 6B æ¨¡å #### ä½¿ç¨ ChatGLM-6B å¾®è°åçæ¨¡å example: [examples/chatglm/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-chatglm/predict_demo.py) ```python from textgen import ChatGlmModel model =
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+chatglm/inference_demo.py) ```python from textgen import ChatGlmModel model =
 ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-
 csc-zh-lora") r = model.predict(
 ["å¯¹ä¸é¢ä¸­ææ¼åçº éï¼\nå°åéåå è¯¥ä¸ºèäººè®©åã\nç­ï¼"])
 print(r) # ['å°åéååºè¯¥ä¸ºèäººè®©åº§ã\néè¯¯å­ï¼å ï¼å'] ```
 PSï¼ç±äºä½¿ç¨äºå¼åä¸­çpeftåºï¼å¯è½ç±äºçæ¬æ´æ°ï¼å¯¼è´LoRAæ¨¡åå è½½å¤±è´¥ï¼å»ºè®®ä½¿ç¨ä¸é¢çè®­ç»æ¹æ³ï¼èªå·±è®­ç»LoRAæ¨¡åã
 #### è®­ç» ChatGLM-6B å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
-data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
-datasets/shibing624/alpaca-zh) 2.
+data/zh_csc_test.tsv)æè[examples/data/json_files/belle_10.json](https://
+github.com/shibing624/textgen/blob/main/examples/data/json_files/belle_10.json)
+2.
 æ¯æAdaLoRAãLoRAãP_TuningãPrefix_Tuningç­é¨ååæ°å¾®è°æ¹æ³ï¼ä¹æ¯æå¨åå¾®è°
 3. æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç» example: [examples/chatglm/
 training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/chatglm/training_chatglm_demo.py) åå¡è®­ç»ï¼ ```shell cd
 examples/chatglm CUDA_VISIBLE_DEVICES=0 python training_chatglm_demo.py --
 do_train --do_predict --num_epochs 1 --output_dir outputs_chatglm ```
 å¤å¡è®­ç»ï¼ ```shell cd examples/chatglm CUDA_VISIBLE_DEVICES=0,1 torchrun
@@ -205,23 +219,23 @@
 m textgen/chatglm/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path path_to_peft_model_dir \ --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --
 peft_model_pathï¼å­æ¾PEFTæ ¼å¼çå¾®è°æ¨¡åæéåéç½®æä»¶çç®å½
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged ```
-### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/llama/
-predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
-llama/predict_demo.py)  show code example and result ```python import sys
-sys.path.append('../..') from textgen import LlamaModel def generate_prompt
+### LLaMA æ¨¡å #### ä½¿ç¨ LLaMA å¾®è°åçæ¨¡å example: [examples/gpt/
+inference_demo.py](https://github.com/shibing624/textgen/blob/main/examples/
+gpt/inference_demo.py)  show code example and result ```python import sys
+sys.path.append('../..') from textgen import GptModel def generate_prompt
 (instruction): return f"""Below is an instruction that describes a task. Write
 a response that appropriately completes the request.\n\n### Instruction:
-{instruction}\n\n### Response:""" model = LlamaModel("llama", "decapoda-
-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
-predict_sentence = generate_prompt
+{instruction}\n\n### Response:""" model = GptModel("llama", "decapoda-research/
+llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b") predict_sentence =
+generate_prompt
 ("é®ï¼ç¨ä¸å¥è¯æè¿°å°çä¸ºä»ä¹æ¯ç¬ä¸æ äºçã\nç­ï¼") r =
 model.predict([predict_sentence]) print(r) #
 ['å°çæ¯å¯ä¸ä¸é¢æ¥æçå½çè¡æã'] ```  #### è®­ç» LLaMA
 å¾®è°æ¨¡å 1.
 æ¯æèªå®ä¹è®­ç»æ°æ®éåè®­ç»åæ°ï¼æ°æ®éæ ¼å¼åè[examples/
 data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/
 data/zh_csc_test.tsv)æè[shibing624/alpaca-zh](https://huggingface.co/
@@ -231,34 +245,29 @@
 æ¯æå¤å¡è®­ç»ï¼æ¯ææ··åç²¾åº¦è®­ç»ï¼ä½¿ç¨æ¹æ³åä¸ï¼ChatGLMå¤å¡è®­ç»ï¼
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/
 textgen/blob/main/examples/llama/training_llama_demo.py) #### åºäºå¾®è°
 (LoRA)æ¨¡åç»§ç»­è®­ç»
 å¦æéè¦åºäºLoraæ¨¡åç»§ç»­è®­ç»ï¼å¯ä»¥ä½¿ç¨ä¸é¢çèæ¬åå¹¶æ¨¡åä¸ºæ°çbase
 modelï¼åå¾®è°è®­ç»å³å¯ã åLoRAæéåå¹¶ï¼éç¨äº Chinese-LLaMA,
 Chinese-LLaMA-Plus, Chinese-Alpacaï¼ æ§è¡ä»¥ä¸å½ä»¤ï¼ ```shell python -
-m textgen/llama/merge_peft_adapter.py \ --base_model_name_or_path
+m textgen/gpt/merge_peft_adapter.py \ --base_model_name_or_path
 path_to_original_base_model_dir \ --peft_model_path
 path_to_chinese_llama_or_alpaca_lora \ --output_type [pth|huggingface] --
 output_dir path_to_output_dir ``` åæ°è¯´æï¼ ``` --
 base_model_name_or_pathï¼å­æ¾HFæ ¼å¼çåºåº§æ¨¡åæéåéç½®æä»¶çç®å½
 --peft_model_pathï¼ä¸­æLLaMA/Alpaca
 LoRAè§£ååæä»¶æå¨ç®å½ï¼ä¹å¯ä½¿ç¨HFä¸çLoraæ¨¡ååç§°ï¼å¦`ziqingyang/
 chinese-alpaca-lora-7b`ä¼èªå¨ä¸è½½å¯¹åºæ¨¡å --output_type:
 æå®è¾åºæ ¼å¼ï¼å¯ä¸ºpthæhuggingfaceãè¥ä¸æå®ï¼é»è®¤ä¸ºhuggingface
 --output_dirï¼æå®ä¿å­å¨éæ¨¡åæéçç®å½ï¼é»è®¤ä¸º./merged --
 offload_dirï¼å¯éï¼ï¼å¯¹äºä½åå­ç¨æ·éè¦æå®ä¸ä¸ªoffloadç¼å­è·¯å¾
-``` #### è®­ç»é¢åæ¨¡å | Notebook | Description | | |:----------|:--------
-----|------:| | [training_medical_model.ipynb](https://github.com/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) |
-è®­ç»å»çå¤§æ¨¡å |[![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/github/shibing624/
-textgen/blob/main/examples/llama/training_medical_model.ipynb) | # Note:
+``` #### è®­ç»é¢åæ¨¡å Note:
 ä¸ºäºå¨é¢çä»ç»è®­ç»å»çå¤§æ¨¡åçè¿ç¨ï¼æ4é¶æ®µè®­ç»æ¹æ³
-[Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
-Learning]åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
+(Pretraining, Supervised Finetuning, Reward Modeling and Reinforcement
+Learning)åç¬æ°å»ºäºä¸ä¸ªrepoï¼[shibing624/MedicalGPT](https://
 github.com/shibing624/MedicalGPT)ï¼è¯·ç§»æ­¥è¯¥repoæ¥çè®­ç»æ¹æ³ã ###
 BLOOM æ¨¡å #### è®­ç» BLOOM å¾®è°æ¨¡å example: [examples/bloom/
 training_bloom_demo.py](https://github.com/shibing624/textgen/blob/main/
 examples/bloom/training_bloom_demo.py) ### ConvSeq2Seq æ¨¡å
 è®­ç»å¹¶é¢æµConvSeq2Seqæ¨¡åï¼ example: [examples/seq2sesq/
 training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/
 main/examples/seq2seq/training_convseq2seq_model_demo.py)  show code example
@@ -436,42 +445,68 @@
 ä¸æå¼åè£éé¢çç²¾åååå¥½ï¼ç¨äºè¡¥æ°´è¡¥æ°´ææä¸éï¼ç©æµéå¸¸å¿«ã
 ç®è¤å¾åæ»ðæ¯ä¸å»éåº¦å¿«ä¸å¤©å°±å°äºã
 åä¸¤å¤©ç®è¤å¹²ç¥è¿ç»­æ·äºä¸¤ä¸ªæä¸æè§è¿ä¸éðè¡¥æ°´ææææ¾ï¼å¯æ³èç¥ç²¾åæ¶²åå¤åè¶³ðæ·ä¸ä»¥åååçå¾èæã
 è¡¥æ°´ææä¸è¬å§ï½ä½æ¯æç¨çé©å½èåæ¥çé¢èçº¸ä¸ç®èï¼å¸æå¥½ç¨ä¼åè´­çï¼æ·ä¸è¸æè§æ¯è¾æ¸ç½ï½ä»·æ ¼è¿ä¸ä¾¿å®ã
 å¸æå¥½ç¨ï¼é¢èç¨è¿äºå¾å¥½ç¨ï¼ç®è¤æ°´å«©åæ»ç½çï¼è¡¥æ°´ä¸éï¼ä»·æ ¼ä¹åéã
 å°±æ¯ç²¾åæ¶²å¤ªå°äºï¼ä¿æ¹¿ææä¸éã
 é¢èçè¡¥æ°´ææéå¸¸å¥½ï¼ä¿æ¹¿ææç¡®å®å¾èµï¼è¿ä¸ªé¢èç¸å¯¹äºè¶åèç½åç¾ç½çé£ä¸¤æ¬¾çé¢èçº¸è¦åä¸äºï¼ççä»·æ ¼åéã
-``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset 1.
-50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_0.5M_CN](https://
-huggingface.co/datasets/BelleGroup/train_0.5M_CN) 2.
+``` å10å¥æ¯çå®ç¨æ·è¯è®ºï¼å10å¥æ¯çæçã  ## ð Dataset
+#### SFT datasets - 50ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/
+train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN) -
 100ä¸æ¡ä¸­æChatGPTæä»¤Belleæ°æ®éï¼[BelleGroup/train_1M_CN](https://
-huggingface.co/datasets/BelleGroup/train_1M_CN) 3.
+huggingface.co/datasets/BelleGroup/train_1M_CN) -
 5ä¸æ¡è±æChatGPTæä»¤Alpacaæ°æ®éï¼[50k English Stanford Alpaca
-dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) 4.
+dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release) -
 2ä¸æ¡ä¸­æChatGPTæä»¤Alpacaæ°æ®éï¼[shibing624/alpaca-zh](https://
-huggingface.co/datasets/shibing624/alpaca-zh) 5.
+huggingface.co/datasets/shibing624/alpaca-zh) -
 69ä¸æ¡ä¸­ææä»¤Guanacoæ°æ®é(Belle50ä¸æ¡+Guanaco19ä¸æ¡)ï¼[Chinese-
 Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-
-Vicuna/guanaco_belle_merge_v1.0) 6. 240ä¸æ¡ä¸­æå»çæ°æ®é
+Vicuna/guanaco_belle_merge_v1.0) - 240ä¸æ¡ä¸­æå»çæ°æ®é
 (åæ¬é¢è®­ç»æ°æ®åæä»¤å¾®è°æ°æ®é)ï¼[shibing624/medical](https://
-huggingface.co/datasets/shibing624/medical) ## â Todo 1. [ ]
-æ°å¢å¤è½®å¯¹è¯æ°æ®å¾®è°æ¹æ³ 2. [ ] add reward model finetuning 3. [ ]
-add rl finetuning 4. [ ] add medical reward dataset 5. [ ] add llama in4
-training 6. [ ] add all training and predict demo in colab ## âï¸ Contact -
-Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/github/issues/
-shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues) -
-é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
+huggingface.co/datasets/shibing624/medical) -
+5ä¸æ¡è±æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[RyokoAI/ShareGPT52K](https://
+huggingface.co/datasets/RyokoAI/ShareGPT52K) -
+80ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[BelleGroup/multiturn_chat_0.8M]
+(https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M) -
+116ä¸æ¡ä¸­æChatGPTå¤è½®å¯¹è¯æ°æ®éï¼[fnlp/moss-002-sft-data](https://
+huggingface.co/datasets/fnlp/moss-002-sft-data) #### Reward Model datasets -
+åççoasst1æ°æ®éï¼[OpenAssistant/oasst1](https://huggingface.co/
+datasets/OpenAssistant/oasst1) - 2ä¸æ¡å¤è¯­è¨oasst1çrewardæ°æ®éï¼
+[tasksource/oasst1_pairwise_rlhf_reward](https://huggingface.co/datasets/
+tasksource/oasst1_pairwise_rlhf_reward) - 11ä¸æ¡è±æhh-
+rlhfçrewardæ°æ®éï¼[Dahoas/full-hh-rlhf](https://huggingface.co/datasets/
+Dahoas/full-hh-rlhf) - 9ä¸æ¡è±ærewardæ°æ®é(æ¥èªAnthropic's Helpful
+Harmless dataset)ï¼[Dahoas/static-hh](https://huggingface.co/datasets/Dahoas/
+static-hh) - 7ä¸æ¡è±ærewardæ°æ®éï¼æ¥æºåä¸ï¼ï¼[Dahoas/rm-
+static](https://huggingface.co/datasets/Dahoas/rm-static) -
+7ä¸æ¡ç¹ä½ä¸­æçrewardæ°æ®éï¼ç¿»è¯èªrm-staticï¼[liswei/rm-static-
+m2m100-zh](https://huggingface.co/datasets/liswei/rm-static-m2m100-zh) -
+7ä¸æ¡è±æRewardæ°æ®éï¼[yitingxie/rlhf-reward-datasets](https://
+huggingface.co/datasets/yitingxie/rlhf-reward-datasets) -
+3åæ¡ä¸­æç¥ä¹é®ç­åå¥½æ°æ®éï¼[liyucheng/zhihu_rlhf_3k](https://
+huggingface.co/datasets/liyucheng/zhihu_rlhf_3k) ## â Todo 1. [x] add
+multiple rounds of dialogue data fine-tuning method 2. [x] add reward model
+finetuning, go to [shibing624/MeidcalGPT](https://github.com/shibing624/
+MedicalGPT) 3. [x] add rl finetuning, go to [shibing624/MeidcalGPT](https://
+github.com/shibing624/MedicalGPT) 4. [x] add medical reward dataset 5. [x] add
+llama in4 training, go to [shibing624/MeidcalGPT](https://github.com/
+shibing624/MedicalGPT) 6. [ ] add all training and predict demo in colab ##
+âï¸ Contact - Issue(å»ºè®®) ï¼[![GitHub issues](https://img.shields.io/
+github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/
+issues) - é®ä»¶æï¼xuming: xuming624@qq.com - å¾®ä¿¡æï¼
 å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-å¬å¸å-NLP* è¿NLPäº¤æµç¾¤ã
 [docs/wechat.jpeg] ## ð Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtextgenï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ ```latex
-@misc{textgen, title={textgen: Text Generation Tool}, author={Xu Ming}, year=
+@misc{textgen, title={textgen: Text Generation Tool}, author={Ming Xu}, year=
 {2021}, howpublished={\url{https://github.com/shibing624/textgen}}, } ``` ##
-ð¤ License ææåè®®ä¸º [The Apache License 2.0](/
-LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå textgençé¾æ¥åææåè®®ã
-## ð Contribute
+ð¤ License This repository is licensed under [The Apache License 2.0]
+(LICENSE). Please follow the [Model Card](https://github.com/facebookresearch/
+llama/blob/main/MODEL_CARD.md) to use the LLaMA model. Please follow the [RAIL
+License](https://huggingface.co/spaces/bigscience/license) to use the BLOOM &
+BLOOMZ model. ## ð Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -
 m pytest`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
 ä¹åå³å¯æäº¤PRã ## ð Acknowledgements - [PaddlePaddle/ERNIE](https:/
 /github.com/PaddlePaddle/ERNIE) - [minimaxir/textgenrnn](https://github.com/
 minimaxir/textgenrnn) - [minimaxir/gpt-2-simple](https://github.com/minimaxir/
 gpt-2-simple) - [asyml/texar](https://github.com/asyml/texar) - [yangjianxin1/
```

### Comparing `textgen-0.2.7/textgen.egg-info/SOURCES.txt` & `textgen-1.0.0/textgen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,40 +11,37 @@
 textgen/augment/__init__.py
 textgen/augment/sentence_level_augment.py
 textgen/augment/text_augment.py
 textgen/augment/tokenizer.py
 textgen/augment/translate_api.py
 textgen/augment/word_level_augment.py
 textgen/augment/word_vocab.py
-textgen/bloom/__init__.py
-textgen/bloom/bloom_model.py
-textgen/bloom/bloom_utils.py
 textgen/chatglm/__init__.py
 textgen/chatglm/chatglm_model.py
 textgen/chatglm/chatglm_utils.py
 textgen/chatglm/merge_peft_adapter.py
 textgen/config/__init__.py
 textgen/config/global_args.py
 textgen/config/model_args.py
 textgen/custom_models/__init__.py
 textgen/custom_models/models.py
 textgen/data/HowNetPOSWord.txt
 textgen/data/stopwords.txt
+textgen/gpt/__init__.py
+textgen/gpt/gpt_model.py
+textgen/gpt/gpt_utils.py
+textgen/gpt/merge_peft_adapter.py
 textgen/language_generation/__init__.py
 textgen/language_generation/language_generation_model.py
 textgen/language_generation/language_generation_utils.py
 textgen/language_modeling/__init__.py
 textgen/language_modeling/language_modeling_model.py
 textgen/language_modeling/language_modeling_utils.py
 textgen/language_modeling/songnet_model.py
 textgen/language_modeling/songnet_utils.py
-textgen/llama/__init__.py
-textgen/llama/llama_model.py
-textgen/llama/llama_utils.py
-textgen/llama/merge_peft_adapter.py
 textgen/seq2seq/__init__.py
 textgen/seq2seq/bart_seq2seq_model.py
 textgen/seq2seq/bart_seq2seq_utils.py
 textgen/seq2seq/conv_seq2seq_model.py
 textgen/seq2seq/data_reader.py
 textgen/seq2seq/seq2seq_model.py
 textgen/seq2seq/seq2seq_trainer.py
```

