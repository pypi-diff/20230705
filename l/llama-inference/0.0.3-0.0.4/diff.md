# Comparing `tmp/llama_inference-0.0.3.tar.gz` & `tmp/llama_inference-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_inference-0.0.3.tar", last modified: Mon Apr 17 10:34:22 2023, max compression
+gzip compressed data, was "llama_inference-0.0.4.tar", last modified: Tue Jul  4 21:58:52 2023, max compression
```

## Comparing `llama_inference-0.0.3.tar` & `llama_inference-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.923315 llama_inference-0.0.3/
--rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.3/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)      834 2023-04-17 06:38:34.000000 llama_inference-0.0.3/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)     1934 2023-04-17 10:34:22.923465 llama_inference-0.0.3/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)     1579 2023-04-17 07:35:21.000000 llama_inference-0.0.3/README.md
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.916378 llama_inference-0.0.3/assets/
--rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.3/assets/llama-inference-api-min.png
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.918709 llama_inference-0.0.3/requirements/
--rw-r--r--   0 aniket     (501) staff       (20)      122 2023-04-17 06:38:34.000000 llama_inference-0.0.3/requirements/chatbot.txt
--rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:22:06.000000 llama_inference-0.0.3/requirements/requirements.txt
--rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-17 10:34:22.923949 llama_inference-0.0.3/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)      314 2023-04-17 06:38:34.000000 llama_inference-0.0.3/setup.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.914654 llama_inference-0.0.3/src/
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.919593 llama_inference-0.0.3/src/chatbot/
--rw-r--r--   0 aniket     (501) staff       (20)       47 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     1803 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/base.py
--rw-r--r--   0 aniket     (501) staff       (20)     2296 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/chain.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.920292 llama_inference-0.0.3/src/chatbot/ui/
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     1692 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/main.py
--rw-r--r--   0 aniket     (501) staff       (20)     1337 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/templates.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.921470 llama_inference-0.0.3/src/llama_inference/
--rw-r--r--   0 aniket     (501) staff       (20)      118 2023-04-17 10:34:09.000000 llama_inference-0.0.3/src/llama_inference/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     4968 2023-04-17 06:38:34.000000 llama_inference-0.0.3/src/llama_inference/model.py
--rw-r--r--   0 aniket     (501) staff       (20)     1136 2023-04-17 06:38:34.000000 llama_inference-0.0.3/src/llama_inference/serve.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.922861 llama_inference-0.0.3/src/llama_inference.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)     1934 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      620 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/requires.txt
--rw-r--r--   0 aniket     (501) staff       (20)       35 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/top_level.txt
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.522865 llama_inference-0.0.4/
+-rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.4/LICENSE
+-rw-r--r--   0 aniket     (501) staff       (20)      834 2023-04-17 06:38:34.000000 llama_inference-0.0.4/MANIFEST.in
+-rw-r--r--   0 aniket     (501) staff       (20)     1905 2023-07-04 21:58:52.522962 llama_inference-0.0.4/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)     1502 2023-07-04 00:20:03.000000 llama_inference-0.0.4/README.md
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.517250 llama_inference-0.0.4/assets/
+-rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.4/assets/llama-inference-api-min.png
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.519130 llama_inference-0.0.4/requirements/
+-rw-r--r--   0 aniket     (501) staff       (20)      122 2023-04-17 06:38:34.000000 llama_inference-0.0.4/requirements/chatbot.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:22:06.000000 llama_inference-0.0.4/requirements/requirements.txt
+-rw-r--r--   0 aniket     (501) staff       (20)      534 2023-07-04 21:58:52.523338 llama_inference-0.0.4/setup.cfg
+-rw-r--r--   0 aniket     (501) staff       (20)      369 2023-07-04 00:20:03.000000 llama_inference-0.0.4/setup.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.514922 llama_inference-0.0.4/src/
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.519768 llama_inference-0.0.4/src/chatbot/
+-rw-r--r--   0 aniket     (501) staff       (20)       61 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/chatbot/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1721 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/chatbot/base.py
+-rw-r--r--   0 aniket     (501) staff       (20)     2227 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/chatbot/chain.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.520594 llama_inference-0.0.4/src/chatbot/ui/
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-17 07:35:21.000000 llama_inference-0.0.4/src/chatbot/ui/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1692 2023-04-17 07:35:21.000000 llama_inference-0.0.4/src/chatbot/ui/main.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1337 2023-04-17 07:35:21.000000 llama_inference-0.0.4/src/chatbot/ui/templates.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.522068 llama_inference-0.0.4/src/llama_inference.egg-info/
+-rw-r--r--   0 aniket     (501) staff       (20)     1905 2023-07-04 21:58:52.000000 llama_inference-0.0.4/src/llama_inference.egg-info/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      614 2023-07-04 21:58:52.000000 llama_inference-0.0.4/src/llama_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        1 2023-07-04 21:58:52.000000 llama_inference-0.0.4/src/llama_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 aniket     (501) staff       (20)      164 2023-07-04 21:58:52.000000 llama_inference-0.0.4/src/llama_inference.egg-info/requires.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       22 2023-07-04 21:58:52.000000 llama_inference-0.0.4/src/llama_inference.egg-info/top_level.txt
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 21:58:52.522703 llama_inference-0.0.4/src/llm_inference/
+-rw-r--r--   0 aniket     (501) staff       (20)      116 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/llm_inference/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     9852 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/llm_inference/model.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1130 2023-07-04 00:20:03.000000 llama_inference-0.0.4/src/llm_inference/serve.py
```

### Comparing `llama_inference-0.0.3/CODE_OF_CONDUCT.md` & `llama_inference-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/CONTRIBUTING.md` & `llama_inference-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/LICENSE` & `llama_inference-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/MANIFEST.in` & `llama_inference-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/assets/llama-inference-api-min.png` & `llama_inference-0.0.4/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/setup.cfg` & `llama_inference-0.0.4/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = llama_inference
-version = attr: llama_inference.__version__
+version = attr: llm_inference.__version__
 author = Aniket Maurya
 author_email = theaniketmaurya@gmail.com
