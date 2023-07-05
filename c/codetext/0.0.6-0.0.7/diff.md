# Comparing `tmp/codetext-0.0.6-1.tar.gz` & `tmp/codetext-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codetext-0.0.6.tar", last modified: Thu Feb  9 15:11:36 2023, max compression
+gzip compressed data, was "/Users/nmd2000/Workspace/parser/dist/.tmp-9ldjo7i3/codetext-0.0.7.tar", last modified: Wed Jul  5 10:02:24 2023, max compression
```

## Comparing `codetext-0.0.6-1.tar` & `codetext-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,57 @@
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)     1078 2023-01-09 13:51:12.000000 codetext-0.0.6/LICENSE
--rw-rw-r--   0 dungnm31  (1005) dungnm31  (1005)     3961 2023-02-09 15:11:36.968070 codetext-0.0.6/PKG-INFO
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)     3339 2023-01-09 13:43:41.000000 codetext-0.0.6/README.md
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)      808 2023-02-09 13:23:45.000000 codetext-0.0.6/pyproject.toml
--rw-rw-r--   0 dungnm31  (1005) dungnm31  (1005)       38 2023-02-09 15:11:36.968070 codetext-0.0.6/setup.cfg
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.964070 codetext-0.0.6/src/
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/src/codetext/
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)        0 2022-12-26 13:55:44.000000 codetext-0.0.6/src/codetext/__init__.py
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/src/codetext/clean/
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)      219 2022-12-26 14:13:02.000000 codetext-0.0.6/src/codetext/clean/__init__.py
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)    31481 2023-02-08 10:14:54.000000 codetext-0.0.6/src/codetext/clean/noise_removal.py
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/src/codetext/parser/
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)      726 2023-02-08 12:20:58.000000 codetext-0.0.6/src/codetext/parser/__init__.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     5979 2023-02-09 12:22:32.000000 codetext-0.0.6/src/codetext/parser/c_sharp_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     6527 2023-02-09 15:06:11.000000 codetext-0.0.6/src/codetext/parser/cpp_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     4863 2023-02-09 12:13:39.000000 codetext-0.0.6/src/codetext/parser/go_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     4352 2023-02-09 12:17:23.000000 codetext-0.0.6/src/codetext/parser/java_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     3832 2023-02-09 12:06:27.000000 codetext-0.0.6/src/codetext/parser/javascript_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     7851 2023-02-08 13:14:44.000000 codetext-0.0.6/src/codetext/parser/language_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     4235 2023-02-09 12:06:46.000000 codetext-0.0.6/src/codetext/parser/php_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     4859 2023-02-09 12:08:54.000000 codetext-0.0.6/src/codetext/parser/python_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     4530 2023-02-09 15:08:00.000000 codetext-0.0.6/src/codetext/parser/ruby_parser.py
--rwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)     5243 2023-02-09 12:56:13.000000 codetext-0.0.6/src/codetext/parser/rust_parser.py
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/src/codetext/utils/
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)      168 2022-12-26 14:06:42.000000 codetext-0.0.6/src/codetext/utils/__init__.py
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)     1056 2022-12-26 13:55:44.000000 codetext-0.0.6/src/codetext/utils/imports.py
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)     3850 2023-01-09 14:44:10.000000 codetext-0.0.6/src/codetext/utils/utils.py
-drwxrwxr-x   0 dungnm31  (1005) dungnm31  (1005)        0 2023-02-09 15:11:36.968070 codetext-0.0.6/src/codetext.egg-info/
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)     3961 2023-02-09 15:11:36.000000 codetext-0.0.6/src/codetext.egg-info/PKG-INFO
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)      785 2023-02-09 15:11:36.000000 codetext-0.0.6/src/codetext.egg-info/SOURCES.txt
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)        1 2023-02-09 15:11:36.000000 codetext-0.0.6/src/codetext.egg-info/dependency_links.txt
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)       65 2023-02-09 15:11:36.000000 codetext-0.0.6/src/codetext.egg-info/requires.txt
--rwxrwxrwx   0 dungnm31  (1005) dungnm31  (1005)        9 2023-02-09 15:11:36.000000 codetext-0.0.6/src/codetext.egg-info/top_level.txt
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/
+-rwxr-xr-x   0 nmd2000    (501) staff       (20)     1078 2023-03-13 06:31:46.000000 codetext-0.0.7/LICENSE
+-rw-r--r--   0 nmd2000    (501) staff       (20)     7196 2023-07-05 10:02:24.000000 codetext-0.0.7/PKG-INFO
+-rwxr-xr-x   0 nmd2000    (501) staff       (20)     6573 2023-07-05 09:38:53.000000 codetext-0.0.7/README.md
+-rwxr-xr-x   0 nmd2000    (501) staff       (20)      885 2023-07-05 10:02:19.000000 codetext-0.0.7/pyproject.toml
+-rw-r--r--   0 nmd2000    (501) staff       (20)       38 2023-07-05 10:02:24.000000 codetext-0.0.7/setup.cfg
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/
+-rw-r--r--   0 nmd2000    (501) staff       (20)        0 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/__init__.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     3137 2023-07-05 09:13:51.000000 codetext-0.0.7/src/codetext/__main__.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/clean/
+-rw-r--r--   0 nmd2000    (501) staff       (20)      219 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/clean/__init__.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    31481 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/clean/noise_removal.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     7122 2023-07-05 08:46:53.000000 codetext-0.0.7/src/codetext/codetext_cli.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/parser/
+-rw-r--r--   0 nmd2000    (501) staff       (20)      937 2023-07-04 09:42:35.000000 codetext-0.0.7/src/codetext/parser/__init__.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     7037 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/c_sharp_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     6627 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/cpp_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     4849 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/go_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     4642 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/java_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     3915 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/javascript_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     7861 2023-07-04 08:41:05.000000 codetext-0.0.7/src/codetext/parser/language_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     4351 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/php_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     4763 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/python_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     4530 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/ruby_parser.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     5437 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/parser/rust_parser.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/tree-sitter/
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/
+-rw-r--r--   0 nmd2000    (501) staff       (20)       38 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/compound-statement-without-trailing-newline.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       51 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/crlf-line-endings.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       74 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/mixed-spaces-tabs.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       73 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/multiple-newlines.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    31929 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/python2-grammar-crlf.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    30981 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/python2-grammar.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    31722 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/python3-grammar-crlf.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    30784 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/python3-grammar.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)    50403 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/python3.8_grammar.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       16 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/simple-statements-without-trailing-newline.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     1236 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/tabs.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       58 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/examples/trailing-whitespace.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/test/
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/test/highlight/
+-rw-r--r--   0 nmd2000    (501) staff       (20)      352 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/test/highlight/keywords.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)       99 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/test/highlight/parameters.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     1297 2023-07-04 09:43:30.000000 codetext-0.0.7/src/codetext/tree-sitter/tree-sitter-python/test/highlight/pattern_matching.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext/utils/
+-rw-r--r--   0 nmd2000    (501) staff       (20)      168 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/utils/__init__.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     1056 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/utils/imports.py
+-rw-r--r--   0 nmd2000    (501) staff       (20)     3850 2023-07-04 06:43:08.000000 codetext-0.0.7/src/codetext/utils/utils.py
+drwxr-xr-x   0 nmd2000    (501) staff       (20)        0 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/
+-rw-r--r--   0 nmd2000    (501) staff       (20)     7196 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/PKG-INFO
+-rw-r--r--   0 nmd2000    (501) staff       (20)     2031 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/SOURCES.txt
+-rw-r--r--   0 nmd2000    (501) staff       (20)        1 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/dependency_links.txt
+-rw-r--r--   0 nmd2000    (501) staff       (20)       52 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/entry_points.txt
+-rw-r--r--   0 nmd2000    (501) staff       (20)       81 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/requires.txt
+-rw-r--r--   0 nmd2000    (501) staff       (20)        9 2023-07-05 10:02:24.000000 codetext-0.0.7/src/codetext.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `codetext-0.0.6/LICENSE` & `codetext-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codetext-0.0.6/pyproject.toml` & `codetext-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codetext"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dung Manh Nguyen", email="dungnm.workspace@gmail.com" },
 ]
 description = "Multilingual programming language parsers for the extract from raw source code into multiple levels of pair data"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -17,12 +17,16 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "tree-sitter>=0.20",
     "Levenshtein>=0.20",
     "langdetect>=1.0.0",
     "bs4>=0.0.1",
+    "tabulate>=0.9.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/AI4Code-Research/CodeText-data"
 "Bug Tracker" = "https://github.com/AI4Code-Research/CodeText-data/issues"
+
+[project.scripts]
+codetext = "codetext.__main__:main"
```

