# Comparing `tmp/smpl_io-1.1.2.tar.gz` & `tmp/smpl_io-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpl_io-1.1.2.tar", max compression
+gzip compressed data, was "smpl_io-1.1.4.tar", max compression
```

## Comparing `smpl_io-1.1.2.tar` & `smpl_io-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-27 17:23:26.869935 smpl_io-1.1.2/LICENSE
--rw-r--r--   0        0        0     2814 2023-05-27 17:23:26.869935 smpl_io-1.1.2/README.md
--rw-r--r--   0        0        0     1670 2023-05-27 17:23:28.677974 smpl_io-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      137 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/grep.py
--rw-r--r--   0        0        0     1024 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/head.py
--rw-r--r--   0        0        0     8396 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/io.py
--rw-r--r--   0        0        0      540 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/read_buffer.py
--rw-r--r--   0        0        0      538 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/sed.py
--rw-r--r--   0        0        0     1008 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/tail.py
--rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 smpl_io-1.1.2/setup.py
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 smpl_io-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-05 12:07:17.549703 smpl_io-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2814 2023-07-05 12:07:17.549703 smpl_io-1.1.4/README.md
+-rw-r--r--   0        0        0     1675 2023-07-05 12:07:19.721717 smpl_io-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/__init__.py
+-rw-r--r--   0        0        0     1113 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/grep.py
+-rw-r--r--   0        0        0     1024 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/head.py
+-rw-r--r--   0        0        0     8721 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/io.py
+-rw-r--r--   0        0        0      540 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/read_buffer.py
+-rw-r--r--   0        0        0      538 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/sed.py
+-rw-r--r--   0        0        0     1008 2023-07-05 12:07:17.549703 smpl_io-1.1.4/smpl_io/tail.py
+-rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 smpl_io-1.1.4/setup.py
+-rw-r--r--   0        0        0     3483 1970-01-01 00:00:00.000000 smpl_io-1.1.4/PKG-INFO
```

### Comparing `smpl_io-1.1.2/LICENSE` & `smpl_io-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/README.md` & `smpl_io-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/pyproject.toml` & `smpl_io-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "smpl_io"
-version = "1.1.2"
+version = "1.1.4"
 description = "simple input and output for python"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/smpl_io"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 smpl_doc =  "^1.0.5"
 requests = "*"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -20,15 +20,15 @@
 pytest-profiling =  "*"
 #pytest-line-profiler-apn = {path="/home/apn/git/pytest-line-profiler", develop = true}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "*"
+sphinx = "<7.0.0"
 sphinx-rtd-theme = "*"
 sphinxcontrib-napoleon = "*"
 #nbsphinx = "*"
 #jupyter-sphinx = "*"
 sphinx-autoapi = "*"
 sphinx_autobuild = "*"
 pandoc = "*"
@@ -38,15 +38,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pandas = ">=1.0.0"
 pre-commit = "^2.20.0"
-poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.23.0"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.25.0"}
 #ipython =  "*"
 #jupyterlab =  "*"
 #jupyter = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `smpl_io-1.1.2/smpl_io/grep.py` & `smpl_io-1.1.4/smpl_io/grep.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import re
 from io import StringIO
+
+import smpl_doc.doc as doc
+
 from .read_buffer import ReadBuffer
-import smpl_doc.doc as doc 
-def grep(pattern, *inps, regex=False,open=True,A=0, B=0):
+
+
+def grep(pattern, *inps, regex=False, open=True, A=0, B=0):
     """
     Searches for ``pattern`` in ``inp``.
 
     >>> from smpl_io import io
     >>> io.write("test.txt","hi\\nho1\\n2\\n3\\n4\\n")
     >>> grep("h","test.txt").read()
     'hi\\nho1\\n'
-    >>> grep("h.*\d","test.txt",regex=True).read()
+    >>> grep("h.*\\\\d","test.txt",regex=True).read()
     'ho1\\n'
     """
     r = StringIO()
     for inp in inps:
