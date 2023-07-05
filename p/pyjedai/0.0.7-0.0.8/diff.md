# Comparing `tmp/pyjedai-0.0.7.tar.gz` & `tmp/pyjedai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.0.7.tar", last modified: Fri Jun 30 14:16:07 2023, max compression
+gzip compressed data, was "pyjedai-0.0.8.tar", last modified: Wed Jul  5 18:56:49 2023, max compression
```

## Comparing `pyjedai-0.0.7.tar` & `pyjedai-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-06-30 14:15:51.000000 pyjedai-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-06-30 14:16:07.510203 pyjedai-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-30 14:15:51.000000 pyjedai-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 14:15:51.000000 pyjedai-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:16:07.510203 pyjedai-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.506203 pyjedai-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/src/pyjedai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18191 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/block_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    52141 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/joins.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28190 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    50691 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/prioritization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23817 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/vector_based_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/src/pyjedai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_block_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_joins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-07-05 18:56:34.000000 pyjedai-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-05 18:56:49.533818 pyjedai-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-05 18:56:34.000000 pyjedai-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-05 18:56:34.000000 pyjedai-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:56:49.533818 pyjedai-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.529818 pyjedai-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/src/pyjedai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18191 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52141 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/joins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25997 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50691 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23995 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23817 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/vector_based_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-07-05 18:56:34.000000 pyjedai-0.0.8/src/pyjedai/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/src/pyjedai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 18:56:49.000000 pyjedai-0.0.8/src/pyjedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:49.533818 pyjedai-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:56:35.000000 pyjedai-0.0.8/tests/test_joins.py
```

### Comparing `pyjedai-0.0.7/LICENSE` & `pyjedai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/PKG-INFO` & `pyjedai-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.7
+Version: 0.0.8
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
-Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
+Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>, Jakub Maciejewski <jacobb.maciejewski@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, http://pyjedai.rtfd.io
 Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: iOS
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
-<br>
-<img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <br>
+    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
-<br><br>
+<br>
+<br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-<!--[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
- <a href='https://pyjedai.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/pyjedai/badge/?version=latest' alt='Documentation Status' />
-</a>
- -->
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -61,79 +54,67 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-<a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
-</a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-<a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
-</a>
+    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
+    </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
+    </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
-<a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
-<img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
-</a>
+    <a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
+        <img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
+    </a>
 </div>
 
-
-
-<details>
-<summary><h4>Details on the Architecture</h4></summary>
-<br>
-The purpose of this framework is to demonstrate how ER can be accomplished by expert and novice users in an intuitive, yet efficient and effective way. pyJedai addresses the following task: Given a source and a target dataset, S and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s ∈ S ∧ t ∈ T}. Its architecture appears in the bellow figure. The first module is the data reader, which specifies the user input. pyJedAI supports both semi-structured and structured data as input. The former, which include SPARQL endpoints and RDF/OWL dumps, are read by <a href="https://rdflib.dev">RDFLib</a>. The latter, which include relational databases as well as CSV and JSON files, are read by <a href="https://pandas.pydata.org">pandas</a>. In this way, pyJedAI is able to interlink any combination of semi-structured and structured data sources, which is a unique feature. <img align="right" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/demo-architecture.png?raw=true?raw=true" alt="pyJedAI-Architecture" width="500"/> The second step in pyJedAI’s pipeline performs block building, a coarsegrained process that clusters together similar entities. The end result consists of a set of candidate pairs, which are examined analytically by the subsequent steps. pyJedAI implements the same established methods for similarity joins and blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes beyond all Link Discovery tools by incorporating recent, state-of-the-art libraries for nearest neighbor search like <a href="https://falconn-lib.org">FALCONN</a> and <a href="https://github.com/facebookresearch/faiss">FAISS</a>. <br>
-
-<br>
-
- The entity matching step estimates the actual similarity between the candidate pairs. Unlike all other Link Discovery tools, which rely exclusively on string similarity measures like edit distance and Jaccard coefficient, pyJedAI leverages the latest advanced NLP techniques, like pre-trained embeddings (e.g., word2vect, fastText and Glove) and transformer language models (i.e., BERT and its variants). More specifically, pyJedAI supports packages like <a href="https://github.com/luozhouyang/python-string-similarity">strsimpy</a>, <a href="https://radimrehurek.com/gensim/">Gensim</a>and <a href="https://huggingface.co">Hugging Face</a>. This unique feature boosts pyJedAI’s accuracy to a significant extent, without requiring any labelled instances from the user. The last step performs entity clustering to further increase the accuracy. The relevant techniques consider the global information provided by the similarity scores of all candidate pairs in order to take local decisions for each pair of entity descriptions. pyJedAI implements and offers the same established algorithms as JedAI, using <a href="https://networkx.org">NetworkX</a> to ensure high time efficiency. Finally, users are able to evaluate, visualize and store the results of the selected pipeline through the intuitive interface of Jupyter notebooks. In this way, pyJedAI facilitates its use by researchers and practitioners that are familiar with the data science ecosystem, regardless of their familiarity with ER and Link
-Discovery, in general.
-
-</details>
-
 # Install
 
+### PyPI
 Install the latest version of pyjedai __[requires python >= 3.8]__:
 ```
 pip install pyjedai
 ```
+More on [PyPI](https://pypi.org/project/pyjedai).
 
-More on [PyPI](pypi.org/project/pyjedai/).
+### Git
 
+Set up locally:
+```
+git clone https://github.com/AI-team-UoA/pyJedAI.git
+```
+go to the root directory with `cd pyJedAI` and type:
+```
+pip install .
+```
 
-### Tutorials
 
-| Tutorial | Notebook |
-|---|:-:|
-| Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) |
-| Dirty Entity Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/DirtyER.ipynb)|
-| Fine-Tuning using Optuna. | [Optuna.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) |
-| User-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) |
-| Raw data to pandas DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Readers.ipynb) |
 
 # Dependencies
 
 <div align="center">
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
-<img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
-<img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
-<img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
-<img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
+    <img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
+    <img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
+    <img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
+    <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
 
 __Status__ 
 
@@ -143,15 +124,19 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
 
 # Java - Wed Application 
 
-For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows.
+<img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
+
+For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
+
+<br>
 
 # Team & Authors
 
 <img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
@@ -163,20 +148,21 @@
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
- <hr>
-  <br>
- <a href="https://stelar-project.eu">
-  <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
- </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- <a href="https://ec.europa.eu/info/index_en">
-  <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
- </a>
- <br><br>
- <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.</b><br>
+    <hr>
+    <br>
+    <a href="https://stelar-project.eu">
+        <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
+    </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://ec.europa.eu/info/index_en">
+        <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
+    </a>
+    <br>
+    <br>
+        <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.
+        </b>
+    <br>
 </div>
-
-
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.7 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.8 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
-gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, http://
-pyjedai.rtfd.io Project-URL: Documentation, http://pyjedai.rtfd.io Project-URL:
-Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues Project-URL: Source
-code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai Keywords:
-deduplication,entity-resolution,link-discovery Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
-Implementation Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Developers Classifier: Natural Language :: English Classifier: Operating
-System :: Microsoft :: Windows Classifier: Operating System :: Unix Classifier:
-Operating System :: iOS Classifier: Topic :: Database Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
+gmail.com>, Jakub Maciejewski
+maciejewski@gmail.com> License: Apache Software License 2.0 Project-URL:
+Homepage, http://pyjedai.rtfd.io Project-URL: Documentation, http://
+pyjedai.rtfd.io Project-URL: Bug Tracker, https://github.com/AI-team-UoA/
+pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
+pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
+discovery Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: Implementation
+Classifier: Intended Audience :: Information Technology Classifier: Intended
+Audience :: Science/Research Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: Unix Classifier: Operating
+System :: iOS Classifier: Topic :: Database Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
----  # Overview pyJedAI is a python framework, aiming to offer experts and
+--- # Overview pyJedAI is a python framework, aiming to offer experts and
 novice users, robust and fast solutions for multiple types of Entity Resolution
 problems. It is builded using state-of-the-art python frameworks. pyJedAI
 constitutes the sole open-source Link Discovery tool that is capable of
 exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
 are publicly available through the Python data science ecosystem. This applies
 to both blocking and matching, thus ensuring high time efficiency, high
 scalability as well as high effectiveness, without requiring any labelled
@@ -41,64 +42,19 @@
 machine learning packages. - Offers supervised and un-supervised ML techniques.
 __Open demos are available in:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 __Google Colab Hands-on demo:__
        [https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/
          Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png]
