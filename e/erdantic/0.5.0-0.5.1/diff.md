# Comparing `tmp/erdantic-0.5.0.tar.gz` & `tmp/erdantic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdantic-0.5.0.tar", last modified: Sat Jul 30 01:47:37 2022, max compression
+gzip compressed data, was "erdantic-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `erdantic-0.5.0.tar` & `erdantic-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 01:47:37.352518 erdantic-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-30 01:46:38.000000 erdantic-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-30 01:46:38.000000 erdantic-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-07-30 01:47:37.352518 erdantic-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-07-30 01:46:38.000000 erdantic-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 01:47:37.352518 erdantic-0.5.0/erdantic/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7543 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)    13858 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/erd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 01:47:37.352518 erdantic-0.5.0/erdantic/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/examples/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/examples/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-07-30 01:46:38.000000 erdantic-0.5.0/erdantic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 01:47:37.352518 erdantic-0.5.0/erdantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-30 01:47:37.000000 erdantic-0.5.0/erdantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-07-30 01:46:38.000000 erdantic-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-30 01:46:38.000000 erdantic-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-30 01:47:37.352518 erdantic-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-07-30 01:46:38.000000 erdantic-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 01:47:37.352518 erdantic-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6285 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     6696 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_erd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-30 01:46:38.000000 erdantic-0.5.0/tests/utils.py
+-rw-r--r--   0        0        0     1072 2023-07-04 22:27:55.082980 erdantic-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3616 2023-07-04 22:27:55.082980 erdantic-0.5.1/README.md
+-rw-r--r--   0        0        0      296 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/__main__.py
+-rw-r--r--   0        0        0     7543 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/base.py
+-rw-r--r--   0        0        0     4623 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/cli.py
+-rw-r--r--   0        0        0     2436 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/dataclasses.py
+-rw-r--r--   0        0        0    13858 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/erd.py
+-rw-r--r--   0        0        0      166 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2246 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2199 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     3710 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/exceptions.py
+-rw-r--r--   0        0        0     3994 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/pydantic.py
+-rw-r--r--   0        0        0     3919 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/typing.py
+-rw-r--r--   0        0        0      205 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/version.py
+-rw-r--r--   0        0        0     1758 2023-07-04 22:27:55.086980 erdantic-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 erdantic-0.5.1/PKG-INFO
```

### Comparing `erdantic-0.5.0/LICENSE` & `erdantic-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/PKG-INFO` & `erdantic-0.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 Metadata-Version: 2.1
 Name: erdantic
-Version: 0.5.0
+Version: 0.5.1
 Summary: Entity relationship diagrams for Python data model classes like Pydantic.
