# Comparing `tmp/wakaranai-0.0.1rc2.tar.gz` & `tmp/wakaranai-0.0.1rc3.tar.gz`

## Comparing `wakaranai-0.0.1rc2.tar` & `wakaranai-0.0.1rc3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/__main__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/quiz.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/src/wakaranai/romaji.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/LICENSE
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/README.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/src/wakaranai/__init__.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/src/wakaranai/__main__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/src/wakaranai/quiz.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/src/wakaranai/romaji.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/LICENSE
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 wakaranai-0.0.1rc3/PKG-INFO
```

### Comparing `wakaranai-0.0.1rc2/src/wakaranai/__main__.py` & `wakaranai-0.0.1rc3/src/wakaranai/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from . import romaji, quiz
+from . import romaji, quiz, __version__
 
 from argparse import ArgumentParser
 
 from colorama import Fore
 
 ROMAJI = {
     "hiragana": romaji.HIRAGANA,
     "katakana": romaji.KATAKANA,
 }
 
 parser = ArgumentParser(
     prog="wakaranai",
     description="An educational tool for learning hiragana and katakana")
-parser.add_argument('-v', '--version', action='version', version="0.0.1")
+parser.add_argument('-v', '--version', action='version', version=__version__)
 parser.add_argument(
     'kana', choices=ROMAJI.keys(),
     help="the kana to be covered by the quiz")
 
 
 def question_fmt(question: quiz.Question) -> str:
     return f'{question}? '
```

### Comparing `wakaranai-0.0.1rc2/src/wakaranai/quiz.py` & `wakaranai-0.0.1rc3/src/wakaranai/quiz.py`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc2/src/wakaranai/romaji.py` & `wakaranai-0.0.1rc3/src/wakaranai/romaji.py`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc2/.gitignore` & `wakaranai-0.0.1rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc2/LICENSE` & `wakaranai-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc2/README.md` & `wakaranai-0.0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `wakaranai-0.0.1rc2/PKG-INFO` & `wakaranai-0.0.1rc3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: wakaranai
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: An educational tool for learning hiragana and katakana
 Project-URL: Source Code, https://github.com/guidanoli/wakaranai
 Project-URL: Bug Tracker, https://github.com/guidanoli/wakaranai/issues
 Author: Guilherme Dantas
 License-File: LICENSE
+Keywords: education,hiragana,japanese,katakana,learning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Japanese
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

