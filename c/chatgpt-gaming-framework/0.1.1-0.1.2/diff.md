# Comparing `tmp/chatgpt_gaming_framework-0.1.1.tar.gz` & `tmp/chatgpt_gaming_framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_gaming_framework-0.1.1.tar", last modified: Wed Jul  5 12:08:34 2023, max compression
+gzip compressed data, was "chatgpt_gaming_framework-0.1.2.tar", last modified: Wed Jul  5 12:17:52 2023, max compression
```

## Comparing `chatgpt_gaming_framework-0.1.1.tar` & `chatgpt_gaming_framework-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.662993 chatgpt_gaming_framework-0.1.1/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     1204 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/.gitignore
--rw-rw-r--   0 razikus   (1000) razikus   (1000)       91 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/AUTHORS.rst
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     1075 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/LICENSE
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      262 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/MANIFEST.in
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     2366 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/Makefile
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      850 2023-07-05 12:08:34.662993 chatgpt_gaming_framework-0.1.1/PKG-INFO
--rw-rw-r--   0 razikus   (1000) razikus   (1000)       88 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/README.md
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.658993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      156 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/__init__.py
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.658993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/memory/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/memory/__init__.py
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      702 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/memory/redismemory.py
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.658993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/models/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/models/__init__.py
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     3516 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/models/chatgptmodel.py
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.662993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/storyteller/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/storyteller/__init__.py
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     2493 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/storyteller/storyteller.py
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.662993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/types/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/types/__init__.py
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      238 2023-07-05 12:05:35.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/types/types.py
-drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:08:34.658993 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      850 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/PKG-INFO
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      770 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        1 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 razikus   (1000) razikus   (1000)        1 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/not-zip-safe
--rw-rw-r--   0 razikus   (1000) razikus   (1000)       44 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/requires.txt
--rw-rw-r--   0 razikus   (1000) razikus   (1000)       25 2023-07-05 12:08:34.000000 chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/top_level.txt
--rw-rw-r--   0 razikus   (1000) razikus   (1000)      396 2023-07-05 12:08:34.662993 chatgpt_gaming_framework-0.1.1/setup.cfg
--rw-rw-r--   0 razikus   (1000) razikus   (1000)     1302 2023-07-05 12:05:48.000000 chatgpt_gaming_framework-0.1.1/setup.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.775349 chatgpt_gaming_framework-0.1.2/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     1204 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/.gitignore
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)       91 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     1075 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/LICENSE
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      262 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/MANIFEST.in
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     2366 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/Makefile
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      850 2023-07-05 12:17:52.775349 chatgpt_gaming_framework-0.1.2/PKG-INFO
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)       88 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/README.md
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.771349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      156 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/__init__.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.771349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/memory/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/memory/__init__.py
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      702 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/memory/redismemory.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.771349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/models/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/models/__init__.py
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     3516 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/models/chatgptmodel.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.775349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/storyteller/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/storyteller/__init__.py
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     2493 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/storyteller/storyteller.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.775349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/types/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        0 2023-06-26 13:24:06.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/types/__init__.py
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      236 2023-07-05 12:17:39.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/types/types.py
+drwxrwxr-x   0 razikus   (1000) razikus   (1000)        0 2023-07-05 12:17:52.771349 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      850 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      770 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        1 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)        1 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/not-zip-safe
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)       44 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/requires.txt
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)       25 2023-07-05 12:17:52.000000 chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/top_level.txt
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)      396 2023-07-05 12:17:52.775349 chatgpt_gaming_framework-0.1.2/setup.cfg
+-rw-rw-r--   0 razikus   (1000) razikus   (1000)     1302 2023-07-05 12:17:47.000000 chatgpt_gaming_framework-0.1.2/setup.py
```

### Comparing `chatgpt_gaming_framework-0.1.1/.gitignore` & `chatgpt_gaming_framework-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/LICENSE` & `chatgpt_gaming_framework-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/Makefile` & `chatgpt_gaming_framework-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/PKG-INFO` & `chatgpt_gaming_framework-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_gaming_framework
-Version: 0.1.1
+Version: 0.1.2
 Summary: ChatGPT (in future other LLM) gaming framework
 Home-page: https://github.com/Razikus/chatgpt_gaming_framework
 Author: Adam Raźniewski
 Author-email: adam.razniewski@gmail.com
 License: MIT license
 Keywords: chatgpt_gaming_framework
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/memory/redismemory.py` & `chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/memory/redismemory.py`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/models/chatgptmodel.py` & `chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/models/chatgptmodel.py`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework/storyteller/storyteller.py` & `chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework/storyteller/storyteller.py`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/PKG-INFO` & `chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-gaming-framework
-Version: 0.1.1
+Version: 0.1.2
 Summary: ChatGPT (in future other LLM) gaming framework
 Home-page: https://github.com/Razikus/chatgpt_gaming_framework
 Author: Adam Raźniewski
 Author-email: adam.razniewski@gmail.com
 License: MIT license
 Keywords: chatgpt_gaming_framework
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgpt_gaming_framework-0.1.1/chatgpt_gaming_framework.egg-info/SOURCES.txt` & `chatgpt_gaming_framework-0.1.2/chatgpt_gaming_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatgpt_gaming_framework-0.1.1/setup.py` & `chatgpt_gaming_framework-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     include_package_data=True,
     keywords='chatgpt_gaming_framework',
     name='chatgpt_gaming_framework',
     packages=find_packages(include=['chatgpt_gaming_framework', 'chatgpt_gaming_framework.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Razikus/chatgpt_gaming_framework',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

