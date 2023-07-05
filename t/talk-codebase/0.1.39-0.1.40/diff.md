# Comparing `tmp/talk_codebase-0.1.39.tar.gz` & `tmp/talk_codebase-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.39.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.40.tar", max compression
```

## Comparing `talk_codebase-0.1.39.tar` & `talk_codebase-0.1.40.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3246 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/README.md
--rw-r--r--   0        0        0      986 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/cli.py
--rw-r--r--   0        0        0     2250 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/config.py
--rw-r--r--   0        0        0     1926 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/consts.py
--rw-r--r--   0        0        0     5399 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-07-05 02:13:31.879485 talk_codebase-0.1.39/talk_codebase/utils.py
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 talk_codebase-0.1.39/PKG-INFO
+-rw-r--r--   0        0        0     3183 2023-07-05 02:20:33.613852 talk_codebase-0.1.40/README.md
+-rw-r--r--   0        0        0      986 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/cli.py
+-rw-r--r--   0        0        0     2250 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/config.py
+-rw-r--r--   0        0        0     1926 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/consts.py
+-rw-r--r--   0        0        0     5629 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-05 02:20:33.617852 talk_codebase-0.1.40/talk_codebase/utils.py
+-rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 talk_codebase-0.1.40/PKG-INFO
```

### Comparing `talk_codebase-0.1.39/README.md` & `talk_codebase-0.1.40/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 * Simple configuration in just a couple of clicks
 * Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
-* It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
+* It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
 * Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
@@ -50,15 +50,14 @@
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
 openai_model_name: gpt-3.5-turbo
 # Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
-# You can find the list of available models here: https://gpt4all.io/models
 local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
 # Path to local model. If you want to use a local model, you need to specify the path to it.
 model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
```

### Comparing `talk_codebase-0.1.39/pyproject.toml` & `talk_codebase-0.1.40/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.39"
+version = "0.1.40"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.39/talk_codebase/cli.py` & `talk_codebase-0.1.40/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.39/talk_codebase/config.py` & `talk_codebase-0.1.40/talk_codebase/config.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.39/talk_codebase/consts.py` & `talk_codebase-0.1.40/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.39/talk_codebase/llm.py` & `talk_codebase-0.1.40/talk_codebase/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 from typing import Optional
 
+import gpt4all
 import questionary
 from halo import Halo
 from langchain import FAISS
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import HuggingFaceEmbeddings, OpenAIEmbeddings
-from langchain.llms import GPT4All
+from langchain.llms import LlamaCpp
 from langchain.schema import HumanMessage, SystemMessage
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 from talk_codebase.consts import MODEL_TYPES
 from talk_codebase.utils import load_files, get_local_vector_store, calculate_cost, StreamStdOut
 
 
@@ -69,17 +70,19 @@
 class LocalLLM(BaseLLM):
 
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = HuggingFaceEmbeddings(model_name='all-MiniLM-L6-v2')
         return self._create_vector_store(embeddings, MODEL_TYPES["LOCAL"], root_dir)
 
     def _create_model(self):
-        llm = GPT4All(
-            model=self.config.get("local_model_name"),
-            max_tokens=int(self.config.get("max_tokens")),
+        gpt4all.GPT4All.retrieve_model(model_name=self.config.get("local_model_name"),
+                                       model_path=self.config.get("model_path"))
+        llm = LlamaCpp(
+            model_path=os.path.join(self.config.get("model_path"), self.config.get("local_model_name")),
+            n_ctx=int(self.config.get("max_tokens")),
             callback_manager=CallbackManager([StreamStdOut()]),
             temp=float(self.config.get("temperature")),
             streaming=True,
             allow_download=True)
         return llm
 
     def send_query(self, query):
```

### Comparing `talk_codebase-0.1.39/talk_codebase/utils.py` & `talk_codebase-0.1.40/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.39/PKG-INFO` & `talk_codebase-0.1.40/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.39
+Version: 0.1.40
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 ## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 * Simple configuration in just a couple of clicks
 * Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
-* It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
+* It supports offline code processing using LlamaCpp and [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
 * Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
@@ -77,15 +77,14 @@
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
 openai_model_name: gpt-3.5-turbo
 # Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
-# You can find the list of available models here: https://gpt4all.io/models
 local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
 # Path to local model. If you want to use a local model, you need to specify the path to it.
 model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
```