### Comparing `codetext-0.0.6/src/codetext/clean/noise_removal.py` & `codetext-0.0.7/src/codetext/clean/noise_removal.py`

 * *Files identical despite different names*

### Comparing `codetext-0.0.6/src/codetext/parser/__init__.py` & `codetext-0.0.7/src/codetext/parser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from .ruby_parser import RubyParser
 from .java_parser import JavaParser
 from .javascript_parser import JavascriptParser
 from .python_parser import PythonParser
 from .cpp_parser import CppParser
 from .c_sharp_parser import CsharpParser
 from .rust_parser import RustParser
-from .language_parser import LanguageParser
+from .language_parser import LanguageParser, get_node_by_kind, get_node_text, \
+    tokenize_code, tokenize_docstring, nodes_are_equal
+    
+SUPPORT_LANGUAGE = [
+    "go", "php", "ruby", "java", "javascript", 
+    "python", "cpp", "c", "c_sharp", "rust"
+]
 
 __all__ = [
     'GoParser', 'PhpParser', 'RubyParser', 'JavaParser', 'JavascriptParser',
     'PythonParser', 'CppParser', 'CsharpParser', 'RustParser', 'LanguageParser',
     'get_node_by_kind', 'get_node_text', 'tokenize_code', 'tokenize_docstring',
     'nodes_are_equal'
 ]