-Home-page: https://github.com/drivendataorg/erdantic
-Author: DrivenData
-Author-email: info@drivendata.org
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
-Project-URL: Documentation, https://erdantic.drivendata.org/
-Project-URL: Source Code, https://github.com/drivendataorg/erdantic
-Description: # erdantic: Entity Relationship Diagrams
-        
-        [![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
-        [![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
-        [![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
-        [![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
-        [![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
-        
-        **erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
-        
-        - [Pydantic](https://pydantic-docs.helpmanual.io/)
-        - [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
-        
-        Features include a convenient CLI, automatic native rendering in Jupyter notebooks, and easy extensibility to other data modeling frameworks. Docstrings are even accessible as tooltips for SVG outputs. Great for adding a simple and clean data model reference to your documentation.
-        
-        <img alt="Example diagram created by erdantic" src="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg">
-        
-        ## Installation
-        
-        erdantic's graph modeling depends on [pygraphviz](https://pygraphviz.github.io/documentation/stable/index.html) and [Graphviz](https://graphviz.org/), an open-source C library. If you are on Linux or macOS, the easiest way to install everything together is to use conda and conda-forge:
-        
-        ```bash
-        conda install erdantic -c conda-forge
-        ```
-        
-        If not using conda, Graphviz must be installed first (before you can install pygraphviz). For recommended options and installation troubleshooting, see the [pygraphviz docs](https://pygraphviz.github.io/documentation/stable/install.html). Then to install erdantic and its Python dependencies from PyPI:
-        
-        ```bash
-        pip install erdantic
-        ```
-        
-        ### Development version
-        
-        You can get the development version from GitHub with:
-        
-        ```bash
-        pip install https://github.com/drivendataorg/erdantic.git#egg=erdantic
-        ```
-        
-        ## Quick Usage
-        
-        The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted path to your data model class and an output path. The rendered format is interpreted from the filename extension.
-        
-        ```bash
-        erdantic erdantic.examples.pydantic.Party -o diagram.png
-        ```
-        
-        You can also import the erdantic Python library and use its functions.
-        
-        ```python
-        import erdantic as erd
-        from erdantic.examples.pydantic import Party
-        
-        # Easy one-liner
-        erd.draw(Party, out="diagram.png")
-        
-        # Or create a diagram object that you can inspect and do stuff with
-        diagram = erd.create(Party)
-        diagram.models
-        #> [PydanticModel(Adventurer), PydanticModel(Party), PydanticModel(Quest), PydanticModel(QuestGiver)]
-        diagram.draw("diagram.png")
-        ```
-        
-        Check out the "Usage Examples" section of our [docs](https://erdantic.drivendata.org/) to see more.
-        
-Platform: UNKNOWN
+Keywords: erd,entity relationship diagram,dataclasses,pydantic
+Author-email: DrivenData <info@drivendata.org>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib_metadata ; python_version < '3.8'
+Requires-Dist: pydantic < 2
+Requires-Dist: pygraphviz
+Requires-Dist: typer
+Requires-Dist: typing_extensions > 4 ; python_version < '3.8'
+Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
+Project-URL: Changelog, https://erdantic.drivendata.org/stable/changelog/
+Project-URL: Documentation, https://erdantic.drivendata.org/
+Project-URL: Repository, https://github.com/drivendataorg/erdantic
+
+# erdantic: Entity Relationship Diagrams
+
+[![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
+[![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
+[![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
+[![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
+[![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
+
+**erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
+
+- [Pydantic](https://pydantic-docs.helpmanual.io/)
+- [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
+
+Features include a convenient CLI, automatic native rendering in Jupyter notebooks, and easy extensibility to other data modeling frameworks. Docstrings are even accessible as tooltips for SVG outputs. Great for adding a simple and clean data model reference to your documentation.
+
+<object type="image/svg+xml" data="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="https://raw.githubusercontent.com/drivendataorg/erdantic/main/docs/docs/examples/pydantic.svg"></object>
+
+## Installation
+
+erdantic's graph modeling depends on [pygraphviz](https://pygraphviz.github.io/documentation/stable/index.html) and [Graphviz](https://graphviz.org/), an open-source C library. If you are on Linux or macOS, the easiest way to install everything together is to use conda and conda-forge:
+
+```bash
+conda install erdantic -c conda-forge
+```
+
+If not using conda, Graphviz must be installed first (before you can install pygraphviz). For recommended options and installation troubleshooting, see the [pygraphviz docs](https://pygraphviz.github.io/documentation/stable/install.html). Then to install erdantic and its Python dependencies from PyPI:
+
+```bash
+pip install erdantic
+```
+
+### Development version
+
+You can get the development version from GitHub with:
+
+```bash
+pip install git+https://github.com/drivendataorg/erdantic.git#egg=erdantic
+```
+
+## Quick Usage
+
+The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted path to your data model class and an output path. The rendered format is interpreted from the filename extension.
+
+```bash
+erdantic erdantic.examples.pydantic.Party -o diagram.png
+```
+
+You can also import the erdantic Python library and use its functions.
+
+```python
+import erdantic as erd
+from erdantic.examples.pydantic import Party
+
+# Easy one-liner
+erd.draw(Party, out="diagram.png")
+
+# Or create a diagram object that you can inspect and do stuff with
+diagram = erd.create(Party)
+diagram.models
+#> [PydanticModel(Adventurer), PydanticModel(Party), PydanticModel(Quest), PydanticModel(QuestGiver)]
+diagram.draw("diagram.png")
+```
+
+Check out the "Usage Examples" section of our [docs](https://erdantic.drivendata.org/) to see more.
+
```

### Comparing `erdantic-0.5.0/README.md` & `erdantic-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # erdantic: Entity Relationship Diagrams
 
 [![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
 [![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
+[![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
 [![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
 [![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
 
 **erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
 
 - [Pydantic](https://pydantic-docs.helpmanual.io/)
 - [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
@@ -30,15 +31,15 @@
 ```
 
 ### Development version
 
 You can get the development version from GitHub with:
 
 ```bash
-pip install https://github.com/drivendataorg/erdantic.git#egg=erdantic
+pip install git+https://github.com/drivendataorg/erdantic.git#egg=erdantic
 ```
 
 ## Quick Usage
 
 The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted path to your data model class and an output path. The rendered format is interpreted from the filename extension.
 
 ```bash
```

### Comparing `erdantic-0.5.0/erdantic/base.py` & `erdantic-0.5.1/erdantic/base.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/cli.py` & `erdantic-0.5.1/erdantic/cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/dataclasses.py` & `erdantic-0.5.1/erdantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/erd.py` & `erdantic-0.5.1/erdantic/erd.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/examples/dataclasses.py` & `erdantic-0.5.1/erdantic/examples/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/examples/pydantic.py` & `erdantic-0.5.1/erdantic/examples/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/exceptions.py` & `erdantic-0.5.1/erdantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/pydantic.py` & `erdantic-0.5.1/erdantic/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.0/erdantic/typing.py` & `erdantic-0.5.1/erdantic/typing.py`

 * *Files identical despite different names*