-*** Details on the Architecture ***
-
-The purpose of this framework is to demonstrate how ER can be accomplished by
-expert and novice users in an intuitive, yet efficient and effective way.
-pyJedai addresses the following task: Given a source and a target dataset, S
-and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s â S
-â§ t â T}. Its architecture appears in the bellow figure. The first module
-is the data reader, which specifies the user input. pyJedAI supports both semi-
-structured and structured data as input. The former, which include SPARQL
-endpoints and RDF/OWL dumps, are read by RDFLib. The latter, which include
-relational databases as well as CSV and JSON files, are read by pandas. In this
-way, pyJedAI is able to interlink any combination of semi-structured and
-structured data sources, which is a unique feature. [pyJedAI-Architecture] The
-second step in pyJedAIâs pipeline performs block building, a coarsegrained
-process that clusters together similar entities. The end result consists of a
-set of candidate pairs, which are examined analytically by the subsequent
-steps. pyJedAI implements the same established methods for similarity joins and
-blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes
-beyond all Link Discovery tools by incorporating recent, state-of-the-art
-libraries for nearest neighbor search like FALCONN and FAISS.
-
-The entity matching step estimates the actual similarity between the candidate
-pairs. Unlike all other Link Discovery tools, which rely exclusively on string
-similarity measures like edit distance and Jaccard coefficient, pyJedAI
-leverages the latest advanced NLP techniques, like pre-trained embeddings
-(e.g., word2vect, fastText and Glove) and transformer language models (i.e.,
-BERT and its variants). More specifically, pyJedAI supports packages like
-strsimpy, Gensimand Hugging_Face. This unique feature boosts pyJedAIâs
-accuracy to a significant extent, without requiring any labelled instances from
-the user. The last step performs entity clustering to further increase the
-accuracy. The relevant techniques consider the global information provided by
-the similarity scores of all candidate pairs in order to take local decisions
-for each pair of entity descriptions. pyJedAI implements and offers the same
-established algorithms as JedAI, using NetworkX to ensure high time efficiency.
-Finally, users are able to evaluate, visualize and store the results of the
-selected pipeline through the intuitive interface of Jupyter notebooks. In this
-way, pyJedAI facilitates its use by researchers and practitioners that are
-familiar with the data science ecosystem, regardless of their familiarity with
-ER and Link Discovery, in general.  # Install Install the latest version of
-pyjedai __[requires python >= 3.8]__: ``` pip install pyjedai ``` More on
-[PyPI](pypi.org/project/pyjedai/). ### Tutorials | Tutorial | Notebook | |---|:
--:| | Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) | | Dirty Entity
-Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/DirtyER.ipynb)| | Fine-Tuning using Optuna. | [Optuna.ipynb](https://
-github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) | | User-
-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) | | Raw data to pandas
-DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/Readers.ipynb) | # Dependencies
+# Install ### PyPI Install the latest version of pyjedai __[requires python >=
+3.8]__: ``` pip install pyjedai ``` More on [PyPI](https://pypi.org/project/
+pyjedai). ### Git Set up locally: ``` git clone https://github.com/AI-team-UoA/
+pyJedAI.git ``` go to the root directory with `cd pyJedAI` and type: ``` pip
+install . ``` # Dependencies
   [https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/
 2560px-Pandas_logo.svg.png]    [https://upload.wikimedia.org/wikipedia/commons/
   thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png]    [https://
  logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png]     [https://
    upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-
                             Jupyter_logo.svg.png]
   [https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-
@@ -119,25 +75,31 @@
 badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
 workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
 pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
 ?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
 github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
 questions and discussions and our recommended starting point. Please report any
 bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application For Java users checkout the initial [JedAI](https://
-github.com/scify/JedAIToolkit). There you can find Java based code and a Web
-Application for interactive creation of ER workflows. # Team & Authors
-[pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-k.github.io) - Jakub
-Maciejewski - [George Papadakis](https://gpapadis.wordpress.com) - [Manolis
-Koubarakis](https://cgi.di.uoa.gr/~koubarak/) Research and development is made
-under the supervision of Pr. Manolis Koubarakis. This is a research project by
-the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and
-Telecommunications at the University of Athens. # License Released under the
-Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/
-blob/main/LICENSE). Copyright Â© 2023 AI-Team, University of Athens
+Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
+(https://github.com/scify/JedAIToolkit). There you can find Java based code and
+a Web Application for interactive creation of ER workflows.
+
+JedAI constitutes an open source, high scalability toolkit that offers out-of-
+the-box solutions for any data integration task, e.g., Record Linkage, Entity
+Resolution and Link Discovery. At its core lies a set of domain-independent,
+state-of-the-art techniques that apply to both RDF and relational data.
+# Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
 
 This project is being funded in the context of STELAR that is an HORIZON-Europe
```

### Comparing `pyjedai-0.0.7/README.md` & `pyjedai-0.0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 <div align="center">
-<br>
-<img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <br>
+    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
-<br><br>
+<br>
+<br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-<!--[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
- <a href='https://pyjedai.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/pyjedai/badge/?version=latest' alt='Documentation Status' />
-</a>
- -->
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -27,79 +21,67 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-<a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
-</a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-<a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
-</a>
+    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
+    </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
+    </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
-<a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
-<img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
-</a>
+    <a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
+        <img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
+    </a>
 </div>
 
-
-
-<details>
-<summary><h4>Details on the Architecture</h4></summary>
-<br>
-The purpose of this framework is to demonstrate how ER can be accomplished by expert and novice users in an intuitive, yet efficient and effective way. pyJedai addresses the following task: Given a source and a target dataset, S and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s ∈ S ∧ t ∈ T}. Its architecture appears in the bellow figure. The first module is the data reader, which specifies the user input. pyJedAI supports both semi-structured and structured data as input. The former, which include SPARQL endpoints and RDF/OWL dumps, are read by <a href="https://rdflib.dev">RDFLib</a>. The latter, which include relational databases as well as CSV and JSON files, are read by <a href="https://pandas.pydata.org">pandas</a>. In this way, pyJedAI is able to interlink any combination of semi-structured and structured data sources, which is a unique feature. <img align="right" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/demo-architecture.png?raw=true?raw=true" alt="pyJedAI-Architecture" width="500"/> The second step in pyJedAI’s pipeline performs block building, a coarsegrained process that clusters together similar entities. The end result consists of a set of candidate pairs, which are examined analytically by the subsequent steps. pyJedAI implements the same established methods for similarity joins and blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes beyond all Link Discovery tools by incorporating recent, state-of-the-art libraries for nearest neighbor search like <a href="https://falconn-lib.org">FALCONN</a> and <a href="https://github.com/facebookresearch/faiss">FAISS</a>. <br>
-
-<br>
-
- The entity matching step estimates the actual similarity between the candidate pairs. Unlike all other Link Discovery tools, which rely exclusively on string similarity measures like edit distance and Jaccard coefficient, pyJedAI leverages the latest advanced NLP techniques, like pre-trained embeddings (e.g., word2vect, fastText and Glove) and transformer language models (i.e., BERT and its variants). More specifically, pyJedAI supports packages like <a href="https://github.com/luozhouyang/python-string-similarity">strsimpy</a>, <a href="https://radimrehurek.com/gensim/">Gensim</a>and <a href="https://huggingface.co">Hugging Face</a>. This unique feature boosts pyJedAI’s accuracy to a significant extent, without requiring any labelled instances from the user. The last step performs entity clustering to further increase the accuracy. The relevant techniques consider the global information provided by the similarity scores of all candidate pairs in order to take local decisions for each pair of entity descriptions. pyJedAI implements and offers the same established algorithms as JedAI, using <a href="https://networkx.org">NetworkX</a> to ensure high time efficiency. Finally, users are able to evaluate, visualize and store the results of the selected pipeline through the intuitive interface of Jupyter notebooks. In this way, pyJedAI facilitates its use by researchers and practitioners that are familiar with the data science ecosystem, regardless of their familiarity with ER and Link
-Discovery, in general.
-
-</details>
-
 # Install
 
+### PyPI
 Install the latest version of pyjedai __[requires python >= 3.8]__:
 ```
 pip install pyjedai
 ```
+More on [PyPI](https://pypi.org/project/pyjedai).
 
-More on [PyPI](pypi.org/project/pyjedai/).
+### Git
 
+Set up locally:
+```
+git clone https://github.com/AI-team-UoA/pyJedAI.git
+```
+go to the root directory with `cd pyJedAI` and type:
+```
+pip install .
+```
 
-### Tutorials
 
-| Tutorial | Notebook |
-|---|:-:|
-| Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) |
-| Dirty Entity Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/DirtyER.ipynb)|
-| Fine-Tuning using Optuna. | [Optuna.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) |
-| User-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) |
-| Raw data to pandas DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Readers.ipynb) |
 
 # Dependencies
 
 <div align="center">
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
-<img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
-<img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
-<img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
-<img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
+    <img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
+    <img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
+    <img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
+    <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
 
 __Status__ 
 
@@ -109,15 +91,19 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
 
 # Java - Wed Application 
 
-For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows.
+<img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
+
+For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
+
+<br>
 
 # Team & Authors
 
 <img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
@@ -129,20 +115,21 @@
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
- <hr>
-  <br>
- <a href="https://stelar-project.eu">
-  <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
- </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- <a href="https://ec.europa.eu/info/index_en">
-  <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
- </a>
- <br><br>
- <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.</b><br>
+    <hr>
+    <br>
+    <a href="https://stelar-project.eu">
+        <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
+    </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://ec.europa.eu/info/index_en">
+        <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
+    </a>
+    <br>
+    <br>
+        <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.
+        </b>
+    <br>
 </div>
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
----  # Overview pyJedAI is a python framework, aiming to offer experts and
+--- # Overview pyJedAI is a python framework, aiming to offer experts and
 novice users, robust and fast solutions for multiple types of Entity Resolution
 problems. It is builded using state-of-the-art python frameworks. pyJedAI
 constitutes the sole open-source Link Discovery tool that is capable of
 exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
 are publicly available through the Python data science ecosystem. This applies
 to both blocking and matching, thus ensuring high time efficiency, high
 scalability as well as high effectiveness, without requiring any labelled
@@ -19,64 +19,19 @@
 machine learning packages. - Offers supervised and un-supervised ML techniques.
 __Open demos are available in:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 __Google Colab Hands-on demo:__
        [https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/
          Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png]
