# Comparing `tmp/kanu-0.8.0.tar.gz` & `tmp/kanu-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.8.0.tar", last modified: Mon Jun 26 05:37:07 2023, max compression
+gzip compressed data, was "kanu-0.9.0.tar", last modified: Wed Jul  5 06:49:05 2023, max compression
```

## Comparing `kanu-0.8.0.tar` & `kanu-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.558762 kanu-0.8.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-26 05:36:52.000000 kanu-0.8.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)     2480 2023-06-26 05:37:07.558601 kanu-0.8.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)     2164 2023-06-26 05:36:52.000000 kanu-0.8.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.557714 kanu-0.8.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)    16190 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     2083 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)    10390 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     3691 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/funcgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)    13066 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/gui.py
--rw-r--r--   0 sbslee     (501) staff       (20)      999 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.558408 kanu-0.8.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)     2480 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      292 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-26 05:37:07.558816 kanu-0.8.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-26 05:36:52.000000 kanu-0.8.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-07-05 06:49:05.929316 kanu-0.9.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-07-05 06:48:39.000000 kanu-0.9.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)     5477 2023-07-05 06:49:05.929162 kanu-0.9.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)     5161 2023-07-05 06:48:39.000000 kanu-0.9.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-07-05 06:49:05.928323 kanu-0.9.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    18751 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     2464 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     1274 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/chatpalm.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     1510 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/constants.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    10746 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     4129 2023-07-05 06:48:39.000000 kanu-0.9.0/kanu/funcgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    13163 2023-07-05 06:48:40.000000 kanu-0.9.0/kanu/gui.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      999 2023-07-05 06:48:40.000000 kanu-0.9.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-07-05 06:48:40.000000 kanu-0.9.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-07-05 06:49:05.928977 kanu-0.9.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)     5477 2023-07-05 06:49:05.000000 kanu-0.9.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      327 2023-07-05 06:49:05.000000 kanu-0.9.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-07-05 06:49:05.000000 kanu-0.9.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-07-05 06:49:05.000000 kanu-0.9.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-07-05 06:49:05.000000 kanu-0.9.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-07-05 06:49:05.929367 kanu-0.9.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-07-05 06:48:40.000000 kanu-0.9.0/setup.py
```

### Comparing `kanu-0.8.0/LICENSE` & `kanu-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.8.0/kanu/__main__.py` & `kanu-0.9.0/kanu/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,23 @@
 import configparser
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog
 import importlib.util
 
+from . import constants
 from .version import __version__
 from .gui import Tooltip
 
-GPT_MODELS = [
-    "gpt-3.5-turbo",
-    "gpt-3.5-turbo-0613",
-    "gpt-3.5-turbo-16k",
-    "gpt-3.5-turbo-16k-0613",
-    "gpt-4",
-    "gpt-4-0613",
-    "gpt-4-32k",
-    "gpt-4-32k-0613",
-]
-CHATGPT_PROMPT = """You are a helpful assistant."""
-DOCGPT_PROMPT = """Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
-
-{context}
-
-Question: {question}
-Helpful Answer:"""
-FUNCGPT_PROMPT = """You are a helpful assistant."""
-FUNCGPT_EXAMPLE = """import json
-
-def get_current_weather(location, unit="fahrenheit"):
-    weather_info = {
-        "location": location,
-        "temperature": "72",
-        "unit": unit,
-        "forecast": ["sunny", "windy"],
-    }
-    return json.dumps(weather_info)
-
-get_current_weather_json = {
-    "name": "get_current_weather",
-    "description": "Get the current weather in a given location",
-    "parameters": {
-        "type": "object",
-        "properties": {
-            "location": {
-                "type": "string",
-                "description": "The city and state, e.g. San Francisco, CA",
-            },
-            "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
-        },
-        "required": ["location"],
-    },
-}
-
-functions = {
-    "get_current_weather": {
-        "function": get_current_weather,
-        "json": get_current_weather_json,
-    }
-}"""
-
 class KANU:
     def __init__(self, root):
         self.container = None
         self.root = root
         self.root.title(f"KANU ({__version__})")
-        self.root.geometry("700x620")
+        self.root.geometry("700x640")
         self.homepage()
 
     def homepage(self):
         if self.container is not None:
             self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
