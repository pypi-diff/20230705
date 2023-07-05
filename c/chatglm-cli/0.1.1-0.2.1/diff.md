# Comparing `tmp/chatglm-cli-0.1.1.tar.gz` & `tmp/chatglm-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-cli-0.1.1.tar", last modified: Fri Jun 30 08:01:05 2023, max compression
+gzip compressed data, was "chatglm-cli-0.2.1.tar", last modified: Wed Jul  5 01:31:55 2023, max compression
```

## Comparing `chatglm-cli-0.1.1.tar` & `chatglm-cli-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318636 chatglm-cli-0.1.1/
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-30 08:01:05.318528 chatglm-cli-0.1.1/PKG-INFO
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318168 chatglm-cli-0.1.1/chatglm_cli.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      295 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       47 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:31:18.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)       26 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       11 2023-06-30 08:01:05.000000 chatglm-cli-0.1.1/chatglm_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-30 08:01:05.318372 chatglm-cli-0.1.1/chatglmcli/
--rw-r--r--   0 mroy       (501) staff       (20)        0 2023-06-28 09:19:02.000000 chatglm-cli-0.1.1/chatglmcli/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     3856 2023-06-30 08:00:44.000000 chatglm-cli-0.1.1/chatglmcli/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-30 08:01:05.318674 chatglm-cli-0.1.1/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1200 2023-06-30 08:01:00.000000 chatglm-cli-0.1.1/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-05 01:31:55.064793 chatglm-cli-0.2.1/
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-07-05 01:31:55.064659 chatglm-cli-0.2.1/PKG-INFO
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-05 01:31:55.064260 chatglm-cli-0.2.1/chatglm_cli.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-07-05 01:31:54.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      295 2023-07-05 01:31:55.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-05 01:31:54.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       47 2023-07-05 01:31:54.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:31:18.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)       26 2023-07-05 01:31:54.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       11 2023-07-05 01:31:55.000000 chatglm-cli-0.2.1/chatglm_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-05 01:31:55.064473 chatglm-cli-0.2.1/chatglmcli/
+-rw-r--r--   0 mroy       (501) staff       (20)        0 2023-06-28 09:19:02.000000 chatglm-cli-0.2.1/chatglmcli/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3856 2023-06-30 08:00:44.000000 chatglm-cli-0.2.1/chatglmcli/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-05 01:31:55.064840 chatglm-cli-0.2.1/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1200 2023-07-05 01:31:51.000000 chatglm-cli-0.2.1/setup.py
```

### Comparing `chatglm-cli-0.1.1/chatglmcli/cmd.py` & `chatglm-cli-0.2.1/chatglmcli/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-cli-0.1.1/setup.py` & `chatglm-cli-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-cli',
-    version='0.1.1',
+    version='0.2.1',
     description='chatglm llm cli',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
@@ -35,15 +35,15 @@
         # 'numpy',
         # 'pypdf',
         # "scikit-learn",
         # 'langchain',
         # 'websockets',
         # 'websocket-client',
         'gradio',
-        'chatglm-llm>=1.4.3',
+        'chatglm-llm>=1.4.4',
         # 'unstructured',
         # 'aiowebsocket',
         ],
     entry_points={
         'console_scripts': [
             'ai-cli=chatglmcli.cmd:main',
         ]
```