-*** Details on the Architecture ***
-
-The purpose of this framework is to demonstrate how ER can be accomplished by
-expert and novice users in an intuitive, yet efficient and effective way.
-pyJedai addresses the following task: Given a source and a target dataset, S
-and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s â S
-â§ t â T}. Its architecture appears in the bellow figure. The first module
-is the data reader, which specifies the user input. pyJedAI supports both semi-
-structured and structured data as input. The former, which include SPARQL
-endpoints and RDF/OWL dumps, are read by RDFLib. The latter, which include
-relational databases as well as CSV and JSON files, are read by pandas. In this
-way, pyJedAI is able to interlink any combination of semi-structured and
-structured data sources, which is a unique feature. [pyJedAI-Architecture] The
-second step in pyJedAIâs pipeline performs block building, a coarsegrained
-process that clusters together similar entities. The end result consists of a
-set of candidate pairs, which are examined analytically by the subsequent
-steps. pyJedAI implements the same established methods for similarity joins and
-blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes
-beyond all Link Discovery tools by incorporating recent, state-of-the-art
-libraries for nearest neighbor search like FALCONN and FAISS.
-
-The entity matching step estimates the actual similarity between the candidate
-pairs. Unlike all other Link Discovery tools, which rely exclusively on string
-similarity measures like edit distance and Jaccard coefficient, pyJedAI
-leverages the latest advanced NLP techniques, like pre-trained embeddings
-(e.g., word2vect, fastText and Glove) and transformer language models (i.e.,
-BERT and its variants). More specifically, pyJedAI supports packages like
-strsimpy, Gensimand Hugging_Face. This unique feature boosts pyJedAIâs
-accuracy to a significant extent, without requiring any labelled instances from
-the user. The last step performs entity clustering to further increase the
-accuracy. The relevant techniques consider the global information provided by
-the similarity scores of all candidate pairs in order to take local decisions
-for each pair of entity descriptions. pyJedAI implements and offers the same
-established algorithms as JedAI, using NetworkX to ensure high time efficiency.
-Finally, users are able to evaluate, visualize and store the results of the
-selected pipeline through the intuitive interface of Jupyter notebooks. In this
-way, pyJedAI facilitates its use by researchers and practitioners that are
-familiar with the data science ecosystem, regardless of their familiarity with
-ER and Link Discovery, in general.  # Install Install the latest version of
-pyjedai __[requires python >= 3.8]__: ``` pip install pyjedai ``` More on
-[PyPI](pypi.org/project/pyjedai/). ### Tutorials | Tutorial | Notebook | |---|:
--:| | Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) | | Dirty Entity
-Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/DirtyER.ipynb)| | Fine-Tuning using Optuna. | [Optuna.ipynb](https://
-github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) | | User-
-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) | | Raw data to pandas
-DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/Readers.ipynb) | # Dependencies
+# Install ### PyPI Install the latest version of pyjedai __[requires python >=
+3.8]__: ``` pip install pyjedai ``` More on [PyPI](https://pypi.org/project/
+pyjedai). ### Git Set up locally: ``` git clone https://github.com/AI-team-UoA/
+pyJedAI.git ``` go to the root directory with `cd pyJedAI` and type: ``` pip
+install . ``` # Dependencies
   [https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/
 2560px-Pandas_logo.svg.png]    [https://upload.wikimedia.org/wikipedia/commons/
   thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png]    [https://
  logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png]     [https://
    upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-
                             Jupyter_logo.svg.png]
   [https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-
@@ -97,25 +52,31 @@
 badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
 workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
 pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
 ?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
 github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
 questions and discussions and our recommended starting point. Please report any
 bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application For Java users checkout the initial [JedAI](https://
-github.com/scify/JedAIToolkit). There you can find Java based code and a Web
-Application for interactive creation of ER workflows. # Team & Authors
-[pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-k.github.io) - Jakub
-Maciejewski - [George Papadakis](https://gpapadis.wordpress.com) - [Manolis
-Koubarakis](https://cgi.di.uoa.gr/~koubarak/) Research and development is made
-under the supervision of Pr. Manolis Koubarakis. This is a research project by
-the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and
-Telecommunications at the University of Athens. # License Released under the
-Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/
-blob/main/LICENSE). Copyright Â© 2023 AI-Team, University of Athens
+Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
+(https://github.com/scify/JedAIToolkit). There you can find Java based code and
+a Web Application for interactive creation of ER workflows.
+
+JedAI constitutes an open source, high scalability toolkit that offers out-of-
+the-box solutions for any data integration task, e.g., Record Linkage, Entity
+Resolution and Link Discovery. At its core lies a set of domain-independent,
+state-of-the-art techniques that apply to both RDF and relational data.
+# Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
 
 This project is being funded in the context of STELAR that is an HORIZON-Europe
```

