# Comparing `tmp/swarms-0.5.6.tar.gz` & `tmp/swarms-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.5.6.tar", last modified: Wed Jul  5 03:54:53 2023, max compression
+gzip compressed data, was "swarms-0.5.7.tar", last modified: Wed Jul  5 12:23:42 2023, max compression
```

## Comparing `swarms-0.5.6.tar` & `swarms-0.5.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.776823 swarms-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 03:54:41.000000 swarms-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 03:54:53.776823 swarms-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-07-05 03:54:41.000000 swarms-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:41.000000 swarms-0.5.6/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 03:54:41.000000 swarms-0.5.6/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-05 03:54:41.000000 swarms-0.5.6/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 03:54:41.000000 swarms-0.5.6/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:54:53.776823 swarms-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 03:54:41.000000 swarms-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.776823 swarms-0.5.6/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-05 03:54:41.000000 swarms-0.5.6/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:54:53.772822 swarms-0.5.6/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 03:54:53.000000 swarms-0.5.6/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-05 03:54:53.000000 swarms-0.5.6/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:54:53.000000 swarms-0.5.6/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 03:54:53.000000 swarms-0.5.6/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 03:54:53.000000 swarms-0.5.6/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.245817 swarms-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:23:32.000000 swarms-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:23:42.245817 swarms-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-07-05 12:23:32.000000 swarms-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:32.000000 swarms-0.5.7/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 12:23:32.000000 swarms-0.5.7/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-05 12:23:32.000000 swarms-0.5.7/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:23:32.000000 swarms-0.5.7/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:23:42.245817 swarms-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 12:23:32.000000 swarms-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34557 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.245817 swarms-0.5.7/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-05 12:23:32.000000 swarms-0.5.7/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:23:42.241817 swarms-0.5.7/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:23:42.000000 swarms-0.5.7/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.5.6/LICENSE` & `swarms-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/PKG-INFO` & `swarms-0.5.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.6
+Version: 0.5.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.6/README.md` & `swarms-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/api/container.py` & `swarms-0.5.7/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/api/main.py` & `swarms-0.5.7/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/api/worker.py` & `swarms-0.5.7/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/setup.py` & `swarms-0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.5.6',
+  version = '0.5.7',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.5.6/swarms/agents/swarms.py` & `swarms-0.5.7/swarms/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/agents/workers/agents.py` & `swarms-0.5.7/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/agents/workers/auto_agent.py` & `swarms-0.5.7/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.5.7/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/agents/workers/multi_modal.py` & `swarms-0.5.7/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/agents/workers/omni_agent.py` & `swarms-0.5.7/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/prompts/prompts.py` & `swarms-0.5.7/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/tools/main.py` & `swarms-0.5.7/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/utils/ansi.py` & `swarms-0.5.7/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms/utils/utils.py` & `swarms-0.5.7/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.6/swarms.egg-info/PKG-INFO` & `swarms-0.5.7/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.6
+Version: 0.5.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.6/swarms.egg-info/SOURCES.txt` & `swarms-0.5.7/swarms.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 README.md
 setup.py
 api/__init__.py
 api/container.py
 api/main.py
 api/worker.py
 swarms/__init__.py
+swarms/swarms.py
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
-swarms/agents/swarms.py
 swarms/agents/workers/__init__.py
 swarms/agents/workers/agents.py
 swarms/agents/workers/auto_agent.py
 swarms/agents/workers/metaprompt_agent.py
 swarms/agents/workers/multi_modal.py
 swarms/agents/workers/omni_agent.py
 swarms/agents/workers/models/__init__.py
```

### Comparing `swarms-0.5.6/swarms.egg-info/requires.txt` & `swarms-0.5.7/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

