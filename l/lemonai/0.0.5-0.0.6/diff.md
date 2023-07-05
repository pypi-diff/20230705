# Comparing `tmp/lemonai-0.0.5.tar.gz` & `tmp/lemonai-0.0.6.tar.gz`

## Comparing `lemonai-0.0.5.tar` & `lemonai-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0   136529 2020-02-02 00:00:00.000000 lemonai-0.0.5/heatmap-example.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.5/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.5/LICENSE
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 lemonai-0.0.5/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 lemonai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0   136529 2020-02-02 00:00:00.000000 lemonai-0.0.6/heatmap-example.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.6/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.6/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.6/LICENSE
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 lemonai-0.0.6/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 lemonai-0.0.6/PKG-INFO
```

### Comparing `lemonai-0.0.5/heatmap-example.png` & `lemonai-0.0.6/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/src/lemonai/api_wrapper.py` & `lemonai-0.0.6/src/lemonai/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/src/lemonai/execute_workflow.py` & `lemonai-0.0.6/src/lemonai/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/src/lemonai/filter_tools.py` & `lemonai-0.0.6/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/src/lemonai/get_integrations.py` & `lemonai-0.0.6/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/src/lemonai/tool.py` & `lemonai-0.0.6/src/lemonai/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     api_key: Optional[str] = None
     access_token: Optional[str] = None
     logger: Logger
     session_id: str
 
     def _run(self, action_input: str) -> Dict:
         
-        self.logger.bind(session_id=self.session_id, operation_name=self.name).info("")
+        self.logger.bind(session_id=self.session_id, operation_name=self.id).info("")
         return self.api_wrapper.run(self.id, action_input, self.params, self.api_key, self.access_token)
 
     async def _arun(self):
         raise NotImplementedError(" Tool does not support async")
```

### Comparing `lemonai-0.0.5/src/lemonai/toolkit.py` & `lemonai-0.0.6/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/.gitignore` & `lemonai-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/LICENSE` & `lemonai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.5/README.md` & `lemonai-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # 🍋 Lemon AI
 
 ## About
 
-**Lemon AI Python client to build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github. Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions. With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.**
+**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github.**
+
+Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
+
+With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.
 
 ## 🖲️ Getting Started
 
 ### Install the Lemon AI Client
 
 To use Lemon AI in your Python project just run:
 
 ```bash
 pip install lemonai
 ```
 
-This will install the corresponding Lemon AI client which you then can import into your script.
+This will install the corresponding Lemon AI client which you can then import into your script.
 
-The tool uses Python packages `langchain` and `loguru`. In the case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
+The tool uses Python packages `langchain` and `loguru`. In case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
 
 Requires Python 3.8.1 and above.
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
 ### Spin Up the Lemon AI Server
 
@@ -117,15 +121,15 @@
 
 By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
 
 ![Heatmap Example](heatmap-example.png)
 
 ## Supported Tools
 
-Below is a list of all supported tools by Lemon AI and their ids (for use in the lemonai.json workflow file):
+Below is a list of all tools supported by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
 ### HackerNews
 
 - Get User: hackernews-get-user
 - Get Article: hackernews-get-article
 
 ### Airtable
```

### Comparing `lemonai-0.0.5/pyproject.toml` & `lemonai-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.0.5/PKG-INFO` & `lemonai-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,29 +14,33 @@
 Requires-Dist: loguru
 Description-Content-Type: text/markdown
 
 # 🍋 Lemon AI
 
 ## About
 
-**Lemon AI Python client to build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github. Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions. With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.**
+**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github.**
+
+Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
+
+With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.
 
 ## 🖲️ Getting Started
 
 ### Install the Lemon AI Client
 
 To use Lemon AI in your Python project just run:
 
 ```bash
 pip install lemonai
 ```
 
-This will install the corresponding Lemon AI client which you then can import into your script.
+This will install the corresponding Lemon AI client which you can then import into your script.
 
-The tool uses Python packages `langchain` and `loguru`. In the case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
+The tool uses Python packages `langchain` and `loguru`. In case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
 
 Requires Python 3.8.1 and above.
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
 ### Spin Up the Lemon AI Server
 
@@ -133,15 +137,15 @@
 
 By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
 
 ![Heatmap Example](heatmap-example.png)
 
 ## Supported Tools
 
-Below is a list of all supported tools by Lemon AI and their ids (for use in the lemonai.json workflow file):
+Below is a list of all tools supported by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
 ### HackerNews
 
 - Get User: hackernews-get-user
 - Get Article: hackernews-get-article
 
 ### Airtable
```