@@ -76,14 +25,16 @@
         l.pack()
         b = tk.Button(self.container, text="ChatGPT", command=lambda: self.config_chatgpt())
         b.pack()
         b = tk.Button(self.container, text="DocGPT", command=lambda: self.config_docgpt())
         b.pack()
         b = tk.Button(self.container, text="FuncGPT", command=lambda: self.config_funcgpt())
         b.pack()
+        b = tk.Button(self.container, text="ChatPaLM", command=lambda: self.config_chatpalm())
+        b.pack()
 
     def config_chatgpt(self):
         self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="ChatGPT")
         l.grid(row=0, column=0, columnspan=2)
@@ -97,27 +48,27 @@
         b = tk.Button(self.container, text="Template", command=self.template_chatgpt_config)
         b.grid(row=4, column=1)
         m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
         m.grid(row=5, column=0, columnspan=2)
         l = tk.Label(self.container, text="Model:")
         l.grid(row=6, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
-        om = ttk.OptionMenu(self.container, self.model, *GPT_MODELS)
+        om = ttk.OptionMenu(self.container, self.model, *constants.GPT_MODELS)
         om.grid(row=7, column=0, columnspan=2)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
         l.grid(row=8, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
-        self.prompt.insert("1.0", CHATGPT_PROMPT)
+        self.prompt.insert("1.0", constants.CHATGPT_PROMPT)
         self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
         sb.grid(row=9, column=2, sticky="ns")
         self.prompt["yscrollcommand"] = sb.set
         l = tk.Label(self.container, text="Temperature ⓘ:")
-        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 2, with 0 indicating almost deterministic behavior.")
         l.grid(row=10, column=0, columnspan=2)
         self.temperature = tk.DoubleVar(self.container, value=0.5)
         e = tk.Entry(self.container, textvariable=self.temperature)
         e.grid(row=11, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
         l.grid(row=12, column=0, columnspan=2)
         e = tk.Entry(self.container)
@@ -136,71 +87,72 @@
         self.deploy_agent("ChatGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
 
     def template_chatgpt_config(self):
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return
         config = configparser.ConfigParser()
-        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": CHATGPT_PROMPT}
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": constants.CHATGPT_PROMPT}
         config["USER"] = {"openai_key": ""}
         with open(file_path, "w") as f:
             config.write(f)
 
     def config_docgpt(self):
         self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=2)
         l = tk.Label(self.container, text="Required packages:")
         l.grid(row=1, column=0, columnspan=2)
-        self.display_required_dependency(2, "langchain")
-        self.display_required_dependency(3, "chromadb")
-        self.display_required_dependency(4, "tiktoken")
+        self.display_required_dependency(2, "openai")
+        self.display_required_dependency(3, "langchain")
+        self.display_required_dependency(4, "chromadb")
+        self.display_required_dependency(5, "tiktoken")
         l = tk.Label(self.container, text="Optional packages:")
-        l.grid(row=5, column=0, columnspan=2)        
-        self.display_optional_dependency(6, "pdfminer.six", "pdfminer", "Required for .pdf documents.")
-        self.display_optional_dependency(7, "unstructured", "unstructured", "Required for .doc and .docx documents.")
-        self.display_optional_dependency(8, "tabulate", "tabulate", "Required for .doc and .docx documents.")
+        l.grid(row=6, column=0, columnspan=2)        
+        self.display_optional_dependency(7, "pdfminer.six", "pdfminer", "Required for .pdf documents.")
+        self.display_optional_dependency(8, "unstructured", "unstructured", "Required for .doc and .docx documents.")
+        self.display_optional_dependency(9, "tabulate", "tabulate", "Required for .doc and .docx documents.")
         m = tk.Message(self.container, width=300, text="Option 1. Upload a configuration file")
-        m.grid(row=9, column=0, columnspan=2)
+        m.grid(row=10, column=0, columnspan=2)
         b = tk.Button(self.container, text="Browse", command=self.parse_docgpt_config)
-        b.grid(row=10, column=0)
+        b.grid(row=11, column=0)
         b = tk.Button(self.container, text="Template", command=self.template_docgpt_config)
-        b.grid(row=10, column=1)
+        b.grid(row=11, column=1)
         m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
-        m.grid(row=11, column=0, columnspan=2)
+        m.grid(row=12, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
         l = tk.Label(self.container, text="Model:")
-        l.grid(row=12, column=0, columnspan=2)
-        om = ttk.OptionMenu(self.container, self.model, *GPT_MODELS)
-        om.grid(row=13, column=0, columnspan=2)
+        l.grid(row=13, column=0, columnspan=2)
+        om = ttk.OptionMenu(self.container, self.model, *constants.GPT_MODELS)
+        om.grid(row=14, column=0, columnspan=2)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
-        l.grid(row=14, column=0, columnspan=2)
+        l.grid(row=15, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
-        self.prompt.insert("1.0", DOCGPT_PROMPT)
-        self.prompt.grid(row=15, column=0, columnspan=2, sticky="nsew")
-        sb.grid(row=15, column=2, sticky="ns")
+        self.prompt.insert("1.0", constants.DOCGPT_PROMPT)
+        self.prompt.grid(row=16, column=0, columnspan=2, sticky="nsew")
+        sb.grid(row=16, column=2, sticky="ns")
         self.prompt["yscrollcommand"] = sb.set
         l = tk.Label(self.container, text="Temperature ⓘ:")
-        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
-        l.grid(row=16, column=0, columnspan=2)
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 2, with 0 indicating almost deterministic behavior.")
+        l.grid(row=17, column=0, columnspan=2)
         self.temperature = tk.DoubleVar(self.container, value=0.5)
         e = tk.Entry(self.container, textvariable=self.temperature)
-        e.grid(row=17, column=0, columnspan=2)
+        e.grid(row=18, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
-        l.grid(row=18, column=0, columnspan=2)
+        l.grid(row=19, column=0, columnspan=2)
         e = tk.Entry(self.container)
-        e.grid(row=19, column=0, columnspan=2)
+        e.grid(row=20, column=0, columnspan=2)
         b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("DocGPT", e.get(), self.model.get(), self.prompt.get("1.0", "end-1c"), self.temperature.get(), 1000, 50))
-        b.grid(row=20, column=0)
+        b.grid(row=21, column=0)
         b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
-        b.grid(row=20, column=1)
+        b.grid(row=21, column=1)
 
     def parse_docgpt_config(self):
         config = configparser.ConfigParser()
         file_path = filedialog.askopenfilename()
         if not file_path:
             return
         config.read(file_path)
@@ -218,15 +170,15 @@
         )
 
     def template_docgpt_config(self):
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return
         config = configparser.ConfigParser()
-        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT, "chunk_size": 1000, "chunk_overlap": 50}
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": constants.DOCGPT_PROMPT, "chunk_size": 1000, "chunk_overlap": 50}
         config["USER"] = {"openai_key": ""}
         config["OPTIONAL"] = {"new_database_directory": "", "document_directory": "", "existing_database_directory": ""}
         with open(file_path, "w") as f:
             config.write(f)
 
     def config_funcgpt(self):
         self.container.pack_forget()
@@ -244,33 +196,33 @@
         b = tk.Button(self.container, text="Template", command=self.template_funcgpt_config)
         b.grid(row=4, column=1)
         m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
         m.grid(row=5, column=0, columnspan=2)
         l = tk.Label(self.container, text="Model:")
         l.grid(row=6, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo-0613")
-        om = ttk.OptionMenu(self.container, self.model, "gpt-3.5-turbo-0613", *GPT_MODELS)
+        om = ttk.OptionMenu(self.container, self.model, "gpt-3.5-turbo-0613", *constants.GPT_MODELS)
         om.grid(row=7, column=0, columnspan=2)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
         l.grid(row=8, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
-        self.prompt.insert("1.0", FUNCGPT_PROMPT)
+        self.prompt.insert("1.0", constants.FUNCGPT_PROMPT)
         self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
         sb.grid(row=9, column=2, sticky="ns")
         self.prompt["yscrollcommand"] = sb.set
         l = tk.Label(self.container, text="Function script:")
         l.grid(row=10, column=0, columnspan=2)
         b = tk.Button(self.container, text="Browse", command=self.get_function_script)
         b.grid(row=11, column=0)
         b = tk.Button(self.container, text="Example", command=self.example_function_script)
         b.grid(row=11, column=1)
         l = tk.Label(self.container, text="Temperature ⓘ:")
-        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 2, with 0 indicating almost deterministic behavior.")
         l.grid(row=12, column=0, columnspan=2)
         self.temperature = tk.DoubleVar(self.container, value=0.5)
         e = tk.Entry(self.container, textvariable=self.temperature)
         e.grid(row=13, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
         l.grid(row=14, column=0, columnspan=2)
         e = tk.Entry(self.container)
@@ -289,15 +241,15 @@
         self.deploy_agent("FuncGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"], config["USER"]["function_script"])
 
     def template_funcgpt_config(self):
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return
         config = configparser.ConfigParser()
-        config["DEFAULT"] = {"model": "gpt-3.5-turbo-0613", "temperature": "0.5", "prompt": FUNCGPT_PROMPT}
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo-0613", "temperature": "0.5", "prompt": constants.FUNCGPT_PROMPT}
         config["USER"] = {"openai_key": "", "function_script": ""}
         with open(file_path, "w") as f:
             config.write(f)
 
     def get_function_script(self):
         file_path = filedialog.askopenfilename()
         if not file_path:
@@ -305,29 +257,97 @@
         self.script = file_path
 
     def example_function_script(self):
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return       
         with open(file_path, "w") as f:
-            f.write(FUNCGPT_EXAMPLE)
+            f.write(constants.FUNCGPT_EXAMPLE)
+
+    def config_chatpalm(self):
+        self.container.pack_forget()
+        self.container = tk.Frame(self.root)
+        self.container.pack()
+        l = tk.Label(self.container, text="ChatPaLM")
+        l.grid(row=0, column=0, columnspan=2)
+        l = tk.Label(self.container, text="Required packages:")
+        l.grid(row=1, column=0, columnspan=2)
+        self.display_required_dependency(2, "google.generativeai")
+        m = tk.Message(self.container, width=300, text="Option 1. Upload a configuration file")
+        m.grid(row=3, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Browse", command=self.parse_chatpalm_config)
+        b.grid(row=4, column=0)
+        b = tk.Button(self.container, text="Template", command=self.template_chatpalm_config)
+        b.grid(row=4, column=1)
+        m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
+        m.grid(row=5, column=0, columnspan=2)
+        l = tk.Label(self.container, text="Model:")
+        l.grid(row=6, column=0, columnspan=2)
+        self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
+        om = ttk.OptionMenu(self.container, self.model, *constants.PaLM_MODELS)
+        om.grid(row=7, column=0, columnspan=2)
+        l = tk.Label(self.container, text="System message ⓘ:")
+        Tooltip(l, "The system message helps set the behavior of the chatbot.")
+        l.grid(row=8, column=0, columnspan=2)
+        self.prompt = tk.Text(self.container, height=9, width=42)
+        sb = tk.Scrollbar(self.container, command=self.prompt.yview)
+        self.prompt.insert("1.0", constants.CHATPALM_PROMPT)
+        self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
+        sb.grid(row=9, column=2, sticky="ns")
+        self.prompt["yscrollcommand"] = sb.set
+        l = tk.Label(self.container, text="Temperature ⓘ:")
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 2, with 0 indicating almost deterministic behavior.")
+        l.grid(row=10, column=0, columnspan=2)
+        self.temperature = tk.DoubleVar(self.container, value=0.5)
+        e = tk.Entry(self.container, textvariable=self.temperature)
+        e.grid(row=11, column=0, columnspan=2)
+        l = tk.Label(self.container, text="PaLM API key:")
+        l.grid(row=12, column=0, columnspan=2)
+        e = tk.Entry(self.container)
+        e.grid(row=13, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("ChatPaLM", e.get(), self.model.get(), self.temperature.get(), self.prompt.get("1.0", "end-1c")))
+        b.grid(row=14, column=0)
+        b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
+        b.grid(row=14, column=1)
+
+    def parse_chatpalm_config(self):
+        config = configparser.ConfigParser()
+        file_path = filedialog.askopenfilename()
+        if not file_path:
+            return
+        config.read(file_path)
+        self.deploy_agent("ChatPaLM", config["USER"]["google_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
+
+    def template_chatpalm_config(self):
+        file_path = filedialog.asksaveasfilename()
+        if not file_path:
+            return
+        config = configparser.ConfigParser()
+        config["DEFAULT"] = {"model": "chat-bison-001", "temperature": "0.5", "prompt": constants.CHATPALM_PROMPT}
+        config["USER"] = {"google_key": ""}
+        with open(file_path, "w") as f:
+            config.write(f)
 
     def deploy_agent(self, agent, *args, **kwargs):
         if agent == "ChatGPT":
             from .chatgpt import ChatGPT
             chatgpt = ChatGPT(self, *args, **kwargs)
             chatgpt.run()
         elif agent == "DocGPT":
             from .docgpt import DocGPT
             docgpt = DocGPT(self, *args, **kwargs)
             docgpt.run()
         elif agent == "FuncGPT":
             from .funcgpt import FuncGPT
             docgpt = FuncGPT(self, *args, **kwargs)
             docgpt.run()
+        elif agent == "ChatPaLM":
+            from .chatpalm import ChatPaLM
+            docgpt = ChatPaLM(self, *args, **kwargs)
+            docgpt.run()
         else:
             raise ValueError(f"Unknown agent {agent}")
         
     def display_required_dependency(self, row, package_name):
         l = tk.Label(self.container, text=package_name)
         l.grid(row=row, column=0)
         l = tk.Label(self.container, text="❌" if importlib.util.find_spec(package_name) is None else "✅")
```

### Comparing `kanu-0.8.0/kanu/chatgpt.py` & `kanu-0.9.0/kanu/chatgpt.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,25 +20,33 @@
     def run(self):
         self.conversation.page()
 
     def send_message(self):
         if not self.messages:
             self.messages.append({"role": "system", "content": self.prompt})
         self.messages += [{"role": "user", "content": self.user_input.get()}]
-        bot_response = openai.ChatCompletion.create(
-            model=self.model,
-            messages=self.messages,
-            temperature=self.temperature,
-        )
-        response = bot_response["choices"][0]["message"]["content"]
-        self.messages += [{"role": "assistant", "content": response}]
-        self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
-        self.session.insert(tk.END, f"Bot: " + response + "\n", "bot")
-        self.calculate_usage(bot_response)
-        self.chatbox.delete(0, tk.END)
+        try: 
+            response = openai.ChatCompletion.create(
+                model=self.model,
+                messages=self.messages,
+                temperature=self.temperature,
+            )
+            answer = response["choices"][0]["message"]["content"]
+            self.messages += [{"role": "assistant", "content": answer}]
+            self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
+            self.session.insert(tk.END, f"Bot: " + answer + "\n", "bot")
+            self.calculate_usage(response)
+            self.chatbox.delete(0, tk.END)
+        except openai.error.InvalidRequestError as e:
+            error = str(e)
+            if "Please reduce the length of the messages." in error:
+                self.system.insert(tk.END, f"System: {error} You can also create a new chat session.\n", "system")
+                self.messages.pop()
+            else:
+                raise
 
     def calculate_usage(self, response):
         total_tokens = response["usage"]["total_tokens"]
         prompt_tokens = response["usage"]["prompt_tokens"]
         completion_tokens = response["usage"]["completion_tokens"]
         prompt_price = tokens2price(self.model, "prompt", prompt_tokens)
         completion_price = tokens2price(self.model, "completion", completion_tokens)
```

### Comparing `kanu-0.8.0/kanu/docgpt.py` & `kanu-0.9.0/kanu/docgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import tkinter as tk
 from tkinter import filedialog
 
+import openai
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import ConversationalRetrievalChain
 from langchain.prompts import PromptTemplate
 from langchain.memory import ConversationBufferMemory
@@ -131,20 +132,27 @@
             memory=self.memory,
             chain_type="stuff",
             combine_docs_chain_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
         )
         self.conversation.page()
 
     def send_message(self):
-        self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
-        with get_openai_callback() as cb:
-            response = self.qa(self.user_input.get())
-            self.calculate_usage(cb)
-        self.session.insert(tk.END, "Bot: " + response["answer"] + "\n", "bot")
-        self.chatbox.delete(0, tk.END)
+        try:
+            with get_openai_callback() as cb:
+                response = self.qa(self.user_input.get())
+                self.calculate_usage(cb)
+            self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
+            self.session.insert(tk.END, "Bot: " + response["answer"] + "\n", "bot")
+            self.chatbox.delete(0, tk.END)
+        except openai.error.InvalidRequestError as e:
+            error = str(e)
+            if "Please reduce the length of the messages." in error:
+                self.system.insert(tk.END, f"System: {error} You can also create a new chat session.\n", "system")
+            else:
+                raise
 
     def calculate_usage(self, cb):
         prompt_price = tokens2price(self.model, "prompt", cb.prompt_tokens)
         completion_price = tokens2price(self.model, "completion", cb.completion_tokens)
         self.price += prompt_price + completion_price
         self.tokens += cb.total_tokens
         message = f"System: Used {cb.prompt_tokens:,} prompt + {cb.completion_tokens:,} completion = {cb.total_tokens:,} tokens (total: {self.tokens:,} or ${self.price:.6f})."
```

### Comparing `kanu-0.8.0/kanu/funcgpt.py` & `kanu-0.9.0/kanu/funcgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,47 +32,52 @@
     def run(self):
         self.conversation.page()
 
     def send_message(self):
         if not self.messages:
             self.messages.append({"role": "system", "content": self.prompt})
         self.messages += [{"role": "user", "content": self.user_input.get()}]
-        bot_response = openai.ChatCompletion.create(
-            model=self.model,
-            messages=self.messages,
-            temperature=self.temperature,
-            functions=[x["json"] for x in self.module.functions.values()],
-            function_call="auto",
-        )
-        message = bot_response["choices"][0]["message"]
-        if message.get("function_call"):
-            function_name = message["function_call"]["name"]
-            function_args = json.loads(message["function_call"]["arguments"])
-            function_response = self.module.functions[function_name]["function"](**function_args)
-            second_response = openai.ChatCompletion.create(
+        try:
+            first_response = openai.ChatCompletion.create(
                 model=self.model,
-                messages=[
-                    {"role": "user", "content": self.user_input.get()},
-                    message,
-                    {
-                        "role": "function",
-                        "name": function_name,
-                        "content": function_response,
-                    },
-                ],
+                messages=self.messages,
+                temperature=self.temperature,
+                functions=[x["json"] for x in self.module.functions.values()],
+                function_call="auto",
             )
-            self.calculate_usage(second_response, function=function_name)
-            response = second_response["choices"][0]["message"]["content"]
-        else:
-            response = bot_response["choices"][0]["message"]["content"]
-        self.messages += [{"role": "assistant", "content": response}]
-        self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
-        self.session.insert(tk.END, f"Bot: " + response + "\n", "bot")
-        self.calculate_usage(bot_response)
-        self.chatbox.delete(0, tk.END)
+            message = first_response["choices"][0]["message"]
+            if message.get("function_call"):
+                function_name = message["function_call"]["name"]
+                function_args = json.loads(message["function_call"]["arguments"])
+                function_response = self.module.functions[function_name]["function"](**function_args)
+                second_response = openai.ChatCompletion.create(
+                    temperature=self.temperature,
+                    model=self.model,
+                    messages=[
+                        {"role": "user", "content": self.user_input.get()},
+                        message,
+                        {"role": "function", "name": function_name, "content": function_response},
+                    ],
+                )
+                self.calculate_usage(second_response, function=function_name)
+                answer = second_response["choices"][0]["message"]["content"]
+            else:
+                answer = first_response["choices"][0]["message"]["content"]
+            self.messages += [{"role": "assistant", "content": answer}]
+            self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
+            self.session.insert(tk.END, f"Bot: " + answer + "\n", "bot")
+            self.calculate_usage(first_response)
+            self.chatbox.delete(0, tk.END)
+        except openai.error.InvalidRequestError as e:
+            error = str(e)
+            if "Please reduce the length of the messages or functions." in error:
+                self.system.insert(tk.END, f"System: {error} You can also create a new chat session.\n", "system")
+                self.messages.pop()
+            else:
+                raise
 
     def calculate_usage(self, response, function=None):
         total_tokens = response["usage"]["total_tokens"]
         prompt_tokens = response["usage"]["prompt_tokens"]
         completion_tokens = response["usage"]["completion_tokens"]
         prompt_price = tokens2price(self.model, "prompt", prompt_tokens)
         completion_price = tokens2price(self.model, "completion", completion_tokens)
```

### Comparing `kanu-0.8.0/kanu/gui.py` & `kanu-0.9.0/kanu/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     def __init__(self, agent):
         self.agent = agent
         self.name = self.agent.__class__.__name__
         if self.name == "ChatGPT":
             self.go_back = self.agent.kanu.config_chatgpt
         elif self.name == "FuncGPT":
             self.go_back = self.agent.kanu.config_funcgpt
+        elif self.name == "ChatPaLM":
+            self.go_back = self.agent.kanu.config_chatpalm
         else:
             self.go_back = self.agent.run
 
     def page(self):
         self.agent.previous = self.agent.kanu.container
         self.agent.kanu.container.pack_forget()
         self.agent.kanu.container = tk.Frame(self.agent.kanu.root)
```

### Comparing `kanu-0.8.0/kanu/utils.py` & `kanu-0.9.0/kanu/utils.py`

 * *Files identical despite different names*

### Comparing `kanu-0.8.0/setup.py` & `kanu-0.9.0/setup.py`

 * *Files identical despite different names*

