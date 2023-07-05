# Comparing `tmp/vilmedic-1.3.0.tar.gz` & `tmp/vilmedic-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vilmedic-1.3.0.tar", last modified: Tue Dec 13 13:00:11 2022, max compression
+gzip compressed data, was "vilmedic-1.3.1.tar", last modified: Wed Jul  5 17:45:58 2023, max compression
```

## Comparing `vilmedic-1.3.0.tar` & `vilmedic-1.3.1.tar`

### file list

```diff
@@ -1,720 +1,232 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.141419 vilmedic-1.3.0/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1069 2021-09-01 17:53:33.000000 vilmedic-1.3.0/LICENSE
--rw-rw-r--   0 jb        (1000) jb        (1000)      562 2022-12-13 13:00:11.141419 vilmedic-1.3.0/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)     8719 2022-07-18 20:35:32.000000 vilmedic-1.3.0/README.md
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.861416 vilmedic-1.3.0/bin/
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.881416 vilmedic-1.3.0/bin/scripts/
--rwxrwxr-x   0 jb        (1000) jb        (1000)     2972 2022-01-22 22:15:55.000000 vilmedic-1.3.0/bin/scripts/vilmedic-download
--rwxrwxr-x   0 jb        (1000) jb        (1000)     1292 2022-11-12 06:15:08.000000 vilmedic-1.3.0/bin/scripts/vilmedic-metrics
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2022-12-13 13:00:11.141419 vilmedic-1.3.0/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)     2662 2022-12-13 12:28:58.000000 vilmedic-1.3.0/setup.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.881416 vilmedic-1.3.0/vilmedic/
--rw-rw-r--   0 jb        (1000) jb        (1000)       63 2022-01-27 21:08:57.000000 vilmedic-1.3.0/vilmedic/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.885416 vilmedic-1.3.0/vilmedic/blocks/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:53:32.000000 vilmedic-1.3.0/vilmedic/blocks/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.885416 vilmedic-1.3.0/vilmedic/blocks/classifier/
--rw-rw-r--   0 jb        (1000) jb        (1000)       34 2021-06-22 11:52:02.000000 vilmedic-1.3.0/vilmedic/blocks/classifier/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      493 2021-09-10 22:50:37.000000 vilmedic-1.3.0/vilmedic/blocks/classifier/classifier.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1390 2021-12-20 18:04:59.000000 vilmedic-1.3.0/vilmedic/blocks/classifier/evaluation.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.885416 vilmedic-1.3.0/vilmedic/blocks/huggingface/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-20 19:19:23.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.889417 vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16652 2022-10-26 23:50:40.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/beam_search.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2378 2022-10-27 00:02:11.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/decoder_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3032 2022-12-03 18:51:06.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/evaluation.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.889417 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2701 2022-12-03 17:53:18.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder/encoder_model.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.889417 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-09-08 04:14:11.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3289 2022-06-09 23:22:56.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/encoder_decoder_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3214 2022-06-09 23:38:08.000000 vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/evaluation.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.889417 vilmedic-1.3.0/vilmedic/blocks/losses/
--rw-rw-r--   0 jb        (1000) jb        (1000)      292 2022-02-01 21:34:21.000000 vilmedic-1.3.0/vilmedic/blocks/losses/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.889417 vilmedic-1.3.0/vilmedic/blocks/losses/mvqa/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3605 2022-01-31 22:18:56.000000 vilmedic-1.3.0/vilmedic/blocks/losses/mvqa/LabelSmoothingCrossEntropyLoss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-20 19:19:23.000000 vilmedic-1.3.0/vilmedic/blocks/losses/mvqa/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.893417 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1486 2022-11-09 21:55:30.000000 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/ConVIRTLoss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5907 2022-01-31 22:11:06.000000 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/GLoRIALoss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      683 2022-01-31 22:06:55.000000 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/InfoNCELoss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3647 2022-02-01 21:34:21.000000 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/VICREGLoss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-20 19:19:23.000000 vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.893417 vilmedic-1.3.0/vilmedic/blocks/rl/
--rw-rw-r--   0 jb        (1000) jb        (1000)     8677 2022-06-30 17:36:35.000000 vilmedic-1.3.0/vilmedic/blocks/rl/SCST.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-04-22 21:17:43.000000 vilmedic-1.3.0/vilmedic/blocks/rl/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.893417 vilmedic-1.3.0/vilmedic/blocks/rnn/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:53:33.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7056 2021-05-24 12:57:53.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/decoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6471 2021-12-20 18:05:00.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/evaluation.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.893417 vilmedic-1.3.0/vilmedic/blocks/rnn/layers/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:53:33.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/layers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3941 2021-04-07 12:18:42.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/layers/attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2362 2021-02-22 13:48:00.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/layers/ff.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1437 2021-04-07 11:33:39.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/layers/hierarchical_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3041 2021-09-03 23:37:52.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/rnn.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7016 2021-03-10 10:11:07.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/textencoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1895 2021-04-07 11:53:42.000000 vilmedic-1.3.0/vilmedic/blocks/rnn/visualdecoder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.897416 vilmedic-1.3.0/vilmedic/blocks/schedulers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      968 2022-05-10 21:23:57.000000 vilmedic-1.3.0/vilmedic/blocks/schedulers/DecreasingCosineAnnealingWarmRestarts.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5750 2022-02-01 20:04:59.000000 vilmedic-1.3.0/vilmedic/blocks/schedulers/LinearWarmupCosineAnnealingLR.py
--rw-rw-r--   0 jb        (1000) jb        (1000)       72 2022-02-01 20:06:31.000000 vilmedic-1.3.0/vilmedic/blocks/schedulers/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.901417 vilmedic-1.3.0/vilmedic/blocks/scorers/
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.901417 vilmedic-1.3.0/vilmedic/blocks/scorers/CheXbert/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/CheXbert/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9925 2022-06-24 07:48:30.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/CheXbert/chexbert.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.905417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/
--rw-r--r--   0 jb        (1000) jb        (1000)        0 2022-04-19 20:50:44.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.909417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bertscore/
--rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bertscore/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2576 2022-06-21 22:22:24.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bertscore/bertscore.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.909417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/
--rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1399 2022-05-13 19:10:13.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/bleu.py
--rwxrwxr-x   0 jb        (1000) jb        (1000)     8713 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/bleu_scorer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.909417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/
--rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/__init__.py
--rwxrwxr-x   0 jb        (1000) jb        (1000)     1869 2022-05-13 19:10:06.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/ciderD.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7740 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/ciderD_scorer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.913417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:15:19.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3638 2022-06-21 20:07:49.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7582 2022-04-15 19:47:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL_scorer.py
--rwxrwxr-x   0 jb        (1000) jb        (1000)     4302 2022-05-13 19:08:38.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/mauve_.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.913417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/meteor/
--rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2022-04-19 16:38:05.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/meteor/__init__.py
--rwxrwxr-x   0 jb        (1000) jb        (1000)     5322 2022-05-13 19:09:45.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/meteor/meteor.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.913417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/rouge/
--rwxrwxr-x   0 jb        (1000) jb        (1000)       23 2022-04-19 16:38:06.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/rouge/__init__.py
--rwxrwxr-x   0 jb        (1000) jb        (1000)     1379 2022-05-13 19:09:22.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/rouge/rouge.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.913417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/
--rwxr-xr-x   0 jb        (1000) jb        (1000)        0 2021-02-17 15:20:17.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.913417 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/lib/
--rwxrwxr-x   0 jb        (1000) jb        (1000)        0 2021-02-17 15:20:17.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/lib/__init__.py
--rw-r--r--   0 jb        (1000) jb        (1000)     2859 2021-02-17 17:58:41.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/spice.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.917417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityMatchExact/
--rw-rw-r--   0 jb        (1000) jb        (1000)     2164 2022-06-19 21:48:43.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityMatchExact/RadEntityMatchExact.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityMatchExact/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.921417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/
--rw-rw-r--   0 jb        (1000) jb        (1000)     4529 2022-03-02 19:59:49.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/BERTNLI.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7563 2022-07-14 22:46:58.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/RadEntityNLI.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13204 2022-05-17 19:02:24.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/nli.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6401 2022-03-16 20:11:54.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/test.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.933417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/
--rw-rw-r--   0 jb        (1000) jb        (1000)     7109 2022-06-23 00:27:35.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/RadGraph.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-03-31 03:16:32.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.933417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/
--rw-rw-r--   0 jb        (1000) jb        (1000)      995 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1041 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/__main__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.941417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3399 2022-03-04 00:37:12.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5994 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/evaluate.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11702 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/find_learning_rate.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6691 2022-03-08 00:10:02.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/predict.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2395 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/print_results.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1553 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/subcommand.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1643 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/test_install.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    29872 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/commands/train.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.949417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/
--rw-rw-r--   0 jb        (1000) jb        (1000)      263 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3780 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/cached_transformers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4525 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/checks.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18357 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/file_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    26005 2022-03-04 23:29:54.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/from_params.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2007 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/lazy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4133 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/logging.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22746 2022-03-31 05:52:50.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/params.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1924 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/plugins.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8809 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/registrable.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.953417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/testing/
--rw-rw-r--   0 jb        (1000) jb        (1000)     2843 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/testing/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2128 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/testing/distributed_test.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18226 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/testing/model_test_case.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2102 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/testing/test_case.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2954 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/tqdm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    20836 2022-07-13 21:41:58.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/common/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.957417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/
--rw-rw-r--   0 jb        (1000) jb        (1000)      707 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9215 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/batch.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6415 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataloader.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.961417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      923 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3753 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/babi.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8487 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/conll2003.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    20986 2022-06-06 19:06:25.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/dataset_reader.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.961417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/dataset_utils/
--rw-rw-r--   0 jb        (1000) jb        (1000)      346 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/dataset_utils/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    17314 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/dataset_utils/span_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4097 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/interleaving_dataset_reader.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3503 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/sequence_tagging.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3649 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/sharded_dataset_reader.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5667 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/dataset_readers/text_classification_json.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.969417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/
--rw-rw-r--   0 jb        (1000) jb        (1000)      959 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6419 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/adjacency_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2570 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/array_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6789 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1275 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/flag_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2365 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/index_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4880 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/label_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5227 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/list_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2267 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/metadata_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6301 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/multilabel_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1977 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/namespace_swapping_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      753 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/sequence_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6157 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/sequence_label_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2742 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/span_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7547 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/fields/text_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4596 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/instance.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.969417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/samplers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      353 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/samplers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7352 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/samplers/bucket_batch_sampler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4617 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/samplers/max_tokens_batch_sampler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5502 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/samplers/samplers.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.973417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      733 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5990 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/elmo_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9970 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/pretrained_transformer_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5255 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/pretrained_transformer_mismatched_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4878 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/single_id_token_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2408 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/spacy_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6859 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/token_characters_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6281 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/token_indexers/token_indexer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.977417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      619 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3539 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/character_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      750 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/letters_digits_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19248 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/pretrained_transformer_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2641 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/sentence_splitter.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5781 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/spacy_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3897 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/token.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2768 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      865 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/tokenizers/whitespace_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    37452 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/data/vocabulary.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.977417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/
--rw-rw-r--   0 jb        (1000) jb        (1000)      153 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.977417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      188 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2270 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/attacker.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19833 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/hotflip.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9464 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/input_reduction.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1930 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/attackers/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.977417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/
--rw-rw-r--   0 jb        (1000) jb        (1000)      354 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3893 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/integrated_gradient.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1198 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/saliency_interpreter.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2892 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/simple_gradient.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3255 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/interpret/saliency_interpreters/smooth_gradient.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.981417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      337 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7507 2022-03-04 22:34:22.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/archival.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7164 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/basic_classifier.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19909 2022-03-05 00:29:00.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9590 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/models/simple_tagger.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.989417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1256 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.993417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/
--rw-rw-r--   0 jb        (1000) jb        (1000)      436 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2357 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/additive_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1740 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2376 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/bilinear_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      803 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/cosine_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      495 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/dot_product_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3353 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/attention/linear_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21567 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/augmented_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15794 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/bimpm_matching.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    17942 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/conditional_random_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    28994 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/elmo.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15105 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/elmo_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16843 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/encoder_base.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4165 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/feedforward.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1346 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/gated_sum.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2682 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/highway.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1245 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/input_variational_dropout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1115 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/layer_norm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12224 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/lstm_cell_with_projection.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1073 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/masked_layer_norm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.993417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/
--rw-rw-r--   0 jb        (1000) jb        (1000)      460 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3443 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/bilinear_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      860 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/cosine_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      564 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/dot_product_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3378 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/linear_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      812 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/matrix_attention/matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3854 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/maxout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2506 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/residual_with_layer_dropout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11369 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/sampled_softmax_loss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3795 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/scalar_mix.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.997418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1863 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2440 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/compose_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1462 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/feedforward_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8183 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/gated_cnn_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1598 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/pass_through_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10634 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4656 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/pytorch_transformer_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1574 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2seq_encoders/seq2seq_encoder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.001417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1469 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2670 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/bert_pooler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2350 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/boe_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2238 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/cls_pooler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5933 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/cnn_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5995 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/cnn_highway_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10173 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/pytorch_seq2vec_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1215 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/seq2vec_encoders/seq2vec_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1126 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/softmax_loss.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.001417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      403 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12581 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/bidirectional_endpoint_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7819 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/endpoint_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3293 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/self_attentive_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2702 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/span_extractors/span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4962 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/stacked_alternating_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6459 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/stacked_bidirectional_lstm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.005417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/text_field_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      383 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/text_field_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4496 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/text_field_embedders/basic_text_field_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2520 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/text_field_embedders/text_field_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2594 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/time_distributed.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.005417 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      945 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3251 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/bag_of_word_counts_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4700 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/elmo_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    29358 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/embedding.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      893 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/empty_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      656 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/pass_through_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15213 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/pretrained_transformer_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4713 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/pretrained_transformer_mismatched_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1654 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/token_characters_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1379 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/modules/token_embedders/token_embedder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.009418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/
--rw-rw-r--   0 jb        (1000) jb        (1000)      178 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4279 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/activations.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16343 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/beam_search.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10283 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/chu_liu_edmonds.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19786 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/initializers.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.013418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/regularizers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      407 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/regularizers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      344 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/regularizers/regularizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1477 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/regularizers/regularizer_applicator.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      929 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/regularizers/regularizers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    87204 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/nn/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.013418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      439 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13243 2022-03-07 19:16:39.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/predictors/predictor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4322 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/predictors/sentence_tagger.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1803 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/predictors/text_classifier.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.017418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2648 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/tools/archive_surgery.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5179 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/tools/create_elmo_embeddings_from_vocab.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      782 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/tools/inspect_cache.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.017418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/
--rw-rw-r--   0 jb        (1000) jb        (1000)      324 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10794 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/checkpointer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.021418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1592 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3056 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/cosine.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4579 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/learning_rate_scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      958 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/linear_with_warmup.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2241 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/noam.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2736 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/polynomial_decay.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7769 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/learning_rate_schedulers/slanted_triangular.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5806 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metric_tracker.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.029418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1513 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5609 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/attachment_scores.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5313 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/auc.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1802 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/average.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7314 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/bleu.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4651 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/boolean_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4977 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/categorical_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5978 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/covariance.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2014 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/entropy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8132 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/evalb_bracketing_scorer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2873 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/f1_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10740 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/fbeta_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2318 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/mean_absolute_error.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1755 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/metric.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3587 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/pearson_correlation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      853 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/perplexity.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8889 2022-04-21 04:56:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/rouge.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3517 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/sequence_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13372 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/span_based_f1_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4517 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/spearman_correlation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3754 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/metrics/unigram_recall.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.029418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/momentum_schedulers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      176 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/momentum_schedulers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1651 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/momentum_schedulers/inverted_triangular.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      384 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/momentum_schedulers/momentum_scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3699 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/moving_average.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1277 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/no_op_trainer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22076 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/optimizers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3085 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15597 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/tensorboard_writer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    50859 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/trainer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18554 2022-02-25 22:39:27.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/training/util.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      463 2022-02-25 22:39:26.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp/version.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.029418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.029418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/
--rw-rw-r--   0 jb        (1000) jb        (1000)      134 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.029418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      136 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6432 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/dataset_readers/stanford_sentiment_tree_bank.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.033418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      127 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15298 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/classification/models/biattentive_classification_network.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.033418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/common/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/common/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10098 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/common/model_card.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    20658 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/common/ontonotes.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.033418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/
--rw-rw-r--   0 jb        (1000) jb        (1000)      455 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.037418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4960 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/dataset_readers/conll.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4838 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/dataset_readers/preco.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7052 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/dataset_readers/winobias.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.037418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9861 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/metrics/conll_coref_scores.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2108 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/metrics/mention_recall.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.037418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       67 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    42651 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/models/coref.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.037418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8019 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/predictors/coref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8720 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/coref/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.037418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/
--rw-rw-r--   0 jb        (1000) jb        (1000)      227 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.041418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      264 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6643 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/dataset_readers/cnn_dm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8915 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/dataset_readers/copynet_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7136 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/dataset_readers/seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.041418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      287 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16059 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/bart.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6907 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/composed_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    45913 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/copynet_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    25761 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/models/simple_seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.041418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)      145 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.045418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/decoder_nets/
--rw-rw-r--   0 jb        (1000) jb        (1000)      295 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/decoder_nets/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3827 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/decoder_nets/decoder_net.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5498 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/decoder_nets/lstm_cell.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6683 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/decoder_nets/stacked_self_attention.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.045418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/seq_decoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      184 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/seq_decoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21624 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/seq_decoders/auto_regressive.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2816 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/modules/seq_decoders/seq_decoder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.045418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       75 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      886 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/generation/predictors/seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.045418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/
--rw-rw-r--   0 jb        (1000) jb        (1000)      195 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.045418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      294 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6010 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/dataset_readers/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4234 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/dataset_readers/next_token_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3865 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/dataset_readers/simple_language_modeling.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.049418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      293 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2592 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/bidirectional_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13681 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7694 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6011 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/models/next_token_lm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.049418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)      198 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.049418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/
--rw-rw-r--   0 jb        (1000) jb        (1000)      363 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1511 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/bert.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1515 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/gpt2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      505 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/language_model_head.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1307 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/language_model_heads/linear.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.049418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      132 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11032 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.053418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/token_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      218 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/token_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2389 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/token_embedders/bidirectional_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8803 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/token_embedders/language_model.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.053418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      170 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1300 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/predictors/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1379 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/predictors/next_token_lm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.053418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.053418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      207 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1124 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/commonsenseqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3035 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/fake.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1491 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/piqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      958 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/swag.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3107 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/dataset_readers/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.057418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       67 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4693 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/models/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.057418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       80 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      735 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/mc/predictors/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.057418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/
--rw-rw-r--   0 jb        (1000) jb        (1000)      205 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.057418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      199 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3856 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/dataset_readers/quora_paraphrase.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5037 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/dataset_readers/snli.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.057418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      232 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9473 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/models/bimpm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9408 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/models/decomposable_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9526 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/models/esim.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.061418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      114 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1955 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pair_classification/predictors/textual_entailment.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2141 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/pretrained.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.061418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/
--rw-rw-r--   0 jb        (1000) jb        (1000)      195 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.061418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      421 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    27611 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/drop.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3673 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/qangaroo.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6776 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/quac.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7572 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12487 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/transformer_squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7741 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/triviaqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22599 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/dataset_readers/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.065418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)      134 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3384 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/metrics/drop_em_and_f1.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2725 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/metrics/squad_em_and_f1.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.069418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      442 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18668 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/bidaf.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7780 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/bidaf_ensemble.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    27385 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/dialog_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    32960 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/naqanet.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13900 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/qanet.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11488 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/transformer_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2149 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/models/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.069418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)       79 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.069418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      313 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7398 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/seq2seq_encoders/multi_head_self_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11382 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/seq2seq_encoders/qanet_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7515 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/modules/seq2seq_encoders/stacked_self_attention.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.073418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      228 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6075 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/predictors/bidaf.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2788 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/predictors/dialog_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4091 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/predictors/transformer_qa.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.073418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11222 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/drop.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2518 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/narrativeqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3680 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/orb.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4396 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/orb_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4830 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/quoref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3430 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1919 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/squad2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3368 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/rc/tools/transformer_qa.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.073418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/
--rw-rw-r--   0 jb        (1000) jb        (1000)      271 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.077418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      476 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10536 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/penn_tree_bank.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4794 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/semantic_dependencies.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11801 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/srl.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4974 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/dataset_readers/universal_dependencies.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.077418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)       88 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7652 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/metrics/srl_eval_scorer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.081418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      455 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    31241 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/biaffine_dependency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21974 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/constituency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16178 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/graph_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21005 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/srl.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13459 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/models/srl_bert.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.081418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      427 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7139 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/biaffine_dependency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5782 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/constituency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8394 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/openie.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9090 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/predictors/srl.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.081418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8456 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/tools/convert_openie_to_conll.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4295 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/structured_prediction/tools/write_srl_predictions_to_conll_format.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.081418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/
--rw-rw-r--   0 jb        (1000) jb        (1000)      169 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      349 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9099 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/ccgbank.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6995 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/conll2000.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      166 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/conll2003.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5004 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/dataset_readers/ontonotes_ner.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       64 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12939 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/models/crf_tagger.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       87 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      163 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/tagging/predictors/sentence_tagger.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      373 2021-12-28 23:40:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/version.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/
--rw-rw-r--   0 jb        (1000) jb        (1000)      114 2022-05-23 21:28:08.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.085418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-05-23 21:26:45.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    25830 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/dataset_readers/document.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8582 2022-03-08 00:08:19.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/dataset_readers/dygie.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.089418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/fields/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-05-23 21:26:45.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/fields/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6430 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/data/fields/adjacency_field_assym.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.093418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       37 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    37289 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/coref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16733 2022-06-15 16:35:35.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/dygie.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9377 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/entity_beam_pruner.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21753 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/events.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7275 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/ner.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12272 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/relation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2131 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/models/shared.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.093418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       50 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2562 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/predictors/dygie.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.093418 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-05-23 21:26:45.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6731 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/event_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      360 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/f1.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2209 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/ner_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1515 2021-12-14 17:21:21.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/dygie/training/relation_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    27837 2022-06-23 05:21:39.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/reward_functions.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5263 2022-07-06 20:44:48.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      501 2022-06-21 20:32:24.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8224 2022-03-16 17:02:34.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/post_processing.py
--rw-r--r--   0 jb        (1000) jb        (1000)     4360 2022-09-12 11:51:22.000000 vilmedic-1.3.0/vilmedic/blocks/scorers/scores.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.093418 vilmedic-1.3.0/vilmedic/blocks/vision/
--rw-rw-r--   0 jb        (1000) jb        (1000)       52 2021-08-03 05:09:09.000000 vilmedic-1.3.0/vilmedic/blocks/vision/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5011 2022-11-01 21:18:03.000000 vilmedic-1.3.0/vilmedic/blocks/vision/cnn.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.097418 vilmedic-1.3.0/vilmedic/blocks/vision/selfsup/
--rw-rw-r--   0 jb        (1000) jb        (1000)       22 2022-04-29 18:59:07.000000 vilmedic-1.3.0/vilmedic/blocks/vision/selfsup/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5254 2022-05-02 21:49:39.000000 vilmedic-1.3.0/vilmedic/blocks/vision/selfsup/moco.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3314 2021-07-13 14:07:57.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vgg_hgap.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.105419 vilmedic-1.3.0/vilmedic/blocks/vision/vit/
--rw-rw-r--   0 jb        (1000) jb        (1000)       65 2022-01-13 19:50:18.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10113 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/ats_vit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5688 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/cait.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12904 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/cct.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9049 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/cross_vit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8234 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/crossformer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5938 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/cvt.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4491 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/deepvit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9662 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/dino.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4466 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/distill.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1564 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/efficient.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1987 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6363 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/levit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4911 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/local_vit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3653 2022-05-19 20:07:47.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/mae.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7812 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/mobile_vit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5797 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/mpp.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5800 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/nest.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5751 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/pit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1739 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/recorder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8890 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/regionvit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7710 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/rvt.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2640 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/simmim.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2956 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/t2t.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7912 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/twins_svt.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4147 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/vit.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4914 2022-01-06 21:14:41.000000 vilmedic-1.3.0/vilmedic/blocks/vision/vit/vit_for_small_dataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      261 2022-01-22 22:17:38.000000 vilmedic-1.3.0/vilmedic/constants.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.109418 vilmedic-1.3.0/vilmedic/datasets/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1436 2021-12-28 21:36:15.000000 vilmedic-1.3.0/vilmedic/datasets/ImLabel.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1565 2022-05-06 21:23:11.000000 vilmedic-1.3.0/vilmedic/datasets/ImSeq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1059 2021-12-28 18:34:32.000000 vilmedic-1.3.0/vilmedic/datasets/ImSeq2Seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1253 2021-12-28 18:29:14.000000 vilmedic-1.3.0/vilmedic/datasets/ImSeqLabel.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1773 2022-06-09 17:17:49.000000 vilmedic-1.3.0/vilmedic/datasets/Seq2Seq.py
--rw-r--r--   0 jb        (1000) jb        (1000)      392 2022-07-13 21:44:23.000000 vilmedic-1.3.0/vilmedic/datasets/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.113418 vilmedic-1.3.0/vilmedic/datasets/base/
--rw-rw-r--   0 jb        (1000) jb        (1000)     7944 2022-11-09 21:46:39.000000 vilmedic-1.3.0/vilmedic/datasets/base/ImageDataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3022 2021-12-28 21:24:18.000000 vilmedic-1.3.0/vilmedic/datasets/base/LabelDataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5917 2022-07-13 20:50:25.000000 vilmedic-1.3.0/vilmedic/datasets/base/TextDataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/datasets/base/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.121419 vilmedic-1.3.0/vilmedic/datasets/base/papers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      809 2022-05-02 20:40:50.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/IndexDataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2115 2022-01-19 23:33:31.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/RCNNDataset.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2022-01-24 21:04:41.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1910 2022-04-27 20:46:53.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/open_image.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4195 2022-06-18 05:09:38.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/report_preprocessing.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.125419 vilmedic-1.3.0/vilmedic/datasets/base/papers/transforms/
--rw-rw-r--   0 jb        (1000) jb        (1000)       86 2022-04-27 21:30:00.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/transforms/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6635 2022-05-02 22:11:00.000000 vilmedic-1.3.0/vilmedic/datasets/base/papers/transforms/swav.py
--rw-r--r--   0 jb        (1000) jb        (1000)     1511 2021-12-01 22:52:17.000000 vilmedic-1.3.0/vilmedic/datasets/base/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.129419 vilmedic-1.3.0/vilmedic/executors/
--rw-r--r--   0 jb        (1000) jb        (1000)      132 2021-06-21 14:26:20.000000 vilmedic-1.3.0/vilmedic/executors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6963 2022-05-06 06:15:09.000000 vilmedic-1.3.0/vilmedic/executors/trainor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10466 2022-06-03 19:36:17.000000 vilmedic-1.3.0/vilmedic/executors/utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3729 2022-07-14 19:32:59.000000 vilmedic-1.3.0/vilmedic/executors/validator.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.129419 vilmedic-1.3.0/vilmedic/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1082 2022-10-21 20:08:37.000000 vilmedic-1.3.0/vilmedic/models/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.129419 vilmedic-1.3.0/vilmedic/models/mvqa/
--rw-rw-r--   0 jb        (1000) jb        (1000)     2037 2022-01-31 22:20:51.000000 vilmedic-1.3.0/vilmedic/models/mvqa/MVQA.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:52:27.000000 vilmedic-1.3.0/vilmedic/models/mvqa/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.129419 vilmedic-1.3.0/vilmedic/models/others/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1907 2022-01-27 21:13:13.000000 vilmedic-1.3.0/vilmedic/models/others/RCNN.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:53:56.000000 vilmedic-1.3.0/vilmedic/models/others/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2908 2022-01-27 21:11:58.000000 vilmedic-1.3.0/vilmedic/models/others/sim_mcan.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.133419 vilmedic-1.3.0/vilmedic/models/rrg/
--rw-rw-r--   0 jb        (1000) jb        (1000)    13744 2021-10-29 21:39:43.000000 vilmedic-1.3.0/vilmedic/models/rrg/PPOTrainer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3132 2022-12-03 18:04:16.000000 vilmedic-1.3.0/vilmedic/models/rrg/RRG.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3356 2022-08-11 17:23:05.000000 vilmedic-1.3.0/vilmedic/models/rrg/RRG_EEG.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6893 2022-03-31 05:28:04.000000 vilmedic-1.3.0/vilmedic/models/rrg/RRG_PPO.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3279 2022-10-26 22:24:01.000000 vilmedic-1.3.0/vilmedic/models/rrg/RRG_SCST.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:52:36.000000 vilmedic-1.3.0/vilmedic/models/rrg/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4116 2021-10-20 22:28:18.000000 vilmedic-1.3.0/vilmedic/models/rrg/core.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.133419 vilmedic-1.3.0/vilmedic/models/rrs/
--rw-rw-r--   0 jb        (1000) jb        (1000)     2033 2022-12-03 20:57:20.000000 vilmedic-1.3.0/vilmedic/models/rrs/RRS.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3024 2022-08-30 19:52:55.000000 vilmedic-1.3.0/vilmedic/models/rrs/RRS_SCST.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1980 2022-06-09 23:24:55.000000 vilmedic-1.3.0/vilmedic/models/rrs/RRS_obsolete.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7987 2022-04-21 05:16:33.000000 vilmedic-1.3.0/vilmedic/models/rrs/SumHugMono_SCST.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8907 2022-03-31 05:28:04.000000 vilmedic-1.3.0/vilmedic/models/rrs/SumHugMulti.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6348 2022-03-31 05:28:04.000000 vilmedic-1.3.0/vilmedic/models/rrs/SumHugMulti2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3707 2022-01-27 21:13:13.000000 vilmedic-1.3.0/vilmedic/models/rrs/SumRNN.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:51:36.000000 vilmedic-1.3.0/vilmedic/models/rrs/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.141419 vilmedic-1.3.0/vilmedic/models/selfsup/
--rw-rw-r--   0 jb        (1000) jb        (1000)    10100 2022-02-24 22:09:21.000000 vilmedic-1.3.0/vilmedic/models/selfsup/GLoRIA.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6490 2022-05-06 04:54:03.000000 vilmedic-1.3.0/vilmedic/models/selfsup/PCL.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9843 2022-05-10 22:47:48.000000 vilmedic-1.3.0/vilmedic/models/selfsup/PCL2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2543 2022-03-11 19:41:06.000000 vilmedic-1.3.0/vilmedic/models/selfsup/SimCLR.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4532 2022-05-10 17:12:10.000000 vilmedic-1.3.0/vilmedic/models/selfsup/SwaV.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3242 2022-03-16 17:03:54.000000 vilmedic-1.3.0/vilmedic/models/selfsup/VICREG.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-09-30 23:45:23.000000 vilmedic-1.3.0/vilmedic/models/selfsup/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.141419 vilmedic-1.3.0/vilmedic/models/selfsup/clip/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3019 2022-01-27 21:13:13.000000 vilmedic-1.3.0/vilmedic/models/selfsup/clip/CLIP.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4100 2022-01-27 21:13:13.000000 vilmedic-1.3.0/vilmedic/models/selfsup/clip/DALLE.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1922 2022-01-27 21:13:13.000000 vilmedic-1.3.0/vilmedic/models/selfsup/clip/VAE.py
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-08-31 21:51:07.000000 vilmedic-1.3.0/vilmedic/models/selfsup/clip/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3565 2022-01-22 21:36:09.000000 vilmedic-1.3.0/vilmedic/models/selfsup/clip/dalle_forward.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3437 2022-11-09 21:55:27.000000 vilmedic-1.3.0/vilmedic/models/selfsup/conVIRT.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      865 2021-12-21 18:54:02.000000 vilmedic-1.3.0/vilmedic/models/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:11.141419 vilmedic-1.3.0/vilmedic/zoo/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2021-12-20 19:19:23.000000 vilmedic-1.3.0/vilmedic/zoo/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5365 2022-12-13 12:50:36.000000 vilmedic-1.3.0/vilmedic/zoo/modeling_auto.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2149 2022-12-13 12:51:26.000000 vilmedic-1.3.0/vilmedic/zoo/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2022-12-13 13:00:10.885416 vilmedic-1.3.0/vilmedic.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)      562 2022-12-13 13:00:10.000000 vilmedic-1.3.0/vilmedic.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)    38439 2022-12-13 13:00:10.000000 vilmedic-1.3.0/vilmedic.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2022-12-13 13:00:10.000000 vilmedic-1.3.0/vilmedic.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2022-02-25 22:02:40.000000 vilmedic-1.3.0/vilmedic.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)      653 2022-12-13 13:00:10.000000 vilmedic-1.3.0/vilmedic.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        9 2022-12-13 13:00:10.000000 vilmedic-1.3.0/vilmedic.egg-info/top_level.txt
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.102704 vilmedic-1.3.1/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1069 2023-01-06 19:33:14.000000 vilmedic-1.3.1/LICENSE
+-rw-rw-r--   0 jb        (1000) jb        (1000)      515 2023-07-05 17:45:58.102704 vilmedic-1.3.1/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9238 2023-02-07 20:11:19.000000 vilmedic-1.3.1/README.md
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.034703 vilmedic-1.3.1/bin/
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.042703 vilmedic-1.3.1/bin/scripts/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     2971 2023-05-19 17:20:25.000000 vilmedic-1.3.1/bin/scripts/vilmedic-download
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     1270 2023-06-29 21:17:30.000000 vilmedic-1.3.1/bin/scripts/vilmedic-metrics
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2023-07-05 17:45:58.102704 vilmedic-1.3.1/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2590 2023-06-29 21:17:51.000000 vilmedic-1.3.1/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.042703 vilmedic-1.3.1/vilmedic/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      467 2023-05-22 23:00:22.000000 vilmedic-1.3.1/vilmedic/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.042703 vilmedic-1.3.1/vilmedic/blocks/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.046703 vilmedic-1.3.1/vilmedic/blocks/classifier/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       34 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/classifier/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      493 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/classifier/classifier.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2307 2023-06-21 23:14:16.000000 vilmedic-1.3.1/vilmedic/blocks/classifier/evaluation.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.046703 vilmedic-1.3.1/vilmedic/blocks/huggingface/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.046703 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16640 2023-03-28 18:25:49.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/beam_search.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2435 2023-03-28 18:11:16.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/decoder_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3576 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/evaluation.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3954 2023-05-11 20:31:37.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/evaluation_force.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.046703 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2701 2023-01-19 21:25:42.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder/encoder_model.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.046703 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3289 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/encoder_decoder_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3252 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/evaluation.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.050704 vilmedic-1.3.1/vilmedic/blocks/losses/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      328 2023-05-05 20:15:54.000000 vilmedic-1.3.1/vilmedic/blocks/losses/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.050704 vilmedic-1.3.1/vilmedic/blocks/losses/mvqa/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3605 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/mvqa/LabelSmoothingCrossEntropyLoss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/mvqa/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.050704 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1486 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/ConVIRTLoss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5907 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/GLoRIALoss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      683 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/InfoNCELoss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3647 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/VICREGLoss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.050704 vilmedic-1.3.1/vilmedic/blocks/rl/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8677 2023-01-31 22:06:19.000000 vilmedic-1.3.1/vilmedic/blocks/rl/SCST.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rl/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.054704 vilmedic-1.3.1/vilmedic/blocks/rnn/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7056 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/decoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6509 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/evaluation.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.054704 vilmedic-1.3.1/vilmedic/blocks/rnn/layers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/layers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3941 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/layers/attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2362 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/layers/ff.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1437 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/layers/hierarchical_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3041 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/rnn.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7016 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/textencoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1895 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/rnn/visualdecoder.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.054704 vilmedic-1.3.1/vilmedic/blocks/schedulers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      968 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/schedulers/DecreasingCosineAnnealingWarmRestarts.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5750 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/schedulers/LinearWarmupCosineAnnealingLR.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)       72 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/schedulers/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.058704 vilmedic-1.3.1/vilmedic/blocks/scorers/
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.058704 vilmedic-1.3.1/vilmedic/blocks/scorers/CheXbert/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/CheXbert/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9870 2023-05-22 22:59:16.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/CheXbert/chexbert.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.058704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.058704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bertscore/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bertscore/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2576 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bertscore/bertscore.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.058704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1399 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/bleu.py
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     8713 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/bleu_scorer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.062704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/__init__.py
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     1869 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/ciderD.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7740 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/ciderD_scorer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.062704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3638 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7582 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL_scorer.py
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     4302 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/mauve_.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.062704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/meteor/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)       21 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/meteor/__init__.py
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     5322 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/meteor/meteor.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/rouge/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)       23 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/rouge/__init__.py
+-rwxrwxr-x   0 jb        (1000) jb        (1000)     1379 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/rouge/rouge.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/lib/
+-rwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/lib/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2859 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/spice.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityMatchExact/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2110 2023-05-22 22:59:42.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityMatchExact/RadEntityMatchExact.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityMatchExact/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4529 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/BERTNLI.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7435 2023-05-22 22:59:42.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/RadEntityNLI.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13204 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/nli.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6401 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/test.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.066704 vilmedic-1.3.1/vilmedic/blocks/scorers/StanfordCTAbdAcc/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6490 2023-06-16 17:58:26.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/StanfordCTAbdAcc/StanfordCTAbdAcc.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:14.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/StanfordCTAbdAcc/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      525 2023-06-14 17:36:19.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8114 2023-05-22 22:59:55.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/post_processing.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4838 2023-06-14 17:36:51.000000 vilmedic-1.3.1/vilmedic/blocks/scorers/scores.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.070704 vilmedic-1.3.1/vilmedic/blocks/vision/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       52 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6053 2023-06-14 20:04:05.000000 vilmedic-1.3.1/vilmedic/blocks/vision/cnn.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.070704 vilmedic-1.3.1/vilmedic/blocks/vision/selfsup/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       22 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/selfsup/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5254 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/selfsup/moco.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3314 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vgg_hgap.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.082704 vilmedic-1.3.1/vilmedic/blocks/vision/vit/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       65 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10113 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/ats_vit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5688 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/cait.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12904 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/cct.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9049 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/cross_vit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8234 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/crossformer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5938 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/cvt.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4491 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/deepvit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9662 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/dino.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4466 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/distill.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1564 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/efficient.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1987 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/extractor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6363 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/levit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4911 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/local_vit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3653 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/mae.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7812 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/mobile_vit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5797 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/mpp.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5800 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/nest.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5751 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/pit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1739 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/recorder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8890 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/regionvit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7710 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/rvt.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2640 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/simmim.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2956 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/t2t.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7912 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/twins_svt.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4147 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/vit.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4914 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/blocks/vision/vit/vit_for_small_dataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      261 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/constants.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.086704 vilmedic-1.3.1/vilmedic/datasets/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1436 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/ImLabel.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1565 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/ImSeq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1059 2023-01-09 20:09:25.000000 vilmedic-1.3.1/vilmedic/datasets/ImSeq2Seq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1307 2023-05-10 22:22:43.000000 vilmedic-1.3.1/vilmedic/datasets/ImSeqAny.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1253 2023-05-10 21:10:14.000000 vilmedic-1.3.1/vilmedic/datasets/ImSeqLabel.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1773 2023-01-09 20:09:07.000000 vilmedic-1.3.1/vilmedic/datasets/Seq2Seq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      423 2023-05-10 21:12:57.000000 vilmedic-1.3.1/vilmedic/datasets/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.086704 vilmedic-1.3.1/vilmedic/datasets/base/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1484 2023-05-11 18:24:40.000000 vilmedic-1.3.1/vilmedic/datasets/base/AnyDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8003 2023-05-22 23:00:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/ImageDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3022 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/LabelDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5917 2023-05-08 22:31:37.000000 vilmedic-1.3.1/vilmedic/datasets/base/TextDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.090704 vilmedic-1.3.1/vilmedic/datasets/base/papers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      809 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/IndexDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2063 2023-05-22 23:00:33.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/RCNNDataset.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1910 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/open_image.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4195 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/report_preprocessing.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.090704 vilmedic-1.3.1/vilmedic/datasets/base/papers/transforms/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       86 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/transforms/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6635 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/papers/transforms/swav.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1511 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/datasets/base/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.090704 vilmedic-1.3.1/vilmedic/executors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      132 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/executors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6961 2023-06-21 21:09:47.000000 vilmedic-1.3.1/vilmedic/executors/trainor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10467 2023-05-19 18:39:06.000000 vilmedic-1.3.1/vilmedic/executors/utils.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3729 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/executors/validator.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.090704 vilmedic-1.3.1/vilmedic/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1238 2023-06-14 19:29:11.000000 vilmedic-1.3.1/vilmedic/models/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.090704 vilmedic-1.3.1/vilmedic/models/mvqa/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2044 2023-06-21 23:13:29.000000 vilmedic-1.3.1/vilmedic/models/mvqa/MVQA.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/mvqa/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.094704 vilmedic-1.3.1/vilmedic/models/others/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1907 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/others/RCNN.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/others/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2908 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/others/sim_mcan.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.094704 vilmedic-1.3.1/vilmedic/models/rrg/
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13744 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/PPOTrainer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3466 2023-06-14 20:12:00.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2421 2023-06-14 20:39:33.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_2D_CT.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3356 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_EEG.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3168 2023-05-11 18:38:38.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_FORCE.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3358 2023-01-09 20:41:18.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_MULTI.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6893 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_PPO.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3279 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/RRG_SCST.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4116 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrg/core.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.098704 vilmedic-1.3.1/vilmedic/models/rrs/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2033 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/RRS.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3024 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/RRS_SCST.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1980 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/RRS_obsolete.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7987 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/SumHugMono_SCST.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8907 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/SumHugMulti.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6348 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/SumHugMulti2.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3707 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/SumRNN.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/rrs/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.098704 vilmedic-1.3.1/vilmedic/models/selfsup/
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10138 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/models/selfsup/GLoRIA.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6490 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/PCL.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9843 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/PCL2.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2543 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/SimCLR.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4532 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/SwaV.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3280 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/models/selfsup/VICREG.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.098704 vilmedic-1.3.1/vilmedic/models/selfsup/clip/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3019 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/clip/CLIP.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4100 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/clip/DALLE.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1922 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/clip/VAE.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/clip/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3565 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/selfsup/clip/dalle_forward.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3475 2023-05-11 18:41:42.000000 vilmedic-1.3.1/vilmedic/models/selfsup/conVIRT.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      865 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/models/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.102704 vilmedic-1.3.1/vilmedic/zoo/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/zoo/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5365 2023-02-24 18:12:14.000000 vilmedic-1.3.1/vilmedic/zoo/modeling_auto.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2149 2023-01-06 19:33:15.000000 vilmedic-1.3.1/vilmedic/zoo/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-05 17:45:58.042703 vilmedic-1.3.1/vilmedic.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      515 2023-07-05 17:45:57.000000 vilmedic-1.3.1/vilmedic.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7033 2023-07-05 17:45:57.000000 vilmedic-1.3.1/vilmedic.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-05 17:45:57.000000 vilmedic-1.3.1/vilmedic.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-01-09 17:47:11.000000 vilmedic-1.3.1/vilmedic.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)      647 2023-07-05 17:45:57.000000 vilmedic-1.3.1/vilmedic.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        9 2023-07-05 17:45:57.000000 vilmedic-1.3.1/vilmedic.egg-info/top_level.txt
```

### Comparing `vilmedic-1.3.0/LICENSE` & `vilmedic-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/PKG-INFO` & `vilmedic-1.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Metadata-Version: 2.1
 Name: vilmedic