```

### Comparing `codetext-0.0.6/src/codetext/parser/c_sharp_parser.py` & `codetext-0.0.7/src/codetext/parser/cpp_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 from typing import List, Dict, Any
+
 import tree_sitter
 import logging
 
-from .language_parser import LanguageParser, get_node_by_kind, get_node_text
+from .language_parser import LanguageParser, get_node_text, get_node_by_kind
 
 logger = logging.getLogger(name=__name__)
 
 
-class CsharpParser(LanguageParser):
+class CppParser(LanguageParser):
     
-    BLACKLISTED_FUNCTION_NAMES = []
+    BLACKLISTED_FUNCTION_NAMES = ['main', 'constructor']
     
     @staticmethod
     def get_docstring(node, blob=None):
         """
         Get docstring description for node
         
         Args:
             node (tree_sitter.Node)
             blob (str): original source code which parse the `node`
         Returns:
             str: docstring
         """
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
-        docstring_node = CsharpParser.get_docstring_node(node)
+        docstring_node = CppParser.get_docstring_node(node)
         docstring = '\n'.join(get_node_text(s) for s in docstring_node)
         return docstring
     
     @staticmethod
     def get_docstring_node(node):
         """
         Get docstring node from it parent node.
-        C# docstring is written line by line and stay outside it own node, see example below.
+        C and C++ share the same syntax. Their docstring usually is 1 single block
+        Expect length of return list == 1
         
         Args:
             node (tree_sitter.Node): parent node (usually function node) to get its docstring
         Return:
-            List: list of docstring nodes
+            List: list of docstring nodes (expect==1)
         Example:
             str = '''
-                // <summary>
-                // Docstring of a method
-                // </summary>
-                // <param name="animal_honk">Argument.</param>
-                // <returns>
-                // None.
-                public void honk(string animal_honk)
-                {                    
-                    Console.WriteLine(animal_honk);
-                    Console.WriteLine("Tuut, tuut!");
+                /**
+                * Find 2 sum
+                *
+                * @param nums List number.
+                * @param target Sum target.
+                * @return postion of 2 number.
+                */
+                vector<int> twoSum(vector<int>& nums, int target) {
+                    ...
                 }
             '''
             ...
-            print(C_sharp.get_docstring_node(function_node))
+            print(CppParser.get_docstring_node(function_node))
             
-            >>> [<Node type=comment, start_point=(5, 12), end_point=(5, 24)>, \
-                <Node type=comment, start_point=(6, 12), end_point=(6, 36)>, \
-                <Node type=comment, start_point=(7, 12), end_point=(7, 25)>, \
-                <Node type=comment, start_point=(8, 12), end_point=(8, 58)>, \
-                <Node type=comment, start_point=(9, 12), end_point=(9, 24)>, \
-                <Node type=comment, start_point=(10, 12), end_point=(10, 20)>]
+            >>> [<Node type=comment, start_point=(x, y), end_point=(x, y)>]
         """
         docstring_node = []
         
         prev_node = node.prev_sibling
         if prev_node and prev_node.type == 'comment':
             docstring_node.append(prev_node)
             prev_node = prev_node.prev_sibling
