# Comparing `tmp/gpt4docstrings-0.0.4.tar.gz` & `tmp/gpt4docstrings-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4docstrings-0.0.4.tar", max compression
+gzip compressed data, was "gpt4docstrings-0.0.5.tar", max compression
```

## Comparing `gpt4docstrings-0.0.4.tar` & `gpt4docstrings-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-06-30 14:19:27.830981 gpt4docstrings-0.0.4/LICENSE
--rw-r--r--   0        0        0     2830 2023-06-30 14:19:27.830981 gpt4docstrings-0.0.4/README.md
--rw-r--r--   0        0        0     1987 2023-06-30 14:19:43.306952 gpt4docstrings-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       83 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/__init__.py
--rw-r--r--   0        0        0       75 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/__main__.py
--rw-r--r--   0        0        0     1558 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/cli.py
--rw-r--r--   0        0        0       67 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/__init__.py
--rw-r--r--   0        0        0     4718 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
--rw-r--r--   0        0        0     4084 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/generate_docstrings.py
--rw-r--r--   0        0        0     1591 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/utils.py
--rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-05 16:19:27.701916 gpt4docstrings-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2830 2023-07-05 16:19:27.701916 gpt4docstrings-0.0.5/README.md
+-rw-r--r--   0        0        0     2026 2023-07-05 16:19:44.246046 gpt4docstrings-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-07-05 16:19:27.709916 gpt4docstrings-0.0.5/src/gpt4docstrings/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-05 16:19:27.709916 gpt4docstrings-0.0.5/src/gpt4docstrings/__main__.py
+-rw-r--r--   0        0        0     1409 2023-07-05 16:19:44.246046 gpt4docstrings-0.0.5/src/gpt4docstrings/cli.py
+-rw-r--r--   0        0        0       67 2023-07-05 16:19:27.709916 gpt4docstrings-0.0.5/src/gpt4docstrings/docstrings_generators/__init__.py
+-rw-r--r--   0        0        0     3420 2023-07-05 16:19:27.709916 gpt4docstrings-0.0.5/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
+-rw-r--r--   0        0        0     4174 2023-07-05 16:19:44.246046 gpt4docstrings-0.0.5/src/gpt4docstrings/generate_docstrings.py
+-rw-r--r--   0        0        0     1591 2023-07-05 16:19:27.709916 gpt4docstrings-0.0.5/src/gpt4docstrings/utils.py
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.5/PKG-INFO
```

### Comparing `gpt4docstrings-0.0.4/LICENSE` & `gpt4docstrings-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.4/README.md` & `gpt4docstrings-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.4/pyproject.toml` & `gpt4docstrings-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "gpt4docstrings"
-version = "0.0.4"
+version = "0.0.5"
 description = "gpt4docstrings"
 authors = ["Miguel Otero Pedrido <miguel.otero.pedrido.1993@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 repository = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 documentation = "https://gpt4docstrings.readthedocs.io"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/MichaelisTrofficus/gpt4docstrings/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.1"
 nox = "^2023.4.22"
 nox-poetry = "^1.0.2"
 redbaron = "^0.9.2"
 openai = "^0.27.8"
 pytest-mock = "^3.11.1"
+docformatter = "^1.7.3"
+pyment = "^0.3.3"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gpt4docstrings-0.0.4/src/gpt4docstrings/cli.py` & `gpt4docstrings-0.0.5/src/gpt4docstrings/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,14 @@
     "-m",
     "--model",
     type=click.STRING,
     default="gpt-3.5-turbo",
     help="The model to be used by `gpt4docstrings`. By default, `gpt-3.5-turbo`.",
 )
 @click.option(
-    "-d",
-    "--docstrings_style",
-    type=click.STRING,
-    default="google",
-    help="Docstring style. Choose between `google`, `numpy` or `reStructuredText`",
-)
-@click.option(
     "-k",
     "--api_key",
     type=click.STRING,
     default="",
     help="OpenAI's API key. If not provided, `gpt4docstrings` will try to access `OPENAI_API_KEY` environment variable.",
 )
 @click.option(
@@ -61,8 +54,9 @@
 
     docstrings_generator = gpt4docstrings.GPT4Docstrings(
         paths=paths,
         excluded=kwargs["exclude"],
         model=kwargs["model"],
         api_key=kwargs["api_key"],
     )
-    docstrings_generator.generate_docstrings()
+    filenames = docstrings_generator.generate_docstrings()
+    print(filenames)
```

### Comparing `gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py` & `gpt4docstrings-0.0.5/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 import ast
 import os
+import textwrap
 import time
+from typing import List
 
 import openai
 
 
 class ChatGPTDocstringGenerator:
     def __init__(
         self,
         api_key: str = None,
         model: str = "gpt-3.5-turbo",
-        docstrings_style: str = "google",
     ):
         self.api_key = api_key if api_key else os.getenv("OPENAI_API_KEY")
         self.model = model
 
-        if docstrings_style not in ["google", "numpy" or "reStructuredText"]:
-            raise ValueError(
-                "Docstring style no found. "
-                "Choose between `google`, `numpy` or `reStructuredText`"
-            )
-
-        self.docstrings_style = (
-            docstrings_style if docstrings_style != "numpy" else "numpydoc"
-        )
-
         if not self.api_key:
             raise ValueError("Please, provide the OpenAI API Key")
 
         openai.api_key = self.api_key
 
-    def _get_completion(self, prompt: str) -> str:
+    def _get_completion(self, prompt: str, stop: List[str] = None) -> str:
         """
         Gets completion of prompt using OpenAI API
 
         Args:
             prompt: ChatGPT prompt
+            stop: Stop chars
 
         Returns:
             ChatGPT response
         """
         max_retries = 5
         retries = 0
         messages = [{"role": "user", "content": prompt}]
 
         while retries < max_retries:
             try:
                 response = openai.ChatCompletion.create(
                     model=self.model,
                     messages=messages,
                     temperature=0,  # TODO: Let user configure temperature??
+                    stop=stop,
                 )
                 return response.choices[0].message["content"]
             except openai.error.APIError:
                 time.sleep(5)
                 retries += 1
 
     def generate_function_docstring(self, source: str) -> dict:
@@ -62,72 +55,58 @@
 
         Args:
             source: The source code of the Python method
 
         Returns:
             A dictionary containing the docstrings generated by ChatGPT
         """
-        while source.endswith("\n"):
-            source = source[:-1]
+        source = source.strip()
+        stripped_source = textwrap.dedent(source)
 
         prompt = (
-            f"Your task is to document the Python function below using"
-            f" {self.docstrings_style} Python docstrings. Output the function with the"
-            f" new docstring. Don't import any additional packages.\n\n"
+            f"{stripped_source} \n\n"
+            f"High quality docstring for the above function."
+            f"Make sure you are using google-style docstrings: \n\n"
+            f'"""'
         )
