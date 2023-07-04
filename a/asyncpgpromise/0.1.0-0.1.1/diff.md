# Comparing `tmp/asyncpgpromise-0.1.0.tar.gz` & `tmp/asyncpgpromise-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpgpromise-0.1.0.tar", last modified: Tue Jul  4 21:52:31 2023, max compression
+gzip compressed data, was "asyncpgpromise-0.1.1.tar", last modified: Tue Jul  4 21:59:45 2023, max compression
```

## Comparing `asyncpgpromise-0.1.0.tar` & `asyncpgpromise-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:52:31.134729 asyncpgpromise-0.1.0/
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:52:31.133703 asyncpgpromise-0.1.0/AsyncPGPromise/
--rw-r--r--   0 knrs       (501) staff       (20)       73 2023-07-04 21:48:15.000000 asyncpgpromise-0.1.0/AsyncPGPromise/__init__.py
--rw-r--r--   0 knrs       (501) staff       (20)     1166 2023-07-04 21:19:45.000000 asyncpgpromise-0.1.0/AsyncPGPromise/asyncpgpromise.py
--rw-r--r--   0 knrs       (501) staff       (20)     2230 2023-07-04 21:52:31.134598 asyncpgpromise-0.1.0/PKG-INFO
--rw-r--r--   0 knrs       (501) staff       (20)     1984 2023-07-04 21:48:25.000000 asyncpgpromise-0.1.0/README.md
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:52:31.134389 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/
--rw-r--r--   0 knrs       (501) staff       (20)     2230 2023-07-04 21:52:31.000000 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/PKG-INFO
--rw-r--r--   0 knrs       (501) staff       (20)      267 2023-07-04 21:52:31.000000 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/SOURCES.txt
--rw-r--r--   0 knrs       (501) staff       (20)        1 2023-07-04 21:52:31.000000 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/dependency_links.txt
--rw-r--r--   0 knrs       (501) staff       (20)        8 2023-07-04 21:52:31.000000 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/requires.txt
--rw-r--r--   0 knrs       (501) staff       (20)       15 2023-07-04 21:52:31.000000 asyncpgpromise-0.1.0/asyncpgpromise.egg-info/top_level.txt
--rw-r--r--   0 knrs       (501) staff       (20)       38 2023-07-04 21:52:31.134772 asyncpgpromise-0.1.0/setup.cfg
--rw-r--r--   0 knrs       (501) staff       (20)      556 2023-07-04 21:52:21.000000 asyncpgpromise-0.1.0/setup.py
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:59:45.637521 asyncpgpromise-0.1.1/
+-rw-r--r--   0 knrs       (501) staff       (20)     2229 2023-07-04 21:59:45.637393 asyncpgpromise-0.1.1/PKG-INFO
+-rw-r--r--   0 knrs       (501) staff       (20)     1983 2023-07-04 21:59:16.000000 asyncpgpromise-0.1.1/README.md
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:59:45.636305 asyncpgpromise-0.1.1/asyncpgpromise/
+-rw-r--r--   0 knrs       (501) staff       (20)       73 2023-07-04 21:48:15.000000 asyncpgpromise-0.1.1/asyncpgpromise/__init__.py
+-rw-r--r--   0 knrs       (501) staff       (20)     1166 2023-07-04 21:19:45.000000 asyncpgpromise-0.1.1/asyncpgpromise/asyncpgpromise.py
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:59:45.637197 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/
+-rw-r--r--   0 knrs       (501) staff       (20)     2229 2023-07-04 21:59:45.000000 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/PKG-INFO
+-rw-r--r--   0 knrs       (501) staff       (20)      267 2023-07-04 21:59:45.000000 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/SOURCES.txt
+-rw-r--r--   0 knrs       (501) staff       (20)        1 2023-07-04 21:59:45.000000 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/dependency_links.txt
+-rw-r--r--   0 knrs       (501) staff       (20)        8 2023-07-04 21:59:45.000000 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/requires.txt
+-rw-r--r--   0 knrs       (501) staff       (20)       15 2023-07-04 21:59:45.000000 asyncpgpromise-0.1.1/asyncpgpromise.egg-info/top_level.txt
+-rw-r--r--   0 knrs       (501) staff       (20)       38 2023-07-04 21:59:45.637563 asyncpgpromise-0.1.1/setup.cfg
+-rw-r--r--   0 knrs       (501) staff       (20)      556 2023-07-04 21:59:36.000000 asyncpgpromise-0.1.1/setup.py
```

### Comparing `asyncpgpromise-0.1.0/AsyncPGPromise/asyncpgpromise.py` & `asyncpgpromise-0.1.1/asyncpgpromise/asyncpgpromise.py`

 * *Files identical despite different names*

### Comparing `asyncpgpromise-0.1.0/PKG-INFO` & `asyncpgpromise-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpgpromise
-Version: 0.1.0
+Version: 0.1.1
 Summary: pg-promise like wrapper for asyncpg
 Home-page: https://github.com/K-NRS/asyncpgpromise
 Author: Kerem Noras
 Author-email: kerem@noras.tech
 Description-Content-Type: text/markdown
 
 # AsyncPGPromise
