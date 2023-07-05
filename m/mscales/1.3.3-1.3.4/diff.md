# Comparing `tmp/mscales-1.3.3.tar.gz` & `tmp/mscales-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.3.tar", last modified: Wed Jul  5 10:49:09 2023, max compression
+gzip compressed data, was "mscales-1.3.4.tar", last modified: Wed Jul  5 11:05:53 2023, max compression
```

## Comparing `mscales-1.3.3.tar` & `mscales-1.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.3/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.3/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.3/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.3/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 10:49:09.287288 mscales-1.3.3/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.3/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.283288 mscales-1.3.3/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.283288 mscales-1.3.3/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.3/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1180 2023-07-05 10:39:39.000000 mscales-1.3.3/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.3/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     8748 2023-07-05 10:47:04.000000 mscales-1.3.3/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.3/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 10:49:09.287288 mscales-1.3.3/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-05 10:49:09.000000 mscales-1.3.3/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.3/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.3/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-05 10:49:09.287288 mscales-1.3.3/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.3/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.3/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.4/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.4/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.4/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.4/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 11:05:53.992607 mscales-1.3.4/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.4/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.4/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/pcsets.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1234 2023-07-05 11:03:13.000000 mscales-1.3.4/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.4/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     8762 2023-07-05 10:57:19.000000 mscales-1.3.4/mscales/pcsets.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.4/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-05 11:05:53.992607 mscales-1.3.4/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-05 11:05:53.000000 mscales-1.3.4/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.4/pyproject.toml
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.4/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-05 11:05:53.992607 mscales-1.3.4/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.4/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.4/versioneer.py
```

### Comparing `mscales-1.3.3/CONTRIBUTING.rst` & `mscales-1.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/LICENSE` & `mscales-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/PKG-INFO` & `mscales-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.3/README.rst` & `mscales-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/Makefile` & `mscales-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/make.bat` & `mscales-1.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/source/conf.py` & `mscales-1.3.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/source/pcsets.rst` & `mscales-1.3.4/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/source/quickstart.rst` & `mscales-1.3.4/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/docs/source/release-history.rst` & `mscales-1.3.4/docs/source/release-history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+v1.3.4 (2023-07-05)
+-------------------
+
+- minor fix
+
 v1.3.3 (2023-07-05)
 -------------------
 
 - enable comparison of PitchClassSets
 
 v1.3.2 (2023-06-30)
 -------------------
```

### Comparing `mscales-1.3.3/mscales/concepts.py` & `mscales-1.3.4/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/mscales/pcsets.py` & `mscales-1.3.4/mscales/pcsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     #     return str(self.pcs)
 
     def __len__(self):
         return len(self.pcs)
 
     def __eq__(self, other) -> bool:
         if isinstance(other, PitchClassSet):
-            return self.pcs == other.pcs
+            return np.array_equal(self.pcs, other.pcs)
 
     def sort(self):
         return PitchClassSet(np.sort(self.pcs))
 
     def to_vector(self):
         v = np.zeros(self.c, dtype=int)
         v[self.pcs] += 1
```

### Comparing `mscales-1.3.3/mscales/plots.py` & `mscales-1.3.4/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/mscales/scales.py` & `mscales-1.3.4/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/mscales/sound.py` & `mscales-1.3.4/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/mscales/utils.py` & `mscales-1.3.4/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/mscales.egg-info/PKG-INFO` & `mscales-1.3.4/mscales.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.3.3/mscales.egg-info/SOURCES.txt` & `mscales-1.3.4/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/setup.py` & `mscales-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.3/versioneer.py` & `mscales-1.3.4/versioneer.py`

 * *Files identical despite different names*

