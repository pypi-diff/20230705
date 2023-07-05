# Comparing `tmp/mscales-1.3.2.tar.gz` & `tmp/mscales-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.2.tar", last modified: Fri Jun 30 10:38:20 2023, max compression
+gzip compressed data, was "mscales-1.3.3.tar", last modified: Wed Jul  5 10:49:09 2023, max compression
```

## Comparing `mscales-1.3.2.tar` & `mscales-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      170 2023-06-30 05:22:16.000000 mscales-1.3.2/AUTHORS.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-06-30 05:22:16.000000 mscales-1.3.2/CONTRIBUTING.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-06-30 05:22:16.000000 mscales-1.3.2/LICENSE
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      360 2023-06-30 05:22:16.000000 mscales-1.3.2/MANIFEST.in
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1409 2023-06-30 10:38:20.429272 mscales-1.3.2/PKG-INFO
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      954 2023-06-30 05:22:16.000000 mscales-1.3.2/README.rst
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.407605 mscales-1.3.2/docs/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      673 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/Makefile
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      797 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/make.bat
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.418438 mscales-1.3.2/docs/source/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/conf.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      419 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/index.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/pcsets.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/quickstart.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1100 2023-06-30 10:33:51.000000 mscales-1.3.2/docs/source/release-history.rst
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)       71 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/scales.rst
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.440105 mscales-1.3.2/mscales/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      230 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/__init__.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      497 2023-06-30 10:38:20.440105 mscales-1.3.2/mscales/_version.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      529 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/concepts.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     8622 2023-06-30 10:26:06.000000 mscales-1.3.2/mscales/pcsets.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/plots.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/scales.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/sound.py
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/mscales/tests/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/__init__.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/conftest.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      160 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/test_examples.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/utils.py
-drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/mscales.egg-info/
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1409 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/PKG-INFO
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      683 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/SOURCES.txt
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)        1 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/dependency_links.txt
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)        6 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/requires.txt
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)        8 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/top_level.txt
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      276 2023-06-30 05:22:16.000000 mscales-1.3.2/pyproject.toml
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)       58 2023-06-30 05:22:16.000000 mscales-1.3.2/requirements.txt
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)      178 2023-06-30 10:38:20.429272 mscales-1.3.2/setup.cfg
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-30 05:22:16.000000 mscales-1.3.2/setup.py
--rw-r--r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-06-30 05:22:16.000000 mscales-1.3.2/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.3/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.3/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.3/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.3/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 10:49:09.287288 mscales-1.3.3/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.3/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.283288 mscales-1.3.3/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.283288 mscales-1.3.3/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.3/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/pcsets.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1180 2023-07-05 10:39:39.000000 mscales-1.3.3/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     8748 2023-07-05 10:47:04.000000 mscales-1.3.3/mscales/pcsets.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.3/pyproject.toml
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.3/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-05 10:49:09.287288 mscales-1.3.3/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.3/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.3/versioneer.py
```

### Comparing `mscales-1.3.2/CONTRIBUTING.rst` & `mscales-1.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/LICENSE` & `mscales-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/PKG-INFO` & `mscales-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -34,11 +34,11 @@
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
 Notes for development
 ---------------------
 
-- `python3 -m pip install -e .``
+- `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.2/README.rst` & `mscales-1.3.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
 Notes for development
 ---------------------
 
-- `python3 -m pip install -e .``
+- `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.2/docs/Makefile` & `mscales-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/docs/make.bat` & `mscales-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/docs/source/conf.py` & `mscales-1.3.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "mscales"
-copyright = "2022, Fabian C. Moss"
+copyright = "2023, Fabian C. Moss"
 author = "Fabian C. Moss"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 import mscales
```

### Comparing `mscales-1.3.2/docs/source/pcsets.rst` & `mscales-1.3.3/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/docs/source/quickstart.rst` & `mscales-1.3.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/docs/source/release-history.rst` & `mscales-1.3.3/docs/source/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+v1.3.3 (2023-07-05)
+-------------------
+
+- enable comparison of PitchClassSets
+
 v1.3.2 (2023-06-30)
 -------------------
 
 - fix prime-form and normal-form calculations
 
 v1.3.1 (2023-06-14)
 -------------------