-Version: 1.3.0
+Version: 1.3.1
 Summary: ViLMedic is a modular framework for multimodal research at the intersection of vision and language in the medical field.
-Home-page: UNKNOWN
 Author: Jean-Benoit Delbrouck
 License: MIT
 Keywords: medical nlp deep-learning pytorch
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `vilmedic-1.3.0/README.md` & `vilmedic-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+### ViLMedic: a framework for research at the intersection of vision and language in medical AI
+
 <p align="center">
-  <a href="https://huggingface.co/spaces/StanfordAIMI/RRG_SPACE"> <b>New!🔥 </b> Checkout our live radiology report generation 📝 space on HuggingFace🤗</a>
+  <img src="https://vilmedic.app/favicon/favicon-64x64.png" alt="" style="width: 14px;"> ViLMedic has a dedicated website at: <a href="https://vilmedic.app/">https://vilmedic.app/</a>
 </p>
 
 <p align="center">
   <img src="docs/logo.png" width="190px">
   <br />
   <br />
   <a href="https://vilmedic.readthedocs.io/en/latest/">
@@ -11,19 +13,57 @@
   </a>
    <a href="https://github.com/jbdel/vilmedic/blob/master/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-red.svg" /></a>
   <img src="https://img.shields.io/badge/Stanford-Medicine-red" />
 </p>
 
 ---
 
-ViLMedic: a framework for research at the intersection of vision and language in medical AI
+
+<p align="center">
+  <a href="https://vilmedic.app/papers/emnlp2022"> <b>New!🔥 </b> Code for Improving the Factual Correctness of Radiology Report Generation with Semantic Rewards</a>
+</p>
+
+<p align="center">
+  <a href="https://huggingface.co/spaces/StanfordAIMI/RRG_SPACE"> <b>New!🔥 </b> Checkout our live radiology report generation 📝 space on HuggingFace🤗</a>
+</p>
+
+
+```bibtex
+@inproceedings{delbrouck-etal-2022-vilmedic,
+    title = "{V}i{LM}edic: a framework for research at the intersection of vision and language in medical {AI}",
+    author = "Delbrouck, Jean-benoit  and
+      Saab, Khaled  and
+      Varma, Maya  and
+      Eyuboglu, Sabri  and
+      Chambon, Pierre  and
+      Dunnmon, Jared  and
+      Zambrano, Juan  and
+      Chaudhari, Akshay  and
+      Langlotz, Curtis",
+    booktitle = "Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
+    month = may,
+    year = "2022",
+    address = "Dublin, Ireland",
+    publisher = "Association for Computational Linguistics",
+    url = "https://aclanthology.org/2022.acl-demo.3",
+    pages = "23--34",
+}
+```
+
+
+# Quickstart
+
+<p align="center">
+More at: <a href="https://vilmedic.app/">https://vilmedic.app/</a>
+</p>
+
 
 ## Installation
 ```
