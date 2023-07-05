# Comparing `tmp/talk_codebase-0.1.37.tar.gz` & `tmp/talk_codebase-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.37.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.38.tar", max compression
```

## Comparing `talk_codebase-0.1.37.tar` & `talk_codebase-0.1.38.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2874 2023-06-30 15:05:43.638540 talk_codebase-0.1.37/README.md
--rw-r--r--   0        0        0      957 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2898 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/cli.py
--rw-r--r--   0        0        0     1702 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/consts.py
--rw-r--r--   0        0        0     5455 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/utils.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0     3361 2023-07-05 01:55:55.808348 talk_codebase-0.1.38/README.md
+-rw-r--r--   0        0        0      986 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/cli.py
+-rw-r--r--   0        0        0     2250 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/config.py
+-rw-r--r--   0        0        0     1926 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/consts.py
+-rw-r--r--   0        0        0     5629 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-07-05 01:55:55.812348 talk_codebase-0.1.38/talk_codebase/utils.py
+-rw-r--r--   0        0        0     4415 1970-01-01 00:00:00.000000 talk_codebase-0.1.38/PKG-INFO
```

### Comparing `talk_codebase-0.1.37/README.md` & `talk_codebase-0.1.38/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 ## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
+* Simple configuration in just a couple of clicks
 * Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
 * It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
 * Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
 
 To install talk-codebase, you need to have:
 
 * Python 3.9
 * An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
