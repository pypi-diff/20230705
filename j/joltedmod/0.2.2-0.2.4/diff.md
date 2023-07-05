# Comparing `tmp/joltedmod-0.2.2.tar.gz` & `tmp/joltedmod-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.2.2.tar", max compression
+gzip compressed data, was "joltedmod-0.2.4.tar", max compression
```

## Comparing `joltedmod-0.2.2.tar` & `joltedmod-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,44 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.2.2/LICENSE
--rw-r--r--   0        0        0     2012 2023-06-18 07:56:10.874764 joltedmod-0.2.2/README.md
--rw-r--r--   0        0        0     1344 2023-06-17 15:04:17.835987 joltedmod-0.2.2/jolted_mod/LLM_service.py
--rw-r--r--   0        0        0      412 2023-06-18 14:40:05.820570 joltedmod-0.2.2/jolted_mod/__init__.py
--rw-r--r--   0        0        0     3749 2023-06-18 08:19:58.255349 joltedmod-0.2.2/jolted_mod/block.py
--rw-r--r--   0        0        0      606 2023-06-18 08:18:31.554627 joltedmod-0.2.2/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.2.2/jolted_mod/cell_type.py
--rw-r--r--   0        0        0     1934 2023-06-17 17:42:19.311605 joltedmod-0.2.2/jolted_mod/config.py
--rw-r--r--   0        0        0     7925 2023-06-18 08:24:25.496650 joltedmod-0.2.2/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     4855 2023-06-18 08:25:07.509677 joltedmod-0.2.2/jolted_mod/main.py
--rw-r--r--   0        0        0       93 2023-06-17 15:54:34.751488 joltedmod-0.2.2/jolted_mod/module_types.py
--rw-r--r--   0        0        0     9644 2023-06-18 14:57:03.509185 joltedmod-0.2.2/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      685 2023-06-18 15:03:38.707349 joltedmod-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 joltedmod-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2012 2023-06-18 07:56:10.874764 joltedmod-0.2.4/README.md
+-rw-r--r--   0        0        0     1344 2023-06-17 15:04:17.835987 joltedmod-0.2.4/jolted_mod/LLM_service.py
+-rw-r--r--   0        0        0      412 2023-06-18 14:40:05.820570 joltedmod-0.2.4/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     3749 2023-06-18 08:19:58.255349 joltedmod-0.2.4/jolted_mod/block.py
+-rw-r--r--   0        0        0      606 2023-06-18 08:18:31.554627 joltedmod-0.2.4/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.2.4/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0     2102 2023-07-05 18:05:53.162269 joltedmod-0.2.4/jolted_mod/config.py
+-rw-r--r--   0        0        0     7925 2023-06-18 08:24:25.496650 joltedmod-0.2.4/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0    20224 2023-06-19 18:39:34.754832 joltedmod-0.2.4/jolted_mod/fastapi_python.ipynb
+-rw-r--r--   0        0        0    43167 2023-06-24 09:02:00.552102 joltedmod-0.2.4/jolted_mod/intro_loops_python.html
+-rw-r--r--   0        0        0    16223 2023-06-19 18:43:26.812902 joltedmod-0.2.4/jolted_mod/intro_loops_python.ipynb
+-rw-r--r--   0        0        0    95517 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0        0        0   164168 2023-06-23 18:52:58.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0        0        0   256782 2023-06-24 09:01:59.570000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0        0        0    78129 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/bootstrap/bootstrap.min.js
+-rw-r--r--   0        0        0     9160 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/clipboard/clipboard.min.js
+-rw-r--r--   0        0        0     6008 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/anchor.min.js
+-rw-r--r--   0        0        0    19728 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/popper.min.js
+-rw-r--r--   0        0        0     3135 2023-06-24 09:01:59.661000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0        0        0    28407 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/quarto.js
+-rw-r--r--   0        0        0     1409 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/tippy.css
+-rw-r--r--   0        0        0    24033 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/intro_loops_python_files/libs/quarto-html/tippy.umd.min.js
+-rw-r--r--   0        0        0     5063 2023-06-24 09:14:22.585835 joltedmod-0.2.4/jolted_mod/main.py
+-rw-r--r--   0        0        0       93 2023-06-17 15:54:34.751488 joltedmod-0.2.4/jolted_mod/module_types.py
+-rw-r--r--   0        0        0    20175 2023-06-19 18:32:05.065376 joltedmod-0.2.4/jolted_mod/nosql_mongo_gpt4.ipynb
+-rw-r--r--   0        0        0    67402 2023-06-24 09:24:16.710929 joltedmod-0.2.4/jolted_mod/quarto.html
+-rw-r--r--   0        0        0    22854 2023-06-24 09:17:52.842055 joltedmod-0.2.4/jolted_mod/quarto.ipynb
+-rw-r--r--   0        0        0    95517 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0        0        0   164168 2023-06-23 18:52:58.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0        0        0   256782 2023-06-24 09:24:15.751000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0        0        0    78129 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/bootstrap/bootstrap.min.js
+-rw-r--r--   0        0        0     9160 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/clipboard/clipboard.min.js
+-rw-r--r--   0        0        0     6008 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/anchor.min.js
+-rw-r--r--   0        0        0    19728 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/popper.min.js
+-rw-r--r--   0        0        0     3135 2023-06-24 09:01:59.661000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0        0        0    28407 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/quarto.js
+-rw-r--r--   0        0        0     1409 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/tippy.css
+-rw-r--r--   0        0        0    24033 2023-06-23 18:53:18.000000 joltedmod-0.2.4/jolted_mod/quarto_files/libs/quarto-html/tippy.umd.min.js
+-rw-r--r--   0        0        0    21045 2023-06-19 18:57:05.606905 joltedmod-0.2.4/jolted_mod/react_typescript.ipynb
+-rw-r--r--   0        0        0     9644 2023-06-18 14:57:03.509185 joltedmod-0.2.4/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0     2321 2023-06-17 21:00:10.332482 joltedmod-0.2.4/jolted_mod/tutorial_template.json
+-rw-r--r--   0        0        0      685 2023-07-05 18:06:27.588677 joltedmod-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 joltedmod-0.2.4/PKG-INFO
```

### Comparing `joltedmod-0.2.2/LICENSE` & `joltedmod-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/README.md` & `joltedmod-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/jolted_mod/LLM_service.py` & `joltedmod-0.2.4/jolted_mod/LLM_service.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/jolted_mod/block.py` & `joltedmod-0.2.4/jolted_mod/block.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/jolted_mod/block_factory.py` & `joltedmod-0.2.4/jolted_mod/block_factory.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/jolted_mod/config.py` & `joltedmod-0.2.4/jolted_mod/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 prompts = {
     "SeedBlock": "Produce output for a textbook or tutorial module as written by a {identity} who is explaining {topic} to {target_audience}",
 
     "ExplanatoryBlock": "This is a {type_of_cell} block in a Jupyter Notebook. Use appropriate headers for chapter sections if of type Markdown. Do not give solutions if this is a Code block. Explain {topic} by {instructional_event} in a way that is relatable to {target_audience}. Be careful not to be overly dramatic and not to talk down to the audience.",
 
-    "ExplanatoryBlockKC": "You are producing a jupyter notebook based tutorial for {target_audience} about {knowledge_component} by {instructional_event}. Assume your output is part of a tutorial that covers the other aspects of {topic}. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
+    "ExplanatoryBlockKC": "You are producing a jupyter notebook based tutorial for {target_audience} about {knowledge_component} by {instructional_event} relevant to the student's background knowledge and expertise. Scale the complexity of the content to the level of expertise of the student. Assume your output is part of a tutorial that covers the other aspects of {topic}. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
 
     "KnowledgeTestingBlock": {
         "markdown": "Design {n} {question_type} of an appropriate difficulty for {target_audience} about that {topic}",
         "code": "Create code with empty methods that have comments for what they should do but no implementation to answer the following question: {context_content}. After that, create 3 assertion tests that the student will use to test if they have implemented their solution correctly",
     },
 
     "KnowledgeTestingBlockKC": {
-        "markdown": "Design {n} {question_type} of an appropriate difficulty for {target_audience} about that {knowledge_component}. Do not produce a solution, just the question. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
+        "markdown": "Design {n} {question_type} of an appropriate difficulty and relevant to the interests of {target_audience} about that {knowledge_component}. Do not produce a solution, just the question. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
         "code": "Create code with empty methods that have comments for what they should do but no implementation to answer the following question: {context_content}. After that, create 3 assertion tests that the student will use to test if they have implemented their solution correctly",
     },
 
 }