-conda create --name vilmedic python==3.9 -y
+conda create --name vilmedic python==3.8 -y
 git clone https://github.com/jbdel/vilmedic
 python setup.py develop
 ```
 
 
 ## Documentation
 
@@ -122,31 +162,11 @@
 
 -->
 
 ## Citation
 
 If you use ViLMedic in your work or use any models published in ViLMedic, please cite:
 
-```bibtex
-@inproceedings{delbrouck-etal-2022-vilmedic,
-    title = "{V}i{LM}edic: a framework for research at the intersection of vision and language in medical {AI}",
-    author = "Delbrouck, Jean-benoit  and
-      Saab, Khaled  and
-      Varma, Maya  and
-      Eyuboglu, Sabri  and
-      Chambon, Pierre  and
-      Dunnmon, Jared  and
-      Zambrano, Juan  and
-      Chaudhari, Akshay  and
-      Langlotz, Curtis",
-    booktitle = "Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
-    month = may,
-    year = "2022",
-    address = "Dublin, Ireland",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2022.acl-demo.3",
-    pages = "23--34",
-}
-```
+
 
 ## License
-ViLMedic is MIT-licensed. The license applies to the pre-trained models as well.
+ViLMedic is MIT-licensed. The license applies to the pre-trained models as well.
```

#### html2text {}

