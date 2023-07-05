# Comparing `tmp/openai_copilot-0.2.2.tar.gz` & `tmp/openai_copilot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_copilot-0.2.2.tar", max compression
+gzip compressed data, was "openai_copilot-0.2.3.tar", max compression
```

## Comparing `openai_copilot-0.2.2.tar` & `openai_copilot-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.2/LICENSE
--rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.2/openai_copilot/__init__.py
--rw-r--r--   0        0        0     2882 2023-06-16 04:26:19.677452 openai_copilot-0.2.2/openai_copilot/agent.py
--rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.2/openai_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.2/openai_copilot/llm.py
--rw-r--r--   0        0        0      674 2023-06-16 04:27:49.757663 openai_copilot-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 openai_copilot-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.3/openai_copilot/__init__.py
+-rw-r--r--   0        0        0     3377 2023-07-05 08:39:26.511791 openai_copilot-0.2.3/openai_copilot/agent.py
+-rw-r--r--   0        0        0     1043 2023-07-05 07:58:16.851415 openai_copilot-0.2.3/openai_copilot/cli.py
+-rw-r--r--   0        0        0      752 2023-06-19 00:40:59.328532 openai_copilot-0.2.3/openai_copilot/llm.py
+-rw-r--r--   0        0        0     2052 2023-07-05 08:40:23.043712 openai_copilot-0.2.3/openai_copilot/output.py
+-rw-r--r--   0        0        0      694 2023-07-05 08:33:35.815582 openai_copilot-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 openai_copilot-0.2.3/PKG-INFO
```

### Comparing `openai_copilot-0.2.2/LICENSE` & `openai_copilot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.2/README.md` & `openai_copilot-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.2/openai_copilot/agent.py` & `openai_copilot-0.2.3/openai_copilot/agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 import os
 from langchain.chat_models import ChatOpenAI
 from langchain.agents import Tool, load_tools
-from langchain.memory import ConversationBufferMemory
+from langchain.agents import AgentType
+from langchain.memory import ConversationSummaryBufferMemory
 from langchain.agents import initialize_agent
-from langchain.tools.python.tool import PythonREPLTool
 from langchain.utilities import GoogleSearchAPIWrapper
+from openai_copilot.output import ChatOutputParser
 
 
 class CopilotLLM:
     '''Wrapper for LLM chain.'''
 
-    def __init__(self, verbose=True, model="gpt-3.5-turbo", additional_tools=None, enable_terminal=False):
+    def __init__(self, verbose=True, model="gpt-4", additional_tools=None, enable_terminal=False):
         '''Initialize the LLM chain.'''
         self.chain = get_chat_chain(verbose, model, additional_tools=additional_tools,
                                     enable_terminal=enable_terminal)
 
     def run(self, instructions):
         '''Run the LLM chain.'''
         try:
@@ -25,40 +26,31 @@
             # Workaround for issue https://github.com/hwchase17/langchain/issues/1358.
             if "Could not parse LLM output:" in str(e):
                 return str(e).split("Could not parse LLM output:")[1]
             else:
                 raise e
 
 
-def get_chat_chain(verbose=True, model="gpt-3.5-turbo", additional_tools=None,
-                   agent="chat-conversational-react-description",
+def get_chat_chain(verbose=True, model="gpt-4", additional_tools=None,
+                   agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION,
                    enable_terminal=False, max_iterations=30,
-                   max_tokens=1024):
+                   max_tokens=None):
     '''Initialize the LLM chain with useful tools.'''
-    if os.getenv("OPENAI_API_TYPE") == "azure":
+    if os.getenv("OPENAI_API_TYPE") == "azure" or (os.getenv("OPENAI_API_BASE") is not None and "azure" in os.getenv("OPENAI_API_BASE")):
         engine = model.replace(".", "")
         llm = ChatOpenAI(model=model, max_tokens=max_tokens,
                          model_kwargs={"engine": engine})
     else:
         llm = ChatOpenAI(model=model, max_tokens=max_tokens)
 
-    default_tools = ["human"]
+    default_tools = ["human", "requests_get", "python_repl"]
     if enable_terminal:
         default_tools += ["terminal"]
     tools = load_tools(default_tools, llm)
 
