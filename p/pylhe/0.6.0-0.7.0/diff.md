# Comparing `tmp/pylhe-0.6.0.tar.gz` & `tmp/pylhe-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylhe-0.6.0.tar", last modified: Thu Apr 20 07:58:57 2023, max compression
+gzip compressed data, was "pylhe-0.7.0.tar", last modified: Tue Jul  4 21:57:19 2023, max compression
```

## Comparing `pylhe-0.6.0.tar` & `pylhe-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-20 07:58:25.000000 pylhe-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 07:58:25.000000 pylhe-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-20 07:58:57.340460 pylhe-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-20 07:58:25.000000 pylhe-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-20 07:58:25.000000 pylhe-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-20 07:58:57.340460 pylhe-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-20 07:58:25.000000 pylhe-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/pylhe/
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-04-20 07:58:25.000000 pylhe-0.6.0/src/pylhe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-20 07:58:25.000000 pylhe-0.6.0/src/pylhe/awkward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:58:57.340460 pylhe-0.6.0/src/pylhe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 07:58:57.000000 pylhe-0.6.0/src/pylhe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:57:19.221808 pylhe-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-04 21:56:48.000000 pylhe-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 21:56:48.000000 pylhe-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-04 21:57:19.221808 pylhe-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-04 21:56:48.000000 pylhe-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-04 21:56:48.000000 pylhe-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-04 21:57:19.221808 pylhe-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-04 21:56:48.000000 pylhe-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:57:19.217808 pylhe-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:57:19.221808 pylhe-0.7.0/src/pylhe/
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-04 21:56:48.000000 pylhe-0.7.0/src/pylhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-04 21:56:48.000000 pylhe-0.7.0/src/pylhe/awkward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:57:19.221808 pylhe-0.7.0/src/pylhe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 21:57:19.000000 pylhe-0.7.0/src/pylhe.egg-info/top_level.txt
```

### Comparing `pylhe-0.6.0/LICENSE` & `pylhe-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylhe-0.6.0/PKG-INFO` & `pylhe-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhe
-Version: 0.6.0
+Version: 0.7.0
 Summary: small package to get structured data out of Les Houches Event files
 Home-page: https://github.com/scikit-hep/pylhe
 Author: Lukas Heinrich, Matthew Feickert, Eduardo Rodrigues
 Author-email: lukas.heinrich@cern.ch, matthew.feickert@cern.ch, eduardo.rodrigues@cern.ch
 License: Apache
 Project-URL: Source, https://github.com/scikit-hep/pylhe
 Project-URL: Tracker, https://github.com/scikit-hep/pylhe/issues
@@ -13,20 +13,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: develop
 Provides-Extra: complete
 License-File: LICENSE
 
@@ -94,16 +93,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.6.0}",
-  version = {v0.6.0},
+  title = "{pylhe: v0.7.0}",
+  version = {v0.7.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

### Comparing `pylhe-0.6.0/README.md` & `pylhe-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.6.0}",
-  version = {v0.6.0},
+  title = "{pylhe: v0.7.0}",
+  version = {v0.7.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 inspected as follows print(event.graph.source) # The graph is nicely displayed
 as SVG in Jupyter notebooks event # To save a DOT graph render the graph to a
 supported image format # (refer to the Graphviz documentation for more)
 event.graph.render(filename="test", format="png", cleanup=True)
 event.graph.render(filename="test", format="pdf", cleanup=True) ``` ## Citation
 The preferred BibTeX entry for citation of `pylhe` is ``` @software{pylhe,
 author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues}, title = "
-{pylhe: v0.6.0}", version = {v0.6.0}, doi = {10.5281/zenodo.1217031}, url =
+{pylhe: v0.7.0}", version = {v0.7.0}, doi = {10.5281/zenodo.1217031}, url =
 {https://github.com/scikit-hep/pylhe}, } ``` ## Contributors We hereby
 acknowledge the contributors that made this project possible ([emoji key]
 (https://allcontributors.org/docs/en/emoji-key)):
         [Matthew_Feickert]                        [Lukas]                  [Eduardo_Rodrigues]     [Johannes   [Henry   [ariaradick] [Junghwan
          Matthew_Feickert                          Lukas                    Eduardo_Rodrigues      Schumann] Schreiner]  ariaradick  John_Goh]
         ð§ ð¨ ð» �        ð§ ð¨ ð» �      ð§ ð» ð�Johannes    Henry        ð» Junghwan
                                                                                                    Schumann  Schreiner               John_Goh
```

### Comparing `pylhe-0.6.0/pyproject.toml` & `pylhe-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylhe-0.6.0/setup.cfg` & `pylhe-0.7.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 	License :: OSI Approved :: Apache Software License
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	graphviz>=0.12.0
 	particle>=0.16
 	awkward>=1.2.0
 	vector>=0.8.1
 
 [options.packages.find]
```

### Comparing `pylhe-0.6.0/setup.py` & `pylhe-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pylhe-0.6.0/src/pylhe/__init__.py` & `pylhe-0.7.0/src/pylhe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     "read_lhe_with_attributes",
     "read_num_events",
     "register_awkward",
     "to_awkward",
 ]
 
 
-# Python 3.7+
 def __dir__():
     return __all__
 
 
 # retrieve mapping of PDG ID to particle name as LaTeX string
 _PDGID2LaTeXNameMap, _ = DirectionalMaps("PDGID", "LATEXNAME", converters=(int, str))
```

### Comparing `pylhe-0.6.0/src/pylhe/awkward.py` & `pylhe-0.7.0/src/pylhe/awkward.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import awkward as ak
 import vector
 
 __all__ = ["register_awkward", "to_awkward"]
 
 
-# Python 3.7+
 def __dir__():
     return __all__
 
 
 def register_awkward():
     """
     .. deprecated:: 0.6.0
```

### Comparing `pylhe-0.6.0/src/pylhe.egg-info/PKG-INFO` & `pylhe-0.7.0/src/pylhe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylhe
-Version: 0.6.0
+Version: 0.7.0
 Summary: small package to get structured data out of Les Houches Event files
 Home-page: https://github.com/scikit-hep/pylhe
 Author: Lukas Heinrich, Matthew Feickert, Eduardo Rodrigues
 Author-email: lukas.heinrich@cern.ch, matthew.feickert@cern.ch, eduardo.rodrigues@cern.ch
 License: Apache
 Project-URL: Source, https://github.com/scikit-hep/pylhe
 Project-URL: Tracker, https://github.com/scikit-hep/pylhe/issues
@@ -13,20 +13,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: develop
 Provides-Extra: complete
 License-File: LICENSE
 
@@ -94,16 +93,16 @@
 ## Citation
 
 The preferred BibTeX entry for citation of `pylhe` is
 
 ```
 @software{pylhe,
   author = {Lukas Heinrich and Matthew Feickert and Eduardo Rodrigues},
-  title = "{pylhe: v0.6.0}",
-  version = {v0.6.0},
+  title = "{pylhe: v0.7.0}",
+  version = {v0.7.0},
   doi = {10.5281/zenodo.1217031},
   url = {https://github.com/scikit-hep/pylhe},
 }
 ```
 
 ## Contributors
```