@@ -74,92 +70,107 @@
             x_current = prev_node.start_point[0]
             x_next = prev_node.next_sibling.start_point[0]
             if x_next - x_current > 1:
                 break
             
             docstring_node.insert(0, prev_node)    
             prev_node = prev_node.prev_sibling
-            
+        
         return docstring_node
     
     @staticmethod
+    def get_function_list(node):
+        res = get_node_by_kind(node, ['function_definition'])
+        return res
+
+    @staticmethod
+    def get_class_list(node):
+        res = get_node_by_kind(node, ['class_specifier'])
+        return res
+        
+    @staticmethod
     def get_comment_node(node):
         """
         Return all comment node inside a parent node
         Args:
             node (tree_sitter.Node)
         Return:
             List: list of comment nodes
         """
         comment_node = get_node_by_kind(node, kind=['comment'])
         return comment_node
     
     @staticmethod
-    def get_function_list(node):
-        res = get_node_by_kind(node, ['local_function_statement', 'method_declaration'])
-        # We don't use "constructor_declaration"
-        return res
-
-    @staticmethod
-    def get_class_list(node):
-        res = get_node_by_kind(node, ['class_declaration'])
-        return res
-
-    @staticmethod
     def get_function_metadata(function_node, blob: str=None) -> Dict[str, Any]:
         """
         Function metadata contains:
             - identifier (str): function name
             - parameters (Dict[str, str]): parameter's name and their type (e.g: {'param_a': 'int'})
-            - type (str): type
+            - return_type (str or NoneType): function's return type
         """
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
             'parameters': {},
-            'return_type': None
+            'return_type': None,
         }
         assert type(function_node) == tree_sitter.Node
         
         for child in function_node.children:
-            if child.type == 'predefined_type':
+            if child.type in ['primitive_type', 'type_identifier']:
                 metadata['return_type'] = get_node_text(child)
-            elif child.type == 'identifier':
-                metadata['identifier'] = get_node_text(child)
-            elif child.type == 'parameter_list':
-                for param_node in child.children:
-                    param_nodes = get_node_by_kind(param_node, ['parameter'])
-                    for param in param_nodes:
-                        param_type = get_node_text(param.children[0])
-                        param_identifier = get_node_text(param.children[1])
-                    
-                        metadata['parameters'][param_identifier] = param_type
+                # search for "function_declarator"
+            elif child.type == 'pointer_declarator':
+                for subchild in child.children:
+                    if subchild.type == 'function_declarator':
+                        child = subchild
+            if child.type == 'function_declarator':
+                for subchild in child.children:
+                    if subchild.type in ['qualified_identifier', 'identifier', 'field_identifier']:
+                        metadata['identifier'] = get_node_text(subchild)
+                    elif subchild.type == 'parameter_list':
+                        param_nodes = get_node_by_kind(subchild, ['parameter_declaration'])
+                        for param in param_nodes:
+                            param_type = param.child_by_field_name('type')
+                            param_type = get_node_text(param_type)
+                            list_name = get_node_by_kind(param, ['identifier'])
+                            if not list_name:
+                                continue
+                            param_name = get_node_text(list_name[0])
+                            metadata['parameters'][param_name] = param_type
+                            # for item in param.children:
+                                
+                            #     if item.type in ['type_identifier', 'primitive_type']:
+                            #         param_type = get_node_text(item)
+                            #     elif item.type == 'identifier':
+                            #         param_identifier = get_node_text(item)
+
         return metadata
 
     @staticmethod
     def get_class_metadata(class_node, blob: str=None) -> Dict[str, str]:
         """
         Class metadata contains:
             - identifier (str): class's name
             - parameters (List[str]): inheritance class
         """
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': '',
+            'parameters': {},
         }
         assert type(class_node) == tree_sitter.Node
         
         for child in class_node.children:
-            if child.type == 'identifier':
+            if child.type == 'type_identifier':
                 metadata['identifier'] = get_node_text(child)
-            elif child.type == 'base_list':
+            elif child.type == 'base_class_clause':
                 argument_list = []
-                for arg in child.children:
-                    if arg.type == 'identifier':
-                        argument_list.append(get_node_text(arg))
-                metadata['parameters'] = argument_list
+                for param in child.children:
+                    if param.type == 'type_identifier':
+                        metadata['parameters'][get_node_text(param)] = None
+                        # argument_list.append(get_node_text(param))
+                # metadata['parameters'] = argument_list
 
         return metadata
