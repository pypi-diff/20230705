# Comparing `tmp/idoctorai-0.6.4.tar.gz` & `tmp/idoctorai-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.6.4.tar", max compression
+gzip compressed data, was "idoctorai-0.6.5.tar", max compression
```

## Comparing `idoctorai-0.6.4.tar` & `idoctorai-0.6.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.4/LICENSE
--rw-r--r--   0        0        0    20905 2023-07-02 07:24:35.136407 idoctorai-0.6.4/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.6.4/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.4/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.4/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.4/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.4/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.4/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     3082 2023-07-02 07:24:07.017384 idoctorai-0.6.4/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.4/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.6.4/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.4/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     4154 2023-07-03 02:41:28.389857 idoctorai-0.6.4/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.4/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.4/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.4/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.6.4/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.4/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.4/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1606 2023-06-19 11:43:16.346788 idoctorai-0.6.4/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1480 2023-07-03 01:11:23.971282 idoctorai-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.4/README.md
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.5/LICENSE
+-rw-r--r--   0        0        0    20972 2023-07-05 00:36:17.406220 idoctorai-0.6.5/pandasai/__init__.py
+-rw-r--r--   0        0        0     1858 2023-07-03 05:12:09.354788 idoctorai-0.6.5/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.5/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.5/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.5/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.5/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.5/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.5/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.5/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.5/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     3082 2023-07-02 07:24:07.017384 idoctorai-0.6.5/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.5/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.5/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.6.5/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.5/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.5/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     4154 2023-07-03 02:41:28.389857 idoctorai-0.6.5/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.5/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.5/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.5/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.5/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.5/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.5/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.6.5/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.5/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.5/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1606 2023-06-19 11:43:16.346788 idoctorai-0.6.5/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1593 2023-07-05 00:36:48.028375 idoctorai-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.5/README.md
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 idoctorai-0.6.5/PKG-INFO
```

### Comparing `idoctorai-0.6.4/LICENSE` & `idoctorai-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/__init__.py` & `idoctorai-0.6.5/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
-    _max_retries: int = 1
+    _max_retries: int = 3
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "df_columns": None,
         "num_rows": None,
         "num_columns": None,
@@ -130,14 +130,15 @@
         self,
         llm=None,
         conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
         enable_cache=True,
+        max_retries=3,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -155,14 +156,16 @@
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
         self._enable_cache = enable_cache
         self._process_id = str(uuid.uuid4())
 
+        self._max_retries = max_retries
+
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
     def conversational_answer(self, question: str, answer: str) -> str:
         """
         Returns the answer in conversational form about the resultant data.
```

### Comparing `idoctorai-0.6.4/pandasai/constants.py` & `idoctorai-0.6.5/pandasai/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 START_CODE_TAG = "<startCode>"
 END_CODE_TAG = "<endCode>"
 
 # List of Python packages that are whitelisted for import in generated code
 #   and are installed by default.
 WHITELISTED_LIBRARIES = [
     "numpy",
+    "sklearn",
+    "statsmodels",
+    "seaborn",
+    "plotly",
+    "ggplot",
 ]
 
 # List of Python packages that are added to the environment by default.
 ENVIRONMENT_DEFAULTS = {
     "pandas": "pd",
     "matplotlib.pyplot": "plt",
 }
```

### Comparing `idoctorai-0.6.4/pandasai/exceptions.py` & `idoctorai-0.6.5/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/_optional.py` & `idoctorai-0.6.5/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/anonymizer.py` & `idoctorai-0.6.5/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/cache.py` & `idoctorai-0.6.5/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/from_excel.py` & `idoctorai-0.6.5/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/notebook.py` & `idoctorai-0.6.5/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/helpers/save_chart.py` & `idoctorai-0.6.5/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/langchain/__init__.py` & `idoctorai-0.6.5/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/azure_openai.py` & `idoctorai-0.6.5/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/base.py` & `idoctorai-0.6.5/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/fake.py` & `idoctorai-0.6.5/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/google_palm.py` & `idoctorai-0.6.5/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/model.py` & `idoctorai-0.6.5/pandasai/llm/model.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/open_assistant.py` & `idoctorai-0.6.5/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/openai.py` & `idoctorai-0.6.5/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/llm/starcoder.py` & `idoctorai-0.6.5/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/base.py` & `idoctorai-0.6.5/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.6.5/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.6.5/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/generate_python_code.py` & `idoctorai-0.6.5/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/generate_response.py` & `idoctorai-0.6.5/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.6.5/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.6.4/pyproject.toml` & `idoctorai-0.6.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.6.4"
+version = "0.6.5"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"},{include="pyproject.toml"}]
 
 
@@ -19,14 +19,20 @@
 openai = "^0.27.5"
 langchain = "0.0.194"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 toml = "^0.10.2"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
 
+scikit-learn = "^1.2.2"
+seaborn = "^0.12.2"
+statsmodels = "^0.14.0"
+plotly = "^5.14.1"
+ggplot = "^0.11.5"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 pytest = "^7.3.1"
 isort = "^5.12.0"
```

### Comparing `idoctorai-0.6.4/PKG-INFO` & `idoctorai-0.6.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.6.4
+Version: 0.6.5
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: ggplot (>=0.11.5,<0.12.0)
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: langchain (==0.0.194)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: openpyxl (==3.1.2)
 Requires-Dist: pandas (==1.5.3)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 ## idoctorai
 
 this is idoctorai, generate code with nlp
```

