# Comparing `tmp/llm_bot-0.0.3a6.tar.gz` & `tmp/llm_bot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.3a6.tar", max compression
+gzip compressed data, was "llm_bot-0.1.1.tar", max compression
```

## Comparing `llm_bot-0.0.3a6.tar` & `llm_bot-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.3a6/llm_bot/__init__.py
--rw-r--r--   0        0        0    18751 2023-05-18 18:39:18.063063 llm_bot-0.0.3a6/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-05-18 18:39:31.515107 llm_bot-0.0.3a6/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.3a6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.1.1/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.1.1/llm_bot/__init__.py
+-rw-r--r--   0        0        0    22479 2023-07-05 15:16:29.213344 llm_bot-0.1.1/llm_bot/core.py
+-rw-r--r--   0        0        0     1009 2023-07-05 18:53:45.106957 llm_bot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 llm_bot-0.1.1/PKG-INFO
```

### Comparing `llm_bot-0.0.3a6/LICENSE` & `llm_bot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.3a6/llm_bot/core.py` & `llm_bot-0.1.1/llm_bot/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
+from os import getenv
 from pathlib import Path
 import pickle
 import tarfile
 from typing import Dict, List, Tuple, Union
 
 import faiss
 from faiss import IndexFlat
+from langchain.chat_models.azure_openai import AzureChatOpenAI
 from langchain.chat_models.openai import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.schema import BaseMessage, HumanMessage, SystemMessage
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import FAISS
 import requests
@@ -21,21 +23,40 @@
 
 class BaseLLMBot(ABC):
     def __init__(
         self,
         text_chunk_size: int = 1000,
         text_chunk_overlap: int = 250,
         text_separators: List[str] = [" ", ".", ",", ";", ":", "!", "?", "\n"],
+        model_name: str = None,
+        deployment_name: str = None,
         temperature: float = 0,
     ):
-        self._stores: Dict[str, FAISS] = None
-        self._chat = ChatOpenAI(temperature=temperature)
+        self._stores: Dict[str, FAISS] = {}
         self._text_chunk_size = text_chunk_size
         self._text_chunk_overlap = text_chunk_overlap
         self._text_separators = text_separators
+        self._model_name = model_name
+        self._deployment_name = deployment_name
+        self._temperature = temperature
+
+        # Initialize the chat
+        if getenv("OPENAI_API_TYPE") == "azure":
+            if not self._deployment_name:
+                self._deployment_name = ""
+            self._chat = AzureChatOpenAI(
+                temperature=self._temperature,
+                deployment_name=self._deployment_name,
+            )
+        else:
+            if not self._model_name:
+                self._model_name = "gpt-3.5-turbo"
+            self._chat = ChatOpenAI(
+                temperature=self._temperature, model_name=self._model_name
+            )
 
     @abstractmethod
     def train(self, name, *args, **kwargs) -> None:
         """
         Builds the index and the vector store from the given data.
         """
 
@@ -459,9 +480,81 @@
 
         # Add the documents to the index
         if name in self._stores:
             self._stores[name].add_documents(documents=docs)
         else:
             embedding = OpenAIEmbeddings()
             self._stores[name] = FAISS.from_documents(
+                documents=docs, embedding=embedding
+            )
+
+
+class MarkdownBot(BaseLLMBot):
+    def train(self, name: str, documents_path: Union[str, Path]) -> None:
+        """
+        Trains the bot using the given documents.
+
+        Args:
+            name (str): The name of the knowledge base.
+            documents_path (Union[str, Path]): The path to the documents to use for training.
+        """
+        # Import stuff (importing here avoids unnecessary dependencies)
+        from langchain.document_loaders import UnstructuredMarkdownLoader
+
+        # Assert that the path exists
+        documents_path = Path(documents_path)
+        assert documents_path.exists(), f"Path {documents_path} does not exist."
+
+        # Load the knowledge base
+        loaders: List[UnstructuredMarkdownLoader] = []
+        for markdown_file in documents_path.glob("**/*.md"):
+            loaders.append(UnstructuredMarkdownLoader(markdown_file))
+        text_splitter = RecursiveCharacterTextSplitter(
+            chunk_size=self._text_chunk_size,
+            chunk_overlap=self._text_chunk_overlap,
+            separators=self._text_separators,
+        )
+        docs: List[Document] = []
+        for loader in loaders:
+            docs.extend(loader.load_and_split(text_splitter=text_splitter))
+
+        # Create the vector store
+        embedding = OpenAIEmbeddings()
+        self._stores[name] = FAISS.from_documents(documents=docs, embedding=embedding)
+
+    def add_to_index(self, name: str, markdown_files: List[Union[str, Path]]) -> None:
+        """
+        Adds the given HTML files to the index.
+
+        Args:
+            name (str): The name of the knowledge base.
+            markdown_files (List[Union[str, Path]]): The Markdown files to add to the index.
+        """
+        # Import stuff (importing here avoids unnecessary dependencies)
+        from langchain.document_loaders import UnstructuredMarkdownLoader
+
+        # Assert that all files exist
+        markdown_files: List[Path] = [Path(html_file) for html_file in markdown_files]
+        for html_file in markdown_files:
+            assert html_file.exists(), f"File {html_file} does not exist."
+
+        # Load the files
+        loaders: List[UnstructuredMarkdownLoader] = []
+        for html_file in markdown_files:
+            loaders.append(UnstructuredMarkdownLoader(html_file))
+        text_splitter = RecursiveCharacterTextSplitter(
+            chunk_size=self._text_chunk_size,
+            chunk_overlap=self._text_chunk_overlap,
+            separators=self._text_separators,
+        )
+        docs: List[Document] = []
+        for loader in loaders:
+            docs.extend(loader.load_and_split(text_splitter=text_splitter))
+
+        # Add the documents to the index
+        if name in self._stores:
+            self._stores[name].add_documents(documents=docs)
+        else:
+            embedding = OpenAIEmbeddings()
+            self._stores[name] = FAISS.from_documents(
                 documents=docs, embedding=embedding
             )
```

### Comparing `llm_bot-0.0.3a6/pyproject.toml` & `llm_bot-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.3a6"
+version = "0.1.1"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 faiss-cpu = "^1.7.4"
-langchain = "^0.0.150"
+langchain = "^0.0.224"
 openai = "^0.27.4"
 tiktoken = "^0.3.3"
 requests = "^2.29.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pre-commit = "^2.18.1"
@@ -29,10 +29,14 @@
 lint = "scripts.lint:main"
 test = "scripts.test:main"
 
 [tool.poetry.group.html.dependencies]
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
 
+
+[tool.poetry.group.markdown.dependencies]
+unstructured = "^0.7.12"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `llm_bot-0.0.3a6/PKG-INFO` & `llm_bot-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.3a6
+Version: 0.1.1
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
-Requires-Dist: langchain (>=0.0.150,<0.0.151)
+Requires-Dist: langchain (>=0.0.224,<0.0.225)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/prefeitura-rio/chatbot-lab
 Description-Content-Type: text/markdown
 
 # Python Project Template
```