-
```

### Comparing `codetext-0.0.6/src/codetext/parser/cpp_parser.py` & `codetext-0.0.7/src/codetext/parser/c_sharp_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 from typing import List, Dict, Any
-
 import tree_sitter
 import logging
 
-from .language_parser import LanguageParser, get_node_text, get_node_by_kind
+from .language_parser import LanguageParser, get_node_by_kind, get_node_text
 
 logger = logging.getLogger(name=__name__)
 
 
-class CppParser(LanguageParser):
+class CsharpParser(LanguageParser):
     
-    BLACKLISTED_FUNCTION_NAMES = ['main', 'constructor']
+    BLACKLISTED_FUNCTION_NAMES = []
     
     @staticmethod
     def get_docstring(node, blob=None):
         """
         Get docstring description for node
         
         Args:
             node (tree_sitter.Node)
             blob (str): original source code which parse the `node`
         Returns:
             str: docstring
         """
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
-        docstring_node = CppParser.get_docstring_node(node)
+        docstring_node = CsharpParser.get_docstring_node(node)
         docstring = '\n'.join(get_node_text(s) for s in docstring_node)
         return docstring
     
     @staticmethod
     def get_docstring_node(node):
         """
         Get docstring node from it parent node.
-        C and C++ share the same syntax. Their docstring usually is 1 single block
-        Expect length of return list == 1
+        C# docstring is written line by line and stay outside it own node, see example below.
         
         Args:
             node (tree_sitter.Node): parent node (usually function node) to get its docstring
         Return:
-            List: list of docstring nodes (expect==1)
+            List: list of docstring nodes
         Example:
             str = '''
-                /**
-                * Find 2 sum
-                *
-                * @param nums List number.
-                * @param target Sum target.
-                * @return postion of 2 number.
-                */
-                vector<int> twoSum(vector<int>& nums, int target) {
-                    ...
+                // <summary>
+                // Docstring of a method
+                // </summary>
+                // <param name="animal_honk">Argument.</param>
+                // <returns>
+                // None.
+                public void honk(string animal_honk)
+                {                    
+                    Console.WriteLine(animal_honk);
+                    Console.WriteLine("Tuut, tuut!");
                 }
             '''
             ...
-            print(CppParser.get_docstring_node(function_node))
+            print(C_sharp.get_docstring_node(function_node))
             
-            >>> [<Node type=comment, start_point=(x, y), end_point=(x, y)>]
+            >>> [<Node type=comment, start_point=(5, 12), end_point=(5, 24)>, \
+                <Node type=comment, start_point=(6, 12), end_point=(6, 36)>, \
+                <Node type=comment, start_point=(7, 12), end_point=(7, 25)>, \
+                <Node type=comment, start_point=(8, 12), end_point=(8, 58)>, \
+                <Node type=comment, start_point=(9, 12), end_point=(9, 24)>, \
+                <Node type=comment, start_point=(10, 12), end_point=(10, 20)>]
         """
         docstring_node = []
         
         prev_node = node.prev_sibling
         if prev_node and prev_node.type == 'comment':
             docstring_node.append(prev_node)
             prev_node = prev_node.prev_sibling
@@ -70,106 +74,107 @@
             x_current = prev_node.start_point[0]
             x_next = prev_node.next_sibling.start_point[0]
             if x_next - x_current > 1:
                 break
             
             docstring_node.insert(0, prev_node)    
             prev_node = prev_node.prev_sibling
-        
+            
         return docstring_node
     
     @staticmethod
-    def get_function_list(node):
-        res = get_node_by_kind(node, ['function_definition'])
-        return res
-
-    @staticmethod
-    def get_class_list(node):
-        res = get_node_by_kind(node, ['class_specifier'])
-        return res
-        
-    @staticmethod
     def get_comment_node(node):
         """
         Return all comment node inside a parent node
         Args:
             node (tree_sitter.Node)
         Return:
             List: list of comment nodes
         """
         comment_node = get_node_by_kind(node, kind=['comment'])
         return comment_node
     
     @staticmethod
-    def get_function_metadata(function_node, blob: str=None) -> Dict[str, Any]:
+    def get_function_list(node):
+        res = get_node_by_kind(node, ['local_function_statement', 'method_declaration'])
+        # We don't use "constructor_declaration"
+        return res
+
+    @staticmethod
+    def get_class_list(node):
+        res = get_node_by_kind(node, ['class_declaration'])
+        return res
+
+    @staticmethod
+    def get_function_metadata(function_node, blob: str = None) -> Dict[str, Any]:
         """
         Function metadata contains:
             - identifier (str): function name
             - parameters (Dict[str, str]): parameter's name and their type (e.g: {'param_a': 'int'})
-            - return_type (str or NoneType): function's return type
+            - type (str): type
         """