-        prompt += "\n" + source + "\n"
-
-        # Use ast in this case because it generates a docstring without unintended indentations
-        tree = ast.parse(self._get_completion(prompt))
-        function_docs = [
-            ast.get_docstring(f)
-            for f in ast.walk(tree)
-            if isinstance(f, ast.FunctionDef)
-        ]
-        return {"docstring": f'"""\n{function_docs[0]}\n"""'}
+        stop_words = ["#", '"""']
+        return {
+            "docstring": f'"""\n{self._get_completion(prompt, stop=stop_words)}\n"""'
+        }
 
     def generate_class_docstring(self, source: str) -> dict:
         """
         Generates docstring for Python class
 
         Args:
             source: The source code of the Python class
 
         Returns:
             A dictionary like the following:
 
                 {'docstring': <class docstring>, '<method1's name>': <docstring for method1>, ...}
         """
-        while source.endswith("\n"):
-            source = source[:-1]
+        source = source.strip()
+        stripped_source = textwrap.dedent(source)
 
         prompt = (
-            f"Your task is to document the Python class delimited by triple quotes using"
-            f" {self.docstrings_style} Python docstrings. Output the class with the new"
-            f" docstrings. Don't import any additional packages.\n\n"
+            f"Create elaborate, high quality docstrings for the Python class below."
+            f"Make sure you are using google-style docstrings."
+            f"The output is the Python class with the new docstrings. \n\n"
+            f" {stripped_source} \n"
         )
-        prompt += "'''\n" + source + "\n'''"
 
         docstrings = {}
 
         # Use ast in this case because it generates a docstring without unintended indentations
         tree = ast.parse(self._get_completion(prompt))
         class_node = [c for c in ast.walk(tree) if isinstance(c, ast.ClassDef)][0]
         method_nodes = [
             f for f in ast.walk(class_node) if isinstance(f, ast.FunctionDef)
         ]
 
         for method_node in method_nodes:
