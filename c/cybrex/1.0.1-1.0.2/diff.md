# Comparing `tmp/cybrex-1.0.1.tar.gz` & `tmp/cybrex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.0.1.tar", last modified: Wed Jul  5 19:29:09 2023, max compression
+gzip compressed data, was "cybrex-1.0.2.tar", last modified: Wed Jul  5 19:31:24 2023, max compression
```

## Comparing `cybrex-1.0.1.tar` & `cybrex-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:29:09.959434 cybrex-1.0.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      623 2023-07-05 19:29:09.959138 cybrex-1.0.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      316 2023-07-05 19:22:12.000000 cybrex-1.0.1/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:29:09.956287 cybrex-1.0.1/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)     1306 2023-07-05 19:02:19.000000 cybrex-1.0.1/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5545 2023-07-05 19:19:55.000000 cybrex-1.0.1/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:29:09.958660 cybrex-1.0.1/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      623 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-05 19:29:09.000000 cybrex-1.0.1/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      562 2023-07-05 19:28:59.000000 cybrex-1.0.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:23:43.000000 cybrex-1.0.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 19:29:09.959586 cybrex-1.0.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:31:24.593670 cybrex-1.0.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      592 2023-07-05 19:31:24.593422 cybrex-1.0.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      316 2023-07-05 19:22:12.000000 cybrex-1.0.2/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:31:24.591047 cybrex-1.0.2/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)     1307 2023-07-05 19:30:23.000000 cybrex-1.0.2/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5558 2023-07-05 19:30:25.000000 cybrex-1.0.2/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:31:24.592855 cybrex-1.0.2/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      592 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-05 19:31:24.000000 cybrex-1.0.2/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-05 19:31:14.000000 cybrex-1.0.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:23:43.000000 cybrex-1.0.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 19:31:24.593759 cybrex-1.0.2/setup.cfg
```

### Comparing `cybrex-1.0.1/PKG-INFO` & `cybrex-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.1
-Summary: Cybrex is an AI allowing to chat with science
+Version: 1.0.2
+Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Cybrex AI
```

### Comparing `cybrex-1.0.1/cybrex/cli.py` & `cybrex-1.0.2/cybrex/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import fire
 from termcolor import colored
 
-from cybrex_ai import CybrexAI
+from .cybrex_ai import CybrexAI
 
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
     async def chat_doc(self, doi: str, question: str):
```

### Comparing `cybrex-1.0.1/cybrex/cybrex_ai.py` & `cybrex-1.0.2/cybrex/cybrex_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os.path
 import uuid
-from typing import Optional, List
+from typing import (
+    List,
+    Optional,
+)
 
 import chromadb
 import pypdf
 import yaml
 from aiokit import AioThing
 from izihawa_configurator import Configurator
 from izihawa_utils.file import mkdir_p
+from langchain.chains import RetrievalQA
 from langchain.chains.summarize import load_summarize_chain
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.embeddings.base import Embeddings
-from langchain.chains import RetrievalQA
 from langchain.llms import OpenAI
 from langchain.schema import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
```

### Comparing `cybrex-1.0.1/cybrex.egg-info/PKG-INFO` & `cybrex-1.0.2/cybrex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.1
-Summary: Cybrex is an AI allowing to chat with science
+Version: 1.0.2
+Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Cybrex AI
```

### Comparing `cybrex-1.0.1/pyproject.toml` & `cybrex-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "Interdimensional Walker" }]
-description = "Cybrex is an AI allowing to chat with science"
+description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
 dynamic = ["dependencies"]
```