### Comparing `pyjedai-0.0.7/pyproject.toml` & `pyjedai-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyjedai"
-version = "0.0.7"
+version = "0.0.8"
 description = "An open-source library that builds powerful end-to-end Entity Resolution workflows."
 readme = "README.md"
 authors = [
     { name = "Konstantinos Nikoletos", email = "nikoletos.kon@gmail.com" },
     { name = "George Papadakis", email = "gpapadis84@gmail.com" },
+    { name = "Jakub Maciejewski", email = "jacobb.maciejewski@gmail.com"}
 ]
 license = {text = "Apache Software License 2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
@@ -31,15 +31,15 @@
     "Operating System :: Unix",
     "Operating System :: iOS",
     "Topic :: Database",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = ["deduplication", "entity-resolution", "link-discovery"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "gensim >= 4.2.0",
     "matplotlib >= 3.1.3",
     "matplotlib-inline >= 0.1.3",
     "networkx >= 2.3",
     "nltk >= 3.7",
     "numpy >= 1.21",
@@ -69,8 +69,8 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "http://pyjedai.rtfd.io"
 "Documentation" = "http://pyjedai.rtfd.io"
 "Bug Tracker" = "https://github.com/AI-team-UoA/pyJedAI/issues"
-"Source code" = "https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai"
+"Source code" = "https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai"
```

### Comparing `pyjedai-0.0.7/src/pyjedai/block_building.py` & `pyjedai-0.0.8/src/pyjedai/block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/block_cleaning.py` & `pyjedai-0.0.8/src/pyjedai/block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/clustering.py` & `pyjedai-0.0.8/src/pyjedai/clustering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/comparison_cleaning.py` & `pyjedai-0.0.8/src/pyjedai/comparison_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/datamodel.py` & `pyjedai-0.0.8/src/pyjedai/datamodel.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/evaluation.py` & `pyjedai-0.0.8/src/pyjedai/evaluation.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/joins.py` & `pyjedai-0.0.8/src/pyjedai/joins.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/logs.py` & `pyjedai-0.0.8/src/pyjedai/logs.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/matching.py` & `pyjedai-0.0.8/src/pyjedai/matching.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,277 +2,126 @@
 """
 import statistics
 from time import time
 
 import matplotlib.pyplot as plt
 import numpy as np
 from networkx import Graph
-from py_stringmatching.similarity_measure.affine import Affine
-from py_stringmatching.similarity_measure.bag_distance import BagDistance
 from py_stringmatching.similarity_measure.cosine import Cosine
 from py_stringmatching.similarity_measure.dice import Dice
-from py_stringmatching.similarity_measure.editex import Editex
 from py_stringmatching.similarity_measure.generalized_jaccard import \
     GeneralizedJaccard
-from py_stringmatching.similarity_measure.hamming_distance import \
-    HammingDistance
 from py_stringmatching.similarity_measure.jaccard import Jaccard
 from py_stringmatching.similarity_measure.jaro import Jaro
-from py_stringmatching.similarity_measure.jaro_winkler import JaroWinkler
 from py_stringmatching.similarity_measure.levenshtein import Levenshtein
-from py_stringmatching.similarity_measure.monge_elkan import MongeElkan
-from py_stringmatching.similarity_measure.needleman_wunsch import \
-    NeedlemanWunsch
 from py_stringmatching.similarity_measure.overlap_coefficient import \
     OverlapCoefficient
-from py_stringmatching.similarity_measure.partial_ratio import PartialRatio
-from py_stringmatching.similarity_measure.partial_token_sort import \
-    PartialTokenSort
-from py_stringmatching.similarity_measure.ratio import Ratio
-from py_stringmatching.similarity_measure.smith_waterman import SmithWaterman
-from py_stringmatching.similarity_measure.soundex import Soundex
-from py_stringmatching.similarity_measure.tfidf import TfIdf
-from py_stringmatching.similarity_measure.token_sort import TokenSort
-from py_stringmatching.similarity_measure.tversky_index import TverskyIndex
-from py_stringmatching.tokenizer.alphabetic_tokenizer import \
-    AlphabeticTokenizer
-from py_stringmatching.tokenizer.alphanumeric_tokenizer import \
-    AlphanumericTokenizer
-from py_stringmatching.tokenizer.delimiter_tokenizer import DelimiterTokenizer
 from py_stringmatching.tokenizer.qgram_tokenizer import QgramTokenizer
 from py_stringmatching.tokenizer.whitespace_tokenizer import \
     WhitespaceTokenizer
-from sklearn.feature_extraction.text import TfidfVectorizer
-# from scipy.spatial.distance import cosine
-from sklearn.metrics.pairwise import cosine_similarity, pairwise_distances
-from tqdm.autonotebook import tqdm
-from sklearn.metrics import jaccard_score
 from scipy.spatial.distance import dice, jaccard
+from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
+from sklearn.metrics.pairwise import pairwise_distances
+from tqdm.autonotebook import tqdm
+from whoosh.scoring import BM25F, PL2, TF_IDF, Frequency
 
 from .datamodel import Data, PYJEDAIFeature
 from .evaluation import Evaluation
-from .utils import WordQgrammsTokenizer
-from whoosh.scoring import TF_IDF, Frequency, PL2, BM25F
+from .utils import WordQgramTokenizer, cosine, get_qgram_from_tokenizer_name
 
 # Package import from https://anhaidgroup.github.io/py_stringmatching/v0.4.2/index.html
 
-def cosine(x, y):
-    """Cosine similarity between two vectors
-    """
-    return cosine_similarity(x.reshape(1, -1), y.reshape(1, -1))[0][0]
-
-available_tokenizers = [
-    'white_space_tokenizer', 'qgram_tokenizer', 'delimiter_tokenizer',
-    'alphabetic_tokenizer', 'alphanumeric_tokenizer'
-]
-
 metrics_mapping = {
-    'levenshtein' : Levenshtein(),
     'edit_distance': Levenshtein(),
-    'jaro_winkler' : JaroWinkler(),
-    'bag_distance' : BagDistance(),
-    'editex' : Editex(),
     'cosine' : Cosine(),
     'jaro' : Jaro(),
-    'soundex' : Soundex(),
-    'tfidf' : TfIdf(),
-    'tversky_index':TverskyIndex(),
-    'ratio' : Ratio(),
-    'partial_token_sort' : PartialTokenSort(),
-    'partial_ratio' : PartialRatio(),
-    'hamming_distance' : HammingDistance(),
     'jaccard' : Jaccard(),
     'generalized_jaccard' : GeneralizedJaccard(),
     'dice': Dice(),
     'overlap_coefficient' : OverlapCoefficient(),
-    'token_sort': TokenSort(),
-    'cosine_vector_similarity': cosine,
     'TF-IDF' : TF_IDF(),
     'Frequency' : Frequency(),
     'PL2' : PL2(),
     'BM25F' : BM25F()
 }
 
+vector_metrics_mapping = {
+    'cosine': cosine
+}
+
 string_metrics = [
-    'bag_distance', 'editex', 'hamming_distance', 'jaro', 'jaro_winkler', 'levenshtein',
-    'edit_distance', 'partial_ratio', 'partial_token_sort', 'ratio', 'soundex', 'token_sort'
+    'jaro', 'edit_distance'
 ]
 
 set_metrics = [
-    'cosine', 'dice', 'generalized_jaccard', 'jaccard', 'overlap_coefficient', 'tversky_index'
-]
-
-bag_metrics = [
-    'tf-idf'
+    'cosine', 'dice', 'generalized_jaccard', 'jaccard', 'overlap_coefficient'
 ]
 
 vector_metrics = [
-    'cosine_vector_similarity'
+    'cosine', 'dice', 'jaccard'
 ]
 
-index_metrics = [
+whoosh_index_metrics = [
     'TF-IDF', 'Frequency', 'PL2', 'BM25F'
 ] 
 
-available_metrics = string_metrics + set_metrics + bag_metrics + vector_metrics + index_metrics
+magellan_metrics = string_metrics + set_metrics
+available_metrics = magellan_metrics + vector_metrics + whoosh_index_metrics
 
+#
+# Tokenizers
+#
+char_qgram_tokenizers = { 'char_'+ str(i) + 'gram':i for i in range(1, 7) }
+word_qgram_tokenizers = { 'word_'+ str(i) + 'gram':i for i in range(1, 7) }
+magellan_tokenizers = ['white_space_tokenizer']
 
-class EntityMatching(PYJEDAIFeature):
-    """Calculates similarity from 0.0 to 1.0 for all blocks
+tfidf_tokenizers = [ 'tfidf_' + cq for cq in char_qgram_tokenizers.keys() ] + \
+                    [ 'tfidf_' + wq for wq in word_qgram_tokenizers.keys() ]
+
+tf_tokenizers = [ 'tf_' + cq for cq in char_qgram_tokenizers.keys() ] + \
+                    [ 'tf_' + wq for wq in word_qgram_tokenizers.keys() ]
+                        
+boolean_tokenizers = [ 'boolean_' + cq for cq in char_qgram_tokenizers.keys() ] + \
+                        [ 'boolean_' + wq for wq in word_qgram_tokenizers.keys() ]
+
+vector_tokenizers = tfidf_tokenizers + tf_tokenizers + boolean_tokenizers
+
+available_tokenizers = [key for key in char_qgram_tokenizers] + [key for key in word_qgram_tokenizers] + magellan_tokenizers + vector_tokenizers
+
+
+class AbstractEntityMatching(PYJEDAIFeature):
+    """Calculates similarity from 0.0 to 1.0
     """
 
-    _method_name: str = "Entity Matching"
-    _method_info: str = "Calculates similarity from 0. to 1. for all blocks"
+    _method_name: str = "Abstract Entity Matching"
+    _method_info: str = "Calculates similarity from 0. to 1."
 
     def __init__(
             self,
             metric: str = 'dice',
-            tokenizer: str = 'white_space_tokenizer',
             similarity_threshold: float = 0.5,
-            qgram: int = 2, # for jaccard
-            tokenizer_return_set = False, # unique values or not,
-            attributes: any = None,
-            tfidf_similarity_metric: str = 'cosine',
-            delim_set: list = None, # DelimiterTokenizer
-            padding: bool = True, # QgramTokenizer
-            prefix_pad: str = '#', # QgramTokenizer (if padding=True)
-            suffix_pad: str = '$' # QgramTokenizer (if padding=True)
         ) -> None:
         self.pairs: Graph
         self.metric = metric
-        self.qgram: int = qgram
-        self.attributes: list = attributes
         self.similarity_threshold = similarity_threshold
-        self.vectors_d1 = None
-        self.vectors_d2 = None
-        self.tokenizer = tokenizer
         self.execution_time = 0
-        self.tfidf_similarity_metric = tfidf_similarity_metric
+        self.qgram=None
         #
         # Selecting tokenizer
         #
         if metric not in available_metrics:
             raise AttributeError(
                 'Metric ({}) does not exist. Please select one of the available. ({})'.format(
                     metric, available_metrics
                 )
             )
         else:
             self._metric = metric
 
-        if metric in set_metrics:
-            self.tokenizer_return_set = True
-        else:
-            self.tokenizer_return_set = tokenizer_return_set
-
-        if tokenizer == 'white_space_tokenizer':
-            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'char_qgram_tokenizer':
-            self._tokenizer = QgramTokenizer(qval=self.qgram,
-                                             return_set=self.tokenizer_return_set,
-                                             padding=padding,
-                                             suffix_pad=suffix_pad,
-                                             prefix_pad=prefix_pad)
-        elif tokenizer == 'word_qgram_tokenizer':
-            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'delimiter_tokenizer':
-            self._tokenizer = DelimiterTokenizer(return_set=self.tokenizer_return_set,
-                                                 delim_set=delim_set)
-        elif tokenizer == 'alphabetic_tokenizer':
-            self._tokenizer = AlphabeticTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'alphanumeric_tokenizer':
-            self._tokenizer = AlphanumericTokenizer(return_set=self.tokenizer_return_set)
-        else:
-            raise AttributeError(
-                'Tokenizer ({}) does not exist. Please select one of the available. ({})'.format(
-                    tokenizer, available_tokenizers
-                )
-            )
-        
-    def predict(self,
-                blocks: dict,
-                data: Data,
-                tqdm_disable: bool = False,
-                vectors_d1: np.array = None,
-                vectors_d2: np.array = None) -> Graph:
-        """Main method of entity matching. Inputs a set of blocks and outputs a graph \
-            that contains of the entity ids (nodes) and the similarity scores between them (edges).
-
-            Args:
-                blocks (dict): blocks of entities
-                data (Data): dataset module
-                tqdm_disable (bool, optional): Disables progress bar. Defaults to False.
-
-            Returns:
-                networkx.Graph: entity ids (nodes) and similarity scores between them (edges)
-        """
-        start_time = time()
-        self.tqdm_disable = tqdm_disable
-        self.vectors_d1 = vectors_d1
-        self.vectors_d2 = vectors_d2
-        
-        if self.metric in vector_metrics:
-            if(vectors_d1 is None):
-                raise ValueError("Embeddings of the first dataset not given")
-            else:
-                self.vectors = vectors_d1
-                if(not data.is_dirty_er):
-                    if(vectors_d2 is None):
-                        raise ValueError("Embeddings of the second dataset not given")
-                    self.vectors = np.concatenate((vectors_d1,vectors_d2), axis=0)
-
-        if not blocks:
-            raise ValueError("Empty blocks structure")
-        self.data = data
-        self.pairs = Graph()
-        all_blocks = list(blocks.values())
-        self._progress_bar = tqdm(total=len(blocks),
-                                  desc=self._method_name+" ("+self.metric+ ", " + str(self.tokenizer) + ")",
-                                  disable=self.tqdm_disable)
-                
-        if self.metric == 'tf-idf':
-            self._calculate_tfidf()
-        
-        if 'Block' in str(type(all_blocks[0])):
-            self._predict_raw_blocks(blocks)
-        elif isinstance(all_blocks[0], set):
-            self._predict_prunned_blocks(blocks)
-        else:
-            raise AttributeError("Wrong type of Blocks")
-        self.execution_time = time() - start_time
-        self._progress_bar.close()
-
-        return self.pairs
-
-    def _predict_raw_blocks(self, blocks: dict) -> None:
-        """Method for similarity evaluation blocks after Block building
-
-        Args:
-            blocks (dict): Block building blocks
-        """
-        if self.data.is_dirty_er:
-            for _, block in blocks.items():
-                entities_array = list(block.entities_D1)
-                for index_1 in range(0, len(entities_array), 1):
-                    for index_2 in range(index_1+1, len(entities_array), 1):
-                        similarity = self._similarity(entities_array[index_1],
-                                                      entities_array[index_2])
-                        self._insert_to_graph(entities_array[index_1],
-                                              entities_array[index_2],
-                                              similarity)
-                self._progress_bar.update(1)
-        else:
-            for _, block in blocks.items():
-                for entity_id1 in block.entities_D1:
-                    for entity_id2 in block.entities_D2:
-                        similarity = self._similarity(entity_id1, entity_id2)
-                        self._insert_to_graph(entity_id1, entity_id2, similarity)
-                self._progress_bar.update(1)
-
-    def _predict_prunned_blocks(self, blocks: dict) -> None:
+    def _predict_candidate_pairs(self, blocks: dict) -> None:
         """Similarity evaluation after comparison cleaning.
 
         Args:
             blocks (dict): Comparison cleaning blocks.
         """
         for entity_id, candidates in blocks.items():
             for candidate_id in candidates:
@@ -281,170 +130,26 @@
             self._progress_bar.update(1)
 
     def _insert_to_graph(self, entity_id1, entity_id2, similarity):
         if self.similarity_threshold is None or \
             (self.similarity_threshold is not None and similarity > self.similarity_threshold):
             self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
 
-    def _calculate_vector_similarity(self, entity_id1: int, entity_id2: int) -> float:
-        if self.metric in vector_metrics:
-            return metrics_mapping[self._metric](self.vectors[entity_id1],
-                                                 self.vectors[entity_id2])
-        else:
-            raise AttributeError("Please select one vector similarity metric from the given: " + ','.join(vector_metrics))
-        
-    def _calculate_tfidf(self) -> None:
-        
-        analyzer = 'char' if self.tokenizer == 'char_qgram_tokenizer' else 'word'
-        vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
-        
-        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
-        self._entities_d1 = d1 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist()
-        
-        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
-        self._entities_d2 = d2 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist() if not self.data.is_dirty_er else None
-                    
-        if self.data.is_dirty_er:
-            pass
-        else:
-            self.corpus = self._entities_d1 + self._entities_d2
-            self.tfidf_vectorizer = vectorizer.fit(self.corpus)
-            
-            if self.tfidf_similarity_metric == 'cosine':
-                self.tfidf_matrix = vectorizer.transform(self.corpus)
-                self.tfidf_similarity_matrix = cosine_similarity(self.tfidf_matrix)
-            elif self.tfidf_similarity_metric == 'jaccard':
-                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus)
-                self.tfidf_similarity_matrix = 1 - pairwise_distances( self.tfidf_matrix.toarray(), metric="jaccard")
-            elif self.tfidf_similarity_metric == 'dice':
-                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus).toarray()
-
-    def _calculate_tfidf_similarity(self, entity_id1: int, entity_id2: int) -> float:
-
-        if self.tfidf_similarity_metric == 'cosine':
-            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
-        elif self.tfidf_similarity_metric == 'jaccard':
-            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
-        elif self.tfidf_similarity_metric == 'dice':
-            return 1-dice(self.tfidf_matrix[entity_id1], self.tfidf_matrix[entity_id2])
-        else:
-            raise AttributeError("Please select one tf-idf similarity metric from the given: cosine, jaccard, dice")
-
-    def _calculate_tfidf(self) -> None:
-        
-        analyzer = 'char' if self.tokenizer == 'char_qgram_tokenizer' else 'word'
-        vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
-        
-        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
-        self._entities_d1 = d1 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist()
-        
-        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
-        self._entities_d2 = d2 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist() if not self.data.is_dirty_er else None
-                    
-        if self.data.is_dirty_er:
-            pass
-        else:
-            self.corpus = self._entities_d1 + self._entities_d2
-            self.tfidf_vectorizer = vectorizer.fit(self.corpus)
-            
-            if self.tfidf_similarity_metric == 'cosine':
-                self.tfidf_matrix = vectorizer.transform(self.corpus)
-                self.tfidf_similarity_matrix = cosine_similarity(self.tfidf_matrix)
-            elif self.tfidf_similarity_metric == 'jaccard':
-                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus)
-                self.tfidf_similarity_matrix = 1 - pairwise_distances( self.tfidf_matrix.toarray(), metric="jaccard")
-            elif self.tfidf_similarity_metric == 'dice':
-                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus).toarray()
-
-    def _calculate_tfidf_similarity(self, entity_id1: int, entity_id2: int) -> float:
-
-        if self.tfidf_similarity_metric == 'cosine':
-            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
-        elif self.tfidf_similarity_metric == 'jaccard':
-            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
-        elif self.tfidf_similarity_metric == 'dice':
-            return 1-dice(self.tfidf_matrix[entity_id1], self.tfidf_matrix[entity_id2])
-        else:
-            raise AttributeError("Please select one tf-idf similarity metric from the given: cosine, jaccard, dice")
-
-    def _similarity(self, entity_id1: int, entity_id2: int) -> float:
-
-        similarity: float = 0.0
-        if self.vectors_d1 is not None and self.metric in vector_metrics:
-            return self._calculate_vector_similarity(entity_id1, entity_id2)
-        elif self.metric == 'tf-idf':
-            return self._calculate_tfidf_similarity(entity_id1, entity_id2)
-
-        if isinstance(self.attributes, dict):
-            for attribute, weight in self.attributes.items():
-                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
-                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
-
-                similarity += weight*metrics_mapping[self._metric].get_sim_score(
-                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
-                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-                )
-        if isinstance(self.attributes, list):
-            for attribute in self.attributes:
-                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
-                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
-                similarity += metrics_mapping[self._metric].get_sim_score(
-                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
-                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-                )
-                similarity /= len(self.attributes)
-        else:
-            # concatenated row string
-            e1 = self.data.entities.iloc[entity_id1].str.cat(sep=' ').lower()
-            e2 = self.data.entities.iloc[entity_id2].str.cat(sep=' ').lower()
-            te1 = self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1
-            te2 = self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-            similarity = metrics_mapping[self._metric].get_sim_score(te1, te2)
-
-        return similarity        
-
     def report(self) -> None:
         """Prints Block Building method configuration
         """
         print(
             "Method name: " + self._method_name +
             "\nMethod info: " + self._method_info +
             ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
             "Attributes:\n\t" + ', '.join(c for c in (self.attributes if self.attributes is not None \
                 else self.data.dataset_1.columns)) +
             "\nRuntime: {:2.4f} seconds".format(self.execution_time)
         )
 
