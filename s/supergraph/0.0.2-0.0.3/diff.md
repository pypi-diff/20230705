# Comparing `tmp/supergraph-0.0.2.tar.gz` & `tmp/supergraph-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supergraph-0.0.2.tar", max compression
+gzip compressed data, was "supergraph-0.0.3.tar", max compression
```

## Comparing `supergraph-0.0.2.tar` & `supergraph-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-30 12:15:06.992475 supergraph-0.0.2/LICENSE
--rw-r--r--   0        0        0     1359 2023-07-05 12:51:27.248547 supergraph-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    34039 2023-07-05 12:51:27.240548 supergraph-0.0.2/supergraph/__init__.py
--rw-r--r--   0        0        0    16888 2023-06-28 14:21:26.078126 supergraph-0.0.2/supergraph/deprecated.py
--rw-r--r--   0        0        0    20898 2023-07-05 11:47:11.316264 supergraph-0.0.2/supergraph/evaluate.py
--rw-r--r--   0        0        0     3843 2023-06-21 13:51:16.039324 supergraph-0.0.2/supergraph/open_colors.py
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 supergraph-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 12:15:06.992475 supergraph-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1359 2023-07-05 12:54:44.821922 supergraph-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    34039 2023-07-05 12:54:44.817922 supergraph-0.0.3/supergraph/__init__.py
+-rw-r--r--   0        0        0    16888 2023-06-28 14:21:26.078126 supergraph-0.0.3/supergraph/deprecated.py
+-rw-r--r--   0        0        0    20898 2023-07-05 11:47:11.316264 supergraph-0.0.3/supergraph/evaluate.py
+-rw-r--r--   0        0        0     3843 2023-06-21 13:51:16.039324 supergraph-0.0.3/supergraph/open_colors.py
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 supergraph-0.0.3/PKG-INFO
```

### Comparing `supergraph-0.0.2/LICENSE` & `supergraph-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supergraph-0.0.2/pyproject.toml` & `supergraph-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "supergraph"
-version = "0.0.2"
+version = "0.0.3"
 license = "Apache2.0"
 description = "Supergraph compiler."
 authors = ["Bas van der Heijden <d.s.vanderheijden@tudelft.nl>"]
 homepage = "https://github.com/bheijden/supergraph"
 repository = "https://github.com/bheijden/supergraph"
 documentation = "https://github.com/bheijden/supergraph"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-networkx = "^2.8.8"
+networkx = "^3.1.0"
 numpy = "^1.24.3"
 tqdm = "^4.65.0"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 # https://python-poetry.org/docs/pyproject/#extras
 # poetry install --all-extras or poetry install -E paper or poetry install --all-extras or poetry install --extras "paper"
```

### Comparing `supergraph-0.0.2/supergraph/__init__.py` & `supergraph-0.0.3/supergraph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import itertools
 import tqdm
 import time
 from typing import List, Dict, Tuple, Set, Any, Union, Callable
 from collections import deque
 import networkx as nx
```

### Comparing `supergraph-0.0.2/supergraph/deprecated.py` & `supergraph-0.0.3/supergraph/deprecated.py`

 * *Files identical despite different names*

### Comparing `supergraph-0.0.2/supergraph/evaluate.py` & `supergraph-0.0.3/supergraph/evaluate.py`

 * *Files identical despite different names*

### Comparing `supergraph-0.0.2/supergraph/open_colors.py` & `supergraph-0.0.3/supergraph/open_colors.py`

 * *Files identical despite different names*

### Comparing `supergraph-0.0.2/PKG-INFO` & `supergraph-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: supergraph
-Version: 0.0.2
+Version: 0.0.3
 Summary: Supergraph compiler.
 Home-page: https://github.com/bheijden/supergraph
 License: Apache2.0
 Author: Bas van der Heijden
 Author-email: d.s.vanderheijden@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: paper
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "paper"
-Requires-Dist: networkx (>=2.8.8,<3.0.0)
+Requires-Dist: networkx (>=3.1.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: wandb (>=0.15.4,<0.16.0) ; extra == "paper"
 Project-URL: Documentation, https://github.com/bheijden/supergraph
 Project-URL: Repository, https://github.com/bheijden/supergraph
```

