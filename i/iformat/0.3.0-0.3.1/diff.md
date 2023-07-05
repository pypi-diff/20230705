# Comparing `tmp/iformat-0.3.0.tar.gz` & `tmp/iformat-0.3.1.tar.gz`

## Comparing `iformat-0.3.0.tar` & `iformat-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.3.0/setup.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 iformat-0.3.0/src/test.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 iformat-0.3.0/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.3.0/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.3.0/LICENSE
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iformat-0.3.0/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 iformat-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 iformat-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.3.1/setup.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 iformat-0.3.1/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.3.1/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 iformat-0.3.1/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 iformat-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 iformat-0.3.1/PKG-INFO
```

### Comparing `iformat-0.3.0/src/iformat/__init__.py` & `iformat-0.3.1/src/iformat/__init__.py`

 * *Files identical despite different names*

### Comparing `iformat-0.3.0/.gitignore` & `iformat-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.3.0/LICENSE` & `iformat-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.3.0/README.md` & `iformat-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 ## `.iformat` method for classes:
 You can add a `.iformat` method to any class to show the return value of that method instead of the default iformat output for classes. It must accept positional arguments `indentLevel`, `indentDepth`, `expansionThreshold`, and `excludedAttrs`, which will be passed the same values as those passed to the `iformat` function call that calls the method. It is reccomended that you add whitespace in front of the output corresponding to `indentLevel * indentDepth`, and that you call `iformat`, with the same passed args (maybe with indentDepth + 1) on any values that are part of the outputted string.
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
 
 https://github.com/FinnE145/iprint
+
 https://pypi.org/project/iformat
```

### Comparing `iformat-0.3.0/pyproject.toml` & `iformat-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.3.0/PKG-INFO` & `iformat-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.3.0
+Version: 0.3.1
 Summary: Indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -41,8 +41,9 @@
 ## `.iformat` method for classes:
 You can add a `.iformat` method to any class to show the return value of that method instead of the default iformat output for classes. It must accept positional arguments `indentLevel`, `indentDepth`, `expansionThreshold`, and `excludedAttrs`, which will be passed the same values as those passed to the `iformat` function call that calls the method. It is reccomended that you add whitespace in front of the output corresponding to `indentLevel * indentDepth`, and that you call `iformat`, with the same passed args (maybe with indentDepth + 1) on any values that are part of the outputted string.
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
 
 https://github.com/FinnE145/iprint
+
 https://pypi.org/project/iformat
```