```

### Comparing `joltedmod-0.2.2/jolted_mod/content_generator.py` & `joltedmod-0.2.4/jolted_mod/content_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/jolted_mod/main.py` & `joltedmod-0.2.4/jolted_mod/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jolted_mod.template_generator import TemplateGenerator
 from jolted_mod.content_generator import ContentGenerator
 from typing import Any, Dict, Optional
 from jolted_mod.module_types import ModuleType
 import asyncio
 
-# import nbformat as nbf
+import nbformat as nbf
 
 
 class JoltedModException(Exception):
     """
     Custom exception type for Jolted Mod.
     """
 
@@ -22,15 +22,15 @@
     try:
         template_generator = TemplateGenerator(topic, identity, target_audience)
         template = template_generator.create_template(
             code=is_code, template_type="notebook"
         )
         return template
     except Exception as e:
-        raise Exception(f"Error occurred: {e}")
+        raise JoltedModException(f"template failed to generate: {e}")
         return {}
 
 
 async def create_notebook_module(
     topic: str,
     identity: str = "professor of computer science",
     target_audience: str = "first year computer science students",
@@ -54,15 +54,15 @@
     try:
         # Generate cell content using the ContentGenerator
         cg = ContentGenerator(model=model)
         tutorial_content = await cg.create_module(template, type=ModuleType.NOTEBOOK)
     except Exception as e:
         raise JoltedModException("Error generating notebook content.") from e
 
-    # nbf.write(tutorial_content, "test.ipynb")
+    nbf.write(tutorial_content, "test.ipynb")
     return tutorial_content
 
 
 async def create_wiki_module(
     topic: str,
     identity: str = "professor of computer science",
     target_audience: str = "first year computer science students",
@@ -135,8 +135,14 @@
             }
         curriculum[topic_name] = topic_content
     return curriculum
 
 
 if __name__ == "__main__":
     # asyncio.run(create_notebook_module("Intro to for loops in python", model="gpt-4"))
-    asyncio.run(create_notebook_module("Intro to for loops in python", model="gpt-4"))
+    asyncio.run(
+        create_notebook_module(
+            topic="Intro to quarto for creating open source textbooks",
+            target_audience="attendees of the society for the improvement of psychological sciences conference",
+            model="gpt-4",
+        )
+    )
```

### Comparing `joltedmod-0.2.2/jolted_mod/template_generator.py` & `joltedmod-0.2.4/jolted_mod/template_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.2/pyproject.toml` & `joltedmod-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.2.2"
+version = "0.2.4"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
 license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
```

### Comparing `joltedmod-0.2.2/PKG-INFO` & `joltedmod-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joltedmod
-Version: 0.2.2
+Version: 0.2.4
 Summary: JoltEd self-documenting learning module
 License: MIT
 Author: Nathan Laundry
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