-    if os.getenv("OPENAI_COPILOT_ENABLE_PYTHON"):
-        tools += [
-            Tool(
-                name="Python",
-                func=PythonREPLTool().run,
-                description="helps to run Python codes"
-            )
-        ]
-
     if os.getenv("GOOGLE_API_KEY") and os.getenv("GOOGLE_CSE_ID"):
         tools += [
             Tool(
                 name="Search",
                 func=GoogleSearchAPIWrapper(
                     k=3,
                     google_api_key=os.getenv("GOOGLE_API_KEY"),
@@ -67,13 +59,28 @@
                 description="search the web for current events or current state of the world"
             )
         ]
 
     if additional_tools is not None:
         tools += additional_tools
 
-    memory = ConversationBufferMemory(
-        memory_key="chat_history", return_messages=True)
+    memory = ConversationSummaryBufferMemory(
+        llm=llm,
+        memory_key="chat_history",
+        return_messages=True)
     chain = initialize_agent(
         tools, llm, agent=agent, memory=memory,
-        verbose=verbose, max_iterations=max_iterations)
+        agent_kwargs={"output_parser": ChatOutputParser()},
+        verbose=verbose, max_iterations=max_iterations,
+        handle_parsing_error=handle_parsing_error)
     return chain
+
+
+def handle_parsing_error(error) -> str:
+    '''Helper function to handle parsing errors from LLM.'''
+    # Workaround for issue https://github.com/hwchase17/langchain/issues/1358.
+    response = str(error).split("Could not parse LLM output:")[1].strip()
+    if not response.startswith('```'):
+        response = response.removeprefix('`')
+    if not response.endswith('```'):
+        response = response.removesuffix('`')
+    return response
```

### Comparing `openai_copilot-0.2.2/openai_copilot/cli.py` & `openai_copilot-0.2.3/openai_copilot/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openai_copilot.llm import init_openai
 from openai_copilot.agent import CopilotLLM
 
 
 @click.command()
 @click.version_option()
 @click.option("--verbose", is_flag=True, default=False, help="Enable verbose information of copilot execution steps")
-@click.option("--model", default="gpt-3.5-turbo", help="OpenAI model to use for copilot execution, default is gpt-3.5-turbo")
+@click.option("--model", default="gpt-4", help="OpenAI model to use for copilot execution, default is gpt-4")
 @click.option("--enable-terminal", is_flag=True, default=False, help="Enable Copilot to run programs within terminal. Enable with caution since Copilot may execute inappropriate commands")
 def cli(verbose, model, enable_terminal):
     '''Your life Copilot powered by OpenAI'''
     init_openai()
     chain = CopilotLLM(
         verbose=verbose, model=model, enable_terminal=enable_terminal)
     while True:
```

### Comparing `openai_copilot-0.2.2/openai_copilot/llm.py` & `openai_copilot-0.2.3/openai_copilot/llm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
-
 import os
 import openai
 
 
 def init_openai():
     """
     Initializes the OpenAI API with the provided API key and sets the API base and version if using Azure.
     """
     if os.getenv("OPENAI_API_KEY") == "":
         raise Exception("Please set OPENAI_API_KEY via environment variable")
 
-    if os.getenv("OPENAI_API_TYPE") == "azure":
+    if os.getenv("OPENAI_API_TYPE") == "azure" or (os.getenv("OPENAI_API_BASE") is not None and "azure" in os.getenv("OPENAI_API_BASE")):
         openai.api_type = "azure"
         openai.api_base = os.getenv("OPENAI_API_BASE")
-        openai.api_version = "2023-03-15-preview"
+        openai.api_version = "2023-05-15"
         openai.api_key = os.getenv("OPENAI_API_KEY")
     else:
         openai.api_key = os.getenv("OPENAI_API_KEY")
         openai.api_base = "https://api.openai.com/v1"
```

### Comparing `openai_copilot-0.2.2/pyproject.toml` & `openai_copilot-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "openai-copilot"
-version = "0.2.2"
+version = "0.2.3"
 description = "OpenAI Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_copilot"}]
 homepage = "https://github.com/feiskyer/openai-copilot"
 repository = "https://github.com/feiskyer/openai-copilot"
 keywords = ["copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 openai-copilot = 'openai_copilot.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 langchain = ">=0.0.171"
-requests = ">=2.28"
+requests = ">=2.31"
 openai = ">=0.27.4"
 google-api-python-client = ">=2.85.0"
 click = ">=8.1.3"
+tiktoken = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openai_copilot-0.2.2/PKG-INFO` & `openai_copilot-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: openai-copilot
-Version: 0.2.2
+Version: 0.2.3
 Summary: OpenAI Copilot
 Home-page: https://github.com/feiskyer/openai-copilot
 Keywords: copilot,openai,chatgpt
 Author: Pengfei Ni
 Author-email: feiskyer@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: google-api-python-client (>=2.85.0)
 Requires-Dist: langchain (>=0.0.171)
 Requires-Dist: openai (>=0.27.4)
-Requires-Dist: requests (>=2.28)
+Requires-Dist: requests (>=2.31)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/feiskyer/openai-copilot
 Description-Content-Type: text/markdown
 
 # OpenAI Copilot
 
 Your life Copilot powered by OpenAI (CLI interface for OpenAI with searching).
```