-description = Inference API for LLaMA
+description = Large Language Models Inference API and Chatbot
 description-file = README.md
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 url = https://github.com/aniketmaurya/LLaMA-inference-api
 license = Apache License 2.0
 keywords = LLM, LLaMA, GPT
```

### Comparing `llama_inference-0.0.3/src/chatbot/base.py` & `llama_inference-0.0.4/src/chatbot/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any, List, Optional
 
 import requests
 from langchain.llms.base import LLM
 from pydantic import BaseModel
 
-from llama_inference import LLaMAInference
+from llm_inference import LLMInference
 
 logger = logging.getLogger(__name__)
 
 
 class DummyLLM(LLM, BaseModel):
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         return f"Bot: {prompt}"
@@ -17,32 +17,30 @@
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Dummy LLM"
 
 
 class LLaMALLM(LLM, BaseModel):
-    checkpoint_path: str = ""
-    tokenizer_path: str = ""
+    checkpoint_dir: str = ""
     model: Any = None
 
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         if not self.model:
-            self.model = LLaMAInference(
-                checkpoint_path=self.checkpoint_path,
-                tokenizer_path=self.tokenizer_path,
-                dtype="bfloat16",
+            self.model = LLMInference(
+                checkpoint_dir=self.checkpoint_dir,
+                precision="bf16-mixed",
             )
 
         return self.model(prompt)
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
-        return "LLaMA LLM"
+        return "Lit-GPT LLM"
 
 
 class ServerLLM(LLM, BaseModel):
     url: str = ""
 
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         """Run the LLM on the given prompt and input."""
```

### Comparing `llama_inference-0.0.3/src/chatbot/chain.py` & `llama_inference-0.0.4/src/chatbot/chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,12 +68,10 @@
         self, url: str, input_key="input", output_key="response", verbose=False
     ) -> None:
         llm = ServerLLM(url=url)
         super().__init__(llm, input_key, output_key, verbose)
 
 
 class LLaMAChatBot(BaseChatBot):
-    def __init__(
-        self, checkpoint_path: str, tokenizer_path: str, verbose=False
-    ) -> None:
-        llm = LLaMALLM(checkpoint_path=checkpoint_path, tokenizer_path=tokenizer_path)
+    def __init__(self, checkpoint_dir: str, verbose=False) -> None:
+        llm = LLaMALLM(checkpoint_dir=checkpoint_dir)
         super().__init__(llm=llm, verbose=verbose)
```

### Comparing `llama_inference-0.0.3/src/chatbot/ui/main.py` & `llama_inference-0.0.4/src/chatbot/ui/main.py`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/src/chatbot/ui/templates.py` & `llama_inference-0.0.4/src/chatbot/ui/templates.py`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.3/src/llama_inference/serve.py` & `llama_inference-0.0.4/src/llm_inference/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 
 import lightning as L
 from lightning.app.components import PythonServer
 from pydantic import BaseModel
 
-from llama_inference.model import LLaMAInference
+from llm_inference.model import LLMInference
 
 
 class PromptRequest(BaseModel):
     prompt: str
 
 
 class Response(BaseModel):
@@ -24,15 +24,15 @@
         tokenizer_path: str = None,
     ):
         super().__init__(input_type, output_type)
         self.checkpoint_path = checkpoint_path
         self.tokenizer_path = tokenizer_path
 
     def setup(self, *args: Any, **kwargs: Any) -> None:
-        self._model = LLaMAInference(
+        self._model = LLMInference(
             checkpoint_path=self.checkpoint_path,
             tokenizer_path=self.tokenizer_path,
             dtype="bfloat16",
         )
 
     def predict(self, request: PromptRequest) -> Any:
         result = self._model(request.prompt)
```

### Comparing `llama_inference-0.0.3/src/llama_inference.egg-info/SOURCES.txt` & `llama_inference-0.0.4/src/llama_inference.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requirements/requirements.txt
 src/chatbot/__init__.py
 src/chatbot/base.py
 src/chatbot/chain.py
 src/chatbot/ui/__init__.py
 src/chatbot/ui/main.py
 src/chatbot/ui/templates.py
-src/llama_inference/__init__.py
-src/llama_inference/model.py
-src/llama_inference/serve.py
 src/llama_inference.egg-info/PKG-INFO
 src/llama_inference.egg-info/SOURCES.txt
 src/llama_inference.egg-info/dependency_links.txt
 src/llama_inference.egg-info/requires.txt
-src/llama_inference.egg-info/top_level.txt
+src/llama_inference.egg-info/top_level.txt
+src/llm_inference/__init__.py
+src/llm_inference/model.py
+src/llm_inference/serve.py
```