-    def _configuration(self) -> dict:
-        conf =  {
-            "Metric" : self.metric,
-            "Attributes" : self.attributes,
-            "Similarity threshold" : self.similarity_threshold,
-            "Tokenizer" : self.tokenizer
-        }
-
-        if self.metric == 'tf-idf':
-            conf["Similarity metric"] = self.tfidf_similarity_metric
-            if self.tokenizer == 'word_qgram_tokenizer' or self.tokenizer == 'char_qgram_tokenizer':
-                conf["QGram size"] = self.qgram
-
-        return conf
-        
     def get_weights_avg(self) -> float:
         return sum([w for _, _, w in self.pairs.edges(data='weight')])/len(self.pairs.edges(data='weight'))
 
     def get_weights_median(self) -> float:
         return [w for _, _, w in sorted(self.pairs.edges(data='weight'))][int(len(self.pairs.edges(data='weight'))/2)]    
     
     def get_weights_standard_deviation(self) -> float:
@@ -461,26 +166,22 @@
         # only one line may be specified; full height
         plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
         plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
         plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
         plt.legend()
         plt.show()
 
-    
     def plot_distribution_of_all_weights_2d(self) -> None:
         title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
         plt.figure(figsize=(10, 6))
         all_weights = [w for _, _, w in self.pairs.edges(data='weight')]
         sorted_weights = sorted(all_weights, reverse=True)
         
         fig, ax = plt.subplots(tight_layout=True)
         hist = ax.hist2d(sorted_weights, sorted_weights)
-        # plt.hist(sorted_weights)
-        # plt.xlim(0, 1)
-        # only one line may be specified; full height
         plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
         plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
         plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
         plt.legend()
         plt.show()
 
     def plot_distribution_of_scores(self) -> None:
@@ -554,15 +255,14 @@
         # Add some text for labels, title and custom x-axis tick labels, etc.
         ax.set_ylabel('Percentage of pairs in each range to all (%)')
         ax.set_title(title)
         ax.set_xlabel('Similarity score range')
         fig.tight_layout()
         plt.show()
 
-
     def evaluate(self,
                  prediction,
                  export_to_df: bool = False,
                  export_to_dict: bool = False,
                  with_classification_report: bool = False,
                  verbose: bool = True) -> any:
 
@@ -605,8 +305,304 @@
                 e1 = self.data._ids_mapping_1[e1] if e1 < self.data.dataset_limit else self.data._ids_mapping_2[e1]
                 e2 = self.data._ids_mapping_1[e2] if e2 < self.data.dataset_limit else self.data._ids_mapping_2[e2]
                 if with_similarity:
                     f.write(f"{e1}, {e2}, {similarity}\n")
                 else:
                     f.write(f"{e1}, {e2}\n")
             f.close()
