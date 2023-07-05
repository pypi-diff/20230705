# Comparing `tmp/salesgpt-0.0.2.tar.gz` & `tmp/salesgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesgpt-0.0.2.tar", last modified: Tue Jun 20 00:06:28 2023, max compression
+gzip compressed data, was "salesgpt-0.0.3.tar", last modified: Tue Jul  4 17:51:44 2023, max compression
```

## Comparing `salesgpt-0.0.2.tar` & `salesgpt-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.434035 salesgpt-0.0.2/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1071 2023-06-19 23:47:34.000000 salesgpt-0.0.2/LICENSE
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       24 2023-06-20 00:03:48.000000 salesgpt-0.0.2/MANIFEST.in
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-06-20 00:06:28.433789 salesgpt-0.0.2/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     5977 2023-06-19 21:49:25.000000 salesgpt-0.0.2/README.md
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      103 2023-06-19 21:56:21.000000 salesgpt-0.0.2/requirements.txt
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.431345 salesgpt-0.0.2/salesgpt/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-19 20:44:34.000000 salesgpt-0.0.2/salesgpt/__init__.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     7853 2023-06-19 21:56:51.000000 salesgpt-0.0.2/salesgpt/agents.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-06-19 21:56:32.000000 salesgpt-0.0.2/salesgpt/chains.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-19 21:56:51.000000 salesgpt-0.0.2/salesgpt/logger.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-19 21:56:32.000000 salesgpt-0.0.2/salesgpt/stages.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-06-20 00:06:07.000000 salesgpt-0.0.2/salesgpt/version.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.432909 salesgpt-0.0.2/salesgpt.egg-info/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      354 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/SOURCES.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/dependency_links.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      157 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/requires.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-06-20 00:06:28.000000 salesgpt-0.0.2/salesgpt.egg-info/top_level.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-06-20 00:06:28.434287 salesgpt-0.0.2/setup.cfg
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1924 2023-06-20 00:03:32.000000 salesgpt-0.0.2/setup.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-06-20 00:06:28.433184 salesgpt-0.0.2/tests/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1585 2023-06-19 21:57:47.000000 salesgpt-0.0.2/tests/test_salesgpt.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.433331 salesgpt-0.0.3/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1071 2023-06-19 23:47:34.000000 salesgpt-0.0.3/LICENSE
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       24 2023-06-30 17:23:56.000000 salesgpt-0.0.3/MANIFEST.in
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-07-04 17:51:44.432949 salesgpt-0.0.3/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     5977 2023-06-30 17:23:56.000000 salesgpt-0.0.3/README.md
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      103 2023-06-30 17:23:56.000000 salesgpt-0.0.3/requirements.txt
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.428948 salesgpt-0.0.3/salesgpt/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/__init__.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     7930 2023-07-04 17:48:11.000000 salesgpt-0.0.3/salesgpt/agents.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/chains.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/logger.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/stages.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-07-04 17:48:59.000000 salesgpt-0.0.3/salesgpt/version.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.431755 salesgpt-0.0.3/salesgpt.egg-info/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      354 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      157 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/requires.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/top_level.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-07-04 17:51:44.433451 salesgpt-0.0.3/setup.cfg
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1924 2023-07-04 17:49:45.000000 salesgpt-0.0.3/setup.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.432250 salesgpt-0.0.3/tests/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1585 2023-06-30 17:23:56.000000 salesgpt-0.0.3/tests/test_salesgpt.py
```

### Comparing `salesgpt-0.0.2/LICENSE` & `salesgpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/PKG-INFO` & `salesgpt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `salesgpt-0.0.2/README.md` & `salesgpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/salesgpt/agents.py` & `salesgpt-0.0.3/salesgpt/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,28 +67,28 @@
 
     def human_step(self, human_input):
         # process human input
         human_input = "User: " + human_input + " <END_OF_TURN>"
         self.conversation_history.append(human_input)
 
     @time_logger
-    def step(self, return_streaming_generator: bool = False):
+    def step(self, return_streaming_generator: bool = False, model_name="gpt-3.5-turbo-0613"):
         """
         Args:
             return_streaming_generator (bool): whether or not return
             streaming generator object to manipulate streaming chunks in downstream applications.
         """
         if not return_streaming_generator:
             self._call(inputs={})
         else:
-            return self._streaming_generator()
+            return self._streaming_generator(model_name=model_name)
 
     # TO-DO change this override "run" override the "run method" in the SalesConversation chain!
     @time_logger
-    def _streaming_generator(self):
+    def _streaming_generator(self, model_name="gpt-3.5-turbo-0613"):
         """
         Sometimes, the sales agent wants to take an action before the full LLM output is available.
         For instance, if we want to do text to speech on the partial LLM output.
 
         This function returns a streaming generator which can manipulate partial output from an LLM
         in-flight of the generation.
 
@@ -124,15 +124,15 @@
             print("\033[92m" + inception_messages[0].content + "\033[0m")
         messages = [message_dict]
 
         return self.sales_conversation_utterance_chain.llm.completion_with_retry(
             messages=messages,
             stop="<END_OF_TURN>",
             stream=True,
-            model="gpt-3.5-turbo-0613",
+            model=model_name,
         )
 
     def _call(self, inputs: Dict[str, Any]) -> None:
         """Run one step of the sales agent."""
 
         # Generate agent's utterance
         ai_message = self.sales_conversation_utterance_chain.run(
```

### Comparing `salesgpt-0.0.2/salesgpt/chains.py` & `salesgpt-0.0.3/salesgpt/chains.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/salesgpt/logger.py` & `salesgpt-0.0.3/salesgpt/logger.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/salesgpt/stages.py` & `salesgpt-0.0.3/salesgpt/stages.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/salesgpt.egg-info/PKG-INFO` & `salesgpt-0.0.3/salesgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `salesgpt-0.0.2/setup.py` & `salesgpt-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.2/tests/test_salesgpt.py` & `salesgpt-0.0.3/tests/test_salesgpt.py`

 * *Files identical despite different names*

