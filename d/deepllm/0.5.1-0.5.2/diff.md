# Comparing `tmp/deepllm-0.5.1.tar.gz` & `tmp/deepllm-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-0.5.1.tar", last modified: Tue Jul  4 06:19:35 2023, max compression
+gzip compressed data, was "deepllm-0.5.2.tar", last modified: Tue Jul  4 19:47:56 2023, max compression
```

## Comparing `deepllm-0.5.1.tar` & `deepllm-0.5.2.tar`

### file list

```diff
@@ -1,56 +1,54 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.246570 deepllm-0.5.1/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.1/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     3440 2023-07-04 06:19:35.246267 deepllm-0.5.1/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     3157 2023-07-04 06:16:09.000000 deepllm-0.5.1/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.226671 deepllm-0.5.1/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)      182 2023-07-03 05:35:16.000000 deepllm-0.5.1/deepllm/__init__.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.229816 deepllm-0.5.1/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.1/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.1/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.1/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.1/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.232501 deepllm-0.5.1/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.1/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.1/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.1/deepllm/demos/demo.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.1/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       45 2023-07-03 02:33:17.000000 deepllm-0.5.1/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.1/deepllm/demos/wikifetch.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.233029 deepllm-0.5.1/deepllm/docs/
--rw-r--r--   0 tarau      (503) staff       (20)  1240180 2023-06-24 23:00:50.000000 deepllm-0.5.1/deepllm/docs/recursor.pdf
--rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.1/deepllm/embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.1/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.1/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.240308 deepllm-0.5.1/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.1/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.1/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.1/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.1/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.1/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.1/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.1/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     2789 2023-07-03 05:51:27.000000 deepllm-0.5.1/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     5811 2023-07-01 18:32:07.000000 deepllm-0.5.1/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     6620 2023-07-03 04:01:40.000000 deepllm-0.5.1/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     4079 2023-07-03 04:04:23.000000 deepllm-0.5.1/deepllm/refiners.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.245636 deepllm-0.5.1/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.1/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.1/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.1/deepllm/tests/test_all.sh
--rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.1/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.1/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.1/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.1/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.1/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.1/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2261 2023-07-03 04:06:01.000000 deepllm-0.5.1/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.1/deepllm/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 06:19:35.228435 deepllm-0.5.1/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     3440 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1201 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-04 06:19:35.000000 deepllm-0.5.1/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-04 06:19:35.246688 deepllm-0.5.1/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      920 2023-07-03 03:20:31.000000 deepllm-0.5.1/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.749222 deepllm-0.5.2/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.2/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     3440 2023-07-04 19:47:56.748920 deepllm-0.5.2/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     3157 2023-07-04 06:16:09.000000 deepllm-0.5.2/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.735948 deepllm-0.5.2/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)      182 2023-07-04 19:36:17.000000 deepllm-0.5.2/deepllm/__init__.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.738261 deepllm-0.5.2/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.2/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.2/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.2/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.2/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.740686 deepllm-0.5.2/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.2/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.2/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.2/deepllm/demos/demo.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.2/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       45 2023-07-03 02:33:17.000000 deepllm-0.5.2/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.2/deepllm/demos/wikifetch.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.2/deepllm/embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.2/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.2/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.743748 deepllm-0.5.2/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.2/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.2/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.2/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.2/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.2/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.2/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.2/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2789 2023-07-03 05:51:27.000000 deepllm-0.5.2/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     5811 2023-07-01 18:32:07.000000 deepllm-0.5.2/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6620 2023-07-03 04:01:40.000000 deepllm-0.5.2/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4079 2023-07-03 04:04:23.000000 deepllm-0.5.2/deepllm/refiners.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.748278 deepllm-0.5.2/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.2/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.2/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.2/deepllm/tests/test_all.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.2/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.2/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.2/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.2/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.2/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.2/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2261 2023-07-03 04:06:01.000000 deepllm-0.5.2/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.2/deepllm/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-04 19:47:56.737277 deepllm-0.5.2/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     3440 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1175 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-04 19:47:56.000000 deepllm-0.5.2/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-04 19:47:56.749328 deepllm-0.5.2/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      920 2023-07-03 03:20:31.000000 deepllm-0.5.2/setup.py
```

### Comparing `deepllm-0.5.1/LICENSE` & `deepllm-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/PKG-INFO` & `deepllm-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.1
+Version: 0.5.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.5.1/README.md` & `deepllm-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/configurator.py` & `deepllm-0.5.2/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/demos/demo.py` & `deepllm-0.5.2/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/demos/wikifetch.py` & `deepllm-0.5.2/deepllm/demos/wikifetch.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/embedders.py` & `deepllm-0.5.2/deepllm/embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/horn_prover.py` & `deepllm-0.5.2/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/interactors.py` & `deepllm-0.5.2/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/local_llms/local_runs.py` & `deepllm-0.5.2/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/local_llms/test_vicuna.py` & `deepllm-0.5.2/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/params.py` & `deepllm-0.5.2/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/prompters.py` & `deepllm-0.5.2/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/recursors.py` & `deepllm-0.5.2/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/refiners.py` & `deepllm-0.5.2/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/tests/test_recursors.py` & `deepllm-0.5.2/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/tests/test_refiners.py` & `deepllm-0.5.2/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm/tools.py` & `deepllm-0.5.2/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.1/deepllm.egg-info/PKG-INFO` & `deepllm-0.5.2/deepllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.1
+Version: 0.5.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.5.1/deepllm.egg-info/SOURCES.txt` & `deepllm-0.5.2/deepllm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 deepllm/apps/requirements.txt
 deepllm/demos/README.md
 deepllm/demos/__init__.py
 deepllm/demos/demo.py
 deepllm/demos/install.sh
 deepllm/demos/requirements.txt
 deepllm/demos/wikifetch.py
-deepllm/docs/recursor.pdf
 deepllm/local_llms/README.md
 deepllm/local_llms/__init__.py
 deepllm/local_llms/install.sh
 deepllm/local_llms/local_runs.py
 deepllm/local_llms/requirements.txt
 deepllm/local_llms/server.sh
 deepllm/local_llms/test_vicuna.py
```

### Comparing `deepllm-0.5.1/setup.py` & `deepllm-0.5.2/setup.py`

 * *Files identical despite different names*