-        
+
+class EntityMatching(AbstractEntityMatching):
+    """Calculates similarity from 0.0 to 1.0 for all blocks
+    """
+
+    _method_name: str = "Entity Matching"
+    _method_info: str = "Calculates similarity from 0. to 1. for all blocks"
+
+    def __init__(
+            self,
+            metric: str = 'dice',
+            tokenizer: str = 'white_space_tokenizer',
+            similarity_threshold: float = 0.5,
+            tokenizer_return_unique_values = False, # unique values or not,
+            attributes: any = None,
+        ) -> None:
+        super().__init__()
+        self.pairs: Graph
+        self.metric = metric
+        self.attributes: list = attributes
+        self.similarity_threshold = similarity_threshold
+        self.tokenizer = tokenizer
+        self.execution_time = 0
+        self._input_type = None
+        self.qgram: int = -1
+        #
+        # Selecting tokenizer
+        #
+        if metric not in available_metrics:
+            raise AttributeError(
+                'Metric ({}) does not exist. Please select one of the available. ({})'.format(
+                    metric, available_metrics
+                )
+            )
+        else:
+            self._metric = metric
+
+        if metric in set_metrics:
+            self.tokenizer_return_set = True
+        else:
+            self.tokenizer_return_set = tokenizer_return_unique_values
+
+        if 'gram' in tokenizer:
+            self.qgram = get_qgram_from_tokenizer_name(tokenizer)
+        
+        if tokenizer == 'white_space_tokenizer':
+            self._input_type = 'white_space'
+            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
+        elif tokenizer in char_qgram_tokenizers.keys():
+            self._input_type = 'char_qgram'
+            self._tokenizer = QgramTokenizer(qval=self.qgram,
+                                             return_set=self.tokenizer_return_set)
+        elif tokenizer in word_qgram_tokenizers.keys():
+            self._input_type = 'word_qgram'
+            self._tokenizer = WordQgramTokenizer(q=self.qgram)
+        elif 'tfidf' in tokenizer:
+            self._input_type = 'tfidf'
+        elif 'tf' in tokenizer:
+            self._input_type = 'tf'
+        elif 'boolean' in tokenizer:
+            self._input_type = 'boolean'
+        else:
+            raise AttributeError(
+                'Tokenizer ({}) does not exist. Please select one of the available. ({})'.format(
+                    tokenizer, available_tokenizers
+                )
+            )
+        
+    def predict(self,
+                blocks: dict,
+                data: Data,
+                tqdm_disable: bool = False) -> Graph:
+        """Main method of entity matching. Inputs a set of blocks and outputs a graph \
+            that contains of the entity ids (nodes) and the similarity scores between them (edges).
+
+            Args:
+                blocks (dict): blocks of entities
+                data (Data): dataset module
+                tqdm_disable (bool, optional): Disables progress bar. Defaults to False.
+
+            Returns:
+                networkx.Graph: entity ids (nodes) and similarity scores between them (edges)
+        """
+        start_time = time()
+        self.tqdm_disable = tqdm_disable
+        
+        if not blocks:
+            raise ValueError("Empty blocks structure")
+        self.data = data
+        self.pairs = Graph()
+        all_blocks = list(blocks.values())
+        self._progress_bar = tqdm(total=len(blocks),
+                                  desc=self._method_name+" ("+self.metric+ ", " + str(self.tokenizer) + ")",
+                                  disable=self.tqdm_disable)
+                
+        if self._input_type in ['tfidf', 'tf', 'boolean']:
+            self._calculate_tf_tfidf()
+
+        if 'Block' in str(type(all_blocks[0])):
+            self._predict_raw_blocks(blocks)
+        elif isinstance(all_blocks[0], set):
+            self._predict_candidate_pairs(blocks)
+        else:
+            raise AttributeError("Wrong type of Blocks")
+        self.execution_time = time() - start_time
+        self._progress_bar.close()
+
+        return self.pairs
+            
+    def _predict_raw_blocks(self, blocks: dict) -> None:
+        """Method for similarity evaluation blocks after Block building
+
+        Args:
+            blocks (dict): Block building blocks
+        """
+        if self.data.is_dirty_er:
+            for _, block in blocks.items():
+                entities_array = list(block.entities_D1)
+                for index_1 in range(0, len(entities_array), 1):
+                    for index_2 in range(index_1+1, len(entities_array), 1):
+                        similarity = self._similarity(entities_array[index_1],
+                                                      entities_array[index_2])
+                        self._insert_to_graph(entities_array[index_1],
+                                              entities_array[index_2],
+                                              similarity)
+                self._progress_bar.update(1)
+        else:
+            for _, block in blocks.items():
+                for entity_id1 in block.entities_D1:
+                    for entity_id2 in block.entities_D2:
+                        similarity = self._similarity(entity_id1, entity_id2)
+                        self._insert_to_graph(entity_id1, entity_id2, similarity)
+                self._progress_bar.update(1)
+
+    def _calculate_tf_tfidf(self) -> None:
+        
+        analyzer = 'char' if 'char' in self.tokenizer else 'word'
+        
+        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
+        self._entities_d1 = d1 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist()
+        
+        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
+        self._entities_d2 = d2 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist() if not self.data.is_dirty_er else None
+
+        if self._input_type == 'tfidf' or self._input_type == 'boolean':
+            vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else \
+                            TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
+        elif self._input_type == 'tf':
+            vectorizer = CountVectorizer(analyzer=analyzer) if self.qgram is None else \
+                            CountVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
+        
+        self._calculate_tf_and_tfidf_similarities(vectorizer)
+
+    def _calculate_tf_and_tfidf_similarities(self, vectorizer) -> None:
+        if self.data.is_dirty_er:
+            raise NotImplementedError("TFIDF for dirty ER is not implemented yet")
+        else:
+            self.corpus = self._entities_d1 + self._entities_d2
+            self.corpus_as_matrix = vectorizer.fit_transform(self.corpus)
+            if self._input_type == 'boolean':
+                # transform to boolean if value is positive to 1 and negative to 0
+                self.similarity_matrix = self.corpus_as_matrix.astype(bool).astype(int)
+                
+            self.similarity_matrix = 1 - pairwise_distances(self.corpus_as_matrix.toarray(), 
+                                                            metric=self.metric)
+
+    def _calculate_vector_similarity(self, entity_id1: int, entity_id2: int) -> float:
+            return self.similarity_matrix[entity_id1][entity_id2]
+
+    def _similarity(self, entity_id1: int, entity_id2: int) -> float:
+
+        similarity: float = 0.0
+        if self._input_type in ['tfidf', 'tf', 'boolean']:
+            return self._calculate_vector_similarity(entity_id1, entity_id2)
+        elif isinstance(self.attributes, dict):
+            for attribute, weight in self.attributes.items():
+                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
+                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
+
+                similarity += weight*metrics_mapping[self._metric].get_sim_score(
+                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
+                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+                )
+        if isinstance(self.attributes, list):
+            for attribute in self.attributes:
+                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
+                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
+                similarity += metrics_mapping[self._metric].get_sim_score(
+                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
+                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+                )
+                similarity /= len(self.attributes)
+        else:
+            # concatenated row string
+            e1 = self.data.entities.iloc[entity_id1].str.cat(sep=' ').lower()
+            e2 = self.data.entities.iloc[entity_id2].str.cat(sep=' ').lower()
+            te1 = self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1
+            te2 = self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+            similarity = metrics_mapping[self._metric].get_sim_score(te1, te2)
+        return similarity
+
+    def _configuration(self) -> dict:
+        return  {
+            "Metric" : self.metric,
+            "Attributes" : self.attributes,
+            "Similarity threshold" : self.similarity_threshold,
+            "Tokenizer" : self.tokenizer
+        }
+
+class VectorBasedMatching(AbstractEntityMatching):
+
+    _method_name: str = "Vector Based Matching"
+    _method_info: str = "Calculates similarity from 0. to 1. for vectors"
+
+    def __init__(
+            self,
+            metric: str = 'cosine',
+            similarity_threshold: float = 0.5,
+        ) -> None:
+        self.pairs: Graph
+        self.metric = metric
+        self.similarity_threshold = similarity_threshold
+        self.vectors_d1 = None
+        self.vectors_d2 = None
+        self.execution_time = 0
+
+        #
+        # Selecting tokenizer
+        #
+        if metric not in vector_metrics:
+            raise AttributeError(
+                'Metric ({}) does not exist. Please select one of the available. ({})'.format(
+                    metric, available_metrics
+                )
+            )
+        else:
+            self._metric = metric
+            
+    def predict(self,
+                blocks: dict,
+                data: Data,
+                vectors_d1: np.array,
+                vectors_d2: np.array = None,
+                tqdm_disable: bool = False,
+        ) -> Graph:
+        """Main method of entity matching. Inputs a set of blocks and outputs a graph \
+            that contains of the entity ids (nodes) and the similarity scores between them (edges).
+
+            Args:
+                blocks (dict): blocks of entities
+                data (Data): dataset module
+                tqdm_disable (bool, optional): Disables progress bar. Defaults to False.
+
+            Returns:
+                networkx.Graph: entity ids (nodes) and similarity scores between them (edges)
+        """
+        start_time = time()
+        self.tqdm_disable = tqdm_disable
+        self.vectors_d1 = vectors_d1
+        # self.vectors_d2 = vectors_d2
+        
+
+        if(vectors_d1 is None):
+            raise ValueError("Embeddings of the first dataset not given")
+        else:
+            self.vectors = vectors_d1
+            if(not data.is_dirty_er):
+                if(vectors_d2 is None):
+                    raise ValueError("Embeddings of the second dataset not given")
+                self.vectors = np.concatenate((vectors_d1,vectors_d2), axis=0)
+        self.data = data
+        self.pairs = Graph()
+        self._progress_bar = tqdm(total=len(blocks),
+                                  desc=self._method_name+" ("+self.metric+ ", " + str(self.tokenizer) + ")",
+                                  disable=self.tqdm_disable)
+        self._predict_candidate_pairs(blocks)
+        self.execution_time = time() - start_time
+        self._progress_bar.close()
+
+        return self.pairs
+
+    def _similarity(self, entity_id1: int, entity_id2: int) -> float:
+        return vector_metrics_mapping[self._metric](self.vectors[entity_id1], self.vectors[entity_id2])
+
+    def _configuration(self) -> dict:
+        conf =  {
+            "Metric" : self.metric,
+            "Similarity threshold" : self.similarity_threshold
+        }
+        
+        return conf
```

### Comparing `pyjedai-0.0.7/src/pyjedai/prioritization.py` & `pyjedai-0.0.8/src/pyjedai/prioritization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/utils.py` & `pyjedai-0.0.8/src/pyjedai/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 
 import numpy as np
+import re
 from nltk import ngrams
 from nltk.tokenize import word_tokenize
 from pyjedai.datamodel import Block, Data
 from typing import List, Tuple
 import random
 from queue import PriorityQueue
 import math
