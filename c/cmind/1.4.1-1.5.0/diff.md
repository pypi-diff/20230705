# Comparing `tmp/cmind-1.4.1.tar.gz` & `tmp/cmind-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.4.1.tar", last modified: Fri Jun  9 07:26:32 2023, max compression
+gzip compressed data, was "cmind-1.5.0.tar", last modified: Wed Jul  5 19:29:19 2023, max compression
```

## Comparing `cmind-1.4.1.tar` & `cmind-1.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.891193 cmind-1.4.1/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6090 2023-06-09 07:26:32.891193 cmind-1.4.1/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5127 2023-05-30 19:25:20.000000 cmind-1.4.1/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.851194 cmind-1.4.1/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-06-09 07:26:00.000000 cmind-1.4.1/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46874 2023-06-06 10:14:36.000000 cmind-1.4.1/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5324 2023-06-09 07:26:00.000000 cmind-1.4.1/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-06-06 10:14:36.000000 cmind-1.4.1/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.4.1/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.861194 cmind-1.4.1/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.841194 cmind-1.4.1/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.871194 cmind-1.4.1/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.871194 cmind-1.4.1/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.881193 cmind-1.4.1/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.881193 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.891193 cmind-1.4.1/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31060 2023-05-30 19:25:20.000000 cmind-1.4.1/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.4.1/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-06-09 07:26:32.861194 cmind-1.4.1/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6090 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      118 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.4.1/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-06-09 07:26:32.000000 cmind-1.4.1/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-06-09 07:26:32.891193 cmind-1.4.1/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2808 2023-06-09 07:26:00.000000 cmind-1.4.1/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6415 2023-07-05 19:29:19.373726 cmind-1.5.0/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5428 2023-07-05 19:28:57.000000 cmind-1.5.0/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2023-06-19 07:06:03.000000 cmind-1.5.0/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46812 2023-06-19 07:06:30.000000 cmind-1.5.0/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5324 2023-06-09 07:26:00.000000 cmind-1.5.0/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-06-06 10:14:36.000000 cmind-1.5.0/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9500 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31292 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6415 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      118 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.5.0/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-07-05 19:29:19.373726 cmind-1.5.0/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2808 2023-06-09 07:26:00.000000 cmind-1.5.0/setup.py
```

### Comparing `cmind-1.4.1/PKG-INFO` & `cmind-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.4.1
+Version: 1.5.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -12,14 +12,17 @@
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
         [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
         
         ### About
         
+        *Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
+        and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+        
         [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
         is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
         It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
         when reproducing experiments from more than 150 research papers and validating them in the real world - 
         there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
         on any platform with any software, hardware, and data.
         
@@ -32,15 +35,15 @@
         Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
         unified README files and synthesize unified containers with a common API.
         It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
         while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
         
         CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
         to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+        connect academia and industry to [organize benchmarking, reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
         and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
         (cost, performance, power consumption, accuracy, etc).
         
         See a few real-world examples of using the CM scripting language:
         - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
         - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
         - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.4.1/README.md` & `cmind-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 
 [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
 [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
 
 ### About
 
+*Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
+and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+
 [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
 is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
 It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
 when reproducing experiments from more than 150 research papers and validating them in the real world - 
 there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
 on any platform with any software, hardware, and data.
 
@@ -24,15 +27,15 @@
 Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
 unified README files and synthesize unified containers with a common API.
 It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
 while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
 
 CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
 to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+connect academia and industry to [organize benchmarking, reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
 and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
 (cost, performance, power consumption, accuracy, etc).
 
 See a few real-world examples of using the CM scripting language:
 - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
 - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
 - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.4.1/cmind/artifact.py` & `cmind-1.5.0/cmind/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,20 @@
         if replace:
             # Check that do not delete important info
             save_info = {}
 
             for k in ['uid', 'alias', 'automation_uid', 'automation_alias']:
                 if k not in meta and k in current_meta:
                     save_info[k]=current_meta[k]
-            
+
             self.original_meta = meta
 
             if len(save_info)>0:
                 self.original_meta.update(save_info)
-        
+
         elif len(meta)>0:
             r = utils.merge_dicts({'dict1':current_meta, 'dict2':meta, 'append_lists':append_lists})
             if r['return'] >0: return 
 
             self.original_meta = r['dict1']
 
         if len(tags)>0:
```

### Comparing `cmind-1.4.1/cmind/automation.py` & `cmind-1.5.0/cmind/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,19 +256,17 @@
                         lst.append(artifact_object)
 
                         # Output to console if forced
                         if console:
                             print (artifact_object.path)
 
                     return {'return':0, 'list':lst}
-        
-        
-        
 
-        
+
+
         # Iterate over pruned repositories
         for repo in pruned_repos:
             path_repo = repo.path_with_prefix
 
             repo_meta = copy.deepcopy(repo.meta)
 
             # May or may not be automation
@@ -289,15 +287,15 @@
                     # Check if artifact is first to get meta about automation UID/alias
                     first_artifact = True
 
                     for artifact in artifacts:
                         path_artifact = os.path.join(path_artifacts, artifact)
 
                         if os.path.isdir(path_artifact):
-                            
+
                             # Check if has CM meta to make sure that it's a CM object
                             path_artifact_meta = os.path.join(path_artifact, self.cmind.cfg['file_cmeta'])
 
                             r = utils.is_file_json_or_yaml(file_name = path_artifact_meta)
                             if r['return']>0: return r
 
                             if r['is_file']:
```

### Comparing `cmind-1.4.1/cmind/cli.py` & `cmind-1.5.0/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/config.py` & `cmind-1.5.0/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/core.py` & `cmind-1.5.0/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/index.py` & `cmind-1.5.0/cmind/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         # Check if home directory exists. Create it otherwise.
         if not os.path.isdir(self.path):
             os.makedirs(self.path)
 
         import json
 
         s = json.dumps(self.meta, indent=2)
-        
+
         r = utils.save_txt(self.full_path_to_index, s)
 
         return r
 
     ############################################################
     def add(self, meta, path, repo, update = False, delete = False):
         """
@@ -115,24 +115,24 @@
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
 
         """
 
         index_meta = self.meta
-        
+
         for y in [meta.get('automation_uid',''), meta.get('automation_alias','')]:
             if y!='' and y not in index_meta: 
                 index_meta[y]={}
 
             uid = True
 
             meta_uid = meta.get('uid','')
             meta_alias = meta.get('alias','')
-            
+
             for z in [meta_uid, meta_alias]:
                 if z!='':
                     if delete:
                         if z in index_meta[y]:
                             for k in [index_meta[y][z].get('alias',''),
                                       index_meta[y][z].get('uid','')]:
                                 if k!='' and k in index_meta[y]:
@@ -184,15 +184,15 @@
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
 
         """
 
         index_meta = self.meta
-        
+
         ret = {'return':0, 'list':[]}
 
         # Check automation from UID to alias with wild cards
         automations = []
         if automation_name[1]!='' and automation_name[1] in index_meta:
             automations.append(automation_name[1])
         else:
@@ -202,41 +202,41 @@
                    if not utils.is_cm_uid(automation) and fnmatch.fnmatch(automation, automation_name[0]):
                        automations.append(automation)
            elif automation_name[0]!='' and automation_name[0] in index_meta:
                automations.append(automation_name[0])
 
         if len(automations)==0:
             return ret
-        
+
         # Check artifacts
         artifacts = []
 
         for automation in automations:
             index_meta_automation = index_meta[automation]
 
             keys_to_delete = []
 
+            check_unique_ids = []
+            
             # First check UID
             if artifact_obj[1]!='':
                 if artifact_obj[1] in index_meta_automation:
-                    self._add_if_exists(index_meta_automation, artifact_obj[1], artifacts, keys_to_delete)
+                    self._add_if_exists(index_meta_automation, artifact_obj[1], artifacts, keys_to_delete, check_unique_ids)
             else:
                if ('*' in artifact_obj[0] or '?' in artifact_obj[0]):
                    import fnmatch
                    for artifact in index_meta_automation:
                        if fnmatch.fnmatch(artifact, artifact_obj[0]):
-                           if index_meta_automation[artifact].get('uid','')!='':
-                               self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete)
+                           self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete, check_unique_ids)
                elif artifact_obj[0]=='':
                    for artifact in index_meta_automation:
                        # Add only 1 (UID) to avoid adding 2 duplicates
-                       if index_meta_automation[artifact].get('uid','')!='':
-                           self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete)
+                       self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete, check_unique_ids)
                elif artifact_obj[0] in index_meta_automation:
-                   self._add_if_exists(index_meta_automation, artifact_obj[0], artifacts, keys_to_delete)
+                   self._add_if_exists(index_meta_automation, artifact_obj[0], artifacts, keys_to_delete, check_unique_ids)
 
             if len(keys_to_delete)>0:
                 for key in keys_to_delete:
                     if key in index_meta_automation:
                         del(index_meta_automation[key])
 
                 self.updated = True
@@ -274,17 +274,30 @@
 
             lst.append(artifact)
 
         return {'return':0, 'list':lst}
 
     ############################################################
     # Internal support function
-    def _add_if_exists(self, meta, key, artifacts, keys_to_delete):
+    def _add_if_exists(self, meta, key, artifacts, keys_to_delete, check_unique_ids):
+
+        # Check that UID was not already added
+        uid = meta[key].get('uid','')
+        if uid =='':
+            uid = key
+
+        if uid in check_unique_ids:
+            return
+
+        check_unique_ids.append(uid)
+
+        # Continue processing
+
         x = meta[key]
-        
+
         if os.path.isdir(x['path']):
             artifacts.append(x)
         else:
             keys_to_delete.append(key)
             # Add related key to delete (UID or alias)
             if x.get('uid','')!='': keys_to_delete.append(x['uid'])
             if x.get('alias','')!='': keys_to_delete.append(x['alias'])
```

### Comparing `cmind-1.4.1/cmind/net.py` & `cmind-1.5.0/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/automation/README.md` & `cmind-1.5.0/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/automation/module.py` & `cmind-1.5.0/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.5.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/automation/module_misc.py` & `cmind-1.5.0/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/ck/README.md` & `cmind-1.5.0/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/ck/module.py` & `cmind-1.5.0/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/core/README.md` & `cmind-1.5.0/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/core/module.py` & `cmind-1.5.0/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/repo/README.md` & `cmind-1.5.0/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repo/automation/repo/module.py` & `cmind-1.5.0/cmind/repo/automation/repo/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
             (CM input dict):
 
             (out) (str): if 'con', output to console
 
             (artifact) (str): repository name (alias)
             (uid) (str): force CM UID for this repository
             (path) (str): specify a path where to create this repository
+            (here) (str): use current path
             (desc) (str): brief repository description (1 line)
             (prefix) (str): extra directory to keep CM artifacts
 
         Returns: 
             (CM return dict):
 
             * return (int): return code == 0 if no error and >0 if error
@@ -298,15 +299,15 @@
         alias = i.get('artifact', '')
         uid = i.get('uid','')
         path = i.get('path', '')
         desc = i.get('desc','')
         prefix = i.get('prefix','')
 
         # If path is not specified, initialize in the current directory!
-        if (path=='' and alias=='') or (alias!='' and path=='.'):
+        if (path=='' and alias=='') or (alias!='' and (path=='.' or i.get('here', False))):
            path = os.path.abspath(os.getcwd())
 
         # Check if there is a repo in a path
         r = self.cmind.access({'action':'detect',
                                'automation':self.meta['alias']+','+self.meta['uid'],
                                'path':path})
         if r['return']>0: return r
@@ -892,32 +893,39 @@
             print ('Reindexing all CM artifacts. Can take some time ...')
         
         out = 'con' if verbose else ''
         
         # Clean index
         self.cmind.index.meta = {}
         
+        import time
+        t1 = time.time()
+
         r = self.cmind.access({'action':'search',
                                'automation':'*',
                                'out':out,
                                'skip_index_search':True,
                                'force_index_add':True})
         if r['return']>0: return r
 
-        # Save
+        t2 = time.time() - t1
+
+        if console:
+            print ('Took {:.1f} sec.'.format(t2))
 
+        # Save
         rx = self.cmind.index.save()
-        # Ignore output for now to continue working even if issues ...
 
+        # Ignore output for now to continue working even if issues ...
         if self.cmind.use_index:
             rx = self.cmind.index.load()
             # Ignore output for now to continue working even if issues ...
 
 
-        return {'return':0}
+        return {'return':0, 'self_time':t2}
 
 
 
 ##############################################################################
 def convert_ck_dir_to_cm(rpath):
     """
     Convert CK directory to the CM format (internal function).
```

### Comparing `cmind-1.4.1/cmind/repo.py` & `cmind-1.5.0/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/repos.py` & `cmind-1.5.0/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind/utils.py` & `cmind-1.5.0/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/cmind.egg-info/PKG-INFO` & `cmind-1.5.0/cmind.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.4.1
+Version: 1.5.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -12,14 +12,17 @@
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
         [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
         
         ### About
         
+        *Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
+        and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+        
         [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
         is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
         It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
         when reproducing experiments from more than 150 research papers and validating them in the real world - 
         there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
         on any platform with any software, hardware, and data.
         
@@ -32,15 +35,15 @@
         Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
         unified README files and synthesize unified containers with a common API.
         It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
         while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
         
         CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
         to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+        connect academia and industry to [organize benchmarking, reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
         and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
         (cost, performance, power consumption, accuracy, etc).
         
         See a few real-world examples of using the CM scripting language:
         - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
         - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
         - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.4.1/cmind.egg-info/SOURCES.txt` & `cmind-1.5.0/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.4.1/setup.py` & `cmind-1.5.0/setup.py`

 * *Files identical despite different names*

