# Comparing `tmp/swarms-0.5.2.tar.gz` & `tmp/swarms-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.5.2.tar", last modified: Tue Jul  4 22:01:36 2023, max compression
+gzip compressed data, was "swarms-0.5.3.tar", last modified: Tue Jul  4 23:39:09 2023, max compression
```

## Comparing `swarms-0.5.2.tar` & `swarms-0.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 22:01:26.000000 swarms-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 22:01:36.158368 swarms-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 22:01:26.000000 swarms-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.154368 swarms-0.5.2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:26.000000 swarms-0.5.2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 22:01:26.000000 swarms-0.5.2/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 22:01:26.000000 swarms-0.5.2/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 22:01:26.000000 swarms-0.5.2/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:01:36.158368 swarms-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-04 22:01:26.000000 swarms-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.154368 swarms-0.5.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.154368 swarms-0.5.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70833 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.158368 swarms-0.5.2/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 22:01:26.000000 swarms-0.5.2/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:01:36.154368 swarms-0.5.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 22:01:36.000000 swarms-0.5.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 22:01:36.000000 swarms-0.5.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:01:36.000000 swarms-0.5.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-04 22:01:36.000000 swarms-0.5.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 22:01:36.000000 swarms-0.5.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.651199 swarms-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 23:39:00.000000 swarms-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 23:39:09.647199 swarms-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 23:39:00.000000 swarms-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-04 23:39:00.000000 swarms-0.5.3/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 23:39:00.000000 swarms-0.5.3/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 23:39:00.000000 swarms-0.5.3/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 23:39:09.651199 swarms-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-04 23:39:00.000000 swarms-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.5.2/LICENSE` & `swarms-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/PKG-INFO` & `swarms-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.2
+Version: 0.5.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.2/README.md` & `swarms-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/api/container.py` & `swarms-0.5.3/api/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from pathlib import Path
 from typing import Dict, List
 
 from fastapi.templating import Jinja2Templates
 
 from swarms.agents.workers.agents import AgentManager
-from swarms.utils import BaseHandler, FileHandler, FileType, StaticUploader, CsvToDataframe
+from swarms.utils.utils import BaseHandler, FileHandler, FileType, StaticUploader, CsvToDataframe
 
 from swarms.tools.main import BaseToolSet, ExitConversation, RequestsGet, CodeEditor, Terminal
 
 from env import settings
 
 
 BASE_DIR = Path(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
```

### Comparing `swarms-0.5.2/api/main.py` & `swarms-0.5.3/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/api/worker.py` & `swarms-0.5.3/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/setup.py` & `swarms-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.5.2',
+  version = '0.5.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.5.2/swarms/agents/swarms.py` & `swarms-0.5.3/swarms/agents/swarms.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 from langchain.tools.human.tool import HumanInputRun
 
 # from swarms.agents.workers.auto_agent import MultiModalVisualAgent
 # from swarms.agents.workers import multimodal_agent_tool
-from swarms.tools import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
-from swarms.tools import math_tool
+from swarms.tools import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool, math_tool
 
 
 openai_api_key = os.environ["OPENAI_API_KEY"]
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
```

### Comparing `swarms-0.5.2/swarms/agents/workers/agents.py` & `swarms-0.5.3/swarms/agents/workers/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentAction, AgentFinish, LLMResult
 from celery import Task
 
-from swarms.utils import ANSI, Color, Style, dim_multiline, logger
+from swarms.utils.utils import ANSI, Color, Style, dim_multiline, logger
 
 
 class EVALCallbackHandler(BaseCallbackHandler):
     @property
     def ignore_llm(self) -> bool:
         return False
```

### Comparing `swarms-0.5.2/swarms/agents/workers/auto_agent.py` & `swarms-0.5.3/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.5.3/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/agents/workers/multi_modal.py` & `swarms-0.5.3/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/agents/workers/omni_agent.py` & `swarms-0.5.3/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/prompts/prompts.py` & `swarms-0.5.3/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/tools/main.py` & `swarms-0.5.3/swarms/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # import llama_index
 # from llama_index import GPTVectorStoreIndex
 # from llama_index.readers.database import DatabaseReader
 
 # from logger import logger
 
-from swarms.utils import logger
+from swarms.utils.logger import logger
 
 class ToolScope(Enum):
     GLOBAL = "global"
     SESSION = "session"
 
 
 SessionGetter = Callable[[], Tuple[str, AgentExecutor]]
@@ -431,15 +431,15 @@
 
 import os
 import subprocess
 import time
 from datetime import datetime
 from typing import Dict, List
 
-from swarms.utils import ANSI, Color, Style # test
+from swarms.utils.utils import ANSI, Color, Style # test
 
 class Terminal(BaseToolSet):
     def __init__(self):
         self.sessions: Dict[str, List[SyscallTracer]] = {}
 
     @tool(
         name="Terminal",
```

### Comparing `swarms-0.5.2/swarms/utils/ansi.py` & `swarms-0.5.3/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms/utils/utils.py` & `swarms-0.5.3/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms.egg-info/PKG-INFO` & `swarms-0.5.3/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.2
+Version: 0.5.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.2/swarms.egg-info/SOURCES.txt` & `swarms-0.5.3/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.5.2/swarms.egg-info/requires.txt` & `swarms-0.5.3/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

