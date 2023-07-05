# Comparing `tmp/idoctorai-0.6.6.tar.gz` & `tmp/idoctorai-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.6.6.tar", max compression
+gzip compressed data, was "idoctorai-0.6.7.tar", max compression
```

## Comparing `idoctorai-0.6.6.tar` & `idoctorai-0.6.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.6/LICENSE
--rw-r--r--   0        0        0    20972 2023-07-05 00:36:17.406220 idoctorai-0.6.6/pandasai/__init__.py
--rw-r--r--   0        0        0     1858 2023-07-03 05:12:09.354788 idoctorai-0.6.6/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.6/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.6/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.6/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.6/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.6/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.6/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.6/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.6/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     3082 2023-07-02 07:24:07.017384 idoctorai-0.6.6/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.6/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.6/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.6.6/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.6/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.6/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     4154 2023-07-03 02:41:28.389857 idoctorai-0.6.6/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.6/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.6/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.6/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.6/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.6/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.6/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.6.6/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.6/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.6/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1691 2023-07-05 11:49:36.112402 idoctorai-0.6.6/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1593 2023-07-05 11:50:22.552969 idoctorai-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.6/README.md
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 idoctorai-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.7/LICENSE
+-rw-r--r--   0        0        0    20972 2023-07-05 00:36:17.406220 idoctorai-0.6.7/pandasai/__init__.py
+-rw-r--r--   0        0        0     1858 2023-07-03 05:12:09.354788 idoctorai-0.6.7/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.7/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.7/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.7/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.7/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.7/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.7/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.7/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.7/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     3353 2023-07-05 12:14:09.793349 idoctorai-0.6.7/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.7/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.7/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.6.7/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.7/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.7/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     4154 2023-07-03 02:41:28.389857 idoctorai-0.6.7/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.7/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.7/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.7/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.7/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.7/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.7/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.6.7/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.7/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.7/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1709 2023-07-05 12:07:41.197774 idoctorai-0.6.7/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1593 2023-07-05 12:14:21.290482 idoctorai-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.7/README.md
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 idoctorai-0.6.7/PKG-INFO
```

### Comparing `idoctorai-0.6.6/LICENSE` & `idoctorai-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/__init__.py` & `idoctorai-0.6.7/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/constants.py` & `idoctorai-0.6.7/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/exceptions.py` & `idoctorai-0.6.7/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/_optional.py` & `idoctorai-0.6.7/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/anonymizer.py` & `idoctorai-0.6.7/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/cache.py` & `idoctorai-0.6.7/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/from_excel.py` & `idoctorai-0.6.7/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/notebook.py` & `idoctorai-0.6.7/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/helpers/save_chart.py` & `idoctorai-0.6.7/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/langchain/__init__.py` & `idoctorai-0.6.7/pandasai/langchain/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 Overall, Assistant is a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether you need help with a specific question or just want to have a conversation about a particular topic, Assistant is here to assist.
 
 {history}
 Human: {human_input}
 Assistant:"""
     
-    template= """
+    template= """Assistant is a large language model trained by OpenAI.
+Assistant is constantly learning and improving, and its capabilities are constantly evolving.Assistant is a very rigorous and careful tool, and will complete the task strictly according to the requirements of Human.
 {history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, llm: AzureOpenAI, **kwargs,):
         # self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
         if llm is None:
```

### Comparing `idoctorai-0.6.6/pandasai/llm/azure_openai.py` & `idoctorai-0.6.7/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/base.py` & `idoctorai-0.6.7/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/fake.py` & `idoctorai-0.6.7/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/google_palm.py` & `idoctorai-0.6.7/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/model.py` & `idoctorai-0.6.7/pandasai/llm/model.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/open_assistant.py` & `idoctorai-0.6.7/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/openai.py` & `idoctorai-0.6.7/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/llm/starcoder.py` & `idoctorai-0.6.7/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/base.py` & `idoctorai-0.6.7/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.6.7/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.6.7/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/generate_python_code.py` & `idoctorai-0.6.7/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/generate_response.py` & `idoctorai-0.6.7/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.6/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.6.7/pandasai/prompts/multiple_dataframes.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
 Don't add too many code comments.The result must be printed at the end of the python code.If the data format is not standard, standardize and format the data first.
-Using the provided dataframes and no other dataframes, return the python code(no duplicate) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
+Using the provided dataframes only and Do not create your own dataframe, return the python code(no duplicate) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             data_text = dataframe.head().to_string()
```

### Comparing `idoctorai-0.6.6/pyproject.toml` & `idoctorai-0.6.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.6.6"
+version = "0.6.7"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"},{include="pyproject.toml"}]
```

### Comparing `idoctorai-0.6.6/PKG-INFO` & `idoctorai-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.6.6
+Version: 0.6.7
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