-        with ReadBuffer(inp,open=open) as f:
+        with ReadBuffer(inp, open=open) as f:
             lines = f.readlines()
             for i, line in enumerate(lines):
                 match = False
                 for j in range(i - A, i + B + 1):
                     if j < 0 or j >= len(lines):
                         continue
                     if pattern in lines[j] or (regex and re.search(pattern, lines[j])):
                         match = True
                 if match:
                     r.write(line)
-    r.seek(0,0)
+    r.seek(0, 0)
     return r
+
+
 grepf = doc.deprecated(
     version="1.0.6.1",
     removed_in="2.0.0",
     reason="Use :func:`smpl_io.grep(..., open=True)` instead.",
-)(grep)
+)(grep)
```

### Comparing `smpl_io-1.1.2/smpl_io/head.py` & `smpl_io-1.1.4/smpl_io/head.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/smpl_io/io.py` & `smpl_io-1.1.4/smpl_io/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     Examples
     --------
     >>> read("nonexistent.txt")
     ''
     >>> write("test.out","hi")
     >>> read("test.out")
     'hi'
+    >>> read("https://raw.githubusercontent.com/APN-Pucky/smpl_io/master/LICENSE").split("\\n")[0].strip()
+    'GNU GENERAL PUBLIC LICENSE'
+
     """
     if to_be_read.startswith("http"):
         return requests.get(to_be_read).text
     else:
         if not os.path.exists(to_be_read):
             return ""
         with open(to_be_read, "r") as f:
@@ -407,15 +410,27 @@
 
 
 alias_open = open
 
 
 def open(to_be_read: str, mode="r"):
     """
-    Return opened buffer of either file or URI
+    Return opened buffer of either file or URI.
+
+    Parameters
+    ----------
+    to_be_read : str
+        file name or URI.
+    mode : str
+        mode to open the file.
+
+    Returns
+    -------
+    buffer
+        opened buffer.
     """
     if mode != "r":
         return alias_open(to_be_read, mode)
     if to_be_read.startswith("http"):
         return StringIO(requests.get(to_be_read).text)
     else:
         if not os.path.exists(to_be_read):
```

### Comparing `smpl_io-1.1.2/smpl_io/read_buffer.py` & `smpl_io-1.1.4/smpl_io/read_buffer.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/smpl_io/sed.py` & `smpl_io-1.1.4/smpl_io/sed.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/smpl_io/tail.py` & `smpl_io-1.1.4/smpl_io/tail.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.2/setup.py` & `smpl_io-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['requests', 'smpl_doc>=1.0.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'smpl-io',
-    'version': '1.1.2',
+    'version': '1.1.4',
     'description': 'simple input and output for python',
     'long_description': '# smpl_io\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_io.svg)\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] \n\n## Documentation\n\n-   <https://apn-pucky.github.io/smpl_io/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl_io\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl_io\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl_io/index.html\n[doc test]: https://apn-pucky.github.io/smpl_io/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl_io.svg\n[pypi link]: https://pypi.org/project/smpl_io/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl_io.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl_io/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl_io/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl_io/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl_io/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl_io&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl_io&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl_io&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl_io&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl_io/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl_io?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl_io?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl_io/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl_io/badge/?version=stable\n[rtd s l]: https://smpl_io.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl_io/badge/?version=latest\n[rtd t l]: https://smpl_io.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/smpl_io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `smpl_io-1.1.2/PKG-INFO` & `smpl_io-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: smpl-io
-Version: 1.1.2
+Version: 1.1.4
 Summary: simple input and output for python
 Home-page: https://github.com/APN-Pucky/smpl_io
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests
 Requires-Dist: smpl_doc (>=1.0.5,<2.0.0)
 Project-URL: Repository, https://github.com/APN-Pucky/smpl_io
```