```diff
@@ -1,29 +1,44 @@
-     New!ð¥_Checkout_our_live_radiology_report_generation_ð_space_on
-                                HuggingFaceð¤
+### ViLMedic: a framework for research at the intersection of vision and
+language in medical AI
+           ViLMedic has a dedicated website at: https://vilmedic.app/
                                [docs/logo.png]
 
  [Documentation_Status] [MIT_License] [https://img.shields.io/badge/Stanford-
                                  Medicine-red]
---- ViLMedic: a framework for research at the intersection of vision and
-language in medical AI ## Installation ``` conda create --name vilmedic
-python==3.9 -y git clone https://github.com/jbdel/vilmedic python setup.py
-develop ``` ## Documentation Learn more about ViLMedic [here](https://
-vilmedic.readthedocs.io/en/latest/). ## Model Zoo ViLMedic hosts a [zoo of
-pretrained models](https://vilmedic.readthedocs.io/en/latest/vilmedic/
-model_zoo/overview.html). ``` from vilmedic import AutoModel model, processor =
-AutoModel.from_pretrained("selfsup/convirt-mimic") batch = processor.inference
-(seq=["no acute cardiopulmonary process"], image=["my_chest_xray.jpg"]) out =
-model(**batch) print(out.keys()) # dict_keys(['loss', 'loss_l', 'loss_v',
-'linguistic', 'visual']) ``` | Name | dataset | Report preprocessing | --------
------ |:-------------:|:-------------:| | **Radiology report generation** |
-rrg/biomed-roberta-baseline-mimic| [mimic-cxr](https://physionet.org/content/
-mimic-cxr-jpg/2.0.0/) | [r2gen](https://github.com/jbdel/vilmedic/blob/main/
-vilmedic/datasets/base/papers/report_preprocessing.py#L6) | rrg/biomed-roberta-
-baseline-indiana| [indiana](https://www.kaggle.com/raddar/chest-xrays-indiana-
+---
+    New!ð¥_Code_for_Improving_the_Factual_Correctness_of_Radiology_Report
+                       Generation_with_Semantic_Rewards
+     New!ð¥_Checkout_our_live_radiology_report_generation_ð_space_on
+                                HuggingFaceð¤
+```bibtex @inproceedings{delbrouck-etal-2022-vilmedic, title = "{V}i{LM}edic: a
+framework for research at the intersection of vision and language in medical
+{AI}", author = "Delbrouck, Jean-benoit and Saab, Khaled and Varma, Maya and
+Eyuboglu, Sabri and Chambon, Pierre and Dunnmon, Jared and Zambrano, Juan and
+Chaudhari, Akshay and Langlotz, Curtis", booktitle = "Proceedings of the 60th
+Annual Meeting of the Association for Computational Linguistics: System
+Demonstrations", month = may, year = "2022", address = "Dublin, Ireland",
+publisher = "Association for Computational Linguistics", url = "https://
+aclanthology.org/2022.acl-demo.3", pages = "23--34", } ``` # Quickstart
+                        More at: https://vilmedic.app/
+## Installation ``` conda create --name vilmedic python==3.8 -y git clone
+https://github.com/jbdel/vilmedic python setup.py develop ``` ## Documentation
+Learn more about ViLMedic [here](https://vilmedic.readthedocs.io/en/latest/).
+## Model Zoo ViLMedic hosts a [zoo of pretrained models](https://
+vilmedic.readthedocs.io/en/latest/vilmedic/model_zoo/overview.html). ``` from
+vilmedic import AutoModel model, processor = AutoModel.from_pretrained
+("selfsup/convirt-mimic") batch = processor.inference(seq=["no acute
+cardiopulmonary process"], image=["my_chest_xray.jpg"]) out = model(**batch)
+print(out.keys()) # dict_keys(['loss', 'loss_l', 'loss_v', 'linguistic',
+'visual']) ``` | Name | dataset | Report preprocessing | ------------- |:------
+-------:|:-------------:| | **Radiology report generation** | rrg/biomed-
+roberta-baseline-mimic| [mimic-cxr](https://physionet.org/content/mimic-cxr-
+jpg/2.0.0/) | [r2gen](https://github.com/jbdel/vilmedic/blob/main/vilmedic/
+datasets/base/papers/report_preprocessing.py#L6) | rrg/biomed-roberta-baseline-
+indiana| [indiana](https://www.kaggle.com/raddar/chest-xrays-indiana-
 university/) | [r2gen](https://github.com/jbdel/vilmedic/blob/main/vilmedic/
 datasets/base/papers/report_preprocessing.py#L6) | rrg/baseline-padchest|
 [padchest](https://bimcv.cipf.es/bimcv-projects/padchest/) | - | **Radiology
 report summarization** | rrs/biomed-roberta-baseline-mimic| [mimic-cxr](https:/
 /physionet.org/content/mimic-cxr-jpg/2.0.0/) | [rouge](https://github.com/
 jbdel/vilmedic/blob/main/vilmedic/datasets/base/papers/
 report_preprocessing.py#L70) | rrs/biomed-roberta-baseline-indiana| [indiana]
@@ -81,18 +96,9 @@
 Natural Language Supervision](https://arxiv.org/abs/2103.00020) | [SimCLR: A
 Simple Framework for Contrastive Learning of Visual Representations](https://
 arxiv.org/abs/2002.05709) | [GLoRIA: A Multimodal Global-Local Representation
 Learning Framework for Label-efficient Medical Image Recognition](https://
 openaccess.thecvf.com/content/ICCV2021/papers/Huang_GLoRIA_A_Multimodal_Global-
 Local_Representation_Learning_Framework_for_Label-
 Efficient_Medical_ICCV_2021_paper.pdf)  ## Citation If you use ViLMedic in your
-work or use any models published in ViLMedic, please cite: ```bibtex
-@inproceedings{delbrouck-etal-2022-vilmedic, title = "{V}i{LM}edic: a framework
-for research at the intersection of vision and language in medical {AI}",
-author = "Delbrouck, Jean-benoit and Saab, Khaled and Varma, Maya and Eyuboglu,
-Sabri and Chambon, Pierre and Dunnmon, Jared and Zambrano, Juan and Chaudhari,
-Akshay and Langlotz, Curtis", booktitle = "Proceedings of the 60th Annual
-Meeting of the Association for Computational Linguistics: System
-Demonstrations", month = may, year = "2022", address = "Dublin, Ireland",
-publisher = "Association for Computational Linguistics", url = "https://
-aclanthology.org/2022.acl-demo.3", pages = "23--34", } ``` ## License ViLMedic
+work or use any models published in ViLMedic, please cite: ## License ViLMedic
 is MIT-licensed. The license applies to the pre-trained models as well.
```

### Comparing `vilmedic-1.3.0/bin/scripts/vilmedic-download` & `vilmedic-1.3.1/bin/scripts/vilmedic-download`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 DATA_ZOO = {
     "RRS": ["1O7UebL2bcVF-vmoY2yyuoBAlG7M5KAKG", "15 Mb"],
     "RRG": ["1xUqztfFJz9pPYCVFJNSqkVDsUWyFqeId", "15 Mb"],
     "CLIP": ["1QdCGl8u5Q1__GezW_zHpwkHNvHkWbce5", "40 Mb"],
     "SELFSUP": ["1es-SrZaUdyyKf-1XnoirQ_Q0nZtQXtv0", "676.7 MB"],
     "MVQA": ["1YOr9fmc-zm8YwhWJIgjkjmF2Y0G_MSsV", "1 MB"],
 }
-
 IMAGE_ZOO = {
-    "indiana-images-512": ["1Cv9u3ZoOb8hZVcObMqHRNxsoAdZpYGt4", "1.27 GB"],
+    "indiana-images-512": ["1oUWkIMu4QEF7p_NINfRsywOG0I6EhT7I", "1.27 GB"],
     "imageclef-vqa-images-512": ["1ByPQ2TdXGz17pYDJKhrV05hka_XYH_pw", "327 MB"],
 }
 
 
 def download_images(data_name, file_id, unzip_dir):
     zip_name = os.path.join("data", data_name) + ".zip"
     target_dir = os.path.join(unzip_dir, data_name)
```

### Comparing `vilmedic-1.3.0/bin/scripts/vilmedic-metrics` & `vilmedic-1.3.1/bin/scripts/vilmedic-metrics`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 import json
 
 
 def main():
     try:
         hyps_file = sys.argv[1]
         refs_file = sys.argv[2]
+        metrics = sys.argv[3].split(",")
         print("Hyp file is", hyps_file)
         print("Ref file is", refs_file)
+        print("Metrics are", metrics)
     except IndexError:
-        print("Usage vilmedic-metrics hyps_file refs_file")
+        print("Usage vilmedic-metrics hyps_file refs_file metric1,metric2,...")
         return
 
     try:
         hyps = [line.strip() for line in open(hyps_file).readlines()]
         refs = [line.strip() for line in open(refs_file).readlines()]
     except FileNotFoundError as e:
         print(e)
         return
 
     print("Computing metrics, this can take a while...")
-    metrics = ["ROUGEL", "ROUGE1", "ROUGE2", "bertscore", "radgraph", "radentitymatchexact", "radentitynli", "chexbert"]
     print(json.dumps(compute_scores(metrics,
                                     refs=refs,
                                     hyps=hyps,
                                     split=None,
                                     seed=None,
                                     config=None,
                                     epoch=None,
```

### Comparing `vilmedic-1.3.0/setup.py` & `vilmedic-1.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,67 +3,65 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 8):
     sys.exit('Sorry, Python >=3.8 is required for ViLMedic.')
 
 setup(
     name='vilmedic',
-    version='1.3.0',
+    version='1.3.1',
     description='ViLMedic is a modular framework for multimodal research at the intersection of vision and language in the medical field.',
     author='Jean-Benoit Delbrouck',
     license='MIT',
     classifiers=[
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
     ],
     keywords='medical nlp deep-learning pytorch',
     python_requires='>=3.8',
     setup_requires="Cython",
-    install_requires=['appdirs==1.4.4',
+    install_requires=['appdirs',
                       'omegaconf==2.0.6',
+                      'urllib3==1.26.14',
+                      'protobuf==3.19.6',
                       'torchvision==0.9.1',
-                      'protobuf==3.19.3',
                       'rouge_score',
                       'youtokentome==1.0.3',
                       'tokenizers==0.11.6',
                       'scikit_image==0.18.2',
                       'scikit-learn==0.24.2',
                       'pydicom==2.2.0',
                       'transformers==4.23.1',
                       'seaborn==0.11.1',
                       'dalle-pytorch==1.4.2',
                       'torchxrayvision==0.0.32',
                       'stanza==1.3.0',
-                      'bert-score==0.3.11',
+                      'bert-score',
                       'torch==1.8.1',
                       'pytorch-lightning==1.4.2',
                       'pytorch-metric-learning==0.9.99',
                       'torch-optimizer==0.1.0',
                       'umap-learn',
                       'opencv-python==4.5.4.60',
                       'mauve-text',
-                      'numba==0.54.1',
+                      'numba',
                       'torchmetrics==0.5.0',
-                      'numpy==1.20.3',
+                      'numpy==1.21',
                       'gdown==4.6.0',
                       'spacy===3.2.3',
-                      # radgraph / allennlp dependencies
-                      'overrides==3.1.0',
-                      'boto3==1.21.13',
-                      'jsonpickle==2.1.0',
-                      'h5py==3.6.0',
-                      'tensorboard',
-                      'tensorboardX==2.5',
-                      ##
+                      'sentencepiece',
+                      'radgraph==0.0.5',
+                      'f1chexbert==0.0.1',
                       'psutil==5.9.0',
                       'lightning-bolts==0.5.0',
                       'faiss-gpu',
-                      'pyedflib'
+                      'pyedflib',
+                      'nibabel',
+                      'monai==1.1.0',
+                      'typing_extensions==4.4.0'
                       ],
     include_package_data=True,
     exclude_package_data={'': ['.git']},
     packages=find_packages(exclude=["bin"]),
-    scripts=[str(p) for p in pathlib.Path(
-        'bin/scripts').glob('*')],
+    scripts=[str(p) for p in pathlib.Path('bin/scripts').glob('*')],
     zip_safe=False)
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/beam_search.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/beam_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 from transformers.generation_utils import BeamSearchDecoderOnlyOutput
 
 
 def _validate_model_kwargs(self, model_kwargs):
     return
 
 
-def prepare_inputs_for_generation(self, input_ids, past=None, attention_mask=None, **model_kwargs):
+def prepare_inputs_for_generation(self, input_ids, past=None, attention_mask=None, **kwargs):
     input_shape = input_ids.shape
     # if model is used as a decoder in encoder-decoder model, the decoder attention mask is created on the fly
     if attention_mask is None:
         attention_mask = input_ids.new_ones(input_shape)
 
     # cut decoder_input_ids if past is used
     if past is not None:
         input_ids = input_ids[:, -1:]
-    return {"input_ids": input_ids, "attention_mask": attention_mask, "past_key_values": past, **model_kwargs}
+    return {"input_ids": input_ids, "attention_mask": attention_mask, "past_key_values": past, **kwargs}
 
 
 def beam_search(
         self,
         input_ids: torch.LongTensor,
         beam_scorer: BeamScorer,
         logits_processor: Optional[LogitsProcessorList] = None,
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/decoder_model.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/decoder_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             self.decoder = AutoModelForCausalLM.from_pretrained(path, config=dec_config)
         else:
             dec_config = BertGenerationConfig(**decoder)
             dec_config.is_decoder = True
             dec_config.add_cross_attention = True
             self.decoder = BertGenerationDecoder(dec_config)
             # self.decoder.generate
+            # self.decoder.prepare_inputs_for_generation
         # Evaluation
         self.decoder.prepare_inputs_for_generation = functools.partial(prepare_inputs_for_generation, self.decoder)
         # We override _validate_model_kwargs width empty function because we add custom model kwargs that triggers
         # errors in original _validate_model_kwargs
         self.decoder._validate_model_kwargs = functools.partial(_validate_model_kwargs, self.decoder)
 
         # Inference
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/decoder/evaluation.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/decoder/evaluation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import tqdm
 import torch
 import functools
 from .beam_search import beam_search
 import torch.nn as nn
 
 
+def get_special_token_ids(model, tokenizer):
+    bos_token_id = model.config.bos_token_id
+    eos_token_id = model.config.eos_token_id
+    pad_token_id = model.config.pad_token_id
+    if None in [bos_token_id, eos_token_id, pad_token_id]:
+        bos_token_id = tokenizer.vocab[tokenizer.cls_token]
+        eos_token_id = tokenizer.vocab[tokenizer.sep_token]
+        pad_token_id = tokenizer.vocab[tokenizer.pad_token]
+
+    return bos_token_id, eos_token_id, pad_token_id
+
+
 def evaluation(models, config, dl, **kwargs):
     models = [m if not isinstance(m, nn.DataParallel) else m.module for m in models]
     hf_models = [model.dec.decoder for model in models]
 
     # We are in an ensembling scenario, we override huggingface beam-search function
     hf_models[0].beam_search = functools.partial(beam_search, hf_models[0])
 
@@ -18,20 +30,23 @@
         tokenizer = dl.dataset.tokenizer
         max_len = dl.dataset.tokenizer_max_len
     except AttributeError:
         ref_str = 'decoder_input_ids'
         tokenizer = dl.dataset.tgt_tokenizer
         max_len = dl.dataset.tgt_tokenizer_max_len
 
+    # Get tokens
+    bos_token_id, eos_token_id, pad_token_id = get_special_token_ids(hf_models[0], tokenizer)
+
     ref_list = []
     hyp_list = []
 
     with torch.no_grad():
         for batch in tqdm.tqdm(dl):
-            batch = {k: v.cuda() for k, v in batch.items()}
+            batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
             # Expanding inputs
             batch_size = batch[ref_str].shape[0]
             expanded_return_idx = (
                 torch.arange(batch_size).view(-1, 1).repeat(1, config.beam_width).view(-1).cuda()
             )
             # Getting encoder infos
             encoder_outputs = []
@@ -50,22 +65,22 @@
                          } for output, mask in zip(encoder_outputs, encoder_attention_masks)
                     ],
                 "hf_models": hf_models
             }
 
             # lets gooooo
             hyps = hf_models[0].generate(
-                input_ids=torch.ones((batch_size, 1), dtype=torch.long).cuda() * hf_models[0].config.bos_token_id,
+                input_ids=torch.ones((batch_size, 1), dtype=torch.long).cuda() * bos_token_id,
                 num_return_sequences=1,
                 max_length=max_len,
                 num_beams=config.beam_width,
                 length_penalty=config.length_penalty,
-                bos_token_id=hf_models[0].config.bos_token_id,
-                eos_token_id=hf_models[0].config.eos_token_id,
-                pad_token_id=hf_models[0].config.pad_token_id,
+                bos_token_id=bos_token_id,
+                eos_token_id=eos_token_id,
+                pad_token_id=pad_token_id,
                 use_cache=True,
                 **model_kwargs
             )
 
             refs = batch[ref_str]
             for h, r in zip(hyps, refs):
                 hyp_list.append(tokenizer.decode(h, skip_special_tokens=True, clean_up_tokenization_spaces=False))
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder/encoder_model.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder/encoder_model.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/encoder_decoder_model.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/huggingface/encoder_decoder/evaluation.py` & `vilmedic-1.3.1/vilmedic/blocks/huggingface/encoder_decoder/evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     tokenizer = dl.dataset.tgt_tokenizer
     max_len = dl.dataset.tgt_tokenizer_max_len
     ref_list = []
     hyp_list = []
 
     with torch.no_grad():
         for batch in tqdm.tqdm(dl):
-            batch = {k: v.cuda() for k, v in batch.items()}
+            batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
             # if len(enc_dec) == 1:
             #     hyps = enc_dec[0].generate(
             #         input_ids=batch["input_ids"],
             #     )
             #
             # else:
             # Expanding inputs
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/losses/mvqa/LabelSmoothingCrossEntropyLoss.py` & `vilmedic-1.3.1/vilmedic/blocks/losses/mvqa/LabelSmoothingCrossEntropyLoss.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/ConVIRTLoss.py` & `vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/ConVIRTLoss.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/GLoRIALoss.py` & `vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/GLoRIALoss.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/InfoNCELoss.py` & `vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/InfoNCELoss.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/losses/selfsup/VICREGLoss.py` & `vilmedic-1.3.1/vilmedic/blocks/losses/selfsup/VICREGLoss.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rl/SCST.py` & `vilmedic-1.3.1/vilmedic/blocks/rl/SCST.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/decoder.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/decoder.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/evaluation.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     refs = []
     pbar = tqdm(dl, total=len(dl))
     for batch in pbar:
         # Get refs
         refs.extend(batch['decoder_input_ids'].tolist())
 
         # Encode source modalities
-        batch = {k: v.cuda() for k, v in batch.items()}
+        batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
         ctx_dicts = [encode(**batch) for encode in encoders]
 
         # Sanity check one of the context dictionaries for dimensions and return batch_size
         batch_size = check_context_ndims(ctx_dicts[0])
 
         # Always use the initial storage
         beam = beam_storage.narrow(1, 0, batch_size).zero_()
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/layers/attention.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/layers/attention.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/layers/ff.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/layers/ff.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/layers/hierarchical_attention.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/layers/hierarchical_attention.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/rnn.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/textencoder.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/textencoder.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/rnn/visualdecoder.py` & `vilmedic-1.3.1/vilmedic/blocks/rnn/visualdecoder.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/schedulers/DecreasingCosineAnnealingWarmRestarts.py` & `vilmedic-1.3.1/vilmedic/blocks/schedulers/DecreasingCosineAnnealingWarmRestarts.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/schedulers/LinearWarmupCosineAnnealingLR.py` & `vilmedic-1.3.1/vilmedic/blocks/schedulers/LinearWarmupCosineAnnealingLR.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/CheXbert/chexbert.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/CheXbert/chexbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from transformers import BertModel, AutoModel, AutoConfig
 from sklearn.metrics import classification_report, accuracy_score
 from sklearn.metrics._classification import _check_targets
 
 import numpy as np
 from sklearn.utils.sparsefuncs import count_nonzero
 
-logging.getLogger("urllib3").setLevel(logging.ERROR)
-
 
 def generate_attention_masks(batch, source_lengths):
     """Generate masks for padded batches to avoid self-attention over pad tokens
     @param batch (Tensor): tensor of token indices of shape (batch_size, max_len)
                            where max_len is length of longest sequence in the batch
     @param source_lengths (List[Int]): List of actual lengths for each of the
                            sequences in the batch
@@ -206,15 +204,15 @@
         differing_labels = count_nonzero(y_true - y_pred, axis=1)
         pe_accuracy = (differing_labels == 0).astype(np.float32)
 
         cr = classification_report(refs_chexbert, hyps_chexbert, target_names=self.target_names, output_dict=True)
         cr_5 = classification_report(refs_chexbert_5, hyps_chexbert_5, target_names=self.target_names_5,
                                      output_dict=True)
 
-        return accuracy, pe_accuracy, cr, cr_5,
+        return accuracy, pe_accuracy, cr, cr_5
 
     def train(self, mode: bool = True):
         mode = False  # force False
         self.training = mode
         for module in self.children():
             module.train(mode)
         return self
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bertscore/bertscore.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bertscore/bertscore.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/bleu.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/bleu/bleu_scorer.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/ciderD.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/ciderD.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD/ciderD_scorer.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD/ciderD_scorer.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL_scorer.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/ciderD_RL/ciderD_RL_scorer.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/mauve_.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/mauve_.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/meteor/meteor.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/rouge/rouge.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/NLG/spice/spice.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/NLG/spice/spice.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityMatchExact/RadEntityMatchExact.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityMatchExact/RadEntityMatchExact.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import torch.nn as nn
 import stanza
 from stanza import Pipeline
 
 import logging
 
-logging.getLogger("stanza").setLevel(logging.WARNING)
 stanza.download('en', processors='tokenize,lemma,pos,ner')
 stanza.download('en', package='radiology')
 
 class RadEntityMatchExact(nn.Module):
     def __init__(self, **kwargs):
         super().__init__()
         self.ner = Pipeline(lang='en', package='radiology', processors={'tokenize': 'default', 'ner': 'radiology'},
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/BERTNLI.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/BERTNLI.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/RadEntityNLI.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/RadEntityNLI.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 from vilmedic.blocks.scorers.RadEntityNLI.nli import SimpleNLI
 from vilmedic.constants import EXTRA_CACHE_DIR
 from vilmedic.zoo.utils import download_model
 
 from torchmetrics.functional.text.bert import BERTScorer
 from itertools import chain, product
 
-import logging
-
-logging.getLogger("stanza").setLevel(logging.WARNING)
-logging.getLogger("filelock").setLevel(logging.CRITICAL)
-
 
 class RadEntityNLI(nn.Module):
     def __init__(self, **kwargs):
         super().__init__()
         # NER types
         self.target_types = {'S-ANATOMY', 'S-OBSERVATION'}
         self.match_exact = RadEntityMatchExact()
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/nli.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/nli.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadEntityNLI/test.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/RadEntityNLI/test.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/RadGraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/cct.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,339 @@
-"""
-The BidirectionalTransformerEncoder from Calypso.
-This is basically the transformer from https://nlp.seas.harvard.edu/2018/04/03/attention.html
-so credit to them.
-
-This code should be considered "private" in that we have several
-transformer implementations and may end up deleting this one.
-If you use it, consider yourself warned.
-"""
-
-from typing import Tuple, Callable
-import math
-import warnings
-
 import torch
+import torch.nn as nn
 import torch.nn.functional as F
 
-from allennlp.common.checks import ExperimentalFeatureWarning
-from allennlp.modules.layer_norm import LayerNorm
-from allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
-from allennlp.common import Registrable
-from allennlp.nn import util
-
-
-def attention(
-    query: torch.Tensor,
-    key: torch.Tensor,
-    value: torch.Tensor,
-    mask: torch.BoolTensor = None,
-    dropout: Callable = None,
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    """Compute 'Scaled Dot Product Attention'"""
-    d_k = query.size(-1)
-    scores = torch.matmul(query, key.transpose(-2, -1)) / math.sqrt(d_k)
-    if mask is not None:
-        scores = scores.masked_fill(~mask, util.min_value_of_dtype(scores.dtype))
-    p_attn = F.softmax(scores, dim=-1)
-    if dropout is not None:
-        p_attn = dropout(p_attn)
-    return torch.matmul(p_attn, value), p_attn
-
-
-def subsequent_mask(size: int, device: str = "cpu") -> torch.BoolTensor:
-    """Mask out subsequent positions."""
-    mask = torch.tril(torch.ones(size, size, device=device, dtype=torch.bool)).unsqueeze(0)
-    return mask
-
+# Pre-defined CCT Models
+__all__ = ['cct_2', 'cct_4', 'cct_6', 'cct_7', 'cct_8', 'cct_14', 'cct_16']
 
-class PositionalEncoding(torch.nn.Module, Registrable):
-    """Implement the Positional Encoding function."""
 
-    def __init__(self, input_dim: int, max_len: int = 5000) -> None:
-        super().__init__()
+def cct_2(*args, **kwargs):
+    return _cct(num_layers=2, num_heads=2, mlp_ratio=1, embedding_dim=128,
+                *args, **kwargs)
 
-        # Compute the positional encodings once in log space.
-        positional_encoding = torch.zeros(max_len, input_dim, requires_grad=False)
-        position = torch.arange(0, max_len).unsqueeze(1).float()
-        div_term = torch.exp(
-            torch.arange(0, input_dim, 2).float() * -(math.log(10000.0) / input_dim)
-        )
-        positional_encoding[:, 0::2] = torch.sin(position * div_term)
-        positional_encoding[:, 1::2] = torch.cos(position * div_term)
-        positional_encoding = positional_encoding.unsqueeze(0)
-        self.register_buffer("positional_encoding", positional_encoding)
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
 
-        return x + self.positional_encoding[:, : x.size(1)]
+def cct_4(*args, **kwargs):
+    return _cct(num_layers=4, num_heads=2, mlp_ratio=1, embedding_dim=128,
+                *args, **kwargs)
 
 
-class PositionwiseFeedForward(torch.nn.Module):
-    """Implements FFN equation."""
+def cct_6(*args, **kwargs):
+    return _cct(num_layers=6, num_heads=4, mlp_ratio=2, embedding_dim=256,
+                *args, **kwargs)
 
-    def __init__(self, input_dim: int, ff_dim: int, dropout: float = 0.1) -> None:
-        super().__init__()
-        self.w_1 = torch.nn.Linear(input_dim, ff_dim)
-        self.w_2 = torch.nn.Linear(ff_dim, input_dim)
-        self.dropout = torch.nn.Dropout(dropout)
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
+def cct_7(*args, **kwargs):
+    return _cct(num_layers=7, num_heads=4, mlp_ratio=2, embedding_dim=256,
+                *args, **kwargs)
 
-        return self.w_2(self.dropout(F.relu(self.w_1(x))))
 
+def cct_8(*args, **kwargs):
+    return _cct(num_layers=8, num_heads=4, mlp_ratio=2, embedding_dim=256,
+                *args, **kwargs)
 
-class TransformerEncoder(torch.nn.Module):
-    """Core encoder is a stack of N layers"""
 
-    def __init__(
-        self, layer: torch.nn.Module, num_layers: int, return_all_layers: bool = False
-    ) -> None:
-        super().__init__()
-        self.layers = util.clone(layer, num_layers)
-        self.norm = LayerNorm(layer.size)
-        self.return_all_layers = return_all_layers
-
-    def forward(self, x, mask):
-        """Pass the input (and mask) through each layer in turn."""
-        all_layers = []
-        for layer in self.layers:
-            x = layer(x, mask)
-            if self.return_all_layers:
-                all_layers.append(x)
-
-        if self.return_all_layers:
-            all_layers[-1] = self.norm(all_layers[-1])
-            return all_layers
-        return self.norm(x)
+def cct_14(*args, **kwargs):
+    return _cct(num_layers=14, num_heads=6, mlp_ratio=3, embedding_dim=384,
+                *args, **kwargs)
 
 
-class SublayerConnection(torch.nn.Module):
-    """
-    A residual connection followed by a layer norm.
-    Note for code simplicity the norm is first as opposed to last.
-    """
+def cct_16(*args, **kwargs):
+    return _cct(num_layers=16, num_heads=6, mlp_ratio=3, embedding_dim=384,
+                *args, **kwargs)
 
-    def __init__(self, size: int, dropout: float) -> None:
-        super().__init__()
-        self.norm = LayerNorm(size)
-        self.dropout = torch.nn.Dropout(dropout)
 
-    def forward(
-        self, x: torch.Tensor, sublayer: Callable[[torch.Tensor], torch.Tensor]
-    ) -> torch.Tensor:
-        """Apply residual connection to any sublayer with the same size."""
-        return x + self.dropout(sublayer(self.norm(x)))
-
-
-class EncoderLayer(torch.nn.Module):
-    """Encoder is made up of self-attn and feed forward (defined below)"""
-
-    def __init__(
-        self, size: int, self_attn: torch.nn.Module, feed_forward: torch.nn.Module, dropout: float
-    ) -> None:
-        super().__init__()
-        self.self_attn = self_attn
-        self.feed_forward = feed_forward
-        self.sublayer = util.clone(SublayerConnection(size, dropout), 2)
-        self.size = size
-
-    def forward(self, x: torch.Tensor, mask: torch.BoolTensor) -> torch.Tensor:
-        """Follow Figure 1 (left) for connections."""
-        x = self.sublayer[0](x, lambda x: self.self_attn(x, x, x, mask))
-        return self.sublayer[1](x, self.feed_forward)
+def _cct(num_layers, num_heads, mlp_ratio, embedding_dim,
+         kernel_size=3, stride=None, padding=None,
+         *args, **kwargs):
+    stride = stride if stride is not None else max(1, (kernel_size // 2) - 1)
+    padding = padding if padding is not None else max(1, (kernel_size // 2))
+    return CCT(num_layers=num_layers,
+               num_heads=num_heads,
+               mlp_ratio=mlp_ratio,
+               embedding_dim=embedding_dim,
+               kernel_size=kernel_size,
+               stride=stride,
+               padding=padding,
+               *args, **kwargs)
 
 
-class MultiHeadedAttention(torch.nn.Module):
-    def __init__(self, num_heads: int, input_dim: int, dropout: float = 0.1) -> None:
+# Modules
+class Attention(nn.Module):
+    def __init__(self, dim, num_heads=8, attention_dropout=0.1, projection_dropout=0.1):
         super().__init__()
-        assert input_dim % num_heads == 0, "input_dim must be a multiple of num_heads"
-        # We assume d_v always equals d_k
-        self.d_k = input_dim // num_heads
         self.num_heads = num_heads
-        # These linear layers are
-        #  [query_projection, key_projection, value_projection, concatenated_heads_projection]
-        self.linears = util.clone(torch.nn.Linear(input_dim, input_dim), 4)
-        self.dropout = torch.nn.Dropout(p=dropout)
-
-    def forward(
-        self,
-        query: torch.Tensor,
-        key: torch.Tensor,
-        value: torch.Tensor,
-        mask: torch.BoolTensor = None,
-    ) -> torch.Tensor:
-        if mask is not None:
-            # Same mask applied to all h heads.
-            # Shape (batch_size, num_heads, timesteps, timesteps)
-            mask = mask.unsqueeze(1).expand([-1, self.num_heads, -1, -1])
-
-        nbatches = query.size(0)
-
-        # 1) Do all the linear projections in batch from d_model => h x d_k
-        query, key, value = [
-            layer(x).view(nbatches, -1, self.num_heads, self.d_k).transpose(1, 2)
-            for layer, x in zip(self.linears, (query, key, value))
-        ]
-
-        # 2) Apply attention on all the projected vectors in batch.
-        x, _ = attention(query, key, value, mask=mask, dropout=self.dropout)
-
-        # 3) "Concat" using a view and apply a final linear.
-        x = x.transpose(1, 2).contiguous().view(nbatches, -1, self.num_heads * self.d_k)
-        return self.linears[-1](x)
-
-
-def make_model(
-    num_layers: int = 6,
-    input_size: int = 512,  # Attention size
-    hidden_size: int = 2048,  # FF layer size
-    heads: int = 8,
-    dropout: float = 0.1,
-    return_all_layers: bool = False,
-) -> TransformerEncoder:
-    """Helper: Construct a model from hyperparameters."""
-    attn = MultiHeadedAttention(heads, input_size, dropout)
-    ff = PositionwiseFeedForward(input_size, hidden_size, dropout)
-    model = TransformerEncoder(
-        EncoderLayer(input_size, attn, ff, dropout), num_layers, return_all_layers=return_all_layers
-    )
-
-    # Initialize parameters with Glorot / fan_avg.
-    for p in model.parameters():
-        if p.dim() > 1:
-            torch.nn.init.xavier_uniform_(p)
-    return model
-
-
-@Seq2SeqEncoder.register("bidirectional_language_model_transformer")
-class BidirectionalLanguageModelTransformer(Seq2SeqEncoder):
-    def __init__(
-        self,
-        input_dim: int,
-        hidden_dim: int,
-        num_layers: int,
-        dropout: float = 0.1,
-        input_dropout: float = None,
-        return_all_layers: bool = False,
-    ) -> None:
-
-        warnings.warn(
-            "This particular transformer implementation is a provisional feature "
-            "that's intended for AI2 internal use and might be deleted at any time. "
-            "If you use it, consider yourself warned!",
-            ExperimentalFeatureWarning,
-        )
+        head_dim = dim // self.num_heads
+        self.scale = head_dim ** -0.5
 
-        super().__init__()
+        self.qkv = nn.Linear(dim, dim * 3, bias=False)
+        self.attn_drop = nn.Dropout(attention_dropout)
+        self.proj = nn.Linear(dim, dim)
+        self.proj_drop = nn.Dropout(projection_dropout)
+
+    def forward(self, x):
+        B, N, C = x.shape
+        qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 1, 4)
+        q, k, v = qkv[0], qkv[1], qkv[2]
+
+        attn = (q @ k.transpose(-2, -1)) * self.scale
+        attn = attn.softmax(dim=-1)
+        attn = self.attn_drop(attn)
+
+        x = (attn @ v).transpose(1, 2).reshape(B, N, C)
+        x = self.proj(x)
+        x = self.proj_drop(x)
+        return x
 
-        self._return_all_layers = return_all_layers
-        self.transformer_layers = num_layers
-        self.num_layers = num_layers
-
-        self._forward_transformer = make_model(
-            input_size=input_dim,
-            hidden_size=hidden_dim,
-            num_layers=num_layers,
-            dropout=dropout,
-            return_all_layers=return_all_layers,
-        )
-        self._backward_transformer = make_model(
-            input_size=input_dim,
-            hidden_size=hidden_dim,
-            num_layers=num_layers,
-            dropout=dropout,
-            return_all_layers=return_all_layers,
-        )
-        self._position = PositionalEncoding(input_dim)
 
-        self.input_dim = input_dim
-        self.output_dim = 2 * input_dim
+class TransformerEncoderLayer(nn.Module):
+    """
+    Inspired by torch.nn.TransformerEncoderLayer and
+    rwightman's timm package.
+    """
+    def __init__(self, d_model, nhead, dim_feedforward=2048, dropout=0.1,
+                 attention_dropout=0.1, drop_path_rate=0.1):
+        super(TransformerEncoderLayer, self).__init__()
+        self.pre_norm = nn.LayerNorm(d_model)
+        self.self_attn = Attention(dim=d_model, num_heads=nhead,
+                                   attention_dropout=attention_dropout, projection_dropout=dropout)
+
+        self.linear1  = nn.Linear(d_model, dim_feedforward)
+        self.dropout1 = nn.Dropout(dropout)
+        self.norm1    = nn.LayerNorm(d_model)
+        self.linear2  = nn.Linear(dim_feedforward, d_model)
+        self.dropout2 = nn.Dropout(dropout)
+
+        self.drop_path = DropPath(drop_path_rate) if drop_path_rate > 0 else nn.Identity()
+
+        self.activation = F.gelu
+
+    def forward(self, src: torch.Tensor, *args, **kwargs) -> torch.Tensor:
+        src = src + self.drop_path(self.self_attn(self.pre_norm(src)))
+        src = self.norm1(src)
+        src2 = self.linear2(self.dropout1(self.activation(self.linear1(src))))
+        src = src + self.drop_path(self.dropout2(src2))
+        return src
 
-        if input_dropout:
-            self._dropout = torch.nn.Dropout(input_dropout)
+
+def drop_path(x, drop_prob: float = 0., training: bool = False):
+    """
+    Obtained from: github.com:rwightman/pytorch-image-models
+    Drop paths (Stochastic Depth) per sample (when applied in main path of residual blocks).
+    This is the same as the DropConnect impl I created for EfficientNet, etc networks, however,
+    the original name is misleading as 'Drop Connect' is a different form of dropout in a separate paper...
+    See discussion: https://github.com/tensorflow/tpu/issues/494#issuecomment-532968956 ... I've opted for
+    changing the layer and argument names to 'drop path' rather than mix DropConnect as a layer name and use
+    'survival rate' as the argument.
+    """
+    if drop_prob == 0. or not training:
+        return x
+    keep_prob = 1 - drop_prob
+    shape = (x.shape[0],) + (1,) * (x.ndim - 1)  # work with diff dim tensors, not just 2D ConvNets
+    random_tensor = keep_prob + torch.rand(shape, dtype=x.dtype, device=x.device)
+    random_tensor.floor_()  # binarize
+    output = x.div(keep_prob) * random_tensor
+    return output
+
+
+class DropPath(nn.Module):
+    """
+    Obtained from: github.com:rwightman/pytorch-image-models
+    Drop paths (Stochastic Depth) per sample  (when applied in main path of residual blocks).
+    """
+    def __init__(self, drop_prob=None):
+        super(DropPath, self).__init__()
+        self.drop_prob = drop_prob
+
+    def forward(self, x):
+        return drop_path(x, self.drop_prob, self.training)
+
+
+class Tokenizer(nn.Module):
+    def __init__(self,
+                 kernel_size, stride, padding,
+                 pooling_kernel_size=3, pooling_stride=2, pooling_padding=1,
+                 n_conv_layers=1,
+                 n_input_channels=3,
+                 n_output_channels=64,
+                 in_planes=64,
+                 activation=None,
+                 max_pool=True,
+                 conv_bias=False):
+        super(Tokenizer, self).__init__()
+
+        n_filter_list = [n_input_channels] + \
+                        [in_planes for _ in range(n_conv_layers - 1)] + \
+                        [n_output_channels]
+
+        self.conv_layers = nn.Sequential(
+            *[nn.Sequential(
+                nn.Conv2d(n_filter_list[i], n_filter_list[i + 1],
+                          kernel_size=(kernel_size, kernel_size),
+                          stride=(stride, stride),
+                          padding=(padding, padding), bias=conv_bias),
+                nn.Identity() if activation is None else activation(),
+                nn.MaxPool2d(kernel_size=pooling_kernel_size,
+                             stride=pooling_stride,
+                             padding=pooling_padding) if max_pool else nn.Identity()
+            )
+                for i in range(n_conv_layers)
+            ])
+
+        self.flattener = nn.Flatten(2, 3)
+        self.apply(self.init_weight)
+
+    def sequence_length(self, n_channels=3, height=224, width=224):
+        return self.forward(torch.zeros((1, n_channels, height, width))).shape[1]
+
+    def forward(self, x):
+        return self.flattener(self.conv_layers(x)).transpose(-2, -1)
+
+    @staticmethod
+    def init_weight(m):
+        if isinstance(m, nn.Conv2d):
+            nn.init.kaiming_normal_(m.weight)
+
+
+class TransformerClassifier(nn.Module):
+    def __init__(self,
+                 seq_pool=True,
+                 embedding_dim=768,
+                 num_layers=12,
+                 num_heads=12,
+                 mlp_ratio=4.0,
+                 num_classes=1000,
+                 dropout_rate=0.1,
+                 attention_dropout=0.1,
+                 stochastic_depth_rate=0.1,
+                 positional_embedding='sine',
+                 sequence_length=None,
+                 *args, **kwargs):
+        super().__init__()
+        positional_embedding = positional_embedding if \
+            positional_embedding in ['sine', 'learnable', 'none'] else 'sine'
+        dim_feedforward = int(embedding_dim * mlp_ratio)
+        self.embedding_dim = embedding_dim
+        self.sequence_length = sequence_length
+        self.seq_pool = seq_pool
+
+        assert sequence_length is not None or positional_embedding == 'none', \
+            f"Positional embedding is set to {positional_embedding} and" \
+            f" the sequence length was not specified."
+
+        if not seq_pool:
+            sequence_length += 1
+            self.class_emb = nn.Parameter(torch.zeros(1, 1, self.embedding_dim),
+                                          requires_grad=True)
         else:
-            self._dropout = lambda x: x
+            self.attention_pool = nn.Linear(self.embedding_dim, 1)
 
-        self.should_log_activations = False
+        if positional_embedding != 'none':
+            if positional_embedding == 'learnable':
+                self.positional_emb = nn.Parameter(torch.zeros(1, sequence_length, embedding_dim),
+                                                   requires_grad=True)
+                nn.init.trunc_normal_(self.positional_emb, std=0.2)
+            else:
+                self.positional_emb = nn.Parameter(self.sinusoidal_embedding(sequence_length, embedding_dim),
+                                                   requires_grad=False)
+        else:
+            self.positional_emb = None
 
-    def get_attention_masks(self, mask: torch.BoolTensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        Returns 2 masks of shape (batch_size, timesteps, timesteps) representing
-        1) non-padded elements, and
-        2) elements of the sequence which are permitted to be involved in attention at a given timestep.
-        """
-        device = mask.device
-        # Forward case:
-        timesteps = mask.size(1)
-        # Shape (1, timesteps, timesteps)
-        subsequent = subsequent_mask(timesteps, device)
-        # Broadcasted logical and - we want zero
-        # elements where either we have padding from the mask,
-        # or we aren't allowed to use the timesteps.
-        # Shape (batch_size, timesteps, timesteps)
-        forward_mask = mask.unsqueeze(-1) & subsequent
-        # Backward case - exactly the same, but transposed.
-        backward_mask = forward_mask.transpose(1, 2)
-
-        return forward_mask, backward_mask
-
-    def forward(self, token_embeddings: torch.Tensor, mask: torch.BoolTensor) -> torch.Tensor:
-        forward_mask, backward_mask = self.get_attention_masks(mask)
-        token_embeddings = self._position(token_embeddings)
-        token_embeddings = self._dropout(token_embeddings)
-        forward_output = self._forward_transformer(token_embeddings, forward_mask)
-        backward_output = self._backward_transformer(token_embeddings, backward_mask)
-
-        if self._return_all_layers:
-            to_return = []
-            for forward, backward in zip(forward_output, backward_output):
-                to_return.append(torch.cat([forward, backward], -1))
-            return to_return
-
-        return torch.cat([forward_output, backward_output], -1)
-
-    def get_regularization_penalty(self):
-        return 0.0
+        self.dropout = nn.Dropout(p=dropout_rate)
+        dpr = [x.item() for x in torch.linspace(0, stochastic_depth_rate, num_layers)]
+        self.blocks = nn.ModuleList([
+            TransformerEncoderLayer(d_model=embedding_dim, nhead=num_heads,
+                                    dim_feedforward=dim_feedforward, dropout=dropout_rate,
+                                    attention_dropout=attention_dropout, drop_path_rate=dpr[i])
+            for i in range(num_layers)])
+        self.norm = nn.LayerNorm(embedding_dim)
+
+        self.fc = nn.Linear(embedding_dim, num_classes)
+        self.apply(self.init_weight)
+
+    def forward(self, x):
+        if self.positional_emb is None and x.size(1) < self.sequence_length:
+            x = F.pad(x, (0, 0, 0, self.n_channels - x.size(1)), mode='constant', value=0)
+
+        if not self.seq_pool:
+            cls_token = self.class_emb.expand(x.shape[0], -1, -1)
+            x = torch.cat((cls_token, x), dim=1)
+
+        if self.positional_emb is not None:
+            x += self.positional_emb
+
+        x = self.dropout(x)
+
+        for blk in self.blocks:
+            x = blk(x)
+        x = self.norm(x)
+
+        if self.seq_pool:
+            x = torch.matmul(F.softmax(self.attention_pool(x), dim=1).transpose(-1, -2), x).squeeze(-2)
+        else:
+            x = x[:, 0]
 
-    def get_input_dim(self) -> int:
-        return self.input_dim
+        x = self.fc(x)
+        return x
 
-    def get_output_dim(self) -> int:
-        return self.output_dim
+    @staticmethod
+    def init_weight(m):
+        if isinstance(m, nn.Linear):
+            nn.init.trunc_normal_(m.weight, std=.02)
+            if isinstance(m, nn.Linear) and m.bias is not None:
+                nn.init.constant_(m.bias, 0)
+        elif isinstance(m, nn.LayerNorm):
+            nn.init.constant_(m.bias, 0)
+            nn.init.constant_(m.weight, 1.0)
+
+    @staticmethod
+    def sinusoidal_embedding(n_channels, dim):
+        pe = torch.FloatTensor([[p / (10000 ** (2 * (i // 2) / dim)) for i in range(dim)]
+                                for p in range(n_channels)])
+        pe[:, 0::2] = torch.sin(pe[:, 0::2])
+        pe[:, 1::2] = torch.cos(pe[:, 1::2])
+        return pe.unsqueeze(0)
+
+
+# CCT Main model
+class CCT(nn.Module):
+    def __init__(self,
+                 img_size=224,
+                 embedding_dim=768,
+                 n_input_channels=3,
+                 n_conv_layers=1,
+                 kernel_size=7,
+                 stride=2,
+                 padding=3,
+                 pooling_kernel_size=3,
+                 pooling_stride=2,
+                 pooling_padding=1,
+                 *args, **kwargs):
+        super(CCT, self).__init__()
+
+        self.tokenizer = Tokenizer(n_input_channels=n_input_channels,
+                                   n_output_channels=embedding_dim,
+                                   kernel_size=kernel_size,
+                                   stride=stride,
+                                   padding=padding,
+                                   pooling_kernel_size=pooling_kernel_size,
+                                   pooling_stride=pooling_stride,
+                                   pooling_padding=pooling_padding,
+                                   max_pool=True,
+                                   activation=nn.ReLU,
+                                   n_conv_layers=n_conv_layers,
+                                   conv_bias=False)
+
+        self.classifier = TransformerClassifier(
+            sequence_length=self.tokenizer.sequence_length(n_channels=n_input_channels,
+                                                           height=img_size,
+                                                           width=img_size),
+            embedding_dim=embedding_dim,
+            seq_pool=True,
+            dropout_rate=0.,
+            attention_dropout=0.1,
+            stochastic_depth=0.1,
+            *args, **kwargs)
+
+    def forward(self, x):
+        x = self.tokenizer(x)
+        return self.classifier(x)
 
-    def is_bidirectional(self) -> bool:
-        return True
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/post_processing.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/post_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 from sklearn.manifold import TSNE
 import matplotlib.pyplot as plt
 import umap
 import omegaconf
 import seaborn as sns
 
 sns.set_theme(style="darkgrid")
-logging.getLogger("numba").setLevel(logging.WARNING)
-logging.getLogger("matplotlib").setLevel(logging.WARNING)
+
 
 
 def plot_attention(results, pp_dir, seed, logger, split, epoch, dl, smooth=True, **kwargs):
     if 'attentions' not in results:
         logger.warn("No attention weights found in results, skipping")
         return
     # Attention are of size num_models x bs x num_layers x num_heads x seq_len x seq_len
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/scorers/scores.py` & `vilmedic-1.3.1/vilmedic/blocks/scorers/scores.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import os
 import numpy as np
 import json
 import torch.nn.functional as F
 import torch
+import logging
+from radgraph import F1RadGraph
+from f1chexbert import F1CheXbert
 from sklearn.metrics import classification_report, roc_auc_score
-from omegaconf import OmegaConf
 from . import *
 
+# RadGraph package overrides logger, need to set back to default
+logging.setLoggerClass(logging.Logger)
+
 REWARD_COMPLIANT = {
     "rougel": [RougeL, 1],
     "rouge2": [Rouge2, 1],
     "rouge1": [Rouge1, 1],
     "bleu": [Bleu, 1],
     "meteor": [Meteor, 1],
     "ciderdrl": [CiderDRL, 1],
     "radentitymatchexact": [RadEntityMatchExact, 1],
     "radentitynli": [RadEntityNLI, 1],
     "chexbert": [CheXbert, 1],
-    "radgraph": [RadGraph, 1],
+    "radgraph": [F1RadGraph, 1],
     "bertscore": [BertScore, 1],
     # "MAUVE": [MauveScorer, 0],
 }
 
 
 def compute_scores(metrics, refs, hyps, split, seed, config, epoch, logger, dump=True):
     scores = dict()
@@ -78,27 +83,31 @@
         elif metric == 'accuracy':
             scores["accuracy"] = round(np.mean(np.array(refs) == np.argmax(hyps, axis=-1)) * 100, 2)
         elif metric == 'f1-score':
             scores["f1-score"] = classification_report(refs, np.argmax(hyps, axis=-1))
         elif metric == 'auroc':
             scores["auroc"] = roc_auc_score(refs, F.softmax(torch.from_numpy(hyps), dim=-1).numpy(), multi_class="ovr")
         elif metric == 'chexbert':
-            accuracy, accuracy_per_sample, chexbert_all, chexbert_5 = CheXbert(
+            accuracy, accuracy_per_sample, chexbert_all, chexbert_5 = F1CheXbert(
                 refs_filename=base.format('refs.chexbert.txt') if dump else None,
                 hyps_filename=base.format('hyps.chexbert.txt') if dump else None) \
                 (hyps, refs)
             scores["chexbert-5_micro avg_f1-score"] = chexbert_5["micro avg"]["f1-score"]
             scores["chexbert-all_micro avg_f1-score"] = chexbert_all["micro avg"]["f1-score"]
+            scores["chexbert-5_macro avg_f1-score"] = chexbert_5["macro avg"]["f1-score"]
+            scores["chexbert-all_macro avg_f1-score"] = chexbert_all["macro avg"]["f1-score"]
         elif metric == 'radentitymatchexact':
             scores["radentitymatchexact"] = RadEntityMatchExact()(refs, hyps)[0]
         elif metric == 'radentitynli':
             scores["radentitynli"] = RadEntityNLI()(refs, hyps)[0]
         elif metric == 'radgraph':
             scores["radgraph_simple"], scores["radgraph_partial"], scores["radgraph_complete"] = \
-                RadGraph(reward_level="full")(refs=refs, hyps=hyps)[0]
+                F1RadGraph(reward_level="all")(refs=refs, hyps=hyps)[0]
+        elif metric == 'stanford_ct_abd_accuracy':
+            scores["stanford_ct_abd"] = StanfordCTAbdAcc()(refs=refs, hyps=hyps)[0]
         else:
             logger.warning("Metric not implemented: {}".format(metric))
 
     if dump:
         with open(metrics_file, 'a+') as f:
             f.write(json.dumps({
                 'split': split,
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/cnn.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/cnn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,70 @@
 import torch
 import torch.nn as nn
+import logging
 from torchvision.models import *
 from torchxrayvision.models import DenseNet as XrvDenseNet, ResNet as XrvResNet
+from monai.networks.nets.densenet import densenet121 as MonaiDensenet121, densenet169 as MonaiDensenet169, \
+    densenet201 as MonaiDensenet201, densenet264 as MonaiDensenet264
+
 from .vgg_hgap import *
-from transformers import DeiTConfig, ViTConfig
-from transformers.models.vit.modeling_vit import ViTModel
-from transformers.models.deit.modeling_deit import DeiTModel
-from transformers.modeling_outputs import BaseModelOutputWithPooling, BaseModelOutputWithPoolingAndNoAttention
-from transformers import ResNetConfig
+from transformers.models.vit.modeling_vit import ViTModel, ViTConfig
+from transformers.models.deit.modeling_deit import DeiTModel, DeiTConfig
+from transformers.modeling_outputs import BaseModelOutputWithPooling, BaseModelOutputWithPoolingAndNoAttention, \
+    BaseModelOutputWithNoAttention
+from transformers import ResNetConfig, PoolFormerConfig
 from transformers.models.resnet.modeling_resnet import ResNetModel as HFResNetModel
+from transformers.models.poolformer.modeling_poolformer import PoolFormerModel as HFPoolFormerModel
+
+
+class _3d_densenet121(MonaiDensenet121):
+    pass
+
+
+class _3d_densenet169(MonaiDensenet169):
+    pass
+
+
+class _3d_densenet201(MonaiDensenet201):
+    pass
+
+
+class _3d_densenet264(MonaiDensenet264):
+    pass
 
 
 def get_network(backbone, output_layer, pretrained, weights=None, **kwargs):
     """
     Create sub-network given a backbone and an output_layer
     """
-    # Create avgpool for densenet, doesnt exist as such
-    if 'densenet' in backbone and output_layer == 'avgpool':
+    # Create avgpool for densenet, does not exist as such
+    if 'densenet' in backbone and '3d' not in backbone and output_layer == 'avgpool':
         sub_network = get_network(backbone, 'features', pretrained, **kwargs)
         sub_network.add_module('relu', nn.ReLU(inplace=True))
         sub_network.add_module('avgpool', nn.AdaptiveAvgPool2d((1, 1)))
         sub_network.add_module('flatten', nn.Flatten(1))
         return sub_network
 
     # HuggingFace Vision transformer
     if "vit" in backbone.lower():
         model = ViTModel(ViTConfig(return_dict=True, **kwargs), add_pooling_layer=False)
         model.layernorm = nn.Identity()
         return model
+
     if "deit" in backbone.lower():
         return DeiTModel(DeiTConfig(return_dict=True, **kwargs), add_pooling_layer=False)
+
     # HuggingFace ResNet
     if "hfresnet" in backbone.lower():
         return HFResNetModel(ResNetConfig(return_dict=True, **kwargs))
 
+    # HuggingFace PoolFormer
+    if "hfpoolformer" in backbone.lower():
+        return HFPoolFormerModel(PoolFormerConfig(return_dict=True, **kwargs))
+
     # Torchxrayvision
     if "xrv" in backbone.lower():
         network = eval(backbone)(weights=weights)
         if hasattr(network, 'model'):  # XrvResNet Fix
             network = network.model
     # PyTorch
     else:
@@ -53,25 +80,33 @@
                 break
         network = nn.Sequential(*sub_network)
 
     return network
 
 
 class CNN(nn.Module):
-    def __init__(self, backbone, permute, dropout_out=0.0, freeze=True, output_layer=None, pretrained=True,
-                 visual_embedding_dim=None, **kwargs):
+    def __init__(self,
+                 backbone,
+                 permute,
+                 dropout_out=0.0,
+                 freeze=False,
+                 output_layer=None,
+                 pretrained=True,
+                 visual_embedding_dim=None,
+                 **kwargs):
         super(CNN, self).__init__()
+
         self.backbone = backbone
         self.output_layer = output_layer
         self.permute = permute
         self.freeze = freeze
         self.pretrained = pretrained
-
         self.cnn = get_network(self.backbone, self.output_layer, self.pretrained, **kwargs)
         self.dropout_out = nn.Dropout(p=dropout_out)
+        self.is3D = "3d" in backbone
 
         assert permute in ["batch_first", "spatial_first", "no_permute"]
 
         if freeze:
             for name, param in self.cnn.named_parameters():
                 param.requires_grad = False
 
@@ -82,14 +117,18 @@
             out = self.dropout_out(out.last_hidden_state)
             return out
 
         if isinstance(self.cnn, HFResNetModel):
             assert isinstance(out, BaseModelOutputWithPoolingAndNoAttention)
             out = out.last_hidden_state
 
+        if isinstance(self.cnn, HFPoolFormerModel):
+            assert isinstance(out, BaseModelOutputWithNoAttention)
+            out = out.last_hidden_state
+
         out = self.dropout_out(out)
         if self.permute == "no_permute":
             out = out
         elif self.permute == "batch_first":
             out = out.view(*out.size()[:2], -1).permute(0, 2, 1)
             if out.shape[1] == 1:  # avgpool case
                 out = out.squeeze(1)
@@ -112,9 +151,9 @@
             '(' + \
             (str(type(self.cnn).__name__) + '(' + str(self.cnn.config) + '), ' if self.backbone.lower() in ['deit',
                                                                                                             'vit'] else '') + \
             'dropout_out=' + str(self.dropout_out.p) + \
             ', freeze=' + str(self.freeze) + \
             (', output_layer=' + str(self.output_layer) if self.output_layer is not None else '') + \
             (', pretrained=' + str(self.pretrained) if self.backbone.lower() not in ['deit', 'vit'] else '') + \
-            ('\n classifier= {}'.format(self.cnn.classifier) if self.output_layer == 'classifier' else '' + ')')
+            ('\n classifier= {}'.format(list(self.cnn.children())[-1]) if self.output_layer == 'classifier' else '' + ')')
         return s
```

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/selfsup/moco.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/selfsup/moco.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vgg_hgap.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vgg_hgap.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/ats_vit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/cait.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/cait.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/cross_vit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/crossformer.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/crossformer.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/cvt.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/cvt.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/deepvit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/deepvit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/dino.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/dino.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/distill.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/distill.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/efficient.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/efficient.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/extractor.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/extractor.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/levit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/levit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/local_vit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/local_vit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/mae.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/mae.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/mobile_vit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/mpp.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/mpp.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/nest.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/nest.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/pit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/pit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/recorder.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/recorder.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/regionvit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/regionvit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/rvt.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/rvt.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/simmim.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/simmim.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/t2t.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/t2t.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/twins_svt.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/vit.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/vit.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/blocks/vision/vit/vit_for_small_dataset.py` & `vilmedic-1.3.1/vilmedic/blocks/vision/vit/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/ImLabel.py` & `vilmedic-1.3.1/vilmedic/datasets/ImLabel.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/ImSeq.py` & `vilmedic-1.3.1/vilmedic/datasets/ImSeq.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/ImSeq2Seq.py` & `vilmedic-1.3.1/vilmedic/datasets/ImSeq2Seq.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/ImSeqLabel.py` & `vilmedic-1.3.1/vilmedic/datasets/ImSeqLabel.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/Seq2Seq.py` & `vilmedic-1.3.1/vilmedic/datasets/Seq2Seq.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/ImageDataset.py` & `vilmedic-1.3.1/vilmedic/datasets/base/ImageDataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import os
 import pydicom
-from pydicom.pixel_data_handlers.util import apply_voi_lut
-
 import numpy as np
 import json
 import PIL
 import skimage
 import logging
-
-from torch.utils.data._utils.collate import default_collate as pytorch_default_collate
 import torchxrayvision as xrv
 from PIL import Image, ImageFile
 from torch.utils.data import Dataset
 from torchvision.transforms import *
 from .utils import load_file
 from .papers.open_image import *
 from .papers.transforms import *
+import nibabel as nib
+from pydicom.pixel_data_handlers.util import apply_voi_lut
+from torch.utils.data._utils.collate import default_collate as pytorch_default_collate
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True  # Are we sure ?
 PIL.Image.MAX_IMAGE_PIXELS = None  # Are we sure ?
-logging.getLogger('PIL').setLevel(logging.WARNING)
 
 
 def vilmedic_collate(batch, multi_image=None):
     # vilmedic_collate only accepts list of tensors (list of images that are transformed)
 
     # Return one image
     if not multi_image or multi_image == 1:
@@ -64,24 +62,24 @@
     if '.npy' in file_path:
         return [[x] for x in np.load(file_path)]
 
     lines = load_file(file_path)
     return [[os.path.join(image_path, image) for image in line.split(',')] for line in lines]
 
 
-def get_transforms(split, resize, crop, custom_transform_train, custom_transform_val, ext, called_by_ensemblor):
-    # If called_by_ensemblor, return custom_transform_val or evaluation transform
+def get_transforms(split, resize, crop, custom_transform_train, custom_transform_validate, ext, called_by_ensemblor):
+    # If called_by_ensemblor, return custom_transform_validate or evaluation transform
     if called_by_ensemblor:
         split = not "train"
 
     if custom_transform_train is not None and split == "train":
         return eval(custom_transform_train)
 
-    if custom_transform_val is not None and not split == "train":
-        return eval(custom_transform_val)
+    if custom_transform_validate is not None and not split == "train":
+        return eval(custom_transform_validate)
 
     if ext in [".npy", ".npz"]:
         return lambda x: x
 
     if ext == '.xrv':
         return transforms.Compose([xrv.datasets.XRayCenterCrop(),
                                    xrv.datasets.XRayResizer(crop),
@@ -112,14 +110,17 @@
         img = xrv.datasets.normalize(img, 255)
         if len(img.shape) > 2:
             img = img[:, :, 0]
         if len(img.shape) < 2:
             print("error, dimension lower than 2 for image")
         return img[None, :, :]
 
+    if ext == '.nib':
+        return nib.load(image).get_fdata().astype('float32')
+
     if ext == '.png':
         return Image.open(image).convert('RGB')
 
     if ext == '.dcm':
         ds = pydicom.dcmread(image)
         if 'WindowWidth' in ds:
             img = apply_voi_lut(ds.pixel_array, ds).astype(float)
@@ -153,15 +154,15 @@
     def __init__(self,
                  root=None,
                  file=None,
                  split=None,
                  image_path=None,
                  load_memory=False,
                  custom_transform_train=None,
-                 custom_transform_val=None,
+                 custom_transform_validate=None,
                  resize=256,
                  crop=224,
                  ext='.jpg',
                  multi_image=None,
                  called_by_ensemblor=None,
                  **kwargs):
 
@@ -181,15 +182,15 @@
         if file is not None:
             self.images = read_images(root, image_path, split, file)
 
         self.transform = get_transforms(split,
                                         self.resize,
                                         self.crop,
                                         custom_transform_train,
-                                        custom_transform_val,
+                                        custom_transform_validate,
                                         self.ext,
                                         called_by_ensemblor)
 
     def __len__(self):
         return len(self.images or [])
 
     def __getitem__(self, index):
@@ -222,15 +223,15 @@
 
     def __repr__(self):
         transform = self.transform
         if hasattr(self.transform, "transforms"):
             transform = self.transform.transforms
 
         return "ImageDataset\n" + \
-               json.dumps({
-                   "split": self.split,
-                   "image_path": self.image_path,
-                   "root": self.root,
-                   "file": self.file,
-                   "transforms": transform,
-                   "ext": self.ext,
-               }, indent=4, sort_keys=False, default=str)
+            json.dumps({
+                "split": self.split,
+                "image_path": self.image_path,
+                "root": self.root,
+                "file": self.file,
+                "transforms": transform,
+                "ext": self.ext,
+            }, indent=4, sort_keys=False, default=str)
```

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/LabelDataset.py` & `vilmedic-1.3.1/vilmedic/datasets/base/LabelDataset.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/TextDataset.py` & `vilmedic-1.3.1/vilmedic/datasets/base/TextDataset.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/papers/IndexDataset.py` & `vilmedic-1.3.1/vilmedic/datasets/base/papers/IndexDataset.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/papers/RCNNDataset.py` & `vilmedic-1.3.1/vilmedic/datasets/base/papers/RCNNDataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import torch
 from torch.utils.data import Dataset
 
 from ..base.ImageDataset import ImageDataset
 import os
 import logging
 
-logging.getLogger('PIL').setLevel(logging.WARNING)
-
 
 class RCNNDataset(Dataset):
     def __init__(self, label, image, bbox, split, ckpt_dir, **kwargs):
         self.split = split
         self.image = ImageDataset(**image, split=split)
 
         self.bbox = open(os.path.join(bbox.root, split + '.' + bbox.file)).readlines()
```

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/papers/open_image.py` & `vilmedic-1.3.1/vilmedic/datasets/base/papers/open_image.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/papers/report_preprocessing.py` & `vilmedic-1.3.1/vilmedic/datasets/base/papers/report_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/papers/transforms/swav.py` & `vilmedic-1.3.1/vilmedic/datasets/base/papers/transforms/swav.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/datasets/base/utils.py` & `vilmedic-1.3.1/vilmedic/datasets/base/utils.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/executors/trainor.py` & `vilmedic-1.3.1/vilmedic/executors/trainor.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                         self.training_scheduler.early_stop_metric,
                         self.training_scheduler.current_best_metric,
                         self.training_scheduler.early_stop,
                         out["custom_print"] if "custom_print" in out else ""
                     )
                     pbar.set_description(log)
 
-                # break
+                break
             # Perform last update if needed
             if (iteration % self.grad_accu != 0) and ('loss' in out):
                 if self.clip_grad_norm is not None:
                     self.scaler.unscale_(self.optimizer)
                     torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=self.config.clip_grad_norm)
                 self.scaler.step(self.optimizer)
                 self.scaler.update()
```

### Comparing `vilmedic-1.3.0/vilmedic/executors/utils.py` & `vilmedic-1.3.1/vilmedic/executors/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     # RandomSampler for train split, during training only
     if split == 'train' and not called_by_validator:
         sampler = BatchSampler(
             RandomSampler(dataset),
             batch_size=config.batch_size,
             drop_last=config.drop_last or False)
-        logger.info('Using' + type(sampler.sampler).__name__)
+        logger.info('Using ' + type(sampler.sampler).__name__)
 
     else:
         sampler = BatchSampler(
             SequentialSampler(dataset),
             batch_size=config.batch_size,
             drop_last=False)
```

### Comparing `vilmedic-1.3.0/vilmedic/executors/validator.py` & `vilmedic-1.3.1/vilmedic/executors/validator.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/__init__.py` & `vilmedic-1.3.1/vilmedic/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 from vilmedic.models.rrs.SumHugMono_SCST import SumHugMono_SCST
 
 from vilmedic.models.selfsup.clip.VAE import VAE
 from vilmedic.models.selfsup.clip.DALLE import DALLE
 from vilmedic.models.selfsup.clip.CLIP import CLIP
 
 from vilmedic.models.rrg.RRG import RRG
+from vilmedic.models.rrg.RRG_FORCE import RRG_FORCE
+from vilmedic.models.rrg.RRG_MULTI import RRG_MULTI
 from vilmedic.models.rrg.RRG_EEG import RRG_EEG
 from vilmedic.models.rrg.RRG_PPO import RRG_PPO
 from vilmedic.models.rrg.RRG_SCST import RRG_SCST
+from vilmedic.models.rrg.RRG_2D_CT import RRG_2D_CT
 
 from vilmedic.models.selfsup.conVIRT import ConVIRT
 from vilmedic.models.selfsup.SimCLR import SimCLR
 from vilmedic.models.selfsup.GLoRIA import GLoRIA
 from vilmedic.models.selfsup.VICREG import VICREG
 from vilmedic.models.selfsup.SwaV import SwaV
 from vilmedic.models.selfsup.PCL import PCL
```

### Comparing `vilmedic-1.3.0/vilmedic/models/mvqa/MVQA.py` & `vilmedic-1.3.1/vilmedic/models/mvqa/MVQA.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn as nn
 from vilmedic.blocks.vision import *
 from vilmedic.blocks.classifier import *
 from vilmedic.blocks.classifier.evaluation import evaluation
-from vilmedic.blocks.losses import LabelSmoothingCrossEntropy
+from vilmedic.blocks.losses import *
 
 from vilmedic.models.utils import get_n_params
 
 from transformers.models.bert.modeling_bert import BertEncoder, BertPooler
 from transformers.models.bert_generation import BertGenerationConfig
 
 
@@ -29,30 +29,31 @@
         self.transformer = BertEncoder(bert_conf)
         self.pooler = BertPooler(bert_conf)
 
         self.classifier = eval(classifier_func)(**classifier)
 
         self.loss_func = eval(loss_func)(**loss).cuda()
 
+        print(self.loss_func)
         # Evaluation
         self.eval_func = evaluation
 
-    def forward(self, images, labels=None, from_training=True, **kwargs):
+    def forward(self, images, labels=None, from_training=True, iteration=None, epoch=None, **kwargs):
         out = self.cnn(images.cuda())
         out = self.adapter(out)
         out = self.transformer(out, output_attentions=True)
 
         attentions = out.attentions  # num_layers, batch_size, num_heads, sequence_length, sequence_length
 
         out = self.pooler(out.last_hidden_state)
         out = self.classifier(out)
 
         loss = torch.tensor(0.)
         if from_training:
             loss = self.loss_func(out, labels.cuda(), **kwargs)
 
-        return {'loss': loss, 'output': out, 'answer': torch.argmax(out, dim=-1), 'attentions': attentions}
+        return {'loss': loss, 'output': out, 'answer': torch.argmax(out, dim=-1)}
 
     def __repr__(self):
         s = super().__repr__() + '\n'
         s += "{}\n".format(get_n_params(self))
         return s
```

### Comparing `vilmedic-1.3.0/vilmedic/models/others/RCNN.py` & `vilmedic-1.3.1/vilmedic/models/others/RCNN.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/others/sim_mcan.py` & `vilmedic-1.3.1/vilmedic/models/others/sim_mcan.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/PPOTrainer.py` & `vilmedic-1.3.1/vilmedic/models/rrg/PPOTrainer.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/RRG.py` & `vilmedic-1.3.1/vilmedic/models/rrg/RRG_FORCE.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import torch
 import torch.nn as nn
 from vilmedic.models.utils import get_n_params
 
 from vilmedic.blocks.vision import *
 from vilmedic.blocks.huggingface.decoder.decoder_model import DecoderModel
-from vilmedic.blocks.huggingface.decoder.evaluation import evaluation
+from vilmedic.blocks.huggingface.decoder.evaluation_force import evaluation
 from einops import rearrange
 
 
-class RRG(nn.Module):
+class RRG_FORCE(nn.Module):
 
-    def __init__(self, decoder, cnn, dl, **kwargs):
+    def __init__(self, decoder, cnn, dl=None, **kwargs):
         super().__init__()
         # Decoder
-        decoder.vocab_size = dl.dataset.seq.tokenizer.vocab_size
+        if dl:
+            decoder.vocab_size = dl.dataset.seq.tokenizer.vocab_size
         self.dec = DecoderModel(decoder)
 
         # Encoder
         visual_embedding_dim = cnn.pop("visual_embedding_dim", None)
         cnn = eval(cnn.pop('proto'))(**cnn)
         if visual_embedding_dim:
             visual_projection = nn.Linear(visual_embedding_dim, self.dec.decoder.config.hidden_size)
```

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/RRG_EEG.py` & `vilmedic-1.3.1/vilmedic/models/rrg/RRG_EEG.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/RRG_PPO.py` & `vilmedic-1.3.1/vilmedic/models/rrg/RRG_PPO.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/RRG_SCST.py` & `vilmedic-1.3.1/vilmedic/models/rrg/RRG_SCST.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrg/core.py` & `vilmedic-1.3.1/vilmedic/models/rrg/core.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/RRS.py` & `vilmedic-1.3.1/vilmedic/models/rrs/RRS.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/RRS_SCST.py` & `vilmedic-1.3.1/vilmedic/models/rrs/RRS_SCST.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/RRS_obsolete.py` & `vilmedic-1.3.1/vilmedic/models/rrs/RRS_obsolete.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/SumHugMono_SCST.py` & `vilmedic-1.3.1/vilmedic/models/rrs/SumHugMono_SCST.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/SumHugMulti.py` & `vilmedic-1.3.1/vilmedic/models/rrs/SumHugMulti.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/SumHugMulti2.py` & `vilmedic-1.3.1/vilmedic/models/rrs/SumHugMulti2.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/rrs/SumRNN.py` & `vilmedic-1.3.1/vilmedic/models/rrs/SumRNN.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/GLoRIA.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/GLoRIA.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     losses = []
     linguistics = []
     visuals = []
 
     pbar = tqdm(dl, total=len(dl))
     for i, batch in enumerate(pbar):
-        batch = {k: v.cuda() for k, v in batch.items()}
+        batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
         out = model(**batch)
         losses.append(out['loss'].mean().cpu().data.numpy())
 
         if not from_training:
             linguistics.append(out['sent_embeddings'].cpu().data)
             visuals.append(out['global_features'].cpu().data)
```

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/PCL.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/PCL.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/PCL2.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/PCL2.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/SimCLR.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/SimCLR.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/SwaV.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/SwaV.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/VICREG.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/VICREG.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     losses = []
     linguistics = []
     visuals = []
 
     pbar = tqdm(dl, total=len(dl))
     for i, batch in enumerate(pbar):
-        batch = {k: v.cuda() for k, v in batch.items()}
+        batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
         out = model(**batch)
         losses.append(out['loss'].mean().cpu().data.numpy())
 
         if not from_training:
             linguistics.append(out['linguistic'].cpu())
             visuals.append(out['visual'].cpu())
```

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/clip/CLIP.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/clip/CLIP.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/clip/DALLE.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/clip/DALLE.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/clip/VAE.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/clip/VAE.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/clip/dalle_forward.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/clip/dalle_forward.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/models/selfsup/conVIRT.py` & `vilmedic-1.3.1/vilmedic/models/selfsup/conVIRT.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     losses = []
     linguistics = []
     visuals = []
 
     pbar = tqdm(dl, total=len(dl))
     for i, batch in enumerate(pbar):
-        batch = {k: v.cuda() for k, v in batch.items()}
+        batch = {k: v.cuda() if isinstance(v, torch.Tensor) else v for k, v in batch.items()}
         out = model(**batch)
         losses.append(out['loss'].mean().cpu().data.numpy())
 
         if not from_training:
             linguistics.append(out['linguistic'].cpu().data)
             visuals.append(out['visual'].cpu().data)
```

### Comparing `vilmedic-1.3.0/vilmedic/models/utils.py` & `vilmedic-1.3.1/vilmedic/models/utils.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/zoo/modeling_auto.py` & `vilmedic-1.3.1/vilmedic/zoo/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic/zoo/utils.py` & `vilmedic-1.3.1/vilmedic/zoo/utils.py`

 * *Files identical despite different names*

### Comparing `vilmedic-1.3.0/vilmedic.egg-info/PKG-INFO` & `vilmedic-1.3.1/vilmedic.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Metadata-Version: 2.1
 Name: vilmedic
-Version: 1.3.0
+Version: 1.3.1
 Summary: ViLMedic is a modular framework for multimodal research at the intersection of vision and language in the medical field.
-Home-page: UNKNOWN
 Author: Jean-Benoit Delbrouck
 License: MIT
 Keywords: medical nlp deep-learning pytorch
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `vilmedic-1.3.0/vilmedic.egg-info/requires.txt` & `vilmedic-1.3.1/vilmedic.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-appdirs==1.4.4
+appdirs
 omegaconf==2.0.6
+urllib3==1.26.14
+protobuf==3.19.6
 torchvision==0.9.1
-protobuf==3.19.3
 rouge_score
 youtokentome==1.0.3
 tokenizers==0.11.6
 scikit_image==0.18.2
 scikit-learn==0.24.2
 pydicom==2.2.0
 transformers==4.23.1
 seaborn==0.11.1
 dalle-pytorch==1.4.2
 torchxrayvision==0.0.32
 stanza==1.3.0
-bert-score==0.3.11
+bert-score
 torch==1.8.1
 pytorch-lightning==1.4.2
 pytorch-metric-learning==0.9.99
 torch-optimizer==0.1.0
 umap-learn
 opencv-python==4.5.4.60
 mauve-text
-numba==0.54.1
+numba
 torchmetrics==0.5.0
-numpy==1.20.3
+numpy==1.21
 gdown==4.6.0
 spacy===3.2.3
-overrides==3.1.0
-boto3==1.21.13
-jsonpickle==2.1.0
-h5py==3.6.0
-tensorboard
-tensorboardX==2.5
+sentencepiece
+radgraph==0.0.5
+f1chexbert==0.0.1
 psutil==5.9.0
 lightning-bolts==0.5.0
 faiss-gpu
 pyedflib
+nibabel
+monai==1.1.0
+typing_extensions==4.4.0
```

