# Comparing `tmp/swarms-0.5.7.tar.gz` & `tmp/swarms-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.5.7.tar", last modified: Wed Jul  5 12:23:42 2023, max compression
+gzip compressed data, was "swarms-0.5.8.tar", last modified: Wed Jul  5 12:31:57 2023, max compression
```

## Comparing `swarms-0.5.7.tar` & `swarms-0.5.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.245817 swarms-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:23:32.000000 swarms-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:23:42.245817 swarms-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-07-05 12:23:32.000000 swarms-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:32.000000 swarms-0.5.7/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 12:23:32.000000 swarms-0.5.7/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-05 12:23:32.000000 swarms-0.5.7/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:23:32.000000 swarms-0.5.7/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:23:42.245817 swarms-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 12:23:32.000000 swarms-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.245817 swarms-0.5.7/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.069546 swarms-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:31:45.000000 swarms-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:31:57.069546 swarms-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-07-05 12:31:45.000000 swarms-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.061546 swarms-0.5.8/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:45.000000 swarms-0.5.8/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 12:31:45.000000 swarms-0.5.8/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-05 12:31:45.000000 swarms-0.5.8/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:31:45.000000 swarms-0.5.8/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:31:57.069546 swarms-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 12:31:45.000000 swarms-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.061546 swarms-0.5.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.065546 swarms-0.5.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.065546 swarms-0.5.8/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.065546 swarms-0.5.8/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.065546 swarms-0.5.8/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.069546 swarms-0.5.8/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.069546 swarms-0.5.8/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-05 12:31:45.000000 swarms-0.5.8/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:31:57.065546 swarms-0.5.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:31:57.000000 swarms-0.5.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 12:31:57.000000 swarms-0.5.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:31:57.000000 swarms-0.5.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 12:31:57.000000 swarms-0.5.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:31:57.000000 swarms-0.5.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.5.7/LICENSE` & `swarms-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/PKG-INFO` & `swarms-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.7
+Version: 0.5.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.7/README.md` & `swarms-0.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,16 @@
 5. **Earn Rewards**: If your contribution is approved, you'll earn a bounty. The amount of the bounty depends on the complexity of the task, the quality of your work, and the value it brings to Swarms.
 
 ## The Three Phases of Our Bounty Program
 
 ### Phase 1: Building the Foundation
 In the first phase, our focus is on building the basic infrastructure of Swarms. This includes developing key components like the Swarms class, integrating essential tools, and establishing task completion and evaluation logic. We'll also start developing our testing and evaluation framework during this phase. If you're interested in foundational work and have a knack for building robust, scalable systems, this phase is for you.
 
-### Phase 2: Enhancing the System
-In the second phase, we'll focus on enhancing Swarms by integrating more advanced features, improving the system's efficiency, and refining our testing and evaluation framework. This phase involves more complex tasks, so if you enjoy tackling challenging problems and contributing to the development of innovative features, this is the phase for you.
+### Phase 2: Optimizing the System
+In the second phase, we'll focus on optimizng Swarms by integrating more advanced features, improving the system's efficiency, and refining our testing and evaluation framework. This phase involves more complex tasks, so if you enjoy tackling challenging problems and contributing to the development of innovative features, this is the phase for you.
 
 ### Phase 3: Towards Super-Intelligence
 The third phase of our bounty program is the most exciting - this is where we aim to achieve super-intelligence. In this phase, we'll be working on improving the swarm's capabilities, expanding its skills, and fine-tuning the system based on real-world testing and feedback. If you're excited about the future of AI and want to contribute to a project that could potentially transform the digital world, this is the phase for you.
 
 Remember, our roadmap is a guide, and we encourage you to bring your own ideas and creativity to the table. We believe that every contribution, no matter how small, can make a difference. So join us on this exciting journey and help us create the future of Swarms.
 
 <!-- **To participate in our bounty program, visit the [Swarms Bounty Program Page](https://swarms.ai/bounty).** Let's build the future together! -->
```

### Comparing `swarms-0.5.7/api/container.py` & `swarms-0.5.8/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/api/main.py` & `swarms-0.5.8/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/api/worker.py` & `swarms-0.5.8/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/setup.py` & `swarms-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.5.7',
+  version = '0.5.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.5.7/swarms/agents/workers/agents.py` & `swarms-0.5.8/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/agents/workers/auto_agent.py` & `swarms-0.5.8/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.5.8/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/agents/workers/multi_modal.py` & `swarms-0.5.8/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/agents/workers/omni_agent.py` & `swarms-0.5.8/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/prompts/prompts.py` & `swarms-0.5.8/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/swarms.py` & `swarms-0.5.8/swarms/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/tools/main.py` & `swarms-0.5.8/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/utils/ansi.py` & `swarms-0.5.8/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms/utils/utils.py` & `swarms-0.5.8/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms.egg-info/PKG-INFO` & `swarms-0.5.8/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.7
+Version: 0.5.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.7/swarms.egg-info/SOURCES.txt` & `swarms-0.5.8/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.5.7/swarms.egg-info/requires.txt` & `swarms-0.5.8/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

