# Comparing `tmp/wakaranai-0.0.1rc1.tar.gz` & `tmp/wakaranai-0.0.1rc2.tar.gz`

## Comparing `wakaranai-0.0.1rc1.tar` & `wakaranai-0.0.1rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/src/wakaranai/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/src/wakaranai/__main__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/src/wakaranai/quiz.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/src/wakaranai/romaji.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/README.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/__main__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/quiz.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/romaji.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/README.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/PKG-INFO
```

### Comparing `wakaranai-0.0.1rc1/src/wakaranai/__main__.py` & `wakaranai-0.0.1rc2/src/wakaranai/__main__.py`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc1/src/wakaranai/quiz.py` & `wakaranai-0.0.1rc2/src/wakaranai/quiz.py`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc1/src/wakaranai/romaji.py` & `wakaranai-0.0.1rc2/src/wakaranai/romaji.py`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc1/.gitignore` & `wakaranai-0.0.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc1/LICENSE` & `wakaranai-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc1/pyproject.toml` & `wakaranai-0.0.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wakaranai"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 authors = [
   { name="Guilherme Dantas" },
 ]
 description = "An educational tool for learning hiragana and katakana"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