-* (Optional) [GPT4All](https://gpt4all.io) model
 
 ```bash
 # Install talk-codebase
 pip install talk-codebase
 
-# Configure talk-codebase
-talk-codebase configure
-
 # If you want some files to be ignored, add them to .gitignore.
 # Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
 talk-codebase chat .
 ```
 
+## Reset configuration
+```bash
+# If you want to reset the configuration, you can run the following command:
+talk-codebase configure
+```
+
 ## Advanced configuration
 
 You can also edit the configuration manually by editing the `~/.config.yaml` file.
 If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
 the path to the configuration file.
 
 ```yaml
@@ -44,17 +47,22 @@
 chunk_size: 500
 
 # Configuration for sampling
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
-model_name: gpt-3.5-turbo
-model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
+# Name of model to use. You can find the list of available models here: https://gpt4all.io/models
+openai_model_name: gpt-3.5-turbo
+# Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
+# Name of local model. If you want to use a local model, you need to specify the name of it.
+local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
+# Path to local model. If you want to use a local model, you need to specify the path to it.
+model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
```

### Comparing `talk_codebase-0.1.37/pyproject.toml` & `talk_codebase-0.1.38/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.37"
+version = "0.1.38"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain = "^0.0.200"
 fire = "^0.5.0"
 openai = "^0.27.7"
 tiktoken = "^0.4.0"
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
 questionary = "^1.10.0"
-gpt4all = "^0.2.3"
 sentence-transformers = "^2.2.2"
 unstructured = "^0.6.10"
+gpt4all = "^1.0.1"
+langchain = "^0.0.223"
+llama-cpp-python = "^0.1.67"
 
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^68.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `talk_codebase-0.1.37/talk_codebase/cli.py` & `talk_codebase-0.1.38/talk_codebase/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,93 @@
 import os
 
-import fire
+import gpt4all
 import questionary
 import yaml
 
-from talk_codebase.llm import factory_llm
-from talk_codebase.consts import DEFAULT_CONFIG
+from talk_codebase.consts import MODEL_TYPES
 
 config_path = os.path.join(os.path.expanduser("~"), ".talk_codebase_config.yaml")
 
 
 def get_config():
-    print(f"🤖 Loading config from {config_path}:")
     if os.path.exists(config_path):
         with open(config_path, "r") as f:
             config = yaml.safe_load(f)
     else:
         config = {}
     return config
 
 
 def save_config(config):
-    home_dir = os.path.expanduser("~")
     with open(config_path, "w") as f:
         yaml.dump(config, f)
 
 
-def configure():
+def configure_model_name_local(config):
+    if config.get("model_type") != MODEL_TYPES["LOCAL"] or config.get("local_model_name"):
+        return
+
+    list_models = gpt4all.GPT4All.list_models()
+
+    def get_model_info(model):
+        return (
+            f"{model['name']} "
+            f"| {model['filename']} "
+            f"| {model['filesize']} "
+            f"| {model['parameters']} "
+            f"| {model['quant']} "
+            f"| {model['type']}"
+        )
+
+    choices = [
+        {"name": get_model_info(model), "value": model['filename']} for model in list_models
+    ]
+
+    model_name = questionary.select("🤖 Select model name:", choices).ask()
+    config["local_model_name"] = model_name
+    save_config(config)
+    print("🤖 Model name saved!")
+
+
+def configure_api_key(config):
+    if config.get("model_type") != MODEL_TYPES["OPENAI"] or config.get("api_key"):
+        return
+    api_key = input("🤖 Enter your OpenAI API key: ")
+    config["api_key"] = api_key
+    save_config(config)
+    print("🤖 API key saved!")
+
+
+def remove_api_key():
+    config = get_config()
+    config["api_key"] = None
+    save_config(config)
+
+
+def remove_model_type():
     config = get_config()
+    config["model_type"] = None
+    save_config(config)
+
+
+def configure_model_type(config):
+    if config.get("model_type"):
+        return
+
     model_type = questionary.select(
         "🤖 Select model type:",
         choices=[
-            {"name": "OpenAI", "value": "openai"},
-            {"name": "Local", "value": "local"},
+            {"name": "Local", "value": MODEL_TYPES["LOCAL"]},
+            {"name": "OpenAI", "value": MODEL_TYPES["OPENAI"]},
         ]
     ).ask()
     config["model_type"] = model_type
-    if model_type == "openai":
-        api_key = input("🤖 Enter your OpenAI API key: ")
-        model_name = input(f"🤖 Enter your model name (default: {DEFAULT_CONFIG['model_name']}): ")
-        config["model_name"] = model_name if model_name else DEFAULT_CONFIG["model_name"]
-        config["api_key"] = api_key
-    elif model_type == "local":
-        model_path = input(f"🤖 Enter your model path: (default: {DEFAULT_CONFIG['model_path']}) ")
-        config["model_path"] = model_path if model_path else DEFAULT_CONFIG["model_path"]
-    save_config(config)
-    print("🤖 Configuration saved!")
-
-
-def loop(llm):
-    while True:
-        query = input("👉 ").lower().strip()
-        if not query:
-            print("🤖 Please enter a query")
-            continue
-        if query in ('exit', 'quit'):
-            break
-        llm.send_query(query)
-
-
-def validate_config(config):
-    for key, value in DEFAULT_CONFIG.items():
-        if key not in config:
-            config[key] = value
-    if config.get("model_type") == "openai":
-        api_key = config.get("api_key")
-        if not api_key:
-            print("🤖 Please configure your API key. Use talk-codebase configure")
-            exit(0)
-    elif config.get("model_type") == "local":
-        model_path = config.get("model_path")
-        if not model_path:
-            print("🤖 Please configure your model path. Use talk-codebase configure")
-            exit(0)
     save_config(config)
-    return config
-
-
-def chat(root_dir):
-    config = validate_config(get_config())
-    llm = factory_llm(root_dir, config)
-    loop(llm)
-
-
-def main():
-    try:
-        fire.Fire({
-            "chat": chat,
-            "configure": configure
-        })
-    except KeyboardInterrupt:
-        print("\n🤖 Bye!")
-    except Exception as e:
-        if str(e) == "<empty message>":
-            print("🤖 Please configure your API key. Use talk-codebase configure")
-        else:
-            raise e
+    print("🤖 Model type saved!")
 
 
-if __name__ == "__main__":
-    main()
+CONFIGURE_STEPS = [
+    configure_model_type,
+    configure_model_name_local,
+    configure_api_key,
+]
```

### Comparing `talk_codebase-0.1.37/talk_codebase/consts.py` & `talk_codebase-0.1.38/talk_codebase/consts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+import os
+from pathlib import Path
+
 from langchain.document_loaders import CSVLoader, UnstructuredWordDocumentLoader, UnstructuredEPubLoader, \
     PDFMinerLoader, UnstructuredMarkdownLoader, TextLoader
 
 EXCLUDE_DIRS = ['__pycache__', '.venv', '.git', '.idea', 'venv', 'env', 'node_modules', 'dist', 'build', '.vscode',
                 '.github', '.gitlab']
 ALLOW_FILES = ['.txt', '.js', '.mjs', '.ts', '.tsx', '.css', '.scss', '.less', '.html', '.htm', '.json', '.py',
                '.java', '.c', '.cpp', '.cs', '.go', '.php', '.rb', '.rs', '.swift', '.kt', '.scala', '.m', '.h',
                '.sh', '.pl', '.pm', '.lua', '.sql']
 EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
 MODEL_TYPES = {
     "OPENAI": "openai",
     "LOCAL": "local",
 }
+DEFAULT_LOCAL_MODEL = "orca-mini-3b.ggmlv3.q4_0.bin"
+DEFAULT_OPENAI_MODEL = "gpt-3.5-turbo"
+DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all").replace("\\", "\\\\")
+
 DEFAULT_CONFIG = {
     "max_tokens": "2056",
     "chunk_size": "2056",
     "chunk_overlap": "256",
     "k": "1",
-    "model_name": "gpt-3.5-turbo-0613",
-    "model_path": "models/ggml-gpt4all-j-v1.3-groovy.bin",
-    "model_type": MODEL_TYPES["OPENAI"],
     "temperature": "0.7",
+    "openai_model_name": DEFAULT_OPENAI_MODEL,
+    "local_model_name": DEFAULT_LOCAL_MODEL,
+    "model_path": DEFAULT_MODEL_DIRECTORY,
 }
 
 LOADER_MAPPING = {
     ".csv": {
         "loader": CSVLoader,
         "args": {}
     },
```

### Comparing `talk_codebase-0.1.37/talk_codebase/llm.py` & `talk_codebase-0.1.38/talk_codebase/llm.py`

 * *Files 18% similar despite different names*

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
 
 
@@ -33,33 +34,25 @@
     def embedding_search(self, query, k):
         return self.vector_store.search(query, k=k, search_type="similarity")
 
     def _create_vector_store(self, embeddings, index, root_dir):
         index_path = os.path.join(root_dir, f"vector_store/{index}")
         new_db = get_local_vector_store(embeddings, index_path)
         if new_db is not None:
-            approve = questionary.select(
-                f"Found existing vector store. Do you want to use it?",
-                choices=[
-                    {"name": "Yes", "value": True},
-                    {"name": "No", "value": False},
-                ]
-            ).ask()
-            if approve:
-                return new_db
+            return new_db
 
         docs = load_files(root_dir)
         if len(docs) == 0:
             print("✘ No documents found")
             exit(0)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=int(self.config.get("chunk_size")),
                                                        chunk_overlap=int(self.config.get("chunk_overlap")))
         texts = text_splitter.split_documents(docs)
         if index == MODEL_TYPES["OPENAI"]:
-            cost = calculate_cost(docs, self.config.get("model_name"))
+            cost = calculate_cost(docs, self.config.get("openai_model_name"))
             approve = questionary.select(
                 f"Creating a vector store will cost ~${cost:.5f}. Do you want to continue?",
                 choices=[
                     {"name": "Yes", "value": True},
                     {"name": "No", "value": False},
                 ]
             ).ask()
@@ -77,24 +70,39 @@
 class LocalLLM(BaseLLM):
 
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = HuggingFaceEmbeddings(model_name='all-MiniLM-L6-v2')
         return self._create_vector_store(embeddings, MODEL_TYPES["LOCAL"], root_dir)
 
     def _create_model(self):
-        llm = GPT4All(model=self.config.get("model_path"), n_ctx=int(self.config.get("max_tokens")), streaming=True)
+        gpt4all.GPT4All.retrieve_model(model_name=self.config.get("local_model_name"),
+                                       model_path=self.config.get("model_path"))
+        llm = LlamaCpp(
+            model_path=os.path.join(self.config.get("model_path"), self.config.get("local_model_name")),
+            n_ctx=int(self.config.get("max_tokens")),
+            callback_manager=CallbackManager([StreamStdOut()]),
+            temp=float(self.config.get("temperature")),
+            streaming=True,
+            allow_download=True)
         return llm
 
     def send_query(self, query):
         k = self.config.get("k")
         docs = self.embedding_search(query, k=int(k))
 
         content = "\n".join([f"content: \n```{s.page_content}```" for s in docs])
-        template = "Given the following content, your task is to answer the question.\nQuestion: {question}\n{content}"
+        template = """
+### System:
+Given the following content, your task is to answer the question. {content}
+
+### User:
+{question}
 
+### Response:
+        """
         prompt = PromptTemplate(template=template, input_variables=["content", "question"]).partial(content=content)
         llm_chain = LLMChain(prompt=prompt, llm=self.llm)
 
         llm_chain.run(query)
 
         file_paths = [os.path.abspath(s.metadata["source"]) for s in docs]
         print('\n'.join([f'📄 {file_path}:' for file_path in file_paths]))
@@ -102,15 +110,15 @@
 
 class OpenAILLM(BaseLLM):
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = OpenAIEmbeddings(openai_api_key=self.config.get("api_key"))
         return self._create_vector_store(embeddings, MODEL_TYPES["OPENAI"], root_dir)
 
     def _create_model(self):
-        return ChatOpenAI(model_name=self.config.get("model_name"),
+        return ChatOpenAI(model_name=self.config.get("openai_model_name"),
                           openai_api_key=self.config.get("api_key"),
                           streaming=True,
                           max_tokens=int(self.config.get("max_tokens")),
                           callback_manager=CallbackManager([StreamStdOut()]),
                           temperature=float(self.config.get("temperature")))
 
     def send_query(self, query):
```

### Comparing `talk_codebase-0.1.37/talk_codebase/utils.py` & `talk_codebase-0.1.38/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.37/PKG-INFO` & `talk_codebase-0.1.38/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.37
+Version: 0.1.38
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: gpt4all (>=0.2.3,<0.3.0)
+Requires-Dist: gpt4all (>=1.0.1,<2.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
-Requires-Dist: langchain (>=0.0.200,<0.0.201)
+Requires-Dist: langchain (>=0.0.223,<0.0.224)
+Requires-Dist: llama-cpp-python (>=0.1.67,<0.2.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
 ## talk-codebase 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
+* Simple configuration in just a couple of clicks
 * Talk-codebase is a tool that allows you to converse with your codebase using LLMs (Large Language Models) to answer your queries.
 * It supports offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or you can use OpenAI if privacy is not a concern for you.
 * Talk-codebase is still under development, but it is a tool that can help you to improve your code. It is only recommended for educational purposes and not for production use.
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Installation
 
 To install talk-codebase, you need to have:
 
 * Python 3.9
 * An OpenAI API [api-keys](https://platform.openai.com/account/api-keys)
-* (Optional) [GPT4All](https://gpt4all.io) model
 
 ```bash
 # Install talk-codebase
 pip install talk-codebase
 
-# Configure talk-codebase
-talk-codebase configure
-
 # If you want some files to be ignored, add them to .gitignore.
 # Once `talk-codebase` is installed, you can use it to chat with your codebase in the current directory by running the following command:
 talk-codebase chat .
 ```
 
+## Reset configuration
+```bash
+# If you want to reset the configuration, you can run the following command:
+talk-codebase configure
+```
+
 ## Advanced configuration
 
 You can also edit the configuration manually by editing the `~/.config.yaml` file.
 If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
 the path to the configuration file.
 
 ```yaml
@@ -70,17 +74,22 @@
 chunk_size: 500
 
 # Configuration for sampling
 k: 4
 max_tokens: 1048
 
 # Configuration for the LLM model
-model_name: gpt-3.5-turbo
-model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
+# Name of model to use. You can find the list of available models here: https://gpt4all.io/models
+openai_model_name: gpt-3.5-turbo
+# Type of model to use. You can choose between `openai` and `local`.
 model_type: openai
+# Name of local model. If you want to use a local model, you need to specify the name of it.
+local_model_name: orca-mini-7b.ggmlv3.q4_0.bin
+# Path to local model. If you want to use a local model, you need to specify the path to it.
+model_path: 'absolute path to local model'
 ```
 
 ## Supports the following extensions:
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
```

