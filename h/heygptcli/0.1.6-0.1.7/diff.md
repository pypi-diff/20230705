# Comparing `tmp/heygptcli-0.1.6.tar.gz` & `tmp/heygptcli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.6.tar", max compression
+gzip compressed data, was "heygptcli-0.1.7.tar", max compression
```

## Comparing `heygptcli-0.1.6.tar` & `heygptcli-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       87 2023-07-03 16:05:18.682204 heygptcli-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/__init__.py
--rw-r--r--   0        0        0      774 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/api.py
--rwxr-xr-x   0        0        0     5292 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/constant.py
--rw-r--r--   0        0        0     3542 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/core.py
--rw-r--r--   0        0        0     2162 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-07-03 16:05:18.682204 heygptcli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-07-05 13:56:10.275182 heygptcli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 13:56:10.275182 heygptcli-0.1.7/heygpt/__init__.py
+-rw-r--r--   0        0        0     1621 2023-07-05 13:56:10.275182 heygptcli-0.1.7/heygpt/__temp.py
+-rw-r--r--   0        0        0      774 2023-07-05 13:56:10.275182 heygptcli-0.1.7/heygpt/api.py
+-rwxr-xr-x   0        0        0     5302 2023-07-05 13:56:10.275182 heygptcli-0.1.7/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-07-05 13:56:10.275182 heygptcli-0.1.7/heygpt/constant.py
+-rw-r--r--   0        0        0     4139 2023-07-05 13:56:10.279182 heygptcli-0.1.7/heygpt/core.py
+-rw-r--r--   0        0        0     2172 2023-07-05 13:56:10.279182 heygptcli-0.1.7/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-07-05 13:56:10.279182 heygptcli-0.1.7/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-07-05 13:56:10.279182 heygptcli-0.1.7/heygpt/utils.py
+-rw-r--r--   0        0        0      688 2023-07-05 13:56:10.279182 heygptcli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 heygptcli-0.1.7/PKG-INFO
```

### Comparing `heygptcli-0.1.6/heygpt/api.py` & `heygptcli-0.1.7/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.6/heygpt/cli.py` & `heygptcli-0.1.7/heygpt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 import typer
 
 from heygpt.utils import log
 from heygpt.constant import load_promps, prompt_items_url, openai_model
 from heygpt.core import (
     sh,
     completion_openai_gpt,
-    completion_bard,
+    completion_palm_text,
     make_prompt,
     wisper,
     print_md,
     ask_prompt_input,
 )
 
 app = typer.Typer(
     help="""
-HeyGPT CLI\n\nA simple command line tool to generate text using OpenAI GPT or Bard base on ready made templated promts.
+HeyGPT CLI\n\nA simple command line tool to generate text using OpenAI GPT or palm base on ready made templated promts.
 \n\n\nFor debug logs use: `export LOG_LEVEL=DEBUG` or `set LOG_LEVEL=DEBUG` on windows."""
 )
 
 
 @app.command(help="Ask query or task to gpt using prompt templates")
 def ask(
-    bard: bool = typer.Option(
-        False, "--bard", "-b", help="Use bard instead of openai."
+    palm: bool = typer.Option(
+        False, "--palm", "-b", help="Use palm instead of openai."
     ),
     no_prompt: bool = typer.Option(
         False, "--no-prompt", "-n", help="Ask without anyprompt templates."
     ),
     text: str = typer.Option(
         str, help="Optional provide text query as an input argument."
     ),
@@ -96,16 +96,16 @@
         text = sys.stdin.read()
     elif text == "":
         rich.print(f"Selected: {command}") if not no_prompt else ...
         print()
         text = Prompt.ask("[blue]Enter text")
 
     # log.debug(text)
-    if bard:
-        content = completion_bard(command=command, text=text, _print=True)
+    if palm:
+        content = completion_palm_text(command=command, text=text, _print=True)
     else:
         completion = completion_openai_gpt(
             command=command,
             text=text,
             model=model,
             _print=True,
             temperature=temperature,
@@ -153,15 +153,15 @@
 
 
 @app.command(help="Configure heygpt.")
 def config(
     prompt_file: str = typer.Option("", help="Prompt file path."),
     prompt_url: str = typer.Option("", help="Prompt file url."),
     openai_key: str = typer.Option("", help="OpenAI API key."),
-    bard_key: str = typer.Option("", help="Bard API key."),
+    palm_key: str = typer.Option("", help="palm API key."),
 ):
     from heygpt.constant import config_path
 
     if not Path(config_path).parent.is_dir():
         Path(config_path).parent.mkdir(parents=True)
     if not Path(config_path).is_file():
         with open(config_path, "w") as c:
@@ -175,16 +175,16 @@
 
         if prompt_file != "":
             configs["prompt_file"] = Path(prompt_file).absolute().as_posix()
         if prompt_url != "":
             configs["prompt_url"] = prompt_url
         if openai_key != "":
             configs["openai_key"] = openai_key
-        if bard_key != "":
-            configs["bard_key"] = bard_key
+        if palm_key != "":
+            configs["palm_key"] = palm_key
 
         new_configs = configs
         print(json.dumps(new_configs))
         f.write(json.dumps(new_configs))
 
 
 if __name__ == "__main__":
```

### Comparing `heygptcli-0.1.6/heygpt/constant.py` & `heygptcli-0.1.7/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.6/heygpt/core.py` & `heygptcli-0.1.7/heygpt/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import requests
 import openai
-from bardapi import Bard
+import google.generativeai as palm
 from rich.console import Console
 from rich.markdown import Markdown
 from prompt_toolkit import prompt
 from prompt_toolkit.completion import FuzzyWordCompleter
 
 from heygpt.constant import configs, genrtare_prompt_url, openai_model
 from heygpt.utils import log
@@ -87,28 +87,47 @@
             out += c
             if _print:
                 console.print(c, end="", markup=True)
 
     return out
 
 
-def completion_bard(text: str, command: str = "", _print=False):
+def completion_palm_text(text: str, command: str = "", _print=False):
     """
-    ref: https://github.com/dsdanielpark/Bard-API
-    Bard is a GPT-3 model trained on 38 million lines of fantasy text.
-
-    This function requires "_BARD_API_KEY" which can get from below steps:
-    Go to https://bard.google.com/
-        : Go to Application → Cookies → __Secure-1PSID. Copy the value of that cookie.
+    ref: https://developers.generativeai.google/api/python/google/generativeai/generate_text
     """
-    if os.environ.get("_BARD_API_KEY") == None:
-        if configs.get("bard_key"):
-            os.environ["_BARD_API_KEY"] = configs.get("bard_key")
+    if os.environ.get("PALM_API_KEY") == None:
+        if configs.get("palm_key"):
+            os.environ["PALM_API_KEY"] = configs.get("palm_key")
+
+    palm.configure(api_key=os.environ.get("PALM_API_KEY"))
+
+    defaults = {
+        "model": "models/text-bison-001",
+        "temperature": 0.7,
+        "candidate_count": 1,
+        "top_k": 40,
+        "top_p": 0.95,
+        "max_output_tokens": 1024,
+        "stop_sequences": [],
+        "safety_settings": [
+            # {"category": "HARM_CATEGORY_DEROGATORY", "threshold": 1},
+            # {"category": "HARM_CATEGORY_TOXICITY", "threshold": 1},
+            # {"category": "HARM_CATEGORY_VIOLENCE", "threshold": 2},
+            # {"category": "HARM_CATEGORY_SEXUAL", "threshold": 2},
+            # {"category": "HARM_CATEGORY_MEDICAL", "threshold": 2},
+            # {"category": "HARM_CATEGORY_DANGEROUS", "threshold": 2},
+        ],
+    }
+    prompt = f"""{command}
+
+    {text}"""
+    response = palm.generate_text(**defaults, prompt=prompt)
 
-    completer = Bard().get_answer(command + "\nTask: " + text)["content"]
+    completer = response.result
     if _print:
         print_md(completer)
     return completer
 
 
 def make_prompt(text: str):
     json_data = {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `heygptcli-0.1.6/heygpt/serve.py` & `heygptcli-0.1.7/heygpt/serve.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import streamlit as st
-from heygpt.core import completion_openai_gpt, completion_bard
+from heygpt.core import completion_openai_gpt, completion_palm_text
 from heygpt.serve_prompts import prompts_title
 
 
 def local_css(file_name="", style=""):
     if file_name != "":
         with open(file_name) as f:
             st.markdown(f"<style>{f.read()}</style>", unsafe_allow_html=True)
@@ -27,15 +27,15 @@
         print_prompt = st.empty()
     with col3:
         st.write("<br><br><br>", unsafe_allow_html=True)
         submit = st.button("Submit")
 
 
 with col1:
-    _options = {"GPT": "gpt-3.5-turbo", "Davinci": "text-davinci-003", "Bard": "bard"}
+    _options = {"GPT": "gpt-3.5-turbo", "Davinci": "text-davinci-003", "Palm": "palm"}
     use_model = st.radio("**Model**", options=_options.keys())
     prompt = st.radio(
         label="**Promots**", options=["None"] + list(prompts_title.keys())
     )
 
 
 with st.container():
@@ -45,25 +45,25 @@
         if prompt != "None":
             _selected_prompt = prompts_title[prompt]
             print_prompt.write(f"**Selected**: {_selected_prompt}")
         else:
             _selected_prompt = ""
 
         if submit:
-            if use_model != "Bard":
+            if use_model != "Palm":
                 completion = completion_openai_gpt(
                     command=_selected_prompt, text=ask, model=_options[use_model]
                 )
                 if "davinci" in use_model.lower():
                     st.markdown(f"```{completion}")
                 else:
                     st.markdown(completion)
 
             else:
-                completion = completion_bard(command=_selected_prompt, text=ask)
+                completion = completion_palm_text(command=_selected_prompt, text=ask)
                 st.markdown(completion)
 
             content = completion
 
     with col3:
         if content != "":
             st.download_button(
```

### Comparing `heygptcli-0.1.6/heygpt/utils.py` & `heygptcli-0.1.7/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.6/pyproject.toml` & `heygptcli-0.1.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
 
@@ -14,19 +14,19 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 fastapi = "^0.97.0"
 uvicorn = "^0.22.0"
 typer = "^0.9.0"
 python-dotenv = "^1.0.0"
-bardapi = "^0.1.11"
 openai = "^0.27.8"
 rich = "^13.4.1"
 prompt-toolkit = "^3.0.38"
 streamlit = "^1.23.1"
+google-generativeai = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 types-requests = "*"
```

