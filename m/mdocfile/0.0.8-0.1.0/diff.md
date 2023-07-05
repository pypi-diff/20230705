# Comparing `tmp/mdocfile-0.0.8.tar.gz` & `tmp/mdocfile-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdocfile-0.0.8.tar", last modified: Thu Apr  6 11:15:39 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mdocfile-0.0.8.tar` & `mdocfile-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.603387 mdocfile-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.599387 mdocfile-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.599387 mdocfile-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-06 11:15:25.000000 mdocfile-0.0.8/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-06 11:15:25.000000 mdocfile-0.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-06 11:15:25.000000 mdocfile-0.0.8/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-06 11:15:25.000000 mdocfile-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-06 11:15:25.000000 mdocfile-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-06 11:15:25.000000 mdocfile-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-06 11:15:25.000000 mdocfile-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-06 11:15:39.603387 mdocfile-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-06 11:15:25.000000 mdocfile-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.599387 mdocfile-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-06 11:15:25.000000 mdocfile-0.0.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.603387 mdocfile-0.0.8/mdocfile/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/global_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/section_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mdocfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.603387 mdocfile-0.0.8/mdocfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 11:15:39.000000 mdocfile-0.0.8/mdocfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-06 11:15:25.000000 mdocfile-0.0.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-06 11:15:39.603387 mdocfile-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-06 11:15:25.000000 mdocfile-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.603387 mdocfile-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:15:39.603387 mdocfile-0.0.8/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    43777 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_data/montage_section.mdoc
--rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_data/tilt_series.mdoc
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_global_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tests/test_section_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-06 11:15:25.000000 mdocfile-0.0.8/tox.ini
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 mdocfile-0.1.0/.github_changelog_generator
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 mdocfile-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mdocfile-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mdocfile-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tox.ini
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mdocfile-0.1.0/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 mdocfile-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 mdocfile-0.1.0/docs/index.md
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 mdocfile-0.1.0/docs/writing.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mdocfile-0.1.0/src/mdocfile/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 mdocfile-0.1.0/src/mdocfile/data_models.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 mdocfile-0.1.0/src/mdocfile/functions.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 mdocfile-0.1.0/src/mdocfile/utils.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data_models.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data/frame_set_multiple.mdoc
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data/frame_set_single.mdoc
+-rw-r--r--   0        0        0    43777 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data/montage_section.mdoc
+-rw-r--r--   0        0        0    68940 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data/montage_section_multiple.mdoc
+-rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 mdocfile-0.1.0/tests/test_data/tilt_series.mdoc
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 mdocfile-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 mdocfile-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 mdocfile-0.1.0/README.md
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 mdocfile-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 mdocfile-0.1.0/PKG-INFO
```

### Comparing `mdocfile-0.0.8/.github/workflows/build-and-deploy-docs.yml` & `mdocfile-0.1.0/.github/workflows/build-and-deploy-docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
           python-version: "3.10"
 
       - name: Install dependencies
         run: |
-          # pip install -e .
           pip install mkdocs mkdocs-material mkdocstrings[python]
       # Build the book
       - name: Build the book
         run: |
           mkdocs build
       # Push the site to github-pages
       - name: GitHub Pages action
```

### Comparing `mdocfile-0.0.8/.gitignore` & `mdocfile-0.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -99,7 +99,8 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
+.idea/
```

### Comparing `mdocfile-0.0.8/LICENSE` & `mdocfile-0.1.0/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-
-BSD License
-
-Copyright (c) 2022, Alister Burt
-All rights reserved.
+Copyright (c) 2023, Alister Burt
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 
@@ -24,8 +20,7 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `mdocfile-0.0.8/PKG-INFO` & `mdocfile-0.1.0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,42 @@
-Metadata-Version: 2.1
-Name: mdocfile
-Version: 0.0.8
-Summary: parse serialEM mdoc files in Python
-Home-page: https://github.com/alisterburt/mdocfile
-Author: Alister Burt
-Author-email: alisterburt@gmail.com
-License: BSD license
-Project-URL: Source Code, https://github.com/alisterburt/mdocfile
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: dev
-License-File: LICENSE
-
-# mdocfile
+# Overview
 
 [![License](https://img.shields.io/pypi/l/mdocfile.svg?color=green)](https://github.com/alisterburt/mdocfile/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/mdocfile.svg?color=green)](https://pypi.org/project/mdocfile)
 [![Python Version](https://img.shields.io/pypi/pyversions/mdocfile.svg?color=green)](https://python.org)
 [![CI](https://github.com/alisterburt/mdocfile/actions/workflows/ci.yml/badge.svg)](https://github.com/alisterburt/mdocfile/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/alisterburt/mdocfile/branch/main/graph/badge.svg)](https://codecov.io/gh/alisterburt/mdocfile)
 
 <p align="center" width="100%">
-    <img width="70%" src="https://user-images.githubusercontent.com/7307488/205445941-8db4ad0e-648a-446e-812d-bd1b81ec19b8.png"> 
+    <img width="70%" src="https://user-images.githubusercontent.
+com/7307488/205445941-8db4ad0e-648a-446e-812d-bd1b81ec19b8.png"> 
 </p>
 
-*mdocfile* is Python package for working with [SerialEM](https://bio3d.colorado.edu/SerialEM/) mdoc files.
+*mdocfile* is Python package for working with 
+[SerialEM](https://bio3d.colorado.edu/SerialEM/) 
+mdoc files.
 
 ---
 
 # Quickstart
 
 `mdocfile.read()` will return the contents of an mdoc file as a pandas 
 dataframe.
 
 ```python
