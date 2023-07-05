# Comparing `tmp/iformat-0.1.1.tar.gz` & `tmp/iformat-0.2.0.tar.gz`

## Comparing `iformat-0.1.1.tar` & `iformat-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.1.1/setup.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 iformat-0.1.1/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.1.1/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.1.1/LICENSE
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 iformat-0.1.1/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 iformat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.2.0/setup.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 iformat-0.2.0/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.2.0/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 iformat-0.2.0/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 iformat-0.2.0/PKG-INFO
```

### Comparing `iformat-0.1.1/src/iformat/__init__.py` & `iformat-0.2.0/src/iformat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+"""iformat is a simple package that prints basic data structures in an indented and readable format. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
 
 https://github.com/FinnE145/iprint
 
 https://pypi.org/project/iformat"""
 
 
 # Copyright (C) 2023  Finn Emmerson
@@ -40,18 +40,19 @@
     if type(i) in _iters:
         return (_brackets(type(i), True if length > et else False, ((il + 1) * id) if length > et else False)[0]\
             + ((",\n" + _indent(il + 1, id)) if length > et else (", ")).join(\
                     [f"{iformat(k, il + 1, id, et)}: {iformat(v, il + 1, id, et)}" for k, v in i.items()]\
                 if type(i) == dict else\
                     [iformat(x, il + 1, id, et) for x in i])\
             + _brackets(type(i), True if length > et else False, (il * id) if length > et else 0)[-1])
+    elif type(i) == function:
+        return f"<function {i.__name__}>"
     else:
-        if hasattr(i, "__dict__"):
-            if "iformat" in dir(i):
-                return i.iformat(il, id, et)
-            else:
-                return (f"{i.__class__.__name__}({', '.join([f'{k} = {iformat(v, il, id, et)}' for k, v in i.__dict__.items()])})")
+        if "iformat" in dir(i):
+            return i.iformat(il, id, et)
+        elif hasattr(i, "__dict__"):
+            return (f"{i.__class__.__name__}({', '.join([f'{k} = {iformat(v, il, id, et)}' for k, v in i.__dict__.items()])})")
         else:
             return str(i)
 
 def iprint(*args, indentDepth = 4, expansionThreshold = 0, sep = " ", end = "\n", file = None, flush = False):
     print(*[iformat(x, 0, indentDepth, expansionThreshold = expansionThreshold) for x in args], sep = sep, end = end, file = file, flush = flush)
```

### Comparing `iformat-0.1.1/.gitignore` & `iformat-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.1.1/LICENSE` & `iformat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.1.1/README.md` & `iformat-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iformat-0.1.1/pyproject.toml` & `iformat-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Provides a function that indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.1.1/PKG-INFO` & `iformat-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.1.1
+Version: 0.2.0
 Summary: Provides a function that indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

