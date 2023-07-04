# Comparing `tmp/llm_inference-0.0.0.tar.gz` & `tmp/llm_inference-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_inference-0.0.0.tar", last modified: Tue Jul  4 22:12:41 2023, max compression
+gzip compressed data, was "llm_inference-0.0.4.tar", last modified: Tue Jul  4 22:45:07 2023, max compression
```

## Comparing `llm_inference-0.0.0.tar` & `llm_inference-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.509085 llm_inference-0.0.0/
--rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llm_inference-0.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llm_inference-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llm_inference-0.0.0/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)      834 2023-04-17 06:38:34.000000 llm_inference-0.0.0/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)     1892 2023-07-04 22:12:41.509199 llm_inference-0.0.0/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)     1485 2023-07-04 22:06:38.000000 llm_inference-0.0.0/README.md
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.501840 llm_inference-0.0.0/assets/
--rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llm_inference-0.0.0/assets/llama-inference-api-min.png
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.503804 llm_inference-0.0.0/requirements/
--rw-r--r--   0 aniket     (501) staff       (20)      122 2023-04-17 06:38:34.000000 llm_inference-0.0.0/requirements/chatbot.txt
--rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:22:06.000000 llm_inference-0.0.0/requirements/requirements.txt
--rw-r--r--   0 aniket     (501) staff       (20)      539 2023-07-04 22:12:41.509618 llm_inference-0.0.0/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)      369 2023-07-04 00:20:03.000000 llm_inference-0.0.0/setup.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.498928 llm_inference-0.0.0/src/
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.504886 llm_inference-0.0.0/src/chatbot/
--rw-r--r--   0 aniket     (501) staff       (20)       61 2023-07-04 00:20:03.000000 llm_inference-0.0.0/src/chatbot/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     1721 2023-07-04 00:20:03.000000 llm_inference-0.0.0/src/chatbot/base.py
--rw-r--r--   0 aniket     (501) staff       (20)     2227 2023-07-04 00:20:03.000000 llm_inference-0.0.0/src/chatbot/chain.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.506620 llm_inference-0.0.0/src/chatbot/ui/
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-17 07:35:21.000000 llm_inference-0.0.0/src/chatbot/ui/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     1692 2023-04-17 07:35:21.000000 llm_inference-0.0.0/src/chatbot/ui/main.py
--rw-r--r--   0 aniket     (501) staff       (20)     1337 2023-04-17 07:35:21.000000 llm_inference-0.0.0/src/chatbot/ui/templates.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.507620 llm_inference-0.0.0/src/llm_inference/
--rw-r--r--   0 aniket     (501) staff       (20)      116 2023-07-04 22:12:33.000000 llm_inference-0.0.0/src/llm_inference/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     9852 2023-07-04 00:20:03.000000 llm_inference-0.0.0/src/llm_inference/model.py
--rw-r--r--   0 aniket     (501) staff       (20)     1130 2023-07-04 00:20:03.000000 llm_inference-0.0.0/src/llm_inference/serve.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-07-04 22:12:41.508901 llm_inference-0.0.0/src/llm_inference.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)     1892 2023-07-04 22:12:41.000000 llm_inference-0.0.0/src/llm_inference.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      604 2023-07-04 22:12:41.000000 llm_inference-0.0.0/src/llm_inference.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2023-07-04 22:12:41.000000 llm_inference-0.0.0/src/llm_inference.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)      164 2023-07-04 22:12:41.000000 llm_inference-0.0.0/src/llm_inference.egg-info/requires.txt
--rw-r--r--   0 aniket     (501) staff       (20)       22 2023-07-04 22:12:41.000000 llm_inference-0.0.0/src/llm_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-04 22:44:56.000000 llm_inference-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-04 22:44:56.000000 llm_inference-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 22:44:56.000000 llm_inference-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-04 22:44:56.000000 llm_inference-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 22:45:07.874839 llm_inference-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-04 22:44:56.000000 llm_inference-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.870839 llm_inference-0.0.4/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   399922 2023-07-04 22:44:56.000000 llm_inference-0.0.4/assets/llama-inference-api-min.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 22:44:56.000000 llm_inference-0.0.4/requirements/chatbot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 22:44:56.000000 llm_inference-0.0.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-04 22:45:07.878839 llm_inference-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 22:44:56.000000 llm_inference-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.870839 llm_inference-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/chatbot/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/llm_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/llm_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/top_level.txt
```

### Comparing `llm_inference-0.0.0/CODE_OF_CONDUCT.md` & `llm_inference-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/CONTRIBUTING.md` & `llm_inference-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/LICENSE` & `llm_inference-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/MANIFEST.in` & `llm_inference-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/PKG-INFO` & `llm_inference-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_inference
-Version: 0.0.0
+Version: 0.0.4
 Summary: Large Language Models Inference API and Applications
 Home-page: https://github.com/aniketmaurya/llm-inference
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT,Falcon
 Requires-Python: >=3.8
```

### Comparing `llm_inference-0.0.0/README.md` & `llm_inference-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/assets/llama-inference-api-min.png` & `llm_inference-0.0.4/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/setup.cfg` & `llm_inference-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/chatbot/base.py` & `llm_inference-0.0.4/src/chatbot/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 from llm_inference import LLMInference
 
 logger = logging.getLogger(__name__)
 
 
 class DummyLLM(LLM, BaseModel):
-    def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
+    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
         return f"Bot: {prompt}"
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Dummy LLM"
 
 
 class LLaMALLM(LLM, BaseModel):
     checkpoint_dir: str = ""
     model: Any = None
 
-    def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
+    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
         if not self.model:
             self.model = LLMInference(
                 checkpoint_dir=self.checkpoint_dir,
                 precision="bf16-mixed",
             )
 
         return self.model(prompt)
@@ -38,15 +38,15 @@
         """Return type of llm."""
         return "Lit-GPT LLM"
 
 
 class ServerLLM(LLM, BaseModel):
     url: str = ""
 
-    def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
+    def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
         """Run the LLM on the given prompt and input."""
         if self.url == "":
             raise Exception("Server URL not set!")
 
         headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
```

### Comparing `llm_inference-0.0.0/src/chatbot/chain.py` & `llm_inference-0.0.4/src/chatbot/chain.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/chatbot/ui/main.py` & `llm_inference-0.0.4/src/chatbot/ui/main.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/chatbot/ui/templates.py` & `llm_inference-0.0.4/src/chatbot/ui/templates.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/llm_inference/model.py` & `llm_inference-0.0.4/src/llm_inference/model.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/llm_inference/serve.py` & `llm_inference-0.0.4/src/llm_inference/serve.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.0/src/llm_inference.egg-info/PKG-INFO` & `llm_inference-0.0.4/src/llm_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-inference
-Version: 0.0.0
+Version: 0.0.4
 Summary: Large Language Models Inference API and Applications
 Home-page: https://github.com/aniketmaurya/llm-inference
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT,Falcon
 Requires-Python: >=3.8
```

### Comparing `llm_inference-0.0.0/src/llm_inference.egg-info/SOURCES.txt` & `llm_inference-0.0.4/src/llm_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

