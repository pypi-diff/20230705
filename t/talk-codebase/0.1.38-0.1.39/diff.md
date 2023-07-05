# Comparing `tmp/talk_codebase-0.1.38.tar.gz` & `tmp/talk_codebase-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.38.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.39.tar", max compression
```

## Comparing `talk_codebase-0.1.38.tar` & `talk_codebase-0.1.39.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3361 2023-07-05 01:55:55.808348 talk_codebase-0.1.38/README.md
--rw-r--r--   0        0        0      986 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/cli.py
--rw-r--r--   0        0        0     2250 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/config.py
--rw-r--r--   0        0        0     1926 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/consts.py
--rw-r--r--   0        0        0     5629 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/utils.py
--rw-r--r--   0        0        0     4415 1970-01-01 00:00:00.000000 talk_codebase-0.1.38/PKG-INFO
+-rw-r--r--   0        0        0     3246 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/README.md
+-rw-r--r--   0        0        0      986 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/cli.py
+-rw-r--r--   0        0        0     2250 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/config.py
+-rw-r--r--   0        0        0     1926 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/consts.py
+-rw-r--r--   0        0        0     5399 2023-07-05 02:13:31.875485 talk_codebase-0.1.39/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-05 02:13:31.879485 talk_codebase-0.1.39/talk_codebase/utils.py
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 talk_codebase-0.1.39/PKG-INFO
```

### Comparing `talk_codebase-0.1.38/README.md` & `talk_codebase-0.1.39/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,19 +47,18 @@
 chunk_size: 500
 
 # Configuration for sampling
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
-# Name of model to use. You can find the list of available models here: https://gpt4all.io/models
 openai_model_name: gpt-3.5-turbo
 # Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
-# Name of local model. If you want to use a local model, you need to specify the name of it.
+# You can find the list of available models here: https://gpt4all.io/models
 local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
 # Path to local model. If you want to use a local model, you need to specify the path to it.
 model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
```

### Comparing `talk_codebase-0.1.38/pyproject.toml` & `talk_codebase-0.1.39/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.38"
+version = "0.1.39"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.38/talk_codebase/cli.py` & `talk_codebase-0.1.39/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.38/talk_codebase/config.py` & `talk_codebase-0.1.39/talk_codebase/config.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.38/talk_codebase/consts.py` & `talk_codebase-0.1.39/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.38/talk_codebase/llm.py` & `talk_codebase-0.1.39/talk_codebase/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 from typing import Optional
 
-import gpt4all
 import questionary
 from halo import Halo
 from langchain import FAISS
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import HuggingFaceEmbeddings, OpenAIEmbeddings
-from langchain.llms import LlamaCpp
+from langchain.llms import GPT4All
 from langchain.schema import HumanMessage, SystemMessage
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 from talk_codebase.consts import MODEL_TYPES
 from talk_codebase.utils import load_files, get_local_vector_store, calculate_cost, StreamStdOut
 
 
@@ -70,19 +69,17 @@
 class LocalLLM(BaseLLM):
 
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = HuggingFaceEmbeddings(model_name='all-MiniLM-L6-v2')
         return self._create_vector_store(embeddings, MODEL_TYPES["LOCAL"], root_dir)
 
     def _create_model(self):
-        gpt4all.GPT4All.retrieve_model(model_name=self.config.get("local_model_name"),
-                                       model_path=self.config.get("model_path"))
-        llm = LlamaCpp(
-            model_path=os.path.join(self.config.get("model_path"), self.config.get("local_model_name")),
-            n_ctx=int(self.config.get("max_tokens")),
+        llm = GPT4All(
+            model=self.config.get("local_model_name"),
+            max_tokens=int(self.config.get("max_tokens")),
             callback_manager=CallbackManager([StreamStdOut()]),
             temp=float(self.config.get("temperature")),
             streaming=True,
             allow_download=True)
         return llm
 
     def send_query(self, query):
```

### Comparing `talk_codebase-0.1.38/talk_codebase/utils.py` & `talk_codebase-0.1.39/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.38/PKG-INFO` & `talk_codebase-0.1.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.38
+Version: 0.1.39
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -74,19 +74,18 @@
 chunk_size: 500
 
 # Configuration for sampling
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
-# Name of model to use. You can find the list of available models here: https://gpt4all.io/models
 openai_model_name: gpt-3.5-turbo
 # Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
-# Name of local model. If you want to use a local model, you need to specify the name of it.
+# You can find the list of available models here: https://gpt4all.io/models
 local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
 # Path to local model. If you want to use a local model, you need to specify the path to it.
 model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
```