+
 import mdocfile
 
 df = mdocfile.read('my_mdoc_file.mdoc')
 ```
 
+---
+
+For writing valid mdoc files, please see [writing mdoc files](./writing.md).
+
 # Installation
 
 pip:
 
 ```shell
 pip install mdocfile
-```
+```
```

### Comparing `mdocfile-0.0.8/mdocfile/functions.py` & `mdocfile-0.1.0/src/mdocfile/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import PathLike
 
 import pandas as pd
 
-from .mdoc import Mdoc
+from .data_models import Mdoc
 
 
 def read(filename: PathLike) -> pd.DataFrame:
     """Read an mdoc file as a pandas dataframe.
 
     Parameters
     ----------
@@ -15,19 +15,19 @@
 
     Returns
     -------
     df : pd.DataFrame
         dataframe containing info from mdoc file
     """
     mdoc = Mdoc.from_file(filename)
-    global_data = mdoc.global_data.dict()
+    global_data = mdoc.global_data.model_dump()
     section_data = {
-        k: [section.dict()[k] for section in mdoc.section_data]
+        k: [section.model_dump()[k] for section in mdoc.section_data]
         for k
-        in mdoc.section_data[0].dict().keys()
+        in mdoc.section_data[0].model_dump().keys()
     }
     df = pd.DataFrame(data=section_data)
 
     # add duplicate copies of global data and mdoc file titles to each row of
     # the dataframe - tidy data is easier to analyse
     for k, v in global_data.items():
         df[k] = [v] * len(df)
```

### Comparing `mdocfile-0.0.8/mdocfile/utils.py` & `mdocfile-0.1.0/src/mdocfile/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 
 def camel_to_snake(word: str) -> str:
     return camel_to_snake_regex.sub('_', word).lower()
 
 
 def find_section_entries(lines: List[str]) -> List[int]:
-    """Find the strings which contains a z-value or montage section entry."""
+    """Find the strings which contains a section entry header."""
     section_idx = [
         idx
         for idx, line
         in enumerate(lines)
-        if line.startswith('[ZValue =') or line.startswith('[MontSection =')
+        if (
+            line.startswith('[ZValue =')
+            or line.startswith('[MontSection =')
+            or line.startswith('[FrameSet =')
+        )
     ]
-    # for idx, line in enumerate(lines):
-    #     if line.startswith('[ZValue =') or line.startswith('[MontSection ='):
-    #         section_idx.append(idx)
+
     return section_idx
 
 
 def find_title_entries(lines: List[str]) -> List[int]:
     """Find mdoc title entries in a list of strings"""
     title_idxs = []
     for idx, line in enumerate(lines):
```

### Comparing `mdocfile-0.0.8/mkdocs.yml` & `mdocfile-0.1.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 edit_uri: edit/main/docs/
 
 copyright: Copyright &copy; 2022 - 2022 teamtomo
 
 
 nav:
   - index.md
+  - writing.md
 
 theme:
   icon:
     logo: material/cube-outline
   name: material
   palette:
     - media: "(prefers-color-scheme: light)"
```

### Comparing `mdocfile-0.0.8/tests/test_data/montage_section.mdoc` & `mdocfile-0.1.0/tests/test_data/montage_section.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.0.8/tests/test_data/tilt_series.mdoc` & `mdocfile-0.1.0/tests/test_data/tilt_series.mdoc`

 * *Files identical despite different names*

