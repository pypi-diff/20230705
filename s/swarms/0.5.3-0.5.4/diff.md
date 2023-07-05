# Comparing `tmp/swarms-0.5.3.tar.gz` & `tmp/swarms-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.5.3.tar", last modified: Tue Jul  4 23:39:09 2023, max compression
+gzip compressed data, was "swarms-0.5.4.tar", last modified: Wed Jul  5 03:15:49 2023, max compression
```

## Comparing `swarms-0.5.3.tar` & `swarms-0.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.651199 swarms-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 23:39:00.000000 swarms-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 23:39:09.647199 swarms-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 23:39:00.000000 swarms-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-04 23:39:00.000000 swarms-0.5.3/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 23:39:00.000000 swarms-0.5.3/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 23:39:00.000000 swarms-0.5.3/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 23:39:09.651199 swarms-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-04 23:39:00.000000 swarms-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 23:39:00.000000 swarms-0.5.3/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:39:09.647199 swarms-0.5.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 23:39:09.000000 swarms-0.5.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.742355 swarms-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 03:15:38.000000 swarms-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 03:15:49.742355 swarms-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-07-05 03:15:38.000000 swarms-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:38.000000 swarms-0.5.4/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 03:15:38.000000 swarms-0.5.4/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-05 03:15:38.000000 swarms-0.5.4/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 03:15:38.000000 swarms-0.5.4/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:15:49.742355 swarms-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 03:15:38.000000 swarms-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.742355 swarms-0.5.4/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.742355 swarms-0.5.4/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-05 03:15:38.000000 swarms-0.5.4/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:15:49.738355 swarms-0.5.4/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 03:15:49.000000 swarms-0.5.4/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-05 03:15:49.000000 swarms-0.5.4/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:15:49.000000 swarms-0.5.4/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 03:15:49.000000 swarms-0.5.4/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 03:15:49.000000 swarms-0.5.4/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.5.3/LICENSE` & `swarms-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/PKG-INFO` & `swarms-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.3
+Version: 0.5.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.3/README.md` & `swarms-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,39 +67,28 @@
 ```bash
 git clone https://github.com/kyegomez/swarms.git
 cd swarms
 pip install -r requirements.txt
 ```
 
 # Method 3
-Simple example by `git cloning https://github.com/kyegomez/swarms.git` `python3 example.py`
+Simple example by:
 
+* `git cloning https://github.com/kyegomez/swarms.git`
 
-## BossNode
+* `cd swarms`
 
-The `BossNode` class is a key component of Swarms. It represents a "boss" in the system that assigns tasks to other components.
+* `python3 -m pip install -r requirements.txt`
 
-Here is an example of how you can use it:
+* `python3 example.py`
 
-```python
-class BossNode:
-    def __init__(self, tools):
-        # initialization code goes here
-
-    def create_task(self, objective):
-        return {"objective": objective}
-
-    def execute_task(self, task):
-        # task execution code goes here
-```
-
-With the `BossNode` class, you can create tasks for your tools to perform. For example, you can create a task to write a summary of a specific topic:
+* or create a new file:
 
 ```python
-from swarms import Swarms
+from swarms.swarms import Swarms
 
 # Retrieve your API key from the environment or replace with your actual key
 api_key = "sksdsds"
 
 # Initialize Swarms with your API key
 swarm = Swarms(openai_api_key=api_key)
```

### Comparing `swarms-0.5.3/api/container.py` & `swarms-0.5.4/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/api/main.py` & `swarms-0.5.4/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/api/worker.py` & `swarms-0.5.4/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/setup.py` & `swarms-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.5.3',
+  version = '0.5.4',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.5.3/swarms/agents/swarms.py` & `swarms-0.5.4/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/agents/workers/agents.py` & `swarms-0.5.4/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/agents/workers/auto_agent.py` & `swarms-0.5.4/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.5.4/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/agents/workers/multi_modal.py` & `swarms-0.5.4/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/agents/workers/omni_agent.py` & `swarms-0.5.4/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/prompts/prompts.py` & `swarms-0.5.4/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/tools/main.py` & `swarms-0.5.4/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/utils/ansi.py` & `swarms-0.5.4/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms/utils/utils.py` & `swarms-0.5.4/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms.egg-info/PKG-INFO` & `swarms-0.5.4/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.3
+Version: 0.5.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.3/swarms.egg-info/SOURCES.txt` & `swarms-0.5.4/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.5.3/swarms.egg-info/requires.txt` & `swarms-0.5.4/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

