# Comparing `tmp/uniquer-1.0.1.tar.gz` & `tmp/uniquer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniquer-1.0.1.tar", max compression
+gzip compressed data, was "uniquer-1.0.2.tar", max compression
```

## Comparing `uniquer-1.0.1.tar` & `uniquer-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-07-03 06:56:48.422968 uniquer-1.0.1/LICENSE
--rw-r--r--   0        0        0     1175 2023-07-03 06:56:48.422968 uniquer-1.0.1/README.md
--rw-r--r--   0        0        0     2071 2023-07-03 06:56:48.422968 uniquer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3219 2023-07-03 06:56:48.422968 uniquer-1.0.1/uniquer/__init__.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 uniquer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 22:00:53.402908 uniquer-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1175 2023-07-04 22:00:53.402908 uniquer-1.0.2/README.md
+-rw-r--r--   0        0        0     2129 2023-07-04 22:00:53.402908 uniquer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3219 2023-07-04 22:00:53.402908 uniquer-1.0.2/uniquer/__init__.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 uniquer-1.0.2/PKG-INFO
```

### Comparing `uniquer-1.0.1/LICENSE` & `uniquer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uniquer-1.0.1/README.md` & `uniquer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `uniquer-1.0.1/pyproject.toml` & `uniquer-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniquer"
-version = "1.0.1"
+version = "1.0.2"
 description = "Unique Iteration"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -27,14 +27,15 @@
 python = '^3.7.2'
 
 [tool.poetry.group.test.dependencies]
 black = '^23.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
 mypy = "^1.3.0"
+nbcpychecker = '^1.0.0'
 pylint = '^2.15'
 pytest = '^7.3'
 
 [tool.poetry.group.doc.dependencies]
 sphinx = '^5.1.1'
 sphinx-rtd-theme = "^1.0.0"
 sphinxemoji = ">=0.2.0"
@@ -102,8 +103,9 @@
     poetry run coverage run --source=uniquer --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint uniquer
     poetry run mypy uniquer
     poetry run make html -C docs
+    poetry run nbcpychecker check
 """
```

### Comparing `uniquer-1.0.1/uniquer/__init__.py` & `uniquer-1.0.2/uniquer/__init__.py`

 * *Files identical despite different names*

### Comparing `uniquer-1.0.1/PKG-INFO` & `uniquer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniquer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unique Iteration
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