@@ -25,15 +25,15 @@
 ```
 
 ## Getting Started
 
 You can create a new `AsyncPGPromise` instance with an existing `asyncpg` connection object:
 
 ```python
-from asyncpg_promise import AsyncPGPromise
+from asyncpgpromise import AsyncPGPromise
 import asyncpg
 
 # First create an asyncpg connection
 conn = await asyncpg.connect(user='user', password='password', database='database', host='127.0.0.1')
 
 # Then pass it to AsyncPGPromise
 pg = AsyncPGPromise(conn)
```

### Comparing `asyncpgpromise-0.1.0/README.md` & `asyncpgpromise-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```
 
 ## Getting Started
 
 You can create a new `AsyncPGPromise` instance with an existing `asyncpg` connection object:
 
 ```python
-from asyncpg_promise import AsyncPGPromise
+from asyncpgpromise import AsyncPGPromise
 import asyncpg
 
 # First create an asyncpg connection
 conn = await asyncpg.connect(user='user', password='password', database='database', host='127.0.0.1')
 
 # Then pass it to AsyncPGPromise
 pg = AsyncPGPromise(conn)
```

### Comparing `asyncpgpromise-0.1.0/asyncpgpromise.egg-info/PKG-INFO` & `asyncpgpromise-0.1.1/asyncpgpromise.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpgpromise
-Version: 0.1.0
+Version: 0.1.1
 Summary: pg-promise like wrapper for asyncpg
 Home-page: https://github.com/K-NRS/asyncpgpromise
 Author: Kerem Noras
 Author-email: kerem@noras.tech
 Description-Content-Type: text/markdown
 
 # AsyncPGPromise
@@ -25,15 +25,15 @@
 ```
 
 ## Getting Started
 
 You can create a new `AsyncPGPromise` instance with an existing `asyncpg` connection object:
 
 ```python
-from asyncpg_promise import AsyncPGPromise
+from asyncpgpromise import AsyncPGPromise
 import asyncpg
 
 # First create an asyncpg connection
 conn = await asyncpg.connect(user='user', password='password', database='database', host='127.0.0.1')
 
 # Then pass it to AsyncPGPromise
 pg = AsyncPGPromise(conn)
```

### Comparing `asyncpgpromise-0.1.0/setup.py` & `asyncpgpromise-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='asyncpgpromise',
-    version='0.1.0',
+    version='0.1.1',
     url='https://github.com/K-NRS/asyncpgpromise',
     author='Kerem Noras',
     author_email='kerem@noras.tech',
     description='pg-promise like wrapper for asyncpg',
     packages=find_packages(),    
     install_requires=['asyncpg'],
     long_description=long_description,
```