```

### Comparing `mscales-1.3.2/mscales/concepts.py` & `mscales-1.3.3/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/mscales/pcsets.py` & `mscales-1.3.3/mscales/pcsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     """Set of pitch classes."""
 
     def __init__(self, pcset, c: int = 12):
         self.c = c
         self.d = len(pcset)
 
         if isinstance(pcset, str):
-            assert all(x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)), "Some pitch classes are not valid."
+            assert all(
+                x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)
+            ), "Some pitch classes are not valid."
             self.pcs = np.array([10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)])
         elif isinstance(pcset, (Iterable, PitchClassSet)):
             self.pcs = np.array(list(pcset))
         else:
             raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")
 
     def __repr__(self):
@@ -86,14 +88,18 @@
 
     # def __str__(self):
     #     return str(self.pcs)
 
     def __len__(self):
         return len(self.pcs)
 
+    def __eq__(self, other) -> bool:
+        if isinstance(other, PitchClassSet):
+            return self.pcs == other.pcs
+
     def sort(self):
         return PitchClassSet(np.sort(self.pcs))
 
     def to_vector(self):
         v = np.zeros(self.c, dtype=int)
         v[self.pcs] += 1
         return v
@@ -112,24 +118,23 @@
         Bring pitch-class set in normal form according to description at:
         https://musictheory.pugetsound.edu/mt21c/NormalForm.html
         """
 
         self = self.sort()
 
         rotations = np.array([np.roll(self.pcs, i) for i in range(self.pcs.shape[0])])
-        for l in range(self.d - 1, 0, -1):
-            spans = [ (r[-1] - r[0]) % self.c for r in rotations[:,:l + 1] ]
+        for length in range(self.d - 1, 0, -1):
+            spans = [(r[-1] - r[0]) % self.c for r in rotations[:, : length + 1]]
             mask = spans == min(spans)
             min_span_rotations = rotations[mask]
-            
+
             # if there is a tie in the first step and we want to obtain all candidates
             # (if there are more than one)
-            if (l == self.d - 1) and (all == True) and (min_span_rotations.shape[0] > 1):
+            if (length == self.d - 1) and all and (min_span_rotations.shape[0] > 1):
                 return min_span_rotations
-            
             # if there is only one candidate left
             elif min_span_rotations.shape[0] == 1:
                 return PitchClassSet(min_span_rotations.flatten())
             else:
                 continue
 
             # if there is an absolute tie, chose the one with smaller first element
@@ -154,15 +159,15 @@
             return candidate1
         elif np.less_equal(candidate2.pcs, candidate1.pcs).all():
             return candidate2
         else:
             return candidate1, candidate2
 
         # # if there had been more than one candidate for normal form
-        
+
         # return sorted.normal_form().transpose(-sorted.normal_form().pcs[0]), transposed
         #     transposed_inverted = transposed_inverted.sort().normal_form()
         # # if np.array_equal(inverted.pcs, transposed_inverted.pcs):
         # #     return transposed
         # if np.less_equal(transposed.pcs, transposed_inverted.pcs).all():
         #     return transposed
         # elif np.less_equal(transposed_inverted.pcs, transposed.pcs).all():
```

### Comparing `mscales-1.3.2/mscales/plots.py` & `mscales-1.3.3/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/mscales/scales.py` & `mscales-1.3.3/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/mscales/sound.py` & `mscales-1.3.3/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/mscales/utils.py` & `mscales-1.3.3/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/mscales.egg-info/PKG-INFO` & `mscales-1.3.3/mscales.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -34,11 +34,11 @@
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
 Notes for development
 ---------------------
 
-- `python3 -m pip install -e .``
+- `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.2/mscales.egg-info/SOURCES.txt` & `mscales-1.3.3/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/setup.py` & `mscales-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.2/versioneer.py` & `mscales-1.3.3/versioneer.py`

 * *Files identical despite different names*