@@ -137,14 +138,34 @@
     print("Number of clusters: ", len(clusters))
     for (cluster_id, entity_ids) in zip(range(0, len(clusters)), clusters):
         print("\nCluster ", "\033[1;32m" + \
               str(cluster_id)+"\033[0m", " contains: " + "[\033[1;34m" + \
             str(len(entity_ids)) + " entities\033[0m]")
         print(entity_ids)
 
+def cosine(x, y):
+    """Cosine similarity between two vectors
+    """
+    return cosine_similarity(x.reshape(1, -1), y.reshape(1, -1))[0][0]
+
+def get_ngrams(text, n ):
+    n_grams = ngrams(word_tokenize(text), n)
+    return [ ' '.join(grams) for grams in n_grams]
+
+def get_qgram_from_tokenizer_name(tokenizer: str) -> int:
+    """Returns the q-gram value from the tokenizer name.
+
+    Args:
+        tokenizer (str): Tokenizer name.
+
+    Returns:
+        int: q-gram value.
+    """
+    return [int(s) for s in re.findall('\d+', tokenizer)][0]
+
 def text_cleaning_method(col):
     """Lower clean.
     """
     return col.str.lower()
 
 def chi_square(in_array: np.array) -> float:
     """Chi Square Method
@@ -197,15 +218,15 @@
     def __init__(self) -> None:
         super().__init__()
         
     @abstractmethod
     def tokenize(self, text: str) -> list:
         pass
 
-class WordQgrammsTokenizer(Tokenizer):
+class WordQgramTokenizer(Tokenizer):
     
     def __init__(self, q: int = 3) -> None:
         super().__init__()
         self.q = q
     
     def tokenize(self, text: str) -> list:
         return [' '.join(gram) for gram in list(ngrams(word_tokenize(text), self.q))]
@@ -216,23 +237,14 @@
     def __init__(self) -> None:
         super().__init__()
         
     @abstractmethod
     def tokenize(self, text: str) -> list:
         pass
 
-class WordQgrammsTokenizer(Tokenizer):
-    
-    def __init__(self, q: int = 3) -> None:
-        super().__init__()
-        self.q = q
-    
-    def tokenize(self, text: str) -> list:
-        return [' '.join(gram) for gram in list(ngrams(word_tokenize(text), self.q))]
-
 class SubsetIndexer(ABC):
     """Stores the indices of retained entities of the initial datasets,
        calculates and stores the mapping of element indices from new to old dataset (id in subset -> id in original)
     """
     def __init__(self, blocks: dict, data: Data, subset : bool):
         self.d1_retained_ids: list[int] = None
         self.d2_retained_ids : list[int] = None
```

### Comparing `pyjedai-0.0.7/src/pyjedai/vector_based_blocking.py` & `pyjedai-0.0.8/src/pyjedai/vector_based_blocking.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/visualization.py` & `pyjedai-0.0.8/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai/workflow.py` & `pyjedai-0.0.8/src/pyjedai/workflow.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/src/pyjedai.egg-info/PKG-INFO` & `pyjedai-0.0.8/src/pyjedai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.7
+Version: 0.0.8
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
-Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
+Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>, Jakub Maciejewski <jacobb.maciejewski@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, http://pyjedai.rtfd.io
 Project-URL: Documentation, http://pyjedai.rtfd.io
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
 Keywords: deduplication,entity-resolution,link-discovery
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: iOS
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
-<br>
-<img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
+    <br>
+    <img align="center" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/pyjedai.logo.drawio.png?raw=true" alt="pyJedAI" width="400"/>
 </div>
-<br><br>
+<br>
+<br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-<!--[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
- <a href='https://pyjedai.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/pyjedai/badge/?version=latest' alt='Documentation Status' />
-</a>
- -->
 # Overview
 
 pyJedAI is a python framework, aiming to offer experts and novice users, robust and fast solutions for multiple types of Entity Resolution problems. It is builded using state-of-the-art python frameworks. pyJedAI constitutes the sole open-source Link Discovery tool that is capable of exploiting the latest breakthroughs in Deep Learning and NLP techniques, which are publicly available through the Python data science ecosystem. This applies to both blocking and matching, thus ensuring high time efficiency, high scalability as well as high effectiveness, without requiring any labelled instances from the user.
 
 ### Key-Features
 
 - Input data-type independent. Both structured and semi-structured data can be processed.
@@ -61,79 +54,67 @@
 - Easy-to-use.
 - Utilizes some of the famous and cutting-edge machine learning packages.
 - Offers supervised and un-supervised ML techniques.
 
 __Open demos are available in:__
 
 <div align="center">
-<a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
-</a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-<a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
-<img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
-</a>
+    <a href="https://nbviewer.org/github/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://nbviewer.org/static/img/nav_logo.svg" width=120/> 
+    </a>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Demo.ipynb">
+        <img align="center" src="https://miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png" width=120/> 
+    </a>
 </div>
 
 __Google Colab Hands-on demo:__ 
 
 <div align="center">
-<a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
-<img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
-</a>
+    <a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
+        <img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
+    </a>
 </div>
 
-
-
-<details>
-<summary><h4>Details on the Architecture</h4></summary>
-<br>
-The purpose of this framework is to demonstrate how ER can be accomplished by expert and novice users in an intuitive, yet efficient and effective way. pyJedai addresses the following task: Given a source and a target dataset, S and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s ∈ S ∧ t ∈ T}. Its architecture appears in the bellow figure. The first module is the data reader, which specifies the user input. pyJedAI supports both semi-structured and structured data as input. The former, which include SPARQL endpoints and RDF/OWL dumps, are read by <a href="https://rdflib.dev">RDFLib</a>. The latter, which include relational databases as well as CSV and JSON files, are read by <a href="https://pandas.pydata.org">pandas</a>. In this way, pyJedAI is able to interlink any combination of semi-structured and structured data sources, which is a unique feature. <img align="right" src="https://github.com/Nikoletos-K/pyJedAI/blob/main/docs/img/demo-architecture.png?raw=true?raw=true" alt="pyJedAI-Architecture" width="500"/> The second step in pyJedAI’s pipeline performs block building, a coarsegrained process that clusters together similar entities. The end result consists of a set of candidate pairs, which are examined analytically by the subsequent steps. pyJedAI implements the same established methods for similarity joins and blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes beyond all Link Discovery tools by incorporating recent, state-of-the-art libraries for nearest neighbor search like <a href="https://falconn-lib.org">FALCONN</a> and <a href="https://github.com/facebookresearch/faiss">FAISS</a>. <br>
-
-<br>
-
- The entity matching step estimates the actual similarity between the candidate pairs. Unlike all other Link Discovery tools, which rely exclusively on string similarity measures like edit distance and Jaccard coefficient, pyJedAI leverages the latest advanced NLP techniques, like pre-trained embeddings (e.g., word2vect, fastText and Glove) and transformer language models (i.e., BERT and its variants). More specifically, pyJedAI supports packages like <a href="https://github.com/luozhouyang/python-string-similarity">strsimpy</a>, <a href="https://radimrehurek.com/gensim/">Gensim</a>and <a href="https://huggingface.co">Hugging Face</a>. This unique feature boosts pyJedAI’s accuracy to a significant extent, without requiring any labelled instances from the user. The last step performs entity clustering to further increase the accuracy. The relevant techniques consider the global information provided by the similarity scores of all candidate pairs in order to take local decisions for each pair of entity descriptions. pyJedAI implements and offers the same established algorithms as JedAI, using <a href="https://networkx.org">NetworkX</a> to ensure high time efficiency. Finally, users are able to evaluate, visualize and store the results of the selected pipeline through the intuitive interface of Jupyter notebooks. In this way, pyJedAI facilitates its use by researchers and practitioners that are familiar with the data science ecosystem, regardless of their familiarity with ER and Link
-Discovery, in general.
-
-</details>
-
 # Install
 
+### PyPI
 Install the latest version of pyjedai __[requires python >= 3.8]__:
 ```
 pip install pyjedai
 ```
+More on [PyPI](https://pypi.org/project/pyjedai).
 
-More on [PyPI](pypi.org/project/pyjedai/).
+### Git
 
+Set up locally:
+```
+git clone https://github.com/AI-team-UoA/pyJedAI.git
+```
+go to the root directory with `cd pyJedAI` and type:
+```
+pip install .
+```
 
-### Tutorials
 
-| Tutorial | Notebook |
-|---|:-:|
-| Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) |
-| Dirty Entity Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/DirtyER.ipynb)|
-| Fine-Tuning using Optuna. | [Optuna.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) |
-| User-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) |
-| Raw data to pandas DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Readers.ipynb) |
 
 # Dependencies
 
 <div align="center">
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
-<img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
-<img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
-<img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
-<img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
-<img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
-<img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
-<img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png" width=120/> &nbsp;&nbsp;
+    <img align="center" src="https://logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png" width=120/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" width=70/>  <br>
+    <img align="center" src="https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-logo.png" width=150/>
+    <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Plotly_logo_for_digital_final_%286%29.png/1200px-Plotly_logo_for_digital_final_%286%29.png" width=150/>
+    <img align="center" src="https://pytorch.org/tutorials/_static/img/thumbnails/cropped/profiler.png" width=160/> 
+    <img align="center" src="https://www.fullstackpython.com/img/logos/scipy.png" width=150/>  <br><br>
+    <img align="center" src="https://www.kornosk.me/resources/language-model/featured.png" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-745fdcbeffe8" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://networkx.org/_static/networkx_logo.svg" width=150/> &nbsp;&nbsp;&nbsp;
+    <img align="center" src="https://raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png" width=70/> 
 </div>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/Nikoletos-K/pyJedAI/blob/main/requirements.txt).
 
 __Status__ 
 
@@ -143,15 +124,19 @@
 
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues).
 
 # Java - Wed Application 
 
-For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows.
+<img align="left" src="https://github.com/scify/JedAIToolkit/blob/master/documentation/JedAI_logo.png?raw=true" alt="pyJedAI" width="130"/>
+
+For Java users checkout the initial [JedAI](https://github.com/scify/JedAIToolkit). There you can find Java based code and a Web Application for interactive creation of ER workflows. <br><br> JedAI constitutes an open source, high scalability toolkit that offers out-of-the-box solutions for any data integration task, e.g., Record Linkage, Entity Resolution and Link Discovery. At its core lies a set of domain-independent, state-of-the-art techniques that apply to both RDF and relational data.
+
+<br>
 
 # Team & Authors
 
 <img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
 - Jakub Maciejewski
@@ -163,20 +148,21 @@
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE).
 
 Copyright © 2023 AI-Team, University of Athens
 
 <div align="center">
- <hr>
-  <br>
- <a href="https://stelar-project.eu">
-  <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
- </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- <a href="https://ec.europa.eu/info/index_en">
-  <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
- </a>
- <br><br>
- <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.</b><br>
+    <hr>
+    <br>
+    <a href="https://stelar-project.eu">
+        <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
+    </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+    <a href="https://ec.europa.eu/info/index_en">
+        <img align="center" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png" width=140/>
+    </a>
+    <br>
+    <br>
+        <b>This project is being funded in the context of <a href="https://stelar-project.eu">STELAR</a> that is an <a href="https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en">HORIZON-Europe</a> project.
+        </b>
+    <br>
 </div>
-
-
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.7 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.8 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
-gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, http://
-pyjedai.rtfd.io Project-URL: Documentation, http://pyjedai.rtfd.io Project-URL:
-Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues Project-URL: Source
-code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai Keywords:
-deduplication,entity-resolution,link-discovery Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
-Implementation Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Developers Classifier: Natural Language :: English Classifier: Operating
-System :: Microsoft :: Windows Classifier: Operating System :: Unix Classifier:
-Operating System :: iOS Classifier: Topic :: Database Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7 Description-
+gmail.com>, Jakub Maciejewski
+maciejewski@gmail.com> License: Apache Software License 2.0 Project-URL:
+Homepage, http://pyjedai.rtfd.io Project-URL: Documentation, http://
+pyjedai.rtfd.io Project-URL: Bug Tracker, https://github.com/AI-team-UoA/
+pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
+pyJedAI/tree/main/pyjedai Keywords: deduplication,entity-resolution,link-
+discovery Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: Implementation
+Classifier: Intended Audience :: Information Technology Classifier: Intended
+Audience :: Science/Research Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: Unix Classifier: Operating
+System :: iOS Classifier: Topic :: Database Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
----  # Overview pyJedAI is a python framework, aiming to offer experts and
+--- # Overview pyJedAI is a python framework, aiming to offer experts and
 novice users, robust and fast solutions for multiple types of Entity Resolution
 problems. It is builded using state-of-the-art python frameworks. pyJedAI
 constitutes the sole open-source Link Discovery tool that is capable of
 exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
 are publicly available through the Python data science ecosystem. This applies
 to both blocking and matching, thus ensuring high time efficiency, high
 scalability as well as high effectiveness, without requiring any labelled
@@ -41,64 +42,19 @@
 machine learning packages. - Offers supervised and un-supervised ML techniques.
 __Open demos are available in:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 __Google Colab Hands-on demo:__
        [https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/
          Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png]
-*** Details on the Architecture ***
-
-The purpose of this framework is to demonstrate how ER can be accomplished by
-expert and novice users in an intuitive, yet efficient and effective way.
-pyJedai addresses the following task: Given a source and a target dataset, S
-and T, respectively, discover the set of links L = {(s,owl:sameAS, t)|s â S
-â§ t â T}. Its architecture appears in the bellow figure. The first module
-is the data reader, which specifies the user input. pyJedAI supports both semi-
-structured and structured data as input. The former, which include SPARQL
-endpoints and RDF/OWL dumps, are read by RDFLib. The latter, which include
-relational databases as well as CSV and JSON files, are read by pandas. In this
-way, pyJedAI is able to interlink any combination of semi-structured and
-structured data sources, which is a unique feature. [pyJedAI-Architecture] The
-second step in pyJedAIâs pipeline performs block building, a coarsegrained
-process that clusters together similar entities. The end result consists of a
-set of candidate pairs, which are examined analytically by the subsequent
-steps. pyJedAI implements the same established methods for similarity joins and
-blocking as JedAI, such as Standard Blocking and Sorted Neighborhood, but goes
-beyond all Link Discovery tools by incorporating recent, state-of-the-art
-libraries for nearest neighbor search like FALCONN and FAISS.
-
-The entity matching step estimates the actual similarity between the candidate
-pairs. Unlike all other Link Discovery tools, which rely exclusively on string
-similarity measures like edit distance and Jaccard coefficient, pyJedAI
-leverages the latest advanced NLP techniques, like pre-trained embeddings
-(e.g., word2vect, fastText and Glove) and transformer language models (i.e.,
-BERT and its variants). More specifically, pyJedAI supports packages like
-strsimpy, Gensimand Hugging_Face. This unique feature boosts pyJedAIâs
-accuracy to a significant extent, without requiring any labelled instances from
-the user. The last step performs entity clustering to further increase the
-accuracy. The relevant techniques consider the global information provided by
-the similarity scores of all candidate pairs in order to take local decisions
-for each pair of entity descriptions. pyJedAI implements and offers the same
-established algorithms as JedAI, using NetworkX to ensure high time efficiency.
-Finally, users are able to evaluate, visualize and store the results of the
-selected pipeline through the intuitive interface of Jupyter notebooks. In this
-way, pyJedAI facilitates its use by researchers and practitioners that are
-familiar with the data science ecosystem, regardless of their familiarity with
-ER and Link Discovery, in general.  # Install Install the latest version of
-pyjedai __[requires python >= 3.8]__: ``` pip install pyjedai ``` More on
-[PyPI](pypi.org/project/pyjedai/). ### Tutorials | Tutorial | Notebook | |---|:
--:| | Clean-Clean Entity Resolution.| [CleanCleanER.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/CleanCleanER.ipynb) | | Dirty Entity
-Resolution. | [DirtyER.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/DirtyER.ipynb)| | Fine-Tuning using Optuna. | [Optuna.ipynb](https://
-github.com/Nikoletos-K/pyJedAI/blob/main/tutorials/Optuna.ipynb) | | User-
-Friendly Approach. WorkFlow module. | [WorkFlow.ipynb](https://github.com/
-Nikoletos-K/pyJedAI/blob/main/tutorials/WorkFlow.ipynb) | | Raw data to pandas
-DataFrame. | [Readers.ipynb](https://github.com/Nikoletos-K/pyJedAI/blob/main/
-tutorials/Readers.ipynb) | # Dependencies
+# Install ### PyPI Install the latest version of pyjedai __[requires python >=
+3.8]__: ``` pip install pyjedai ``` More on [PyPI](https://pypi.org/project/
+pyjedai). ### Git Set up locally: ``` git clone https://github.com/AI-team-UoA/
+pyJedAI.git ``` go to the root directory with `cd pyJedAI` and type: ``` pip
+install . ``` # Dependencies
   [https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/
 2560px-Pandas_logo.svg.png]    [https://upload.wikimedia.org/wikipedia/commons/
   thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png]    [https://
  logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png]     [https://
    upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-
                             Jupyter_logo.svg.png]
   [https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-
@@ -119,25 +75,31 @@
 badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
 workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
 pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
 ?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
 github.com/Nikoletos-K/pyJedAI/discussions) is the discussion forum for general
 questions and discussions and our recommended starting point. Please report any
 bugs that you find [here](https://github.com/Nikoletos-K/pyJedAI/issues). #
-Java - Wed Application For Java users checkout the initial [JedAI](https://
-github.com/scify/JedAIToolkit). There you can find Java based code and a Web
-Application for interactive creation of ER workflows. # Team & Authors
-[pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-k.github.io) - Jakub
-Maciejewski - [George Papadakis](https://gpapadis.wordpress.com) - [Manolis
-Koubarakis](https://cgi.di.uoa.gr/~koubarak/) Research and development is made
-under the supervision of Pr. Manolis Koubarakis. This is a research project by
-the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and
-Telecommunications at the University of Athens. # License Released under the
-Apache-2.0 license [(see LICENSE.txt)](https://github.com/Nikoletos-K/pyJedAI/
-blob/main/LICENSE). Copyright Â© 2023 AI-Team, University of Athens
+Java - Wed Application [pyJedAI] For Java users checkout the initial [JedAI]
+(https://github.com/scify/JedAIToolkit). There you can find Java based code and
+a Web Application for interactive creation of ER workflows.
+
+JedAI constitutes an open source, high scalability toolkit that offers out-of-
+the-box solutions for any data integration task, e.g., Record Linkage, Entity
+Resolution and Link Discovery. At its core lies a set of domain-independent,
+state-of-the-art techniques that apply to both RDF and relational data.
+# Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/Nikoletos-K/pyJedAI/blob/main/LICENSE). Copyright Â© 2023
+AI-Team, University of Athens
 ===============================================================================
 
   [https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png]
               [https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/
               Flag_of_Europe.svg/1200px-Flag_of_Europe.svg.png]
 
 This project is being funded in the context of STELAR that is an HORIZON-Europe
```

### Comparing `pyjedai-0.0.7/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.0.8/src/pyjedai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/tests/test_block_building.py` & `pyjedai-0.0.8/tests/test_block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/tests/test_block_cleaning.py` & `pyjedai-0.0.8/tests/test_block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/tests/test_clustering.py` & `pyjedai-0.0.8/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.7/tests/test_comparison_cleaning.py` & `pyjedai-0.0.8/tests/test_comparison_cleaning.py`

 * *Files identical despite different names*