-        if blob:
-            logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
             'parameters': {},
-            'return_type': None,
+            'return_type': None
         }
         assert type(function_node) == tree_sitter.Node
         
         for child in function_node.children:
-            if child.type in ['primitive_type', 'type_identifier']:
+            if child.type in ['predefined_type', 'generic_name']:
                 metadata['return_type'] = get_node_text(child)
-                # search for "function_declarator"
-            elif child.type == 'pointer_declarator':
-                for subchild in child.children:
-                    if subchild.type == 'function_declarator':
-                        child = subchild
-            if child.type == 'function_declarator':
-                for subchild in child.children:
-                    if subchild.type in ['qualified_identifier', 'identifier']:
-                        metadata['identifier'] = get_node_text(subchild)
-                    elif subchild.type == 'parameter_list':
-                        param_nodes = get_node_by_kind(subchild, ['parameter_declaration'])
-                        for param in param_nodes:
-                            param_type = param.child_by_field_name('type')
-                            param_type = get_node_text(param_type)
-                            list_name = get_node_by_kind(param, ['identifier'])
-                            if not list_name:
-                                continue
-                            param_name = get_node_text(list_name[0])
+            elif child.type == 'identifier':
+                if child.next_named_sibling.type != 'parameter_list':
+                    metadata['return_type'] = get_node_text(child)
+                else:
+                    metadata['identifier'] = get_node_text(child)
+            elif child.type == 'parameter_list':
+                for param_node in child.children:
+                    param_nodes = get_node_by_kind(param_node, ['parameter'])
+                    for param in param_nodes:
+                        if len(param.children) > 1:
+                            param_type = get_node_text(param.children[0])
+                            param_name = get_node_text(param.children[1])
                             metadata['parameters'][param_name] = param_type
-                            # for item in param.children:
+                        
+                        else:
+                            param_name = get_node_text(param.children[0])
+                            metadata['parameters'][param_name] = None
+                        # for node in param.children:
+                        #     if node.type in ['array_type', 'implicit_type', \
+                        #         'nullable_type', 'pointer_type', 'function_pointer_type', \
+                        #         'predefined_type', 'tuple_type']:
+                        #         param_type = get_node_text(node)
+                        #     elif node.type == 'identifier':
+                        #         param_identifier = get_node_text(node)
                                 
-                            #     if item.type in ['type_identifier', 'primitive_type']:
-                            #         param_type = get_node_text(item)
-                            #     elif item.type == 'identifier':
-                            #         param_identifier = get_node_text(item)
-
+                        # param_type = get_node_text(param.child_by_field_name('type'))
+                        # param_identifier = get_node_text(param.child_by_field_name('name'))
         return metadata
 
     @staticmethod
     def get_class_metadata(class_node, blob: str=None) -> Dict[str, str]:
         """
         Class metadata contains:
             - identifier (str): class's name
             - parameters (List[str]): inheritance class
         """
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': '',
+            'parameters': {},
         }
         assert type(class_node) == tree_sitter.Node
         
         for child in class_node.children:
-            if child.type == 'type_identifier':
+            if child.type == 'identifier':
                 metadata['identifier'] = get_node_text(child)
-            elif child.type == 'base_class_clause':
-                argument_list = []
-                for param in child.children:
-                    if param.type == 'type_identifier':
-                        argument_list.append(get_node_text(param))
-                metadata['parameters'] = argument_list
+            elif child.type == 'base_list':
+                for arg in child.children:
+                    if arg.type == 'identifier':
+                        metadata['parameters'][get_node_text(arg)] = None
+                        # argument_list.append(get_node_text(arg))
+                # metadata['parameters'] = argument_list
 
         return metadata
+
```

### Comparing `codetext-0.0.6/src/codetext/parser/go_parser.py` & `codetext-0.0.7/src/codetext/parser/go_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         """
         Return all comment node inside a parent node
         Args:
             node (tree_sitter.Node)
         Return:
             List: list of comment nodes
         """