-            # TODO: This sucks right now because we need to manually modify the indentation.
-            #  Need to think about some clever way to obtain the docstrings with the correct indentation
-            method_docstring = f'"""\n{ast.get_docstring(method_node)}\n"""'
-            indented_method_docstring = ""
-            for doc_line in method_docstring.split("\n"):
-                # TODO: Right now I have to add tabs instead of spaces which generates a
-                #  `PEP 8: W191 indentation contains tabs`. Right now the way to fix this is to manually
-                #  refactor the classes or to use tools like `black` for code formatting.
-                indented_method_docstring += "\t" + doc_line + "\n"
-            docstrings[method_node.name] = indented_method_docstring
+            docstrings[method_node.name] = f'"""\n{ast.get_docstring(method_node)}\n"""'
 
         docstrings["docstring"] = f'"""\n{ast.get_docstring(class_node)}\n"""'
 
         return docstrings
```

### Comparing `gpt4docstrings-0.0.4/src/gpt4docstrings/generate_docstrings.py` & `gpt4docstrings-0.0.5/src/gpt4docstrings/generate_docstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 
 class GPT4Docstrings:
     def __init__(
         self,
         paths: Union[str, List[str]],
         excluded=None,
         model: str = "gpt-3.5-turbo",
-        docstrings_style: str = "google",
         api_key: str = None,
     ):
         self.paths = paths
         self.excluded = excluded or ()
         self.common_base = pathlib.Path("/")
         self.docstring_generator = ChatGPTDocstringGenerator(
-            api_key=api_key, model=model, docstrings_style=docstrings_style
+            api_key=api_key, model=model
         )
 
     def _filter_files(self, files: List[str]):
         """
         Filter files that are explicitly excluded
 
         Args:
@@ -59,15 +58,18 @@
         """
         filenames = []
 
         for path in self.paths:
             if os.path.isfile(path):
                 if not path.endswith(".py"):
                     return sys.exit(1)
-                filenames.append(path)
+
+                if not any(fnmatch(path, exc + "*") for exc in self.excluded):
+                    filenames.append(path)
+
                 continue
 
             for root, _, fs in os.walk(path):
                 full_paths = [os.path.join(root, f) for f in fs]
                 filenames.extend(self._filter_files(full_paths))
 
         if not filenames:
@@ -106,14 +108,15 @@
                         method_node.type == "def"
                         and not utils.check_is_private_method(method_node)
                         and not method_node.value[0].type == "string"
                     ):
                         method_node.value.insert(0, docstring_dict[method_node.name])
 
         utils.write_updated_source_to_file(source, filename)
+        os.system(f"docformatter --in-place {filename}")
 
     def _generate_docstrings(self, filenames: List[str]):
         """
         Traverses the filenames and generate docstrings for undocumented classes / functions
         inside each file.
 
         Args:
@@ -122,7 +125,8 @@
         for filename in filenames:
             self._generate_file_docstrings(filename)
 
     def generate_docstrings(self):
         """Generates docstrings for undocumented classes / functions"""
         filenames = self.get_filenames_from_paths()
         self._generate_docstrings(filenames)
+        return filenames
```

### Comparing `gpt4docstrings-0.0.4/src/gpt4docstrings/utils.py` & `gpt4docstrings-0.0.5/src/gpt4docstrings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.4/PKG-INFO` & `gpt4docstrings-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: gpt4docstrings
-Version: 0.0.4
+Version: 0.0.5
 Summary: gpt4docstrings
 Home-page: https://github.com/MichaelisTrofficus/gpt4docstrings
 License: MIT
 Author: Miguel Otero Pedrido
 Author-email: miguel.otero.pedrido.1993@gmail.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: docformatter (>=1.7.3,<2.0.0)
 Requires-Dist: nox (>=2023.4.22,<2024.0.0)
 Requires-Dist: nox-poetry (>=1.0.2,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pyment (>=0.3.3,<0.4.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: redbaron (>=0.9.2,<0.10.0)
 Project-URL: Changelog, https://github.com/MichaelisTrofficus/gpt4docstrings/releases
 Project-URL: Documentation, https://gpt4docstrings.readthedocs.io
 Project-URL: Repository, https://github.com/MichaelisTrofficus/gpt4docstrings
 Description-Content-Type: text/markdown
```