-        comment_node = get_node_by_kind(function_node, comment_node, kind='comment')
+        comment_node = get_node_by_kind(function_node, kind='comment')
         return comment_node
     
     @staticmethod
     def get_docstring_node(node):
         """
         Get docstring node from it parent node.
         Go's docstring is written line by line
```

### Comparing `codetext-0.0.6/src/codetext/parser/java_parser.py` & `codetext-0.0.7/src/codetext/parser/java_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,44 +84,53 @@
     
     @staticmethod
     def get_class_metadata(class_node, blob: str=None) -> Dict[str, str]:
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': '',
+            'parameters': {},
         }
         argument_list = []
         for child in class_node.children:
             if child.type == 'identifier':
                 metadata['identifier'] = get_node_text(child)
             elif child.type == 'superclass' or child.type == 'super_interfaces':
                 for subchild in child.children:
                     if subchild.type == 'type_list' or subchild.type == 'type_identifier':
-                        argument_list.append(get_node_text(subchild))
+                        metadata['parameters'][get_node_text(subchild)] = None
+                        # argument_list.append(get_node_text(subchild))
                     
-        metadata['parameters'] = argument_list
+        # metadata['parameters'] = argument_list
         return metadata
 
     @staticmethod
-    def get_function_metadata(function_node, blob: str=None) -> Dict[str, str]:
-        if blob:
-            logger.info('From version `0.0.6` this function will update argument in the API')
+    def get_function_metadata(function_node, blob: str = None) -> Dict[str, str]:
         metadata = {
             'identifier': '',
             'parameters': {},
             'return_type': None
         }
         
+        return_kinds = ["void_type", 
+                        "integral_type",
+                        "floating_point_type",
+                        "boolean_type",
+                        "type_identifier",
+                        "scoped_type_identifier",
+                        "generic_type"]
+        
+
         for child in function_node.children:
             if child.type == 'identifier':
-                metadata['identifier'] = get_node_text(child)
-            elif child.type == 'type_identifier':
+                metadata['identifier'] = get_node_text(child)    
+            elif child.type in return_kinds:
                 metadata['return_type'] = get_node_text(child)
             elif child.type == 'formal_parameters':
                 param_list = get_node_by_kind(child, ['formal_parameter'])  # speed_parameter
                 for param in param_list:
                     param_type = get_node_text(param.child_by_field_name('type'))
                     identifier = get_node_text(param.child_by_field_name('name'))
                     metadata['parameters'][identifier] = param_type
         
-        return metadata
+        
+        return metadata
```

### Comparing `codetext-0.0.6/src/codetext/parser/javascript_parser.py` & `codetext-0.0.7/src/codetext/parser/javascript_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,20 +91,21 @@
 
     @staticmethod
     def get_class_metadata(class_node, blob=None):
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': '',
+            'parameters': {},
         }
         param = []
         for child in class_node.children:
             if child.type == 'identifier':
                 metadata['identifier'] = get_node_text(child)
             elif child.type == 'class_heritage':
                 for subchild in child.children:
                     if subchild.type == 'identifier':
-                        param.append(get_node_text(subchild))
+                        metadata['parameters'][get_node_text(subchild)] = None
+                        # param.append(get_node_text(subchild))
                         
-        metadata['parameters'] = param
+        # metadata['parameters'] = param
         return metadata
```

### Comparing `codetext-0.0.6/src/codetext/parser/language_parser.py` & `codetext-0.0.7/src/codetext/parser/language_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,20 +225,20 @@
     @staticmethod
     @abstractmethod
     def get_comment_node(node) -> List[tree_sitter.Node]:
         pass
     
     @staticmethod
     @abstractmethod
-    def get_class_metadata(class_node, blob):
+    def get_class_metadata(class_node, blob=None):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_function_metadata(function_node, blob) -> Dict[str, str]:
+    def get_function_metadata(function_node, blob=None) -> Dict[str, str]:
         pass
     
     
     # @staticmethod
     # @abstractmethod
     # def get_function_definitions(tree, blob) -> List:
     #     pass
```

### Comparing `codetext-0.0.6/src/codetext/parser/php_parser.py` & `codetext-0.0.7/src/codetext/parser/php_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,22 +95,24 @@
     
     @staticmethod
     def get_class_metadata(class_node, blob: str=None):
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': '',
+            'parameters': {},
         }
         assert type(class_node) == tree_sitter.Node
         
         for child in class_node.children:
             if child.type == 'name':
                 metadata['identifier'] = get_node_text(child)
             elif child.type == 'base_clause':
                 argument_list = []
                 for param in child.children:
                     if param.type == 'name':
-                        argument_list.append(get_node_text(param))
-                metadata['parameters'] = argument_list 
+                        name = get_node_text(param)
+                        metadata['parameters'][name] = None
+                        # argument_list.append(get_node_text(param))
+                # metadata['parameters'] = argument_list 
     
         return metadata
```

### Comparing `codetext-0.0.6/src/codetext/parser/python_parser.py` & `codetext-0.0.7/src/codetext/parser/python_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,23 +101,20 @@
 
     @staticmethod
     def get_class_metadata(class_node, blob: str=None) -> Dict[str, str]:
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': [],
+            'parameters': {},
         }
         for child in class_node.children:
             if child.type == 'identifier':
                 metadata['identifier'] = get_node_text(child)
             elif child.type == 'argument_list':
-                args = []
                 argument_list = get_node_text(child).split(',')
                 for arg in argument_list:
                     item = re.sub(r'[^a-zA-Z0-9\_]', ' ', arg).split()
-                    if len(item) > 0:
-                        args.append(item[0].strip())
-                metadata['parameters'] = args
+                    metadata['parameters'][item[0].strip()] = None
 
         # get __init__ function
         return metadata
```

### Comparing `codetext-0.0.6/src/codetext/parser/ruby_parser.py` & `codetext-0.0.7/src/codetext/parser/ruby_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,26 +109,26 @@
     
     @staticmethod
     def get_class_metadata(class_node, blob=None):
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': [],
+            'parameters': {},
         }
         
         assert type(class_node) == tree_sitter.Node
         
         for child in class_node.children:
             if child.type == 'constant':
                 metadata['identifier'] = get_node_text(child)
             if child.type == 'superclass':
                 for subchild in child.children:
                     if subchild.type == 'constant':
-                        metadata['parameters'].append(get_node_text(subchild))
+                        metadata['parameters'][get_node_text(subchild)] = None
 
         return metadata
         
 
     @staticmethod
     def get_comment_node(function_node):
         comment_node = get_node_by_kind(function_node, kind='comment')
```

### Comparing `codetext-0.0.6/src/codetext/parser/rust_parser.py` & `codetext-0.0.7/src/codetext/parser/rust_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,20 @@
             elif child.type in ['parameters']:
                 params = get_node_by_kind(child, ['parameter', 'variadic_parameter', 'self_parameter'])
                 for item in params:
                     if item.type == 'self_parameter':
                         metadata['parameters'][get_node_text(item)] = None
                     
                     else:
-                        # param_name = ''
+                        param_name = ''
                         for subchild in item.children:
-                            if subchild.type == 'identifier':
+                            if subchild.type == 'mutable_specifier':
+                                param_name = 'self'
+                                break
+                            elif subchild.type == 'identifier':
                                 param_name = get_node_text(subchild)
                                 break
                         param_type = item.child_by_field_name('type')
                         
                         if param_type:
                             param_type = get_node_text(param_type)
                             metadata['parameters'][param_name] = param_type
@@ -116,15 +119,15 @@
     
     @staticmethod
     def get_class_metadata(class_node, blob=None):
         if blob:
             logger.info('From version `0.0.6` this function will update argument in the API')
         metadata = {
             'identifier': '',
-            'parameters': [],
+            'parameters': {},
         }
         
         assert type(class_node) == tree_sitter.Node
         
         if class_node.type == 'mod_item':
             for child in class_node.children:
                 if child.type ==  'identifier':
@@ -132,16 +135,16 @@
         
         else:
             identifier = get_node_by_kind(class_node, ['type_identifier'])
             
             metadata['identifier'] = get_node_text(identifier[0])
             if len(identifier) > 1:
                 for param in identifier[1:]:
-                    metadata['parameters'].append(get_node_text(param))
+                    metadata['parameters'][get_node_text(param)] = None
 
         return metadata
         
 
     @staticmethod
     def get_comment_node(function_node):
-        comment_node = get_node_by_kind(function_node, kind='comment')
+        comment_node = get_node_by_kind(function_node, kind=['comment', 'line_comment', 'block_comment'])
         return comment_node
```

### Comparing `codetext-0.0.6/src/codetext/utils/imports.py` & `codetext-0.0.7/src/codetext/utils/imports.py`

 * *Files identical despite different names*

### Comparing `codetext-0.0.6/src/codetext/utils/utils.py` & `codetext-0.0.7/src/codetext/utils/utils.py`

 * *Files identical despite different names*

